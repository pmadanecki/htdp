HTDP
High-Throughput Tabular Data Processor 

HIGH-THROUGHPUT TABULAR DATA PROCESSOR (HTDP) is Java application that is intended to facilitate data exploration and  reduction tasks in large text files resulting from high throughput technologies, e.g. massively parallel sequencing or microarrays. The software has been optimized for microarray and deep parallel sequencing data, however it can accept any character delimited tabular data sets. In the latter case the first row of the data set should be designated as header row and should contain the names of the corresponding columns. HTDP can also import, process and convert Variant Call Format (VCF) files ver. 4.0, 4.1 and 4.2 (http://samtools.github.io/hts-specs/VCFv4.2.pdf).
HTDP provides quick filtering functionality and can process data consisting of single or multiple input files. Files in different supported formats can be processed at the same time. The processed data can be exported as tab delimited file. The user interface provides two modes of operation: “basic mode” (default) and “advanced mode”.
Data filtering in the basic mode is carried out via selection of search terms from the pull down list or manual input of alphanumeric strings into a simple form (up to 8 queries). Data filtering in the advanced mode is carried out based on user defined unlimited queries. Subsequent queries are added to the queue, which constitutes a set of filtering criteria. This set of filtering criteria is applied to every row in the input file(s).
HTDP is distributed under GPL License version 3.0.
Nullsoft Scriptable Install System (NSIS, https://sourceforge.net/projects/nsis/) was used to generate windows installer. NSIS is licensed as zlib/libpng licensed software with parts licensed under bzip2 and Common Public License version 1.0. The installer automates installation process and is applicable in Windows only.
Apache Derby database (Apache License, Version 2.0) is required to compile HTDP (http://db.apache.org/derby/).

Screenshots:
https://github.com/pmadanecki/htdp/issues/1

Repository structure:
bin – binary files (for automatic [windows] and manual [] installation)
src – source code (the software is developed using NetBeans IDE [https://netbeans.org/] so whole NetBeans project directory tree was compressed and deposited)
docs – user manual and other documentation (example data files were deposited in publicly available repository: https://osf.io/pw2dx/)

Install:
Depending on your operating system use:
htdpinstaller.exe - Windows installer
htdp.tgz - tar archive for manual installation (Linux and other java supported operationg systems)
Both files may be downloaded from bin directory.
 System requirements:
Windows XP, Windows 7 or Linux with Java run time environment v. 1.6 or later (64-bit version)*.
At least 1 GB of RAM, depending on the amount of input data and complexity of queries.

*Default Java version is 32-bit and its maximum theoretical heap limit is 4GB. To increase the amount of allocated memory and therefore the performance of this program, the 64-bit version should be used.

Windows (automated installation):
Run the installation program (htdpinstaller.exe) and follow the on screen tips.
The installation program will create program group “HIGH-THROUGHPUT TABULAR DATA PROCESSOR” in Windows Start Menu.
The program group contains the shortcut to the “HIGH-THROUGHPUT TABULAR DATA PROCESSOR” as well as to the uninstall program.
Additional shortcut to the “HIGH-THROUGHPUT TABULAR DATA PROCESSOR” will be created on Windows desktop.

Windows (manual installation):
Copy HTDP.jar file and lib folder from the installation archive to selected folder on local hard drive. Run the program using the following command:

java -Xmx800M  -jar "/path/to/the/program/folder/HTDPjar

Linux:
Copy HTDP.jar file from the installation archive to selected folder on local hard drive. Run the program using the following command:
java -Xmx800M  -jar "/path/to/the/program/folder/HTDP.jar


Troubleshooting 
When software does not start
check java installation, 
try runing without memory reservation - use: 
java -jar /path/to/the/program/folder/HTDP.jar 
instead of 
java -Xmx800M -jar /path/to/the/program/folder/HTDP.jar 

