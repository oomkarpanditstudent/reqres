# reqres
Repository for a test assignment.

The APIs are automated using Postman and Javascript with Chai Assertions.

The documentation for APIs is present online here: 
https://documenter.getpostman.com/view/12108577/T1DmDeNa?version=latest

To Execute Test:

via Command Line (Newman)- Requirement: Node > v10 and Newman Package

  1. Install Node
  2. Install Newman -> npm install -g newman
  3. Clone the repository - git clone https://github.com/oomkarpanditstudent/reqres.git
  4. Open windows terminal/command prompt and navigate to the folder with all the files.
  5. Execute tests by running this command 
          newman run ReqResApiAutomated.json -e Production.env  --folder Functional-Tests -r cli,progress
      
      This will execute all the Functional Test and report will appear on the terminal windows with results of test execution.
 
