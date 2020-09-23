# PFA Performance Tests

This repo includes the basic PFA scenarios scripted using Jmeter 5.3 for Performance Testing PFA Platform. 
**Note** - This does not cover component level performance testing
**Scenarios Covered :**
Main User Scenarios  
- User creation and activation 
- Login 
- NewsFeeds 
- Recognize 
- Catalog 
- Boost 

Utility Scenarios 

- Change Budget 
- Change Points 

## Steps to run the Scripts
### 1) Pre Requisits
 - Download Apache Jmeter
 - Download the Jmeter Scripts in this repo
 
### 2) Adjust User defined variables
#### 2.1) Environment Varibales 
For now the script are configured to execute on "qa04" environment, with the users exists on that environment. Adjust the "**User Defined Variables**" in the Jmeter script depending on your environment.

#### 2.2) Execution Varibales 
Thread execution configurations differ for the Main user scenarios and utility scenarios. Utility scenarios are configured to execute only once and the main user user scenarios are configured to execute with 60 concurrent users for 5 minutes.
| Thread Group | Variable | Default Value |
| ------ | ------ |------ |
| PFA Utility Scenarios |threads|1 |
| PFA Utility Scenarios |loop count |1 |
| PFA General User Scenarios |threads |60 |
| PFA General User Scenarios |loop count |infinite |
| PFA General User Scenarios |lexecution time |300s |
 
### 3)  Execute in GUI Mode
- Open the given "PFAPerfTest_V01.jmx" file with Jmeter
- Adjust the environment and execution varibales as required
- Run the test

### 4) Execute in headless mode
- Go to $JMETER_HOME/bin via Terminal (>> cd $JMETER_HOME/bin)
- Execute jmeter in headless mode "./jmeter -n -t PFAPerfTest_V01.jmx -l PFAPerTestReport.jtl"
