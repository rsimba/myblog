---
  2 layout: "post"
  3 title: "Introduction to DevOps"
  4 date: "2021-03-11 5:57"
  5 categories: DevOps
---
By definition, DevOps is a software development approach and culture based on **Lean** and **Agile** principles in which different departments that are part of software delivery process collaborate to accelerate the business. In summary, DevOps comes down to the culture, the tools, the practices, that you use to get code into production fast.

Althought its mainly adopted by the IT industry, DevOps has its fundamental ideas inspired by different practices (such as **Lean**, **TINA-C**, and **Agile**) and industries (such as **Manufacturing**). In order to understand the  basics of DevOps and its origins, its important to define some terms and processes that are part of the overal DevOps methodology.

## Software Development and Delivery
Just like in any other industry, IT companies have different goods and services available to their consumers, a good can be, for example, an application software, and service can be a connectivity or a support service.

Technology today is primarily consumed via application software, and we see that the biggest and more profitable companies are based in technology and most of them have have a complete business models based on software. However, how different companies build software? First there is there is a Development team, they design an application and write code to specify a product actions; then Quality Ensurance team review code to make sure the application work as intended; then there is an operation IT team which consists of release engineer and database server or network administrators, they setup the network, push code to a product serve, take care of security and monitor performance - they make the product available to end users and it must work well.

In order for a considerably amount of customers to consume a software service, companies need a way to ship it in large scale and this is where a delivery system, called **software supply chain**, is needed. When developing and delivering an application software to the end customers, there are a chain of processes and moving parts that are crucial for the success of the all process. It all starts with the customer requirements for an application and ends with the delivery and maintenance of it.

From the project management point of view, different methods were created to guide companies when developing and deliverying application softwares. The most known been the **Software Development Life Cycle** (SDLC) and **System Development Methodology** (SDM).


### Software Development  Life Cycle (SDLC)
An application software can be as simple as five lines of code, asking a user to type something on the keyboard and return an output or a full blown application with thousands of lines of code. The process of developing and delivering an application software can be complex, time consuming, and costly. To avoid these mentioned challenges and solve some of the problems involved during the software development and delivery process, a standard project management framework, called **Software Development Life Cycle** (SDLC), was developed by the industry with the goal to help guide companies or developers to develop software with the lowest cost and highest quality in the shortest time possible.

SDLC is a sequential model that devides software developemtn into different phases. Each phase is designed for performing specific activity during SDLC phase.

SDLC, describes a step-by-step process through which an application software goes through from the inception to retirement, which helps an organization to develop software in a well-structured way and maintain the quality, while carrying out testing and validation of the user specifications, before putting the software into a live environment. In general, SDLC offers seven well defined steps or phases for software developement and delivery:
1. Planning 
2. Requirement gathering and analysis
3. Design
4. Implementation, or coding
5. Testing
6. Deployment / release
7. Maintenance

The steps above helps us understand how a software is conceptualized, developed, and maintained. It all starts with a customer who has the business idea for a specific application and once he finds a company that will help him develop his idea. In the company side, the customer first point of contact is a **Product Owner** also known as Project Manager and they are going to discuss terms of their agreement, sign a deal and accept the project.

The first phase planning the requirements. Together the customer and product owner will outline the requirements of the application. Once the requirements have been taken, the next phase is requirement analysis where the involved team (operations, developers, product owners, and testers) all meet up and define each outlined requirments and give more planning details. Once all the requirements are analyzed by the team and defined, the product owner will take all the defined requirements and create tickets in the project management system. This is where stockholders, business team, program managers, technical leads, everybody sit together and plan on what needs to be build (the scope of the application and the milestone by which the software should be ready).

Next step is the design phase where the product will be planned according to the requirements. This is where the architect and technical team get involved, they participate in deciding the architecture of the solution.

Next phase is the implementation and coding where the operation team will set up the hardware for the servers where developers will start writing the code while the design continue planning the user interface and tests will anylize the requirements and start to build test cases for the test plans.

Next is testing phase where testers start test and executing test cases from the test plan created before, validate that all the requirements have been met, make sure that all the functionality works as expected, find many bugs as possibly can.

Next is the deployment phase where the operation team will end up mirroring the development enviroment system that test have been done and get them ready for production. Once all these tasks are completed, the application will go live to all users.

The final phase is maintenance the servers and environment are maintained and making sure that the amount of load doesnt bring down the servers. This is also where bugs can be found and reported, and based to these reports, bugs are discovered, fixed and do another deployment to production. Once in the maintenance phase, new features will come through, new requirements will come through and we start the all process again and be able to get new stuff out into the existing application.

### System Developement Methodology (SDM)
SDM is a formalized approach to implementing the SDLC (a series of steps to perform and deliverables to produce). At which order the seven steps will be performed, the frequency and duration of these steps 

SDM are different methologies used to manage the different phases of SDLC, in another words, how the different seven (7) phases of the SDLC are performed. There are several SDM methodologies and the common ones been:
- **Waterfall**: It was built on step at the time, only when a step is thorougly completed that that a project team will go on to the next step. This makes Waterfall a sequential method by nature.
- **Agile**: In this steps there are different cycles that are similar to the steps in the SDLC cycle and each cycle is doing the same steps again and again. In agile, they don't believe in developing a software sequentially like in waterfall model, they feel that developing small portion of the application through several itration and when more frequent demostrate to the stockholders, there are better chances of building a higher quality software. In this method, a business analyst and a stockholder identifies one or more features that are required for the application as part of the **discovery** step; then these features are **designed** by the technical team and **developed**, and then **tested**. After all this process, its then show case to the stockholders and if they like it, you then enter the next cycle which is pretty much a similar one but for another new feature. In every cycle, you are incremently building small chunk of software and at every stage you are validating the correctness of the software based build from the stockholders thus miniziming the chances of going wrong
- **DevOps**.

With the waterfall method, the customer feedback is not taken until all the life cycles are finished which could have taken months or a years and all this time would be wasted because the client did not approve it.

With Agile, since the customer is able to give feedback in the end of each cycle, only one cycle might be wasted (the team effor spent in that single cycle or maybe days or weeks). The customer feedback is taken and incorpotated in the next cycle, and this is the power of agile comparing to waterfall. 

## DevOps
DevOps is a hybrid methodology bring the goods of Waterfall and Agile. Usually the project teams build certain features and when they see that a good quality of amount of software is ready for deployment, thats when they to the production and release the software for use. DevOps believes in time to market and don't believe in waiting for a product to be ready for deployment. With DevOps, at the end of the test phase, they immediatelly decide to package the software and release it to the environment and start operating and monitoring. This is usually seem in a very competitive environment, they have not time waste and no time to wait. DevOps is similar to agile except for the difference been they release at the end of every cycle through a strategy called continuous integration and continuous delivery. 

### How DevOps Works
DevOps works based on the adoption (by **people**, **process**, and **technology**) of several **principles**, **practices**, and **tools**. 

#### Principles
DevOps is first and foremost a cultural movement meaning that people play a key role in adopting DevOps before any process or tool. In order to build a DevOps culture, a set of principles centered on collaboration across roles have been developed.

The DevOps movement is still developing its culture and its cire values can be simplified using the CAMS acronym, which stands for **Culture**, **Automation**, **Measurement**, and **Sharing**.
- **Culture**: The primary critical success factor is to build a collaboration and respectful culture across entire IT organization. If there is no culture, all automation atempts will be fruitless.
- **Automation**: After understanding the culture in an organization, the tools should be in place to initiate automatin process for DevOps. Tools for release management, provisioning, configuration management, systems integration, monitoring and control, and virtualization are the important aspects in building a DevOps culture.
- **Measurement**: "If yo can't measure, you can't improve". A successful DevOps implementation should measure eveyrything possible as often as it can, performance metrics, process metrics, and even people metrics. Some populat tools include Collected, Nagios, Ganglia, Splunk, and Tcollector.
- **Sharing**: Sharing is the loop-back in the CAMS cycle. Creatig a culture where people share ideas and problems is critical. Another interesting motivation in the DevOps movement is the way sharing DevOps success stores helps others.

#### Practices 
DevOps practices are a set of pratical ideas of its principles implementations and they are usually resumed as the following:
- **Continuous Integration**: Is a practice where developers regularly merge their code changes into a central repository, after which automated builds and tests are rung. The key goals of CI are to find and address bugs quicker, improve software quality, and reduce the time it yakes to validate and release new software updates.
- **Continuous Delivery**: It is a practice where code changes are automatically builtm tested, and prepared for a release to production. It expands upon continuous integration by deployong all code changes to a testing environment and/or a production environment after the build stage.
- **Microservices**: It is a design approach to build a single applciaiton as a set of small services. Each service runs in its own process and communicates with other services through a well-defined interface using a lightweight mechanism, typically an HTTP-based API.
- **Infrastructure as Code**: It is a practice in which infrastructure is provisioned and managed using code and software development techniques, such as version control and continuous integration. Engineers can interface with infrastructure with infrastructure using code-based tools and treat infrastructure in a manner similar to how they treat application code.
    - **Configuration Management**: Developers and system admins use code to automate oeprating system and host configuration, operational tasks, and more. The use of code makes configuration changes repeatable and standardized. It frees developers and sysadmins from manually configuring operating systems, system applicaitons, or server software.
    - **Policy as code**: With infrastructure and its configuration codified with the cloud, organizations can monitor and enforce compliance dynamically and at scale
- **Monitoring and Logging**: Organizations monitor metrics and logs to see how application and infrastructure performance impacts the experience of their product's end user. By capturingm, categorizing, and then analyzing data and logs generated by applicaiotns and infrastructure, organizations understand how changes or updates impact users, sheeding insights into the root causes of problems or unexpected changes.
- **Communication and Collaboration**: Increased communication and collaboration in an organization is one of the key cultura aspects of DevOps. The use of DevOps tooling and automation of the software delivery process establishes collaboration by phsycally bringing together the workflows and responsabilities of development and operations.

### Tools
Several tools are available to facilitate the DevOps workflow and its practical implementation. These tools are usually categorized based on the specific DevOps practice:
- Configuration management: 
    - Ansible
    - Chef
    - Puppet
- CI/CD:
    - Jenkins
    - GitLab CI
- Containerization and orchestration: 
    - Docker 
    - OpenShift 
    - Kubernetes
- Monitoring and alerting: 
    - Nagios 
    - Prometheus

# Summary


