---
layout: page
title: Salesforce Technologies
permalink: 
parent: Web Technologies
nav_order: 2
---
We will give an overview of Salesforce Web Technologies now. Salesforce currently supports two types of user experiences.

The first one is Salesforce Classic. The Salesforce Classic was the only user experience in Salesforce before 2014 and as you can see from this image here, this was built on older technology stack prevalent at that time.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_44_07.png" width="100%" />

After 2014, Salesforce has started supporting a new type of user experience called Single page view, which is called Salesforce Lightning.

Now, this is a modern UI. This not only looks better, it also helps you increase your productivity. From one page itself,you will have tons of options to do your work.

Let's say you want to update your opportunity stage, you have Lightning path right there.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_45_31.png" width="100%" />

I'm talking about that green line, so you can click on one of the elements and , your opportunity stage is updated.

You can see all your related records on the same page on the right side bar. This definitely helps you increase your productivity, Lightning is much faster than the Salesforce Classic.

Now, let's talk about the technologies that you can use to build any of these UI.

If you want to build Salesforce Classic UI, then you have to use the Visualforce pages. Visualforce is a Salesforce proprietary language that you can use to build your UI pages or UI components.

If you want to build the Salesforce Lightning UI, then you have two technologies here. The first framework is the Aura Components framework and the second is Lightning Web Component framework.

The **Aura Component framework** was introduced in 2014 and it's more mature than compared to the Lightning Web Components framework which were introduced in the December 2018.

> **_NOTE:_**  **Aura Components** are units of an application that are both self-contained and reusable. They serve as modular pieces of the user interface and can range in size from a single line of text to an entire application. The framework comes with a set of pre-built components, including the base Lightning components that have Lightning Design System styling and can be found in the lightning namespace. By assembling and configuring components, new components can be formed within an app, and they are rendered to produce HTML DOM elements in the browser.

Components can contain other components, as well as HTML, CSS, JavaScript, or any other web-enabled code. This allows for the creation of apps with complex user interfaces. The implementation details of a component are encapsulated, enabling the consumer of a component to focus on building their app while the component author can innovate and make changes without affecting consumers. Components can be configured by setting the named attributes that they expose in their definition, and they interact with their environment by listening to or publishing events.

> **_NOTE:_** **The Lightning Component framework** is a user interface (UI) framework designed for creating single-page applications for both mobile and desktop devices. Since Spring '19 (API version 45.0), developers have been able to create Lightning components using two programming models: the original Aura Components model, and the newer Lightning Web Components model. Lightning Web Components are custom HTML elements that are built using HTML and modern JavaScript. It's possible for both Lightning Web Components and Aura components to exist and work together on a single page.

Both Lightning Web Components and Aura Components can be configured to function within the Lightning App Builder and Experience Builder. The end-users and administrators don't need to know which programming model was used to develop the components, as they'll simply be viewed as Lightning components to them.

Both of these frameworks allow you to achieve the similar functionality or to build similar components but they have different tech stack. Lightning Web Component framework is much faster than the Aura component because it is based on the latest web standards, where the Aura component framework was a complete Salesforce proprietary frameworkand each and every feature of this framework was built within the framework itself.

The **Lightning Web Component** framework relies on the latest web components framework and that is the reason the Lightning Web Components are much faster than the Aura component framework.

For more details refer to the following links:

[Lwc vs Aura what Architects need to know](https://medium.com/salesforce-architects/lwc-vs-aura-what-architects-need-to-know-695af25e4535)

[Lightning Aura Components Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/intro_framework.htm)

## Salesforce Backend

Let's talk about the Salesforce back end.
Salesforce uses relational database as its database, Salesforce uses Oracle database as the backend along with  Big Data stack, NoSQL databases  and now real time data using data lake called Genie.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_47_01.png" width="70%" />

But as a Salesforce user, you will never be directly interacting with the relational database, ratheryou will be interacting with the Salesforce Objects.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_47_21.png" width="70%" />

You will be creating your objects, which in database terms, are tables where you will be storing your records or rows. Salesforce back end language is Apex, which is very similar to the Java language.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_47_40.png" width="70%" />

You can use the Apex to read the data from your Salesforce objects or to update, delete or create the
data in your Salesforce objects. Apart from the Apex language, Salesforce has some declarative tools as well, which can also directly interact with your objects or your Salesforce database

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_45_54.png" width="70%" />

These tools are Workflow Rules, Process builder, Visual Flows and Approval Processes. We will be talking
about these declarative tools
But for now, just know that apart from Apex, there are some declarative tools that can also read and update your Salesforce data.

Let us see, how a Salesforce object stores your data.
You can say that a Salesforce object is a database table (or a virtual table) where you can store your data.

In this example, we have a user object which can store the user data. We have a table which can store the first name of users the last name of the user and the email of the user.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_50_32.png" width="70%" />

And we can see that it has two records,one for Manish Choudhari and the second one for the Harry Potter. Now, this first name, last name and email,

These are called Fields. So, the first name is the field 1 in user object.

Then we have another field called Last Name, and then we have another field called e-mail. In database terms, you can also call these columns.

<img src="/salesforcedev/docs/assets/images/screenshot-www.udemy.com-2023.03.07-22_50_48.png" width="70%" />

And, the Manish Choudhari and Harry Potter are the records. So, this table or this object has two records. In database terms, you can also call these records as row or the table row. So, just to reiterate, a Salesforce object is just a schema to store your data and it stores your data in tabular format.