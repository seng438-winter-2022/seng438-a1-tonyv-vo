>   **SENG 438 - Software Testing, Reliability, and Quality**

**Lab. Report \#1 – Introduction to Testing and Defect Tracking**

| Group \#:       | G38  |
|-----------------|---|
| Student Names:  |   |
|     Tony Vo            |   |
|     Chace Nielson            |   |
|     Chad Holst            |   |
|     Olisehemeka Chukwuma            |   |

**Table of Contents**

[1 Introduction	1](#_Toc439194677)

[2 High-level description of the exploratory testing plan	1](#_Toc439194678)

[3 Comparison of exploratory and manual functional testing	1](#_Toc439194679)

[4 Notes and discussion of the peer reviews of defect reports	1](#_Toc439194680)

[5 How the pair testing was managed and team work/effort was
divided	1](#_Toc439194681)

[6 Difficulties encountered, challenges overcome, and lessons
learned	1](#_Toc439194682)

[7 Comments/feedback on the lab and lab document itself	1](#_Toc439194683)

# Introduction
In this assignment, we were given two versions of an ATM system. The first program, version 1.0, was a primitive, first-release version of the system. The second program, version 1.1, was an updated version, which strived to solve some of the bugs found in the first version of the program. 

This lab presented three different kinds of software testing: exploratory testing, manual functional testing and regression testing. The first two testing methods were done on version 1.0, while the last testing method was done on version 1.1. The tests were performed as follows:

- In exploratory testing, a general plan was developed and the group was split into two teams, composed of two people each. Each team was assigned a general functionality of the program to extensively test. The exploratory tests were performed by exploring the program and trying its many functionalities. A bug was recorded if a team member saw that the outcome was not a result that they had expected. The plan was very general and limited to the sections a group member should test to avoid as much overlap as possible.The testing was also conducted individually to allow more bugs to be found and reported. This provided more opportunities for testing functionalities.
- In manual functionality testing, a test suite containing all of the ATM system’s functionality, including the initial system state, input, and expected outcome were given. A bug was recorded if the output did not meet the expected outcome from the test case as the actual outcome differentiated from the expected outcome. Each team member took on 10 test cases from the test suite to evenly divide the work. 
- In regression testing, version 1.1 of the ATM system was tested using the same method done in the manual functional testing. Existing bugs were either marked as “resolved” if they did not appear again or “in-progress” if the bug was still present in the newer version. 

Before this assignment, none of the group members knew much about exploratory and manual testing. One group member stated that he knew that exploratory testing involved testing the program without a plan or having a list of the full functionalities and the expected outputs. Prior to this class, all of our testing experience was through scripted testing that was done with JUnit 4 for Java programs in the course ENSF 409.

# High-level description of the exploratory testing plan
For us to effectively reveal as many defects of the ATM system as possible, our group initially set up pair testing with the groups being Tony and Chad and the second group being Chace and Oliseh. The teams split up general functionalities to test and had one member record while the other member used the application to look for issues. After spending some time working in pairs we decided that it would also be beneficial to spend time exploring the application individually in our own time. We decided to assign each individual a main functionality. Through having each individual perform more exploratory tests on specific functionality, we became familiar with our assigned function. This also allowed us to use our time effectively and creatively. The following is the general idea of how we assigned each functionality to each individual. While we stuck to these assignments for the most part we were also able to expand our search to other functionalities if it felt necessary.

- Tony: Deposits
- Chad: Withdrawal
- Chace: Transaction 
- Oliseh: Transfer 

We each decided to cover a function extensively as our goal was to become experts of the function of our domain. Considering exploratory testing is not systematic, we decided that having our specific domain would optimize the exploratory testing process.

Furthermore, we decided to enter varying amounts of money to test the ATM functions. These amounts included an amount under $1, values between $1 and $9, values between $10 and $99, $100, and $1000. As such, this allowed us to test both common paths and abnormal paths that may be taken by a customer. We found some values were treated differently by the system and therefore it made sense to report them as individual issues.

# Comparison of exploratory and manual functional testing
Although freedom can allow for finding bugs that may not be found using a structured form of testing; exploratory testing can have repercussions for providing too much freedom. This can affect the efficiency of exploratory testing. We noticed that it is possible to perform the same test and consider it a different test while performing exploratory testing. This increased time spent on each test. For example, our member responsible for the withdrawal functionality had selected each multiple of $20 to test the withdrawal output; through testing each value, our member had thought that each value would be considered a different test as the withdrawal output is different for each selection. Conversely, following the manual scripted testing, the member realized that the test suite considered all $20 multiple options as a single test. It follows that manual testing provides a more structured form of testing and reduces the chance of deviation which decreases efficiency. Conclusively, we trade the freedom of using exploratory for the efficiency of manual functional testing.

In addition, manual functional testing provided us with the expected outcome, but exploratory testing, by its definition, did not have any detailed plan or expected outcomes. Therefore, manual functional testing was easier to coordinate since it was easy to assign a range of test cases to each team member, while in exploratory testing, there was more uncertainty in the inputs and outputs used for each test.

# Notes and discussion of the peer reviews of defect reports
During the peer review process, we noticed that due to our extensive exploratory testing plans, both groups did not report any new bugs that were found during the manual. Many bugs reported on Backlog were duplicated. Through peer review, we were able to find each other's duplicates but also had issues defining what should be considered a duplicate as we could not examine the underlying code.

# How the pair testing was managed and team work/effort was divided 
Pair testing was used for the exploratory testing. To do this, we divided into groups of 2 as follows:

- Tony and Chad
- Olisehemeka and Chace

During the exploratory testing, we had one person testing the ATM system’s functionalities while the other person watched and recorded the bugs onto Backlog. However, we decided to move to testing the test cases by ourselves in the manual functional testing and regression testing to speed up the testing process. Afterwards, we communicated our progress to each other and reported any similar test cases to prevent redundant issues in Backlog. Through this method, the teamwork and effort were evenly divided amongst all four group members.

# Difficulties encountered, challenges overcome, and lessons learned
Making pair testing time-efficient was the main difficulty of the lab. Part of the problem stemmed from this being the first time our group used Backlog and pair testing to report bugs. We found that as we performed the exploratory tests, the member responsible for recording was inactive for long stretches while the other member looked for bugs. The member testing the application also became inactive while the other member reported the bug in Backlog. However, part of this problem was our inexperience using Backlog and with testing in general. While it provided difficulty at first, it provided a learning opportunity to split up work the way we felt would benefit our group.

The lab did have its fair share of challenges for us to work on. For instance, our first challenge was to set up an account on Backlog and grant all members access. There was an issue with setting up the unique IDs of the account. We believe this occurred because many groups were using the specific names we were trying to use. After we created an account, we were able to grant all members of the group access to the project after some trial and error with settings granting each other access. Many of these issues can be attributed to our group being new to Backlog and testing. As we progressed through all the tests we became much more competent at using the system.

Another issue we faced was learning about the need for communication when performing the exploratory testing. We had a few instances where the same bug was reported twice either by a pair or an individual. Once we realized this, we spent more time checking previously reported bugs. We also realized that it was still better to have the bug reported, even if we had a similar bug reported elsewhere, but we still made our best efforts to avoid redundancy.

Another challenge was deciding if similar bugs found in different functionalities were the same or different. This was more purposeful reporting of the same bug found in a different section of the application. For instance, the card number was wrong when you accessed different functionalities throughout the application. We reported these similar bugs within different functionalities to give the full range of where that bug persisted.

Using the Backlog platform to store the issues was a learning experience in understanding team bug reporting, the depth that issues need to be reported, and how bugs can be organized in a professional workplace. Seeing how Backlog worked  allowed our team to report bugs so they are visible to other members. It was a great learning experience to understand this system. It also became apparent that the level of detail in explaining issues had great significance. If there isn’t enough information the issue might be hard for others to understand and replicate and therefore harder to resolve. It was also interesting to get used to working in a group while combining individual testing and using pair testing to understand all the possible issues with the system. The lab enabled us to get a taste for industry and the ideas associated with testing.	

# Comments/feedback on the lab and lab document itself
When we started pair testing for the first time, it felt a bit slow as the person recording would often be watching and not recording anything until a bug was found. While it did feel a bit like one person was wasting time, it also helped with being thorough and having multiple sets of eyes watch the process. If the lab session had discussed the best way to go about pair testing that would have been very helpful for our group to be time-efficient. However, it was still an interesting learning experience to figure out the best way to work together and work on our group unity.

The lab document held a lot of information and while we found most of it useful, It may have been beneficial to have the intro assignment a bit more condensed. It was a bit difficult to follow along with all the new material introduced in the lab.

Overall, this was an enjoyable lab experience and felt more tied to the industry than most labs and assignments. It provided a good look at the testing process and the teamwork that will be essential in the industry. We found the lab informative, well organized, and a good way to develop real-world skills. The various types of testing all had pros and cons and showed clearly what benefits they each have in group environments.
