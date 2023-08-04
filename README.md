<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Provision Azure Infrastructure
- Deploy Azure Virtual Machines
- Configure AD Forest and Domains
- Establish Identity Synchronization
- Implement Security and Access Controls

<h2>Deployment and Configuration Steps</h2>

<p>

  ![image](https://github.com/AEY982312/configure-ad/assets/116044851/2e7ba430-189a-49a7-b730-40af064ec245)

<p>
Set up the necessary infrastructure in Azure to host your on-premises AD. This typically involves creating a virtual network (VNet) and configuring subnets, security groups, and network security rules. You may also need to establish a secure connection between your on-premises network and the Azure VNet, such as a site-to-site VPN or Azure ExpressRoute. Ensure that the VMs are provisioned with sufficient resources and meet the requirements for running AD. You can use Azure Marketplace images that come pre-configured with the necessary Windows Server operating system and AD roles, or you can bring your own custom VM images.
</p>
<br />

<p>

  ![image](https://github.com/AEY982312/configure-ad/assets/116044851/cea99c2a-d300-413a-904b-5560cacb8df3)

</p>
<p>
Once the VMs are deployed, promote them to domain controllers and configure the AD forest and domains. This involves defining the forest structure, such as the forest root domain and any child domains, and configuring DNS settings. Configure AD replication between the domain controllers to ensure data consistency.
</p>
<br />

<p>

  ![image](https://github.com/AEY982312/configure-ad/assets/116044851/cb4cf5bd-8fb5-46f8-b13a-49d6b1a4cdd5)


</p>
<p>
If you have an existing on-premises AD infrastructure, you'll want to synchronize identities between your on-premises AD and the Azure AD tenant associated with your Azure subscription. This can be achieved using Azure AD Connect, which allows for directory synchronization and enables features like password hash synchronization and single sign-on. Implrementing security and access control Ensure that proper security measures are in place to protect your AD deployment. This includes configuring network security groups to control inbound and outbound traffic, implementing Azure AD Privileged Identity Management (PIM) to manage administrative access, enabling Azure AD Conditional Access policies to enforce multi-factor authentication, and regularly monitoring and reviewing security logs and events.
</p>
<br />
