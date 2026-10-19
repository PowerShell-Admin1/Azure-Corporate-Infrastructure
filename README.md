# **Azure-Corporate-Infrastructure**


Enterprise-grade Azure infrastructure demonstrating networking, compute, monitoring, security, governance and operational best practices aligned with Microsoft AZ-104 Azure Administrator objectives.




##**Projects Overview**


This project showcases the design, deployment and management of a secure Azure infrastructure environment. The solution incorporates core Azure services including Virtual Networks, Virtual Machines, Network Security Groups, Monitoring, Identity Management and Governance controls.

The project demonstrates practical cloud administration skills commonly required for Azure Administrator, Cloud Engineer and Infrastructure Engineer roles.


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## Architecture

- Internet

- Azure Virtual Network

- Azure Bastion

- Windows Server VM

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

 
Designed and implemented a secure Azure networking architecture using multiple Virtual Networks, VNet Peering and Azure Bastion. The networking layer was configured to provide workload isolation, secure connectivity between environments and protected administrative access to virtual machines.

<img width="1596" height="732" alt="Newtwork" src="https://github.com/user-attachments/assets/b3e0ad0b-d55c-44a0-9097-aad365544ea9" /> 


The environment consists of four Virtual Networks hosted within the az104-rg1 resource group, including dedicated networks for Core Services and Manufacturing workloads.   


**#VNet Peering** 

<img width="1047" height="806" alt="Vnet Peering1" src="https://github.com/user-attachments/assets/03d6bc3d-22af-4fcc-8aa9-31bde0e8eb7e" /> 

<img width="1061" height="813" alt="Vnet Peering 2" src="https://github.com/user-attachments/assets/5332c443-85fe-4166-9182-ea578f78cd21" /> 


VNet Peering was configured to enable secure communication between virtual networks without requiring traffic to traverse the public internet. This allows resources hosted in separate networks to communicate using Microsoft's private Azure backbone infrastructure.


**#Secure Administration with Azure Bastion** 


<img width="1002" height="595" alt="Screenshot 2026-10-19 100410" src="https://github.com/user-attachments/assets/ef473394-caa4-48df-887e-00b29777b3db" /> 

Azure Bastion was deployed within the CoreServicesVnet network to provide secure browser-based RDP connectivity to virtual machines without exposing management ports to the internet. 


**Measurable Outcomes** 

- Successfully deployed 4 Azure Virtual Networks within the UK South region.

- Implemented VNet Peering to enable private connectivity between network environments.

- Created dedicated network boundaries for Core Services and Manufacturing workloads. 

- Deployed Azure Bastion to eliminate the need for direct public RDP access to virtual machines.

- Reduced network exposure by removing dependency on publicly accessible management ports.

- Built a scalable network foundation capable of supporting compute, storage, monitoring and security services.

- Centralised network resources within a single Azure Resource Group for simplified administration and governance. 


**Skills Demonstrated** 

- Azure Virtual Networks (VNets)

- VNet Peering

- Azure Bastion 

- Network Segmentation

- Secure Remote Administration

- Cloud Network Architecture

- Enterprise Networking

- Network Security Best Practices


**3. Network Security Groups**  

Implemented Network Security Groups (NSGs) to control traffic flow between Azure resources and enforce network security requirements. Custom inbound and outbound rules were configured to support application access while restricting unnecessary connectivity.


<img width="1591" height="597" alt="NSGs" src="https://github.com/user-attachments/assets/f0b88db5-067a-49fc-b062-1a4933a1d507" /> 

<img width="1597" height="832" alt="NSG" src="https://github.com/user-attachments/assets/7274e7ee-664a-4e20-89be-f5722e46ccd0" />

<img width="1580" height="811" alt="NSG Deny Rule" src="https://github.com/user-attachments/assets/dd7a792c-0f3c-420c-a5f8-93dd5f5bae61" /> 


**Measurable Outcomes**  
  
- Deployed 5 Network Security Groups across the Azure environment.

- Applied custom inbound security rules to permit only required application traffic on TCP ports 80 and 443.

- Configured RDP access controls using a dedicated security rule on port 3389.

- Implemented outbound Internet restrictions through a custom deny rule.

- Applied security controls at subnet level to support workload isolation.

- Enforced least-privilege network access by limiting permitted traffic paths.

- Maintained Azure default deny rules to protect resources from unauthorised access.


**Skills Demonstrated** 

- Azure Network Security Groups (NSGs)

- Network Access Control

- Inbound & Outbound Security Rules

- Application Security Groups (ASGs)


**4. Virtual Machine Deployment** 

Designed and deployed Windows Server virtual machines to support Core Services and Manufacturing workloads within a secure Azure infrastructure environment. Compute resources were configured across dedicated virtual networks and availability zones to improve workload separation, resilience and operational management.


**#CoreServices Virtual Machine ** 

<img width="1165" height="857" alt="VM1" src="https://github.com/user-attachments/assets/fbe5ecf9-c630-46e6-ac5c-afa93cfd2890" />  

The CoreServiceVM was deployed within the CoreServicesVnet network and configured with Windows Server 2025 Datacenter. Administrative access is provided through Azure Bastion to support secure management without exposing direct RDP access to the internet.


**#Manufacturing Virtual Machine** 

<img width="1102" height="860" alt="VM2 " src="https://github.com/user-attachments/assets/a942a750-c0f6-49e5-a23a-099dafdf6435" /> 

The ManufacturingVM was deployed within the ManufacturingVnet network to provide network separation between business workloads. The virtual machine was configured with dedicated networking resources and integrated with the overall monitoring and security framework. 


**#Vistual Machine Scale Set (VMSS)** 

To demonstrate scalable cloud infrastructure, a Virtual Machine Scale Set (VMSS) was deployed using Azure's Uniform Orchestration model. The VMSS provides a platform for highly available workloads and supports horizontal scaling to accommodate increased demand.


**Measurable Outcomes ** 

- Successfully deployed and configured 2 Windows Server 2025 Datacenter virtual machines.

- Implemented workload isolation using dedicated VNets and subnets for Core Services and Manufacturing environments.

- Deployed virtual machines across Availability Zones 1 and 2 to improve resilience.

- Configured Azure Bastion connectivity to provide secure browser-based VM administration.

- Successfully deployed a Virtual Machine Scale Set with 2 running instances to demonstrate scalable infrastructure capabilities.

- Established a compute platform capable of supporting enterprise applications and future workload expansion.


**Skills Demonstrated**  

- Windows Server 2025 Administration

- Virtual Machine Scale Sets (VMSS)

- Availability Zones

- Azure Bastion

- Azure Infrastructure Management

- High Availability Design



**5. Storage Services** 

Implemented Azure Storage solutions to provide secure, resilient and scalable data storage for business workloads. The environment includes both Azure Blob Storage and Azure File Storage, configured with redundancy, data protection and secure access controls to support enterprise requirements. 


**#Azure Blob Storage** 

<img width="1570" height="901" alt="Blob " src="https://github.com/user-attachments/assets/992aff4e-9129-4a7f-8546-d67630c66799" /> 
 
The storage account rgblog1 was deployed using Azure StorageV2 and configured to support blob-based data storage. Security settings were implemented to enforce encrypted connections while providing controlled access to storage resources. 


**#Azure File Storage** 

<img width="1427" height="757" alt="File " src="https://github.com/user-attachments/assets/f2606da6-2048-4ec0-b821-bc6ff260c0ae" /> 

The storage account rgfile was deployed using the Azure FileStorage account type to provide managed file share services. Geo-redundant storage was configured to improve data resilience and disaster recovery capabilities. 
 
**#Security and Data Protection** 

The storage environment was configured with Azure security best practices, including: 











