# reqres
Repository for a test assignment.

The APIs are automated using Postman and Javascript with Chai Assertions.

The documentation for APIs is present online here: 
https://documenter.getpostman.com/view/12108577/T1DmDeNa?version=latest

To Execute Tests:

via Command Line (Newman)- Requirement: Node > v10 and Newman Package

  1. Install Node
  2. Install Newman -> npm install -g newman
  3. Clone the repository - git clone https://github.com/oomkarpanditstudent/reqres.git
  4. Open windows terminal/command prompt and navigate to the folder with all the files.
  5. Execute Functional tests by running this command 
          newman run ReqResApiAutomated.json -e Production.env  --folder Functional-Tests -r cli,progress
      
          Above will execute all the Functional Test and report will appear on the terminal windows with results of test execution.
          
 6.  To execute E2E integration tests with a data file by this command
         
          newman run ReqResApiAutomated.json -e Production.env -d create-user-data.csv --folder Data-Driven-Looped-User-Creation -r cli,progress
          
via Postman UI:

  1. Clone the repository - git clone https://github.com/oomkarpanditstudent/reqres.git
  2. Install Postman tool
  3. Import Collection
  4. Run Collection
  5. Select Environment as Production
  6. If running the Data-Driven-Looped-User-Creation then select the .csv file from the cloned repository. It will reflect the interations as per the data.
  7. Select the relevant folders to run. Ignore folder Data-Driven-Looped-User-Creation, as it is best to run this independently to avoid unnecessary iterations.
  8. Run tests by clicking on the Req-Res-API-Automation-Test button.
  
  
