# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

#### Azure Virtual Machine (IaaS)
- Cost is higher
- Scalability and Availability are developer's responsibility, managed via VM scale sets and load balancers
- Full control over VM but heavy operational overhead

#### Azure App Service (PaaS)
- Cost is lower and more predicatable
- Scalability and Availability are automatic and fast
- Almost zero server management

#### Chosen solution
**Azure App Service (Web App)** 
##### Justification for choosing App Service over VM
- The application is described as a lightweight article management system so it's a perfect fit for PaaS.
- No need for access or control over the OS. 
- Significantly lower operational overhead.
- Faster and cheaper scaling.
- Lower total cost.
- Higher SLA and better availability.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

- Requirement for accessing or controlling OS.
- Extremly high compute requirements the exceed the App Service limits.