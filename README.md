# Kenon Sahirani -  Data & AI Journey
 
*Learning Journal Entry #1 Week 1, Day 1 Uplift Code Camp, Python for Data and AI*
 
## Part 1: Core Reflection

### 1. Introduce yourself. Who are you, and what should classmates/future readers know about you?

Answer: I'm Kenon Sahirani. Before this bootcamp I was building applications with Java and Spring
Boot, and doing full-stack work with the MERN stack (I built a project called The Coloring
Bliss, including a PayMongo payment integration). I've also done freelance work where I saw
firsthand how operations teams are starting to lean on AI for things like sales reporting
which is part of what pulled me toward this field.

### 2. Why did you join the bootcamp? What brought you here, specifically?

Answer: During freelance work, I watched the operations team start using AI to generate sales reports work that used to take people hours was suddenly automated in minutes. That was the moment it clicked that this shift isn't coming, it's already here, and I didn't want to be someone who has to catch up to it later. Coming from a Java/Spring Boot and MERN background, I already knew how to build software; I joined this bootcamp specifically to add the data and AI layer on top of that so I'm not just building applications, but building the intelligent parts of them too.

### 3. Which Data or AI application interests you the most, and why?

Answer: What interests me most is recommendation engines and demand forecasting in retail I built an e-commerce app (The Coloring Bliss) with a payment integration, so I already know what it's like to watch real transactions flow through a system. What I couldn't do at the time was use that transaction data to actually predict anything which products to restock, which customers were likely to buy again. Seeing that gap in my own project is what makes this application concrete to me rather than abstract.

### 4. What do you hope to build by the end of the 20 weeks?

Answer: By the end of the 20 weeks, I want to build a full-stack application that goes beyond what I could do with just Java/MERN something like an e-commerce or sales dashboard that doesn't just display data, but actually predicts something useful from it, like which products are likely to sell out or which customers are at risk of not coming back. I already know how to build the application layer; what I want out of this bootcamp is the ability to put a real model inside it instead of just static logic, and deploy the whole thing as a working product I can point to.

### 5. Reflect on one thing you learned today and one question you still have?

Answer: One thing that clicked today was the "How These Fields Relate" diagram I used to think Data Science was just a subset of AI, but it actually sits alongside it, using ML as one of several tools rather than being contained by it.

My question is: If AI adoption is part of why the Philippine IT-BPM sector recently revised its 2028 hiring targets downward, what does the number of new data/AI jobs available by the time I finish this bootcamp actually mean, compared to the jobs that AI itself is displacing in other roles?

## Part 2: Applied Deep-Dive - Based on my previous freelancing project.

**Industry: Finance**

### What real problem does AI solve in this industry?

Answer: Financial institutions use AI primarily for **fraud detection** - flagging transactions that
deviate from a customer's normal spending pattern in real time, before money actually leaves
an account. The real problem this solves is scale: a human reviewer cannot manually check
millions or thousands of transactions a day, but a model trained on historical fraud cases can score each
transaction in milliseconds and flag the suspicious ones for review. -- My Example here is Bud the AI bot.

### What data would a system need to solve it?

Answer: A system like this needs transaction-level data (amount, merchant, location, time), account
history (typical spending patterns per user), and labeled examples of past confirmed fraud
to train on. Device and location metadata often gets added too, to catch account takeovers.

### What could go wrong if the system is biased, wrong, or misused and who would that affect?

Answer: The risk is that these models are trained on **historical** fraud labels, which means they
inherit whatever blind spots or biases existed in how fraud was investigated in the past.

A biased model could disproportionately flag legitimate transactions from certain
demographics or regions as **suspicious** freezing accounts and blocking access to someone's
own money based on a pattern correlation rather than actual wrongdoing.

A real harm that falls hardest on the customers least able to absorb the disruption (small business owners,
people living paycheck to paycheck).

This is exactly why the **"Historical outcomes baked into labels"** bias watch-out from today's Responsible AI discussion matters here specifically: the labels themselves encode the past, and the past isn't necessarily fair.