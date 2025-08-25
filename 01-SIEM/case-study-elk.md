# 📝 Case Study: Investigating with ELK 101

## 🔹 Overview
In this case study, I explored the **Elastic Stack (ELK)** and focused on **analyzing VPN logs** for a US-based company to identify anomalies and suspicious activity. The study covers **Kibana Discover tab, KQL queries, visualizations, and dashboards**.

---

## 🔍 Key Tasks & Learnings

### Task 1: Introduction
- Explored **Kibana interface** and Elastic Stack components.
- Learned to perform **searches, apply filters, and create visualizations**.
- Understood **VPN log structure** in the `vpn_connections` index.

---

### Task 2: Incident Handling Scenario
- Investigated **anomalous VPN activity** for January 2022.
- Applied SOC analyst techniques to detect:
  - Unauthorized access attempts
  - Suspicious user activity (e.g., terminated user **Johny Brown** still connecting)
  - Patterns in failed connections

---

### Task 3: ElasticStack Overview
The Elastic Stack (ELK Stack) is a collection of open-source components used to gather, search, analyze, and visualize data in real-time.

**Components:**
- **Elasticsearch:** Full-text search and analytics engine storing JSON-formatted documents. Provides a RESTful API for queries and data interaction.  
- **Logstash:** Data processing engine that ingests data from multiple sources, applies filters/normalization, and sends it to Elasticsearch or Kibana.  
  - Input: Source of data (supports multiple plugins)  
  - Filter: Normalizes/transforms data  
  - Output: Sends data to destinations like Elasticsearch or Kibana  
- **Beats:** Lightweight agents that collect and send specific data (e.g., Winlogbeat for Windows logs, Packetbeat for network traffic).  
- **Kibana:** Web-based visualization tool for analyzing and visualizing data stored in Elasticsearch. Enables dashboards and visualizations.
  
---

### Task 4: Kibana Overview
Kibana is a core component of the Elastic Stack used to display, visualize, and search logs.  
Important tabs include: **Discover**, **Visualization**, and **Dashboard**.

---

### Task 5: Discover Tab
The Discover tab is a central workspace for searching, filtering, and investigating ingested logs.

**Key Features:**  
- Logs/Documents: Each event stored as a document with multiple fields.  
- Search Bar: Run queries and filters.  
- Time Filter: Filter logs based on time range.  
- Timeline Chart: Spot anomalies or spikes.  
- Index Pattern: Select which indices to explore. Example: `vpn_connections`.  
- Fields Pane: Filter logs by field values.  
- Create Table: Customize and save tables from log fields.

**Questions & Answers:**  
1. Select the index vpn_connections and filter from 31st December 2021 to 2nd Feb 2022. How many hits are returned?
   I used the Time Filter in the top right corner to set the date range from 31st December 2021 to 2nd February 2022 and then pressed refresh.
   ![Filtered Hits Screenshot](screenshots/T5-Q1.png)
   **Answer:** 2861
3. Which IP address has the max number of connections?
   **Answer:** 238.163.231.224  
5. Which user is responsible for max traffic?
   **Answer:** James  
7. Create a table with the fields IP, UserName, Source_Country and save.
   **Answer:** No answer needed
9. Apply Filter on UserName Emanda; which SourceIP has max hits?
   **Answer:** 107.14.1.247
11. On 11th Jan, which IP caused the spike observed in the time chart?
    **Answer:** 172.201.60.191
13. How many connections were observed from IP 238.163.231.224, excluding the New York state?
    **Answer:** 48 


