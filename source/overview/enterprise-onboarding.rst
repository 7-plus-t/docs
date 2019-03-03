Enterprise On-Boarding Overview
===============================

.. note:: If you're looking to deploy Mattermost for fewer than 25 to 50 people, it's quick and easy with a wide range of quick start guides at XXX. The following overview is for large or sophisticated enterprise deployments, with hundreds to thousands of users in high trust data centers. 

Project planning and definition 
- Success Metrics // reduction of email, MAU, DAU 
- Project Plan // development, testing, pilot, roll out 
- Network Diagram - https://docs.mattermost.com/_images/network.PNG
- Hardware Sizing 
- Site Reliability Engineering Plan  

Pilot with staging and production 
- Procure trial license 
- Set up staging server in high availability and verify proper redundancy is in place. 
- On-board users to staging server 
- Set up initial set of integrations to get comfortable with API
- Set up process for pushing configuration changes to production 
- (Optional) Set up Mattermost Load Test to vet hardware sizing 

Internal branding for web, PC & mobile 
- Apply custom branding options to user login screen and across the site
- (Optional) Compile mobile apps with specific server URL as default, deployed internally 
- (Optional) Compile desktop apps with specific server URL as default, deployed internally  
- (Optional) Customize user experience through open source web, mobile and desktop apps 

Integrations with custom systems 
- Set up integrations server to interact with customer systems using Mattermost webhooks, drivers, bots and APIs
- (Optional) Build off of open source templates 
- (Optional) Configure integrations with redundancy (link) 

Corporate directory synchronization 
- Organize Mattermost users in AD/LDAP so they can be referenced in a single group (Note: nested SGs not supported). 
- (Optional) Combine multiple AD/LDAP instances using a forrest 
- Bulk load users into channels and roles based on AD/LDAP groups and other user meta-data
- (Optional) Synchronize specific channels with membership in AD/LDAP groups (roadmap). 
- Deploy & test AD/LDAP synchronization and activation and deactivation of users 

Role & permissions configuration 
- Define roles and permissions for system admin, team admin, and channel admins 
- (Optional) Define custom roles for administering Mattermost teams and channels (roadmap) 

Securing and deploying mobile apps
- (Optional) Compile mobile apps to internal enterprise app store 
- (Optional) Deploy with EMM solutions using SDKs or AppDome 

Scale, security & penetration testing 
- Conduct internal penetration test 
- Validate hardware is properly configured by running Mattermost Load Test  
- Finalize plan for security updates 
- Upgrade plan 
- Disaster Recover Plan 
- Standby Plan - Blue/Green set up for application servers and read databases. 

Help desk & end user training
- Finalize help desk plan and common escalations
- Prepare end user announcement with links to help resources 
- (Optional) Create your own copy of Mattermost end user help documentation  

Roll out announce & phased onboarding 
- Bulk load users by phase and configure user Account Settings 
- Mass email newly loaded users to let them know how to use the system, including how to set up mobile app

Discovery 
---------

**Requirements definition** is drafted after identifying stakeholders and priorities, including key requirements and scenarios. Development of high level solution design document and project plan to achieve priorities.

- Example of
https://docs.mattermost.com/_images/network.PNG



Design Planning 
---------------

**Solution design plan** translating business requirements into specific plans, including: 

- Infrastructure (hardware, software, and network resources) 
- Staffing for rollout (project management, change management, technical operations, development staff for customziations)
- Staffing for on-going support (help desk support and technical administration) 
- Internal communications plan (announcements and materials for pilot, phased roll-out, training and resources) 
- Customizations (plans for white-labelling, integrations, and micro-apps) 
- Training (organizing and developing training content and delivery for end users, operations staff and developers)

Pilot 
-----

**Pilot deployment** set up to evaluate solution prototype: 

- Deploy Mattermost either manually using install guides or under your own orchestration framework using open source installers. 
- Set up staging and production environments 
- (Optional) Deploy Mattermost in high availability configuration.
- (Optional) Deploy Mattermost Load Testing Framework (MLTF) to simulate production-level load. 

**Verification and planning** for full-scale roll-out, including: 

- On-board pilot deployment users to evaluate the solution and to discuss and prioritize potential extensions and customizations. 
- Monitor system load during pilot to project and prepare for production level deployment. 
- Verification of security, privacy and compliance requirements 

Phased Roll-out 
---------------

Based on stakeholder priorities and pilot program feedback, customizations are developed prior to phrased roll-out: 

- Corporate directory integration 
- Automated import of users and channels from other systems using CLI, APIs or drivers
- Configuration of user accounts, default settings, roles and permissions  
- Whitelabelling of login screens, email templates, and desktop and mobile applications 

Rolling Invitations 
-------------------

- End users segmented and invitations email sent out in phases to ensure smooth on-boarding 
- Feedback from user group meetings and surveys collected, analysized and incorporated into on-going plan 




