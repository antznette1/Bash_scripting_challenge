# **Bash Scripting Challenge - AWS re/Start Class**

## **Introduction**

Welcome to my Bash scripting challenge, part of the AWS re/Start class! This project demonstrates the intricacies of Bash scripting and how I overcame a unique challenge to enhance my cloud computing skills.


## **Challenge Overview**

### **The Task**

Create a batch of 25 sequentially numbered files. The twist? The script must intelligently continue numbering from where the last batch ended, based on the highest number already present in the directory.
Development Environment

Connection: Accessed my EC2 instance using PuTTY.
Directory Setup: Created a new directory named files and navigated into it.
    

![image](https://github.com/antznette/Bash-Scripting_challenge/assets/85882006/19b74b63-99cc-4bcb-8e64-dec4f324a887)


Script Creation: Utilized nano to write the script in a file named new_files.
Saved with Control + O and exited to the console using Control + X.

![image](https://github.com/antznette/Bash-Scripting_challenge/assets/85882006/4c95a83d-00d9-406b-9cce-47156d4d62d0)


 
### **Permission Adjustment**

Modified the script's permissions with chmod to make it executable.

### **Execution and Challenges**

Initial Run: On executing the script, the files were created but not listed serially. Used ls -lv for a serial listing.
    

![image](https://github.com/antznette/Bash-Scripting_challenge/assets/85882006/fb594967-ee0c-4a48-885a-c574f1993d8e)



### **Running Scrpt 2**

Octal Confusion: Discovered a quirk in Bash where numbers with leading zeros (like "008" and "009") are treated as octal, leading to confusion in the script.


### **Solution**

Developed an improved script (script2 in the repository) that addressed these challenges. The key was handling Bash's octal interpretation and ensuring serial file creation.

Key Script Features:

Octal Handling: Implemented a method to correctly interpret numbers with leading zeros as decimal.
Serial File Creation: Ensured the script picks up the numbering correctly and maintains a sequential order.


![image](https://github.com/antznette/Bash-Scripting_challenge/assets/85882006/66df6cb3-c42d-4339-9600-077a3cf5515a)



### **Conclusion**

This challenge was more than a scripting task; it was a deep dive into Bash's behavior and a testament to the power of problem-solving in coding. As I delve further into cloud computing, these scripting abilities are proving invaluable for automation and efficient resource management.

Feel free to explore the scripts in this repository and share your experiences or feedback!
