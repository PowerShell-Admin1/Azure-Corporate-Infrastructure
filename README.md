# **Azure-Corporate-Infrastructure**


Enterprise-grade Azure infrastructure demonstrating networking, compute, monitoring, security, governance and operational best practices aligned with Microsoft AZ-104 Azure Administrator objectives.




##**Projects Overview**


This project showcases the design, deployment and management of a secure Azure infrastructure environment. The solution incorporates core Azure services including Virtual Networks, Virtual Machines, Network Security Groups, Monitoring, Identity Management and Governance controls.

The project demonstrates practical cloud administration skills commonly required for Azure Administrator, Cloud Engineer and Infrastructure Engineer roles.


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## Architecture

- Internet

- Azure Virtual Network

- Management Subnet ---Azure Bastion

- Application Subnet --- Windows Server VM

- Data Subnet --- Storage Account

- Network Security Groups 

- Azure Monitor

- Log Analytics Workspace

- Microsoft Entra ID



--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## Key Technologies

**Compute**

- Azure Virtual Machines

- Virtual Machine Extentions

- Managed Disks

- Availability Configuration


  **Networking**

  - Azure Virtual Networks
 
  - Subnets
 
  - Network Security Groups (NSGs)
 
  - Azure Bastion
 
  - DNS Configuration
 

    **Security**

    - Microsoft Entra ID
   
    - Role-Based Access Control (RBAC)
   
    - Recourse Lock
   

      **Monitoring**

      - Azure Monitor
     
      - Log Analytics
     
      - Alerts and Metrics
     
      - Activity Logs
     

      **Governance**
   
      - Resource Groups
     
      - Tags
     
      - Cost Management
     
      - Azure Policy




------------------------------------------------------------------------------------------------------------------------------------------------------------------
     

 ## Project Objectives


 - Deploy secure Azure infrastructure

 - Configure network segmentation

 - Implement least-privilege access controls

 - Monitor infrastructure health and performance

 - Apply governance and cost-management practices

 - Demonstrate production-ready cloud administration skills


----------------------------------------------------------------------------------------------------------------------------------------------------------------   
 
  
## Implementation Evidence 


**1. Resource Group Deployment**

Created a dedicated Azure Resource Group to organise and manage all project resources. Applied a consistent naming convention and resource structure to simplify administration and governance.

<img width="1057" height="825" alt="Screenshot 1ResourceGroup-WithTags" src="https://github.com/user-attachments/assets/77205a5f-0b5d-4ed2-b853-942b1cfae115" />

<img width="1082" height="671" alt="Screenshot 2ResourceGroup-WithLock" src="https://github.com/user-attachments/assets/b3f6b629-be44-4d86-bddf-5255de6ac46a" />


    
**Measurable Outcomes**
- Successfully deployed 24 Azure resources and configurations within a single managed Resource Group.

- Implemented standardised resource tag and lock across the environment to improve governance and resource tracking.

- Organised networking, security, monitoring and compute resources within a single administrative boundary.

- Established a production-labelled environment to support enterprise infrastructure management practices.

**Skills Demonstrated**

- Azure Resource Groups

- Azure Resource Manager (ARM)

- Resource Tag & Lock

- Cost & Resource Management

- Azure Deployment Management


**2. Virtual Network Configuration** 

Designed and deployed multiple Azure Virtual Networks to provide network isolation and support different business workloads. The environment was configured to support secure communication and scalable infrastructure deployment. 


<img width="1596" height="732" alt="Newtwork" src="https://github.com/user-attachments/assets/b3e0ad0b-d55c-44a0-9097-aad365544ea9" /> 

<img width="1047" height="806" alt="Vnet Peering1" src="https://github.com/user-attachments/assets/03d6bc3d-22af-4fcc-8aa9-31bde0e8eb7e" /> 

<img width="1061" height="813" alt="Vnet Peering 2" src="https://github.com/user-attachments/assets/5332c443-85fe-4166-9182-ea578f78cd21" /> 


**Measurable Outcomes** 

- Successfully deployed 4 Azure Virtual Networks within the UK South region.

- Established separate network environments for core services and manufacturing workloads.

- Created the network foundation required for virtual machines, security controls and monitoring services.

- Organised network resources within a centralised Resource Group for easier administration.


**Skills Demonstrated** 

- Azure Virtual Networks (VNets)

- Network Design

- Subnets

- IP Address Planning


**3. Network Security Groups**  



  









