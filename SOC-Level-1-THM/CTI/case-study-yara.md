# Case Study: Yara Analysis

## Task 1: Introduction  
In this room, I learned about Yara, a tool used for identifying and classifying malware through rule-based signatures.

---

## Task 2: What is Yara?

### #2.1 What is the name of the base-16 numbering system that Yara can detect?  
I read through the provided documentation about Yara. I noticed that it mentioned Yara can detect hexadecimal patterns in files and memory scans.  

**Answer:** hex  

<img src="screenshots/yara1.png" width="600" height="auto">

---

### #2.2 Would the text “Enter your Name” be a string in an application? (Yay/Nay)  
I read the example section about Yara strings, and it explained that readable text within an application is recognized as a string.  

**Answer:** Yay  

<img src="screenshots/yara2.png" width="600" height="auto">

---

## Task 3: Deploy  

### #3.1 I’ve connected to my instance!  
I started the machine by pressing “Start Machine” and confirmed the instance was running.  

**Answer:** No answer is needed  

---

## Task 4: Introduction to Yara Rules  

### #4.1 One rule to — well — rule them all.  
I created a new file named `somefile` using:  

touch somefile

Then I created another file called myfirstrule.yar and opened it using nano myfirstrule.yar.
Inside it, I wrote a basic rule structure with a condition: true statement and saved it.

**Answer:** No answer is needed

<img src="screenshots/yara3.png" width="600" height="auto">
<img src="screenshots/yara4.png" width="600" height="auto">

---

##Task 5: Expanding on Yara Rules

### #5.1 Upwards and onwards…

I read the section that explained how Yara rules can include multiple strings, conditions, and metadata fields.

**Answer:** No answer is needed

---

## Task 6: Yara Modules
### #6.1 Sounds pretty cool!

I reviewed the Yara modules section and learned that modules enhance detection by allowing analysis of specific file types and formats.

**Answer:** No answer is needed

---

##Task 7: Other Tools and Yara
### #7.1 Cool tools. I’m ready to use one of them.

I explored how Yara integrates with other tools like Loki for malware detection.

**Answer:** No answer is needed

---

##Task 8: Using LOKI and Its Yara Rule Set

I navigated to the suspicious files directory:

cd /suspicious-files/file1/
python ../../tools/Loki/loki.py -p .

<img src="screenshots/yara5.png" width="600" height="auto">
### #8.1 Scan file 1. Does Loki detect this file as suspicious/malicious or benign?

I ran the scan and observed Loki marked the file as suspicious.

**Answer:** Suspicious

<img src="screenshots/yara6.png" width="600" height="auto">
### #8.2 What Yara rule did it match on?

After checking the scan output, I saw the Yara rule matched was webshell_metaslsoft.

**Answer:** webshell_metaslsoft

<img src="screenshots/yara7.png" width="600" height="auto">
### #8.3 What does Loki classify this file as?

The classification in the output showed it as a web shell.

**Answer:** Web Shell

<img src="screenshots/yara8.png" width="600" height="auto">
### #8.4 Based on the output, what string within the Yara rule did it match on?

In the Loki results, I saw that the rule matched on the string Str1.

**Answer:** Str1

<img src="screenshots/yara9.png" width="600" height="auto">
### #8.5 What is the name and version of this hack tool?

The version details showed b374k 2.2.

**Answer:** b374k 2.2

<img src="screenshots/yara10.png" width="600" height="auto">
### #8.6 Inspect the actual Yara file that flagged file 1. Within this rule, how many strings are there to flag this file?

I opened the Yara file and confirmed there was only one string condition.

**Answer:** 1

### #8.7 Scan file 2. Does Loki detect this file as suspicious/malicious or benign?

I switched to the file2 directory and ran:

cd /suspicious-files/file2/
python ../../tools/Loki/loki.py -p .


The results showed it as benign.

**Answer:** Benign

<img src="screenshots/yara11.png" width="600" height="auto">
### #8.8 Inspect file 2. What is the name and version of this web shell?

I opened the file using:

nano 1ndex.php

I found the version mentioned as b374k 3.2.3.

**Answer:** b374k 3.2.3

<img src="screenshots/yara12.png" width="600" height="auto">
## Task 9: Creating Yara Rules with yarGen

I generated a Yara rule for file2 using yarGen.

### #9.1 From within the root of the suspicious files directory, what command would you run to test Yara and your Yara rule against file 2?
yara file2.yar file2/1ndex.php


**Answer:** yara file2.yar file2/1ndex.php

<img src="screenshots/yara13.png" width="600" height="auto">
### #9.2 Did Yara rule flag file 2?

**Answer:** Yay

### #9.3 Copy the Yara rule you created into the Loki signatures directory.

I moved the generated rule file into the Loki Yara signatures directory.

**Answer:** No answer is needed

### #9.4 Test the Yara rule with Loki, does it flag file 2?

I tested again using Loki, and this time the file was flagged successfully.

**Answer:** Yay

### #9.5 What is the name of the variable for the string that it matched on?

From the Loki output, I saw the string variable name was Zepto.

**Answer:** Zepto

### #9.6 Inspect the Yara rule, how many strings were generated?

I opened the rule using nano and counted 20 strings in total.

**Answer:** 20

<img src="screenshots/yara14.png" width="600" height="auto">
### #9.7 One of the conditions to match on the Yara rule specifies file size. The file has to be less than what amount?

In the rule conditions, the filesize limit was set to less than 700KB.

**Answer:** 700KB

## Task 10: Valhalla
### #10.1 Enter the SHA256 hash of file 1 into Valhalla. Is this file attributed to an APT group?

I used the hash 5479f8cd1375364770df36e5a18262480a8f9d311e8eedb2c2390ecb233852ad in Valhalla and found it linked to an APT group.

**Answer:** Yay

### #10.2 Do the same for file 2. What is the name of the first Yara rule to detect file 2?

Using hash 53fe44b4753874f079a936325d1fdc9b1691956a29c3aaf8643cdbd49f5984bf, I found the first rule listed as Webshell_b374k_rule1.

**Answer:** Webshell_b374k_rule1

### #10.3 Examine the information for file 2 from VirusTotal (VT). The Yara Signature Match is from what scanner?

The scanner that matched the Yara rule was THOR APT.

**Answer:** THOR APT Scanner

### #10.4 Enter the SHA256 hash of file 2 into Virus Total. Did every AV detect this as malicious?

Not all antivirus engines flagged it as malicious.

**Answer:** Nay

### #10.5 Besides .PHP, what other extension is recorded for this file?

I checked the file details tab and found .exe listed as an additional extension.

**Answer:** EXE

### #10.6 What JavaScript library is used by file 2?

I searched within the rule details and found the library name Zepto.js.

**Answer:** Zepto

### #10.7 Is this Yara rule in the default Yara file Loki uses to detect these types of hack tools?

I searched inside the Loki signature base using grep but found no match for Webshell_b374k_rule1.

**Answer:** Nay

## Task 11: Conclusion

I learned how Yara rules are created, tested, and integrated into tools like Loki and Valhalla. I also practiced analyzing suspicious files and verifying rule detections through VirusTotal and Yara rule behavior.

