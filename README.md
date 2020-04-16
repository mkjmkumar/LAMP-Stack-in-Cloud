# LAMP-Stack-in-Cloud
1. Requirement Overview
The acronym LAMP (Linux, Apache, MySQL, PHP) refers to an open source stack, used to run dynamic and static content of servers. A small startup organization uses the LAMP stack of software. Dynamic nature of demand and projected future growth in traffic drives the need for a massively scalable solution to enable the availability (and reliability) of its web-based application. This document is a representation of an enhanced solution using AWS cloud-based services. The proposed solution is to move into the AWS cloud can provide a much greater impetus to improve on the current state-of-the-art and reducing maintenance and move the infrastructure to a more secure and scalable environment. This solution does not include the events and streaming processing-based stack because that would require the leap to change the existing framework. Also, Analytics based on Big Data components are out of the scope. Therefore, the proposed solution in this document is an offer for a small team so that it can be managed seamlessly with less development effort.

1.1. Objective
Recommend a manageable, secure, scalable, high performance, efficient, elastic, highly available, fault-tolerant and recoverable architecture that allows the startup to organically grow. The architecture should specifically address the requirements/concerns as described below.

• Scaling

• Disaster Recovery planning

• Ability for Service Providers to send notifications to consumer 

• Ability to run analytics on top of collected data, with analytics they should be able to visualize & understand app data usage

• Their ability to configure their database and data access layer for high performance and throughput

• Effective distribution of load

• Security of data at rest and in transit 

• An archival strategy for inactive objects greater than 6 months

• Ability to easily manage and replicate multiple environments based on their blueprint architecture

1.1. Processes Overview
Below is the short diagram of the interaction between the components of LAMP architecture. The proposed cloud solution will focus on the interaction between servers, virtual machine and client web browser via the network and data flow showcase using AWS services.

No alt text provided for this image
1.2. Quality goals
Moving to AWS cloud could bring scalability (Horizontal and vertical), elasticity based on consumer demand, efficiency, security, simplicity, on-demand network access to a shared pool, ease-of-use, ease-of-deployment.

2. Architecture Constraints
Explanation on hardware and infrastructure decisions (for example, size of EC2 and version/choice of programming language) is not shown in this architecture diagram.

3. Proposed Architecture
3.1 Logical Architecture
No alt text provided for this image
3.2. Solution Strategy and Building Blocks
A short summary and explanation of the fundamental decisions and solution strategies that shape the system’s architecture.

a. Scalability and High Availability is achieved using Elastic Load Balancer (ELB) and Elastic Compute Cloud (EC2). Any compute resource server can easily be added or removed based upon increase or decrease in the demand from the consumer.

b. Disaster recovery can be addressed by choosing different availability zones for any EC2 and database resource. Along with that multiple replica’s volume (EBS) attached to database servers.
