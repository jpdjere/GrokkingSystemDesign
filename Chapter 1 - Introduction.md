# Introduction to Modern System Design

## What is system design?

**System design** is the process of defining components and their integrations, APIs, and data models to build large-scale systems that meet a specified set of functional and non-functional requirements.

System design uses the concepts of **computer networking**, **parallel computing**, and **distributed systems** to craft systems that scale well and are performant. 

![](2024-07-24-09-03-17.png)

Distributed systems scale well by nature. However, they are inherently complex. And the discipline of system design helps tame this complexity and get the work done.

System design aims to build systems that are reliable, effecitve and maintainable, among other characteristics:

- **Reliable systems** handle faults, failures and errors.
- **Effective systems** meet all user needs and business requirements.
- **Maintainable systems** are flexible and easy to scale up or down. The ability to add new features also comes under the umbrella of maintainability.

## Modern system design using building blocks

We have separated out commonly-used design elements, such as load balancers, as the basic building blocks for high-level system design. This serves two puposes:

1. It allows us to discuss the builduing blocks in detail, and discuss their intersting mini-design problems.
2. When we tacke a design problem, we can concentrate on problem-specific aspects, mention the building block we'll use and how we'll use it. This helps us remove duplicate discussions of commonly-occurring design elements.

We have identified 16 builduing blocks that are crucial in designing modern systems.

![](2024-07-24-09-03-02.png)

## About this course

This coruse is about designing systems that scale with increasing users, remain available under different faults, and meet functional goals with good performance. Real-world system building is an iterative process where we start with a reasonably good design, measure how it performs, and improve the design in the next iteration.

The focus of this course is to immerse ourselves into carefully-selected system design endeavors to enable ourselves to tackle any novel design problem; be it in a system design interview or a task at the office. This course aims to teach concepts instead of giving out boilerplate designs. Some gaps that this course fills are:

- **A fresh look at system design:** Many system design courses provide a formula to attack a specific problem. While this might seems attractive in a high-stress situation like an interview, it might encourage memorizing a design solution instead of actually understanding the problem and devising an appropriate solution. That why we aim to attack a design problem from the first principles, which gives a fresh feel to it.

- **Going deep and broad:** We tackle some traditional problems, but with added in-depth discussions on them. We give proper rationale for why use some components despite their trade-offs. For example, we explain why we use a particular database, a cacheing system or a load balancing techinque in a design.
  
  We adress some new design problem as well that touch upon not only only scalability but also availability, maintainability, consistency and fault-tolerance. Collectively, traditional and new problems cover all aspects of modern system design activity.

- **Iterative process:** Systems, in reality, improve over iterations. We often start with something simple, but when bottlenecks arise in one or mor of the system's parts, a new design becomes necessary. In some design problems, we make one design, identify bottleneces, and improve on it. Working under time constraints might not permit iterations on the designs. However, we still recommend two iterations - first, where do we our best to come up with a design (that takes about 80% of the available time), and a second iteration for improvements. Another choice is to change things as we figure out new insights. Inevitably, we discover new details as we spend more time working with a problem.

- **Interactive learning:** We provide ample opportunities to get experience with system design. Some design problems guide learners through many steps to design a system. We also have a few exaples where the learner designs the full system end-to-end without any guided steps. We reinforce the important concepts by testing learners with questions and quizzes.

## Who should take this course?

System design is for any software engineer who wants to advance in their career:

- **Interview preparation:** Lately, system design is becoming an important part of software development interviews. This course helps software engineers prepare for interviews. We have an elaborate guide on preparation for a system design interview in the second chapter of this course for learners who are interested.

- **Sofware developers**: System design is primarily for back-end developers who aim to become principal engineers or solution architects. It's because these engineers handle actual user data. Once the data is submitted to back-end systems by the frontend, effective handling of data makes the overall application successful. However, full stack or front-end developers may also want to learn SD to improve their work. Also, support engineers, also called SREs, who work on-call in the production environment have to deal with all sorts of problems daily. SD concepts enable SREs to efficiently find the root causes for complex problems.

- ****