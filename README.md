# aws-notes

TYPES OF CLOUD:
1. Public
2. Private
3. Hybrid

   Advantages
   1. Scalibility
   2. Flexibility
   3. Redendency

   Disadvantages
   1. Less control over underlying infra.
   2. Data Security and Privacy risks.
   3. Unexpected expences
   4. Integration complexity with existing       system

Cloud Secvives Model:
1.Iaas
2.Paas
3.Saas

*Compute Services:
1.EC2: Elastic Compute Cloud
2.ECS: Elastic container service
3.Lambda Servives: Serverless

*Storage Services
1.S3: Simple storage service
2.EBS: Block storage
3.EFS: Object Storage
4.Glacier: Archival service

* Diff btw block storage and object storage
  
NETWORK SERVICES
1. VPC: Virtual Private Cloud
2. DNS: Route53
3. Direct Connect

   
DATA IS THE NEW OIL Oracle is the better

CLOUD COMPUTING - is the delivery of computing services wherein they provide servers, storage, databases, networking, software, analytics, and intelligence over the internet ("the cloud") for faster innovation, flexible resources, and economies of scale.
On-demand delivery
Pay-as-you-go model
Provision only the size you need(exactly right type and size)
Access resources instantly



BENEFITS OF CLOUD

Faster time to market - Instead of investing funds in creating a new data structure, the org relies on clouds like AWS and utilises these funds in their business.

Scalability and flexibility - cloud offers an unlimited amount of virtual resources

Cost savings

Better collaboration - teams can still collaborate in different geographical regions.

Advanced security - cloud ensures data security.

Data loss prevention - customers cant lose their data in S3.


DISADVANTAGES OF CLOUD

Risk of vendor lock-in- it's impossible for the organisation to move from one cloud to another.

Less control over underlying cloud infrastructure - If a company wants more control of their compliance(at the under-neath layer), then it must refrain from using the cloud.

Concerns about security risks like data privacy and online threats

Integration complexity with existing systems

Unforeseen costs and unexpected expenses.


GARTNER's MAGIC QUADRANT - A big org that does analytics part.


PUBLIC CLOUD v/s PRIVATE CLOUD -

Public Cloud	Private Cloud
a. Hosted at service provider site.	a. Hosted at Enterprise or Service Provider site.
b. Supports connectivity over the Internet.	b. Supports connectivity over internet/private network(WAN)
c. Suitable for information not very sensitive.	c. Suitable for very sensitive information
d. Cheaper than Private cloud.	d. Costlier than the public cloud.
e. Utilises shared infrastrucure.	e. Doesn't utilise shared infrastructure.
f. Supports multiple customers.	f. Supports one customer.
g. Requires high-level of security	g. Requires medium-level security.
h. May use VLANs, access list, VRF file, MPLs to logic	
i. Eg: Open Nebula	i. Eg: Eucalyptus
image

CLOUD SERVICE MODEL
IaaS(Infrastructure as a Service)

PaaS(Platform as a Service)

SaaS(Software as a Service)



7. SERVICE MODELS

image

Elastic Beanstalk, Zoho cloud, Salesforce - software service provider.


AMAZON WEB SERVICES (AWS)

Offers 200 fully featured services

COMPUTE SERVICES

Elastic Compute Cloud (EC2) - manage scanning of both EC2 and ECS

Elastic Container Service (ECS) - provides containers

Lambda - Serverless - to make a database architecture serverless.


STORAGE SERVICES

Simple Storage Service (S3) - is an object storage which means it is already pre-formatted and doesn't allow formatting at a later stage. Storage is k/a buckets. can put necessary authentication, passwords, and authorization.

Elastic Block Store (EBS) - that storage which can be formatted at any point of time and is generally which are attached to an OS. Provides volume which can be attached to our EC@ instances.

Elastic File System (EFS) - is a shared file system which is used in BRDB solutions (multiple clients working on a single desk i.e. database.) can be used in logging instances. Provides seamless storage.

Archival Service - Glacier - AWS Glacier provides cheapest storage where data is not used regularly.

RAID 5(Redundant Array of Independent Disks) - data is sliced in 3 disks. 1disk - 1, 5,9,10 2disk - 2, 6,7 3disk - 3,4,8. If 1 disk is damaged, still it can be recovered. are done on hardware.


NETWORK SERVICES
Virtual Private Cloud (VPC) - Internal network.

Domain Name Service - Route 53

Direct Connect - Direct Connect(costliest service) is a service provided by AWS where they connect your data centre to AWS through a wired connection.


S3
S3
Object Storage with durability of 99.99999%, 11 9's
Infinitely scaling storage
Can keep files in buckets
S3 is a global service but buckets are created in specific regions
Globally unique bucket names.
Durability - 11 9's durability = if 1,00,00,000 objects are stored, avg incurred loss of a single object once every 10,000 years.

S3 standard has 99.99% availabilty = not available 53 minutes a year.

SECURITY

User based - IAM policies

Resource based

Bucket policies
Bucket ACLs
Object ACLs
Public vs Private accessible Buckets

Object versioning

State-of-the-art in transit and at-rest encryption

STORAGE CLASSES image


EC2

Most popular AWS offering
Infrastructure as a code service
Provides rented Virtual machines
EC2 uses EBS and instance store to store data
EC2 uses ELB to ditribute data
EC2 uses autoscaling for scaling purposes
Bootstrapping can be done using userdata scripts.
Instance store vs EBS |---|---| |a. Fastest storage.|| |b. Once shut, data is wiped off.||

EC2 Instance Type a. C-type instances - CPU intensive which provides more CPU b. M-type instances - General purpose instances which have balanced memory and CPU c. R-type instances - which has more RAM d. T-type instances

EC2

Security Groups- short workload, predictable pricing, pay by second

Reserved (1 and 3 years)

Reserved instances - a commitment to an account of usage, long workload, 1 and 3 years upfront commitment, can save up to 72% of billing.

Spot Instances - short workloads, cheap, can lose instances (less reliable)

Dedicated hosts - book an entire physical server, control instance placement, most expensive EC2, use case - BYOL, compliance or regulations.

Dedicated instances - no other customers will share your hardware.

ELASTIC LOAD BALANCERS (ELB)

Implementation of Horizontal Scaling
Required for High availability
Types of load balancers
Classic Load Balancer - Layer 4 and 7. works as a reverse proxy. Can do virtual hosting based on port number
Application Load Balancer - Layer 7. Certain things like virtual hosting based on path can only work in layer 7. Eg: Apache Web Server.
Network Load Balancer - Layer 4
AUTOSCALING

Self-healing Implementation for dynamic loads.
Can create and terminate instances automatically
Manual scaling: update the size of an ASG manually
Dynamic Scaling: Respond to changing demand
Simple/Step scaling
When a CloudWatch alarm is triggered (eg CPU>70%), then add 2 units
When a CloudWatch alarm is triggered (Eg CPU<30%), then remove 1
SIMPLE/STEP SCALING
To keep avg ASG CPU around 40% -Scheduled scaling
Anticipate a scaling based on known usage patterns
As scheduled patterns
Releases
No releases published
Packages
No packages published
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact
Skip to content
Sign up
KRIISHSHARMA
/
AWS
Public
 0 stars  1 fork  Activity
Code
Issues
Pull requests
KRIISHSHARMA/AWS
Latest commit
@KRIISHSHARMA
KRIISHSHARMA
…
last week
Git stats
Files
README.md
What is cloud computing
cloud computing is the delivery of computing services including servers,storage,databases,networking,software etc.
benfits
faster time to market
scalability and flexibility
cost savings
better collaboration
advanced security
data loss prevention
disadvantage
risk of vendor lock-in
less control over underlying cloud insfra
concerns about security risks like data privacy and online threats
integration complexity with exisiting systems
unforseen costs and unexpected expenses
Screenshot from 2023-11-26 11-13-28

Screenshot from 2023-11-26 11-14-43

example of private implementation softwares : openstack , opennebula
Hyperscalars : A hyperscaler is a type of large-scale data center that offers massive computing resources, typically in the form of an elastic cloud platform. Organizations use them to deploy and manage large-scale applications and services.
Screenshot from 2023-11-26 11-17-36

Screenshot from 2023-11-26 11-19-52

Compute services
EC2
ECS/EKS : containerized services `
Fargate
lambda : serverless
Storage Services
S3
EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) .
EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances
Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly returns request)
Network Services
VPC : own insolated environment in a public cloud
Domain Name Service - Route 53
Screenshot from 2023-11-26 17-59-50

public subnet : can receive traffic from outerworld
private subnet : cannot receive traffic from outerworld but may or may not send traffic to outerworld
Screenshot from 2023-11-26 18-03-33 Screenshot from 2023-11-26 18-05-39

Screenshot from 2023-11-26 13-40-57 Screenshot from 2023-11-26 13-46-08 Screenshot from 2023-11-26 13-47-33 Screenshot from 2023-11-26 13-57-52 Screenshot from 2023-11-26 13-59-20

Apache web server works on layer 7 , using single apache server one can deploy multiple applications on different ports based on paths (URLbased) (virtual hosts) . virtual hosting can only work on layer 7
Application based LB
key pair : kind of like a password (public key is username; private key is password)

PPK (PuTTY Private Key) and PEM (Privacy Enhanced Mail) are two file formats that are commonly used for SSH and SSL/TLS connections. While PPK files are primarily used with PuTTY on Windows, PEM files are more widely supported and can be used with various tools and platforms
security groups : A security group controls the traffic that is allowed to reach and leave the resources that it is associated with. For example, after you associate a security group with an EC2 instance, it controls the inbound and outbound traffic for the instance. When you create a VPC, it comes with a default security group. (acts as a firewall)

Screenshot from 2023-11-26 15-39-41 Screenshot from 2023-11-26 15-39-41 Screenshot from 2023-11-26 15-40-34 Screenshot from 2023-11-26 15-40-51

Creating a target group
Your load balancer routes requests to the targets in a target group and performs health checks on the targets.
LB routes traffic to target group then traffic group routes traffic to the back end ec2 instances or IP addresses etc
Screenshot from 2023-11-26 15-49-16 Screenshot from 2023-11-26 15-49-16 Screenshot from 2023-11-26 15-50-48

Screenshot from 2023-11-26 16-19-25 Screenshot from 2023-11-26 16-24-54

Autoscalling
Screenshot from 2023-11-26 16-44-57

Creating launch template
Screenshot from 2023-11-26 16-59-20 Screenshot from 2023-11-26 17-01-18 Screenshot from 2023-11-26 17-17-33 Screenshot from 2023-11-26 17-19-34

Screenshot from 2023-11-26 17-05-17 Screenshot from 2023-11-26 17-08-50 Screenshot from 2023-11-26 17-11-22 Uploading Screenshot from 2023-11-26 17-22-51.png…

Creating scalling policies
Screenshot from 2023-11-26 17-34-29 Screenshot from 2023-11-26 17-35-23

Artificial load
htop
Screenshot from 2023-11-26 17-39-48

currently 0

making instance count to a high number

seq 999999999999999999999 > /dev/null &
Screenshot from 2023-11-26 17-43-25

Screenshot from 2023-11-26 17-58-10 Screenshot from 2023-11-26 17-58-29 Screenshot from 2023-11-26 18-11-32

going to the DNS name and reloading will take you to diff targets(3)
this is round robin at work
AWS CLI : The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.
BOTO library in python
Screenshot from 2023-11-27 16-45-38 Screenshot from 2023-11-27 16-47-42

sudo snap install aws-cli
aws configure
Screenshot from 2023-11-27 17-08-27

in security credentials , before creating access key copy and paste PU , PrK and fill location and format in terminal
give user access
Screenshot from 2023-11-27 17-30-18

Screenshot from 2023-11-27 17-31-17 Screenshot from 2023-11-27 17-31-32

after creating instance
aws ec2 describe-instances
Screenshot from 2023-11-27 17-35-01 Screenshot from 2023-11-27 17-35-01 Screenshot from 2023-11-27 17-46-10 Screenshot from 2023-11-27 18-12-04 Screenshot from 2023-11-27 18-12-32 Screenshot from 2023-11-27 18-14-02 Screenshot from 2023-11-27 18-17-35 Screenshot from 2023-11-27 18-26-06

docker image to create art load
pods : Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers.
download

daemon sets : works on nodes where pods are running , can manage all your agents eg if we are runninf 5 ec2 instances behind the k8s cluster then we can run 1 daemon set and that daemon set wil take care of all the agents
CLOUD 9
cloud based IDE (vscode , pycharm etc)
provides IDE on browsers
Screenshot from 2023-12-02 16-01-33 Screenshot from 2023-12-02 16-12-26 Screenshot from 2023-12-02 16-12-51

after confiugring aws cli on cloud 9 (scroll up)
configure EKS ctl and kubectl link for installation
Screenshot from 2023-12-02 16-35-44 Screenshot from 2023-12-02 16-55-57 Screenshot from 2023-12-02 16-56-13 Screenshot from 2023-12-02 16-57-22

launching a cluster

eksctl create cluster --name test --version 1.28 --nodegroup-name ng.default --node-type t3.micro --nodes 2 --managed
Screenshot from 2023-12-02 17-05-19

yaml file for nginx container launched with official nginx image

   apiVersion: apps/v1
kind: Deployment
metadata:
    labels:
        environment: test
    name: test
spec:
    replicas: 1
    selector:
        matchLabels:
             environment: test
    template:
        metadata:
            labels:
                environment: test
        spec:
            containers:
            - image: nginx:1.16
              name: nginx
  nano nginx-deployment.yaml
kubectl is the thing using which we will be creating , launching the resources , creating pods , troubleshooting cluster using kubectl
we will apply this file using kubectl
  kubectl apply -f nginx-deployment.yaml
Screenshot from 2023-12-02 17-51-03

to see pods used by kubectl Screenshot from 2023-12-02 17-58-35

autoscaler used by eks Screenshot from 2023-12-02 18-00-51

can scale it Screenshot from 2023-12-02 18-03-17

install matrix server , will continue to moniter the cpu matrix ,without this will not show how much resources are utilised

kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
creating php-apache autoscaling yaml file for horizontal pod autoscaling
apiVersion: apps/v1
kind: Deployment
metadata:
  name: php-apache
spec:
  selector:
    matchLabels:
      run: php-apache
  template:
    metadata:
      labels:
        run: php-apache
    spec:
      containers:
      - name: php-apache
        image: registry.k8s.io/hpa-example
        ports:
        - containerPort: 80
        resources:
          limits:
            cpu: 500m
          requests:
            cpu: 200m
---
apiVersion: v1
kind: Service
metadata:
  name: php-apache
  labels:
    run: php-apache
spec:
  ports:
  - port: 80
  selector:
    run: php-apache
---

apiVersion: autoscaling/v1
kind: HorizontalPodAutoscaler
metadata:
  name: php-apache
  namespace: default
spec:
  scaleTargetRef:
     apiVersion: apps/v1
     kind: Deployment
     name: php-apache
  minReplicas: 1
  maxReplicas: 10
  targetCPUUtilizationPercentage: 50
nano hpa.yaml
deploying
kubectl apply -f hpa.yaml
Screenshot from 2023-12-02 18-46-22 Screenshot from 2023-12-02 19-07-14

artificial load

kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
creating a load balancer type service Screenshot from 2023-12-02 19-20-07

https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

creating nodeport service Screenshot from 2023-12-02 19-26-13 Screenshot from 2023-12-02 19-34-42

Screenshot from 2023-12-02 19-33-13

EKS
Screenshot from 2023-12-02 16-04-58 Screenshot from 2023-12-02 16-08-06

Releases
No releases published
Packages
No packages published
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact

Skip to content
Sign up
KRIISHSHARMA
/
AWS
Public
 0 stars  1 fork  Activity
Code
Issues
Pull requests
KRIISHSHARMA/AWS
Latest commit
@KRIISHSHARMA
KRIISHSHARMA
…
last week
Git stats
Files
README.md
What is cloud computing
cloud computing is the delivery of computing services including servers,storage,databases,networking,software etc.
benfits
faster time to market
scalability and flexibility
cost savings
better collaboration
advanced security
data loss prevention
disadvantage
risk of vendor lock-in
less control over underlying cloud insfra
concerns about security risks like data privacy and online threats
integration complexity with exisiting systems
unforseen costs and unexpected expenses
Screenshot from 2023-11-26 11-13-28

Screenshot from 2023-11-26 11-14-43

example of private implementation softwares : openstack , opennebula
Hyperscalars : A hyperscaler is a type of large-scale data center that offers massive computing resources, typically in the form of an elastic cloud platform. Organizations use them to deploy and manage large-scale applications and services.
Screenshot from 2023-11-26 11-17-36

Screenshot from 2023-11-26 11-19-52

Compute services
EC2
ECS/EKS : containerized services `
Fargate
lambda : serverless
Storage Services
S3
EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) .
EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances
Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly returns request)
Network Services
VPC : own insolated environment in a public cloud
Domain Name Service - Route 53
Screenshot from 2023-11-26 17-59-50

public subnet : can receive traffic from outerworld
private subnet : cannot receive traffic from outerworld but may or may not send traffic to outerworld
Screenshot from 2023-11-26 18-03-33 Screenshot from 2023-11-26 18-05-39

Screenshot from 2023-11-26 13-40-57 Screenshot from 2023-11-26 13-46-08 Screenshot from 2023-11-26 13-47-33 Screenshot from 2023-11-26 13-57-52 Screenshot from 2023-11-26 13-59-20

Apache web server works on layer 7 , using single apache server one can deploy multiple applications on different ports based on paths (URLbased) (virtual hosts) . virtual hosting can only work on layer 7
Application based LB
key pair : kind of like a password (public key is username; private key is password)

PPK (PuTTY Private Key) and PEM (Privacy Enhanced Mail) are two file formats that are commonly used for SSH and SSL/TLS connections. While PPK files are primarily used with PuTTY on Windows, PEM files are more widely supported and can be used with various tools and platforms
security groups : A security group controls the traffic that is allowed to reach and leave the resources that it is associated with. For example, after you associate a security group with an EC2 instance, it controls the inbound and outbound traffic for the instance. When you create a VPC, it comes with a default security group. (acts as a firewall)

Screenshot from 2023-11-26 15-39-41 Screenshot from 2023-11-26 15-39-41 Screenshot from 2023-11-26 15-40-34 Screenshot from 2023-11-26 15-40-51

Creating a target group
Your load balancer routes requests to the targets in a target group and performs health checks on the targets.
LB routes traffic to target group then traffic group routes traffic to the back end ec2 instances or IP addresses etc
Screenshot from 2023-11-26 15-49-16 Screenshot from 2023-11-26 15-49-16 Screenshot from 2023-11-26 15-50-48

Screenshot from 2023-11-26 16-19-25 Screenshot from 2023-11-26 16-24-54

Autoscalling
Screenshot from 2023-11-26 16-44-57

Creating launch template
Screenshot from 2023-11-26 16-59-20 Screenshot from 2023-11-26 17-01-18 Screenshot from 2023-11-26 17-17-33 Screenshot from 2023-11-26 17-19-34

Screenshot from 2023-11-26 17-05-17 Screenshot from 2023-11-26 17-08-50 Screenshot from 2023-11-26 17-11-22 Uploading Screenshot from 2023-11-26 17-22-51.png…

Creating scalling policies
Screenshot from 2023-11-26 17-34-29 Screenshot from 2023-11-26 17-35-23

Artificial load
htop
Screenshot from 2023-11-26 17-39-48

currently 0

making instance count to a high number

seq 999999999999999999999 > /dev/null &
Screenshot from 2023-11-26 17-43-25

Screenshot from 2023-11-26 17-58-10 Screenshot from 2023-11-26 17-58-29 Screenshot from 2023-11-26 18-11-32

going to the DNS name and reloading will take you to diff targets(3)
this is round robin at work
AWS CLI : The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.
BOTO library in python
Screenshot from 2023-11-27 16-45-38 Screenshot from 2023-11-27 16-47-42

sudo snap install aws-cli
aws configure
Screenshot from 2023-11-27 17-08-27

in security credentials , before creating access key copy and paste PU , PrK and fill location and format in terminal
give user access
Screenshot from 2023-11-27 17-30-18

Screenshot from 2023-11-27 17-31-17 Screenshot from 2023-11-27 17-31-32

after creating instance
aws ec2 describe-instances
Screenshot from 2023-11-27 17-35-01 Screenshot from 2023-11-27 17-35-01 Screenshot from 2023-11-27 17-46-10 Screenshot from 2023-11-27 18-12-04 Screenshot from 2023-11-27 18-12-32 Screenshot from 2023-11-27 18-14-02 Screenshot from 2023-11-27 18-17-35 Screenshot from 2023-11-27 18-26-06

docker image to create art load
pods : Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers.
download

daemon sets : works on nodes where pods are running , can manage all your agents eg if we are runninf 5 ec2 instances behind the k8s cluster then we can run 1 daemon set and that daemon set wil take care of all the agents
CLOUD 9
cloud based IDE (vscode , pycharm etc)
provides IDE on browsers
Screenshot from 2023-12-02 16-01-33 Screenshot from 2023-12-02 16-12-26 Screenshot from 2023-12-02 16-12-51

after confiugring aws cli on cloud 9 (scroll up)
configure EKS ctl and kubectl link for installation
Screenshot from 2023-12-02 16-35-44 Screenshot from 2023-12-02 16-55-57 Screenshot from 2023-12-02 16-56-13 Screenshot from 2023-12-02 16-57-22

launching a cluster

eksctl create cluster --name test --version 1.28 --nodegroup-name ng.default --node-type t3.micro --nodes 2 --managed
Screenshot from 2023-12-02 17-05-19

yaml file for nginx container launched with official nginx image

   apiVersion: apps/v1
kind: Deployment
metadata:
    labels:
        environment: test
    name: test
spec:
    replicas: 1
    selector:
        matchLabels:
             environment: test
    template:
        metadata:
            labels:
                environment: test
        spec:
            containers:
            - image: nginx:1.16
              name: nginx
  nano nginx-deployment.yaml
kubectl is the thing using which we will be creating , launching the resources , creating pods , troubleshooting cluster using kubectl
we will apply this file using kubectl
  kubectl apply -f nginx-deployment.yaml
Screenshot from 2023-12-02 17-51-03

to see pods used by kubectl Screenshot from 2023-12-02 17-58-35

autoscaler used by eks Screenshot from 2023-12-02 18-00-51

can scale it Screenshot from 2023-12-02 18-03-17

install matrix server , will continue to moniter the cpu matrix ,without this will not show how much resources are utilised

kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
creating php-apache autoscaling yaml file for horizontal pod autoscaling
apiVersion: apps/v1
kind: Deployment
metadata:
  name: php-apache
spec:
  selector:
    matchLabels:
      run: php-apache
  template:
    metadata:
      labels:
        run: php-apache
    spec:
      containers:
      - name: php-apache
        image: registry.k8s.io/hpa-example
        ports:
        - containerPort: 80
        resources:
          limits:
            cpu: 500m
          requests:
            cpu: 200m
---
apiVersion: v1
kind: Service
metadata:
  name: php-apache
  labels:
    run: php-apache
spec:
  ports:
  - port: 80
  selector:
    run: php-apache
---

apiVersion: autoscaling/v1
kind: HorizontalPodAutoscaler
metadata:
  name: php-apache
  namespace: default
spec:
  scaleTargetRef:
     apiVersion: apps/v1
     kind: Deployment
     name: php-apache
  minReplicas: 1
  maxReplicas: 10
  targetCPUUtilizationPercentage: 50
nano hpa.yaml
deploying
kubectl apply -f hpa.yaml
Screenshot from 2023-12-02 18-46-22 Screenshot from 2023-12-02 19-07-14

artificial load

kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
creating a load balancer type service Screenshot from 2023-12-02 19-20-07

https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

creating nodeport service Screenshot from 2023-12-02 19-26-13 Screenshot from 2023-12-02 19-34-42

Screenshot from 2023-12-02 19-33-13

EKS
Screenshot from 2023-12-02 16-04-58 Screenshot from 2023-12-02 16-08-06

Releases
No releases published
Packages
No packages published
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact
Manage cookiesDo not share my personal information
