# DevOps-TechTalk

------

Team Members:
------
- Akansha Chandre ()
- Amruta Shintre ashintr)
- Vaibhav Rajadhyaksha (vrajadh)

# Description
FindBugs is an open source tool for static code analysis of java programs. It scans the compiled bytecode in the compiled class files to identify common bug patterns. The software is distributed as a stand alone GUI application , along with plugins that are available for Eclipse , IntelliJ, Netbeans and other IDE's. 

Static analysis is a method of program debugging that is done by examining the code without executing it. Since static analysis scans the entire code base, it has high probabilities of finding vulnerabilities in remote parts fo the application. Also you can define project specific rules that are expected to be followed. Another major advantage is that this technique helps find bugs early in the development cycle.

# Installation Instructions:

#### Extracting Distribution :

One can go to the following url and download either the tar or zip format binary distributions. We can then extract into a directory of choice using the belwo commands.

Extracting a gzipped tar format distribution:

**gunzip -c findbugs-3.0.1.tar.gz | tar xvf -**

Extracting a zip format distribution:

**unzip findbugs-3.0.1.zip**

#### Installing as an Eclipse Plugin:

1. In Eclipse go to the help Tab
2. Click on the install new software option
3. For older versions of eclipse paste the following url : http://findbugs.cs.umd.edu/eclipse . For higher versions e.g 4.6 use the following url: https://github.com/findbugsproject/findbugs/releases/tag/3.0.2_preview2 . Click add and follow the instructions to install the plugin. 
