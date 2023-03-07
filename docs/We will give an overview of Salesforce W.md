We will give an overview of Salesforce Web Technologies now.

Salesforce currently supports two types of user experiences.

The first one is Salesforce Classic.

The Salesforce Classic was the only user experience in Salesforce before 2014 and as you can see from this screenshot here, this was built on older technology stack prevalent at that time.

After 2014, Salesforce has started supporting a new type of user experience called Single page view, which is called Salesforce Lightning.

Now, this is a modern UI.
This not only looks better, it also helps you increase your productivity. From one page itself,you will have tons of options to do your work.

Let's say you want to update your opportunity stage, you have Lightning path right there.

I'm talking about that green line, so you can click on one of the elements and , your opportunity stage is updated.

You can see all your related records on the same page on the right side bar.

So, this definitely helps you increase your productivity,

and as per Salesforce, the Lightning is much faster than the Salesforce Classic.

Now, let's talk about the technologies that you can use to build any of these UI.

If you want to build Salesforce Classic UI, then you have to use the Visualforce

pages. Visualforce is a Salesforce proprietary language that you can use to build your UI pages or

UI components.

If you want to build the Salesforce Lightning UI, then you have two technologies here.

The first one is the Aura Components framework

and the second one is Lightning Web Component framework.

The Aura Component framework was introduced in 2014 and it's more mature than compared to the Lightning

Web Components framework which were introduced in the December 2018.

Both of these frameworks allow you to achieve the similar functionality or to build similar components

but they have different tech stack. As per Salesforce,

the Lightning Web Component framework is much faster than the Aura component because it is based on the

latest web standards, where the Aura component framework was a complete Salesforce proprietary framework

and each and every feature of this framework was built within the framework itself.

The Lightning Web Component framework kind of relies on the latest web standards or the latest web stack

which are natively available in your Web browser

and that is the reason the Lightning Web Components are much faster than the Aura component framework.

If you want to get my view on the Salesforce Classic vs the Salesforce Lightning UI, I love

Salesforce Lightning UI,

and that's because it's modern and helps you achieve more in less time.

And anyways, the Salesforce Classic is running out of its fuel and soon will be discontinued by the

Salesforce,

maybe like in coming few years.

So, this was about the Salesforce front end,

now let's talk about the Salesforce back end.

Salesforce uses Oracle as its database

but as a Salesforce user, you will never be directly interacting with the Oracle database, rather

you will be interacting with the Salesforce Objects.

So, you will be creating your objects, which in database terms, are tables where you will be storing

your records or rows. Salesforce back end language is Apex, which is very similar to the Java language.

You can use the Apex to read the data from your Salesforce objects or to update, delete or create the

data in your Salesforce objects. Apart from the Apex language,

Salesforce has some declarative tools as well, which can also directly interact with your objects or

your Salesforce database

and these tools are Workflow Rules, Process builder, Visual Flows and Approval Processes. We will be talking

about these declarative tools in our coming videos,

but for now, just know that apart from Apex, there are some declarative tools that can also read

and update your Salesforce data.

Now, let's see, how a Salesforce object stores your data.

You can say that a Salesforce object is a database table where you can store your data.

In this example, we have a user object which can store the user data.

So, we have a table which can store the first name of users,

the last name of the user and the email of the user.

And we can see that it has two records,

one for Manish

Choudhari

and the second one for the Harry Potter.

Now, this first name, last name and email,

These are called Fields.

So, the first name is the field 1 in user object.

Then we have another field called Last Name, and then we have another field called e-mail. In database

terms,

you can also call these columns.

And, the Manish Choudhari and Harry Potter are the records.

So, this table or this object has two records. In database terms,

you can also call these records as row or the table row.

So, just to reiterate, a Salesforce object

is just a schema

to store your data and it stores your data in tabular format.

