Camel-CXF-Calculator 
====================
This project is an usecase or sample for exposing a cxf soap based webservice using wsdl. This WSDL exposes only single operation called calculate. 

This project uses 
* Blueprint DSL for camel routes and DI
* CXF Bean component and its dataformat is set to MESSAGE
* JAXB Dataformat for Marshalling and Unmarshalling the request
* CBR EIP for routing the request to the appropriate Processor class based on the operationName
* Processor class for consuming the request and setting the response back to the caller 
* &lttransform&gt for sending the response back to the caller
* JaxWS factory bean for creating client call from java code 

This is an OSGI-Based project and it is packed as bundle
