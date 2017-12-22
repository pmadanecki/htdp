GDP
Genome Data Processor

Repository structure:
bin – binary files (for automatic [windows] and manual [] installation)
src – source code (the software is developed using NetBeans IDE [https://netbeans.org/] so whole NetBeans project directory tree was compressed and deposited)
docs – user manual and other documentation (example data files were deposited in publicly available repository: https://osf.io/pw2dx/)

Install:
Depending on your operating system use:
gdpinstaller.exe - Windows installer
gdp.tgz - tar archive for manual installation (Linux and other java supported operationg systems)
Both files may be downloaded from bin directory.
 System requirements:
Windows XP, Windows 7 or Linux with Java run time environment v. 1.6 or later (64-bit version)*.
At least 1 GB of RAM, depending on the amount of input data and complexity of queries.

*Default Java version is 32-bit and its maximum theoretical heap limit is 4GB. To increase the amount of allocated memory and therefore the performance of this program, the 64-bit version should be used.

Windows (automated installation):
Run the installation program (gdpinstaller.exe) and follow the on screen tips.
The installation program will create program group “GENOMIC DATA PROCESSOR” in Windows Start Menu.
The program group contains the shortcut to the “GENOMIC DATA PROCESSOR” as well as to the uninstall program.
Additional shortcut to the “GENOMIC DATA PROCESSOR” will be created on Windows desktop.

Windows (manual installation):
Copy GeneVariantsComparator.jar file and lib folder from the installation archive to selected folder on local hard drive. Run the program using the following command:

java -Xmx800M  -jar "/path/to/the/program/folder/GeneVariantsComparator.jar

Linux:
Copy GeneVariantsComparator.jar file from the installation archive to selected folder on local hard drive. Run the program using the following command:
java -Xmx800M  -jar "/path/to/the/program/folder/GeneVariantsComparator.jar


Troubleshooting 
When software does not start
check java installation, 
try runing without memory reservation - use: 
java -jar /path/to/the/program/folder/GeneVariantsComparator.jar 
instead of 
java -Xmx800M -jar /path/to/the/program/folder/GeneVariantsComparator.jar 

