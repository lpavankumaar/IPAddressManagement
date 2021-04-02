# IP Address Management (IPAM)

IP address management (IPAM) is a means of planning, tracking, and managing the Internet Protocol address space used in a network.

## Pre-Requisites

1. Enable Macros when you open the worksheet
2. IP Addresses Considered For Cloud Segregation: 

    |**Cloud Provider**|IP address range|Classification|Number of addresses|
    |--------------|----------------|--------------|-------------------|    
    |Microsoft Azure|10.0.0.0 – 10.255.255.255|Class A|16777216|
    |Amazon Web Services| 172.16.0.0 – 172.31.255.255|Class B|1048576
    
_Note: The above requirment has to be considered based on the organization requirement_

## IP Submit Form 

Project and Network Details to be filled in the IP Submit Form (_All details in the **WHITE** color to be filled mandatory_) 

### Project Details

|Category|Details|
|-----------|-------|
|Project Name| _Name of the Project_|
|Application Name|_Name of the Application_|
|Business Unit|_Name of the Business Unit_|	
|Cloud Provider|_Choose Cloud Provider from Drop Down section_|	
|Requested By|_Name of the Requestor_| 	
|Number of Virtual Networks|_Number of VNET's planned for this project_|
|Number of Resources|_Number of resources (approximate count) planned for this project_|

### Network Details

|Category|Details|
|-----------|-------|
|VNET / VPC Name|_Name of the VNET / VPC_|	
|CIDR Block|_CIDR Block for the Project_| 	
|Network Size (Count)|_Auto Fill_|
|Netmask|_Auto Fill_|	
|Wildcard Mask|_Auto Fill_|	
|First IP Address|_Auto Fill_|	
|Last IP Address|_Auto Fill_|	
|CIDR Availability|_Auto Fill_ **(Available / Duplicate)**|	
|Cloud IP Range Choice|_Auto Fill_ **(VALID / INVALID)**|	
|Final Request Validation|_Auto Fill_ **(VALID / INVALID)**|

**_Note:_** 
1. If there are more virtual networks are needed for any project, justification to be provided and to be approved by concerned authorities
2. If the project need to allocate more than 256 IP addreses, justification to be provided and to be approved by concerned authorities
3. Before applying the CIDR block in the Form, need to check the last IP range used under IP Check Spreadsheet. 

### Validation

1. To complete the validation, the following has to be in **GREEN**	
    * CIDR Availability: Should be **Available**  		
    * Cloud IP Range Choice: Should be **VALID**		
    * Final Request Validation: Should be **VALID**		
2. If there are any conditions listed above are **RED**, the form to be re-visited with proper CIDR block and choice of the Cloud Provider		
3.   Once All the Validations are in **GREEN**, then submit by Clicking Submit Form

## IP Management Tracker

This sheet provides the inventory of the projects and its CIDR blocks used. If there are any duplications of CIDR Block / VNET Name, it will get highlighted with RED.	
			
## IP Check

This will provide overview of IP CIDR Block ranges used in the environment. Also it provides information of the IP ranges used across cloud provider and the last IP range is used.	


