SoapAPI-TestSample-soapui-project

1. Projekt 'Calculator' sklada sie z czterech prostych requestow (Add, Multiply, Divide, Subtract),
   realizujacych podstawowe dzialania matematyczne i korzysta z WSDL'a: 
   http://www.dneonline.com/calculator.asmx?wsdl

2. Opis projektu:
   Dane do kolejnych dzialan (requestow) przypisywane sa ze zmiennych (Properties) oraz wynikow dzialania 
   poprzednich requestow (response). Koncowy wynik jest weryfikowany przez Script Assertion w requescie 'Subtract'

3. Celem tego prostego projektu 'end-to-end' jest zaprezentowanie podstawowych umiejetnosci z zakresu testowania SOAP API 
   w SoapUI, ktore nabylem korzystajac z online'owych tutoriali. 

4. Zakres wiedzy:
   - Tworzenie Projektu, TestSuite, Test Case, Test Step (PropertyTransfer, Grovy Script, Property Step)
   - Tworzenie i odwolywanie sie do zmiennych (Properties) na roznych poziomach (Project, Test Suite itd.)
   - Tworzenie prostych Groovy Script'ow. Przekazywanie parametrow pomiedzy requestami/test stepami:
     > Korzystanie z klasy XmlHolder do parsowania request/response
     > Korzystanie z klasy testRunner do odwolywania sie do zmiennych na roznych poziomach.
     > Korzystanie z metod getNodeValue/setNodeValue do odwolania sie do wezlow (Node)
   - Korzystnie z 'Property Transfer' do przekazywania parametrow pomiedzy requestami.
   - Tworzenie podstawowych asercji (Contains, Valid/Invalid HTTP Status Codes, ResponseSLA, SOAP Respnse, XPathMatch itd.)
   - Tworzenie prostych Script Assertions:
     > Korzystanie z klasy messageExchane do odwolania sie do odpowiedzi (responseContent)
     > Korzystanie z klasy context do odwolania sie do zmiennych na roznych poziomach (Project, Test Suite itd.)
     Opisywane asercje sa uzyte w ostatnim test step'ie 'Subtract' 
      