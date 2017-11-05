---
layout: post
title:  "From Silicon to Bits"
date:   2017-09-15 22:56:48 -0700
categories: blog  
---

About eight months ago, I made a career transition from semiconductor industry to internet advertising industry. 

There are many reasons behind my change, one of which is that I just wanted to get out of my comfort zone and explore new things in my life.

Having been in the semiconductor industry for over 10 years (15 years if counting my days as a Ph.D. student), working in both front-end (logic synthesis) and back-end (place & route), I think I've already understood the overall process of how a VLSI chip is created from design to implementation, although as many technologies devils are still hiding in the detail.

On the other hand, I feel there is a wild world out there especially in the big data and artificial intelligence area where companies and research results are booming in recent years.

As a result, I am attracted to Quantcast, an online advertising tech company with cornucopia of user data and state of the art machine learning models to learn and extract patterns from these user data. At Quantcast, I feel excited and very lucky to work with so many brilliant colleagues.  And there are new things to learn almost every day.

First thing is BIG DATA. I know it's a buzz word now from Silicon Valley to Zhongguan Cun in Beijing. But Quantcast does get an ocean of user data from its analytic tools deployed on over 300 million websites across the world. The second thing is machine learning. I have been very interested in this field for years and took several online classes at Coursera. However, working on course project (even Kaggle projects) are very different from working on real world problems. At Quantcast, the challenge in machine learning is not only limited in improving performance (accuracy, auroc, aupr), but also how to deploy the model and how to apply the models in its real-time bidding system. It is a very challenging job working on both machine learning and real-time bidding systems, two hard problems at the same time. Third thing is open source. Semiconductor industry is about secrecy. Some of the famous semiconductor companies do not even allow their employees to talk about their work to colleagues across team in the same company. The software engineers in semiconductor industry have limited involvement in open source software development community. At Quantcast, even our distributed system (QFS) is free on Github. And most of the tools we are developing upon is based on open source license. It is much more fulfilling (and more self disciplined) when you write code not only for your team/company but for a school of peer developers and users.

Having mentioned the major differences between semiconductor industry and internet software industry, I also found that there are a few surprising similarities between these two seemly different industries.

First of all, if you are from a pure software background, never worked in hardware and picture hardware engineers plugging wires on circuits board in daily job, I need to explain a little background of hardware (chip design) engineers' daily job. Since 30 years ago the main task of hardware (chip) engineers are writing code using a hardware description language called Verilog (another popular language option is VHDL). This language is also module based very much like C++/Java. There are compilers, called electronic design automation software, that translate and optimize the hardware language into binary files (called GDSII). And manufacturers can fabricate CMOS chips based on these GDSII files. (I am greatly simplifying the process here, which involves many iterations of optimization and verification) 

1) Front-end and Back-end: Just like in internet software stack, there are also front-end and back-end in semiconductor design. The front-end is usually referring to logic synthesis which is the process of compiling the Verilog language into a logic netlist composed by gates such as NAND and NOR etc. The back-end usually includes placement and routing which is the map the logic gates onto a physical die with accurate physical location and geometry.

2) Serverless vs Fabless: It has been a trend in internet software industry to go serverless. Basically, software startups no longer need to host their services on their own servers, instead they can pay the server maitainance and operation fees to cloud server vendors such as Amazon AWS, Google Cloud, Microsoft Azzure etc. A similar trend had been going on in semiconductor industry 20 years ago, when small semicondutor startups only focus on chip design (i.e. writing Verilog code) and leave the manufacturing to semicondutor foundries such as TSMC, Samsung, Global Foundry etc.

3) Deployment vs Tapeout. Deployment is the process of putting what engineers developed, be a new feature or bug fix, into product that consumers can access directly. The process often includes testing, stating and release. This process is called "tapeout" in semiconductor industry with similar process but longer cycles.

4) Big data vs Moore's Law: Thanks to Moore's Law, the amount of data in designing a semiconductor chip is already as huge as the data in some Internet companies, although the data types are very different. For example, there can often be over one billion gates placed in a small chip, the connections between these gates are in the square order of the number of gates, the physical and electric properties in each gate need to be modeled with relative accuracy. Therefore storing and processing these information in a single chip is a challenging task. Similar approaches such as hierarchical design flow and clustering are used in both industries to tackle this big data problem.

5) Machine learning. This is the place where two industries differ a lot. In semiconductor industries, no real machine learning technique has been applied in real applications. One of the main reasons is the secrecy of this industry that caused no one wants to release their data and withough sufficient training data no good machine learning models can be trained. I have seen companies in semicondutor industries try to apply machine learning techniques, however, the outcome really depends on how open this industry is going to or willing to be.

