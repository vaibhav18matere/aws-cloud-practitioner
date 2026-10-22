# AWS-Cloud-Practitioner-CLF-C02
### AWS Certified Cloud Practitioner Certification Course (CLF-C02) - Notes and Study Material
- Practice Exam - https://www.exampro.co/clf-c02
- Syllabus


| Topic |     Percentage |          Questions       |
| :-------- | :------- | :------------------------- |
| Cloud Concepts |24% | 15/16 Questions |
| Security And Compliance |34% | 19/20 Questions |
| Cloud Technology And Services |30% | 22 Questions |
| Billing, Pricing And Support |12% | 8 Questions |

```
  Passing Eligibility - 700/1000 Marks (70%)
```

```
Location : Online/ At Center Center
AWS Uses Scale Scoring
Total 65 Questions : 50 Scored and 15 Unscored (difficult or out of scope questions)
You can get afford to wrongly score 15/50 questions
No penalty for wrong questions
Questions : 1. Mutiple Choice Questions 2. Multiple Answer Questions
There are 15 unscored questions, whic will not count in final score
Time - 1.5 Hrs i.e. 90 Minutes
1.5 Minutes Per Question
If you get really hard or weird question then keep yourself cool, it might be unscore question.
Cetification Valid for 3 Years, if you want to appear again it costs half.
```
 
### Benefits of On-prem
1. On demand
2. Shared Resources
3. For Anyone
4. Elasticity
5. Pay As You Go Model

- It is comparativerly easy to scale up than scaling down

### Problems
1. Buying Hardware
2. Installation
3. Expansion
4. Operations

### Types of Cloud Services
1. IaaS - Infrastructure as a Service
- AWS EC2, Azure Virual Machine

2. PaaS - Platform as a Service
- AWS Elastic Beanstalk, Azure Webapps

3. SaaS - Software as a Service
- Salesforce, Twitter etc

### Control Over Cloud
1. Private Cloud - 
- You own the hardware
- Install and own software
- Only you willuse it (security)
2. Public Cloud
- Economy of scale
- Elasticity
3. Hybrid Cloud
- Combination of both
- Internet or Private link
4. Multi Cloud
- AWS, Azure, Open Stack

### AWS - Amazon Web Services

### AWS Shared Responsibility Model

#### AWS is resopnsible for 
1. Hardsware / Global Infrastructure
- Regions
- Availability Zones
- Edge Locations
2. Software
- Compute
- Storage
- Database
- Networking

#### Customer is responsible for
1. Client side data, encryption, authentication, IAM,
2. Server side encryption (file system AND/OR data)
3. Networking traffic protection (encryption, identity, integriry)
4. Operating Systems, Network and Firewall Configurations
5. Platform, Applications, IAM,
6. Customer Data

### IAM

1. Group (attached with policy) ex. Admin, Dev, Tester, Monitor
2. Role
3. User
   
#### Policy 
1. defines the permission
2. It's a json document
3. it is implicitely dennied - be default everything is not allowed
4. We should not add a policy directly to user.
5. Create group, add policy to that group and add user in a particular group
6. Least Previledge Permission Policy / "Least Previledge Possible"
7. AWS Supports 6 types of policies
   - Identity Based Policy : gives permission to an identity.
   - Resource Based Policy : ex. S3 bucket - publically available.
   - Permission Boundaries : maximum permissions that the identity based policies can grant to an entity but does not gramt permissions. It does not set the permissions it allows what you can set. for ex. you can give permissions to EC2 but not bean stock.
   - Organization (SCP) Service Control Policy : For ex. you can set a policy that perticular unit thay it can only create 5 EC2 instances, not more than that. SCP do not grant permisioon, they CONTROL what permissions are availableto be granted for that organizational unit. 
   - Access Control List (ACL) : Cross account permission policy
   - Session Policy : 
  
#### Root User : 
1. Created when first time AWS account creation email and has full permissions
2. Enable MFA
3. Create new user from root user
4. New user has a zero/ no permissions by default
5. You can create 5000+ accounts
6. Use policies and prefer Groups
7. ARN : Amazon Resource Name and regular name
8. Username & Password or Access Keys

#### AWS Authentication
1. You Know : Password
2. You Have : OTP, Mobile, USB
3. You Are : Fingerprint, Face lock etc

- Rotate keys and Password
- Do not use root account for any task
- IAM Access Analyser
- Regularly check and remove users, roles, permissions policies and credentials "that are not being in use" - re-evaluate
- You can also add conditions like IP range or geo location based access
