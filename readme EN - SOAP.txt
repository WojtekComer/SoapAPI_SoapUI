SoapAPI-TestSample-soapui-project

1. 'Calculator' project consists of four simple requests (Add, Multiply, Divide, Subtract) performing basic math calculations.
   It uses WSDL http://www.dneonline.com/calculator.asmx?wsdl

2. Project description:
   Data for consecutive requests are passed from so called Properties (variables) or calculation results (other request's responses). 
   Final result is verified by Script Assertion included in 'Subtract' request/step.

3. The purpose of this simple 'end-to-end' project is to present some basic SoapUI SOAP API testing skills that I acquired during my 
   online tutorial self-studying 

4. Scope of knowledge:
   - Creating Project, TestSuite, Test Case, Test Step (PropertyTransfer, Grovy Script, Property Step)
   - Creating and accessing Properties (variables) at different levels (Project, Test Suite, Test Case, TestStep)
   - Creating simple Groovy Scripts. Passing Parameters between requests/test steps:
     > Using XmlHolder class to parse request/response
     > Using testRunner class to access Properties (variables) at different levels.
     > Using getNodeValue/setNodeValue methods for accessing nodes.
   - Using 'Property Transfer' step to pass Parameters between requests.
   - Creating basic assertions (Contains, Valid/Invalid HTTP Status Codes, ResponseSLA, SOAP Response, XPathMatch etc.)
   - Creating basic Script Assertions:
     > Using messageExchane class to access 'responseContent'
     > Using context class to access properties at different levels (Project, Test Suite etc.)
     Mentioned assertion examples are used in 'Subtract' request/step. 
      