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

# How it works

After installing the plugin , we can simply go to the projects and run find bugs on the entire project folder, packages or individual source code files as depicted in the below screenshot.

![Alt text](https://github.com/rajadhva/DevOps-TechTalk/blob/master/Screenshots/find_bugs_main)

The Errors/Warnings that are found by the analysis can be opened in a separate perspective in eclipse as shown below. The warnings are classified into 4 separete types which are namely, scariest, scary, troubling and ofConcern. We cann double click on the type of warnign being thrown which takes us to the line of code where the issue exists.

![Alt text](https://github.com/rajadhva/DevOps-TechTalk/blob/master/Screenshots/bug_types.png)

In the bottom pane we get a complete description of the type of bug along with an xml representation of the same which can be used to generate bug reports.

![Alt text](https://github.com/rajadhva/DevOps-TechTalk/blob/master/Screenshots/bug_description.png)

We can also configure the various settings by going into the properties tab . It includes specifying include/exclude filter flies to include/exclude certain bug types. We can also determine the lowest level of warnings that we want to see low/medium/high. Also we can directly select/deselect certain bugs as a part of configuring it.

![Alt text](https://github.com/rajadhva/DevOps-TechTalk/blob/master/Screenshots/properties config.png)

# Examples :

# Advantages :

1. There isnt a steep learning curve when it comes to getting started with FindBugs. you just need to install the plugin and run Findbugs on the package/source code you want to analyze.
2. Find Bugs offers granular control by providng us with include and exclude filters. The exclude filter as the name suggests can be used to exclude reporting of certain bugs.The include filter is used to report targetted bugs. Some bugs might not be relevant and if there's a consensus among the team as to which bugs to target during static analysis , the filters feature is very helpful 
3. It is great in finding potential security, performance ans style errors. It provides suggestions for good practices like method naming guidelines to improve code readability and maintainability. It also captures security defects and performance issues such as invoking the constructors ineffciently.
4. The fact that it runs on the bytecode makes it extremely efficient with respect to time taken to perform the analysis.

# Disadvantages :

1. The issue highlighted by the tool may not always be intuitive and may require understanding on the part of the person performing the analysis. For eg: Incorrect lazy initilaztion and update of static field , might not be a very familiar to a person who comes from a functional progrmming background.
2. There are always chances of false postives when it comes to static analysis tools. However based on research, Findbugs is known to produce the least false positives  as compared to other tools.
3. FindBugs needs the compiled class file i.e bytecode to run the analysis.

