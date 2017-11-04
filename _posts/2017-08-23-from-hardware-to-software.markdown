---
layout: post
title:  "From Silicon to Bits"
date:   2017-09-15 22:56:48 -0700
categories: blog  
---

About eight months ago, I made a career transition from semiconductor industry to online advertising tech industry. 

There are many reasons behind my change, one of which is that I just wanted to get out of my comfort zone.

Having been in the semiconductor instustry for 10 years (15 years if counting my Ph.D. research years), I feel I already got pretty much the big picture of how a chip is created from thiry thousand feet high, although devils are always in the detail in each stage of the flow.

Now I am working as a software engineer in the machine learning modeling team at an online advertising technology company (Quantcast) and there are tons of new things to learn.

First thing is BIG DATA. I know it's a buzz word now from Silicon Valley to Zhongguan Cun in Beijing. But Quantcast does get an ocean of user data from its analytic tools deployed on over 300 million websites across the world. The second thing is machine learning. I have been very interested in this field for years and took several online classes at Coursera. However, working on course project (even Kaggle projects) are very different from working on real-problems in industry. At Quantcast, the challenge in machine learning is not only limited in improving performance (accuracy, auroc, aupr), but also how to deploy the model and how to apply the model in its real-time bidding system. It is a very exciting experience working on both machine learning and real-time bidding systems, two hardest problems at the same time. Third thing is open source. Semiconductor industry is about secrecy. Some of the famous semiconductor companies do not even allow their employees to talk about their work to colleagues across team in the same company. The software engineers in semiconductor industry has no access to or practice in open source software development community. At Quantcast, even our distributed system (QFS) is free on github. And most of the tools we are developing upon is based on open source license. It is much more fulfilling (and more self disciplined) when you write code not only for your team/corporation but a wild world in the Internet.

Having mentioned the major differences between semiconductor industry and internet software industry, I also want to stree that there are surprising similarity between these two seemly different industries.

1) Process. If you are from a pure software background and never worked in hardware, you should probably get rid of your mindset that hardware designers are plugging wires into circuit boards. No more! Since 30 years ago the main task of hardware (chip) engineers are writing code using a hardware description language called Verilog (another popular option is VHDL). This language is also module based very much like C++/Java. There are compilers, called electronic design automation software, that translate and optimize the hardware language into binary files (called GDSII). And manufacturors can fabricate CMOS chips based on these GDSII files. (I am greatly simplifying the process here, which involves many iterations of optimization and verification) 

2) Serverless vs Fabless. It has been a trend in internet software industry to go serverless. Basically, software startups no longer need to host their services on their own servers, instead they can pay the server maitainance and operation fees to cloud server vendors such as Amazon AWS, Google Cloud, Microsoft Azzure etc. A similar trend had been going on in semiconductor industry 20 years ago, when small semicondutor startups only focus on chip design (i.e. writing Verilog code) and leave the manufacturing to semicondutor foundries such as TSMC, Samsung, Global Foundry etc.

3) Deployment vs Tapeout. Deployment is the process of putting what engineers developed, be a new feature or bug fix, into product that consumers can access directly. The process often includes testing, stating and release. This process is called "tapeout" in semiconductor industry with similar process but longer cycles.

4) Big data. Although not in the same scale, the data processing in semiconductor is also quite huge too in the deep submicron technology. In a small chip, there can often be over one billion components and how to partition and process them efficiently is a major challange in the electronic design automation software (the hardware compiler). Similar approaches such as hierarchical design flow are used in both industries are adopted to tackle this data processing challange.

5) Machine learning. This is the place where two industries differ a lot. In semiconductor industries, no real machine learning technique has been applied in real applications. One of the main reasons is the secrecy of this industry that caused no one wants to release their data and withough sufficient training data no good machine learning models can be trained. I have seen companies in semicondutor industries try to apply machine learning techniques, however, the outcome really depends on how open this industry is going to or willing to be.

