---
layout: page
title: Introducing Apex
permalink: 
nav_order: 1
parent: Apex
---
# Introducing Apex

Apex is a strongly typed Object Oriented language to execture flows and transactional statements on Salesforce platform servers.

For more details on Apex introduction refer to 

[Apex Intro](https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_intro.htm)

## Quick Start

Create a new class in Developer Console 

1. From the File menu, select New  Apex Class.
2. For the class name, enter `AccountUtil` and then click OK.



<figure>
<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-13_at_9.27.51_PM.png" width="40%" />
 <figcaption>Fig.- New Apex file </figcaption>
</figure>



```java
public class AccountUtil {

}
```


<figure>
<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-13_at_9.28.06_PM.png" width="50%" />"
 <figcaption>Fig.- Screenshot of Dev Console with the new class created </figcaption>
</figure>

## Add a method to the class

Update all accounts description. We create a static method updateAllAccounts()
> **Static methods, variables, and initialization code** have these characteristics.
>They’re associated with a class, are allowed only in outer classes.
>They’re initialized only when a class is loaded.
>They aren’t transmitted as part of the view state for a Visualforce page.<br/>
> **Instance methods, member variables, and initialization code** have these characteristics. <br/>
> They’re associated with a particular object.
> They have no definition modifier.
> They’re created with every object instantiated from the class in which they’re declared.


```java
public static void updateAllAccounts() {
    // Get all accounts
    Account[] accounts = [SELECT Id, Description FROM Account];
    // loop through them and update the Description field
    for (Account acct : accounts) {
        acct.Description = 'Updated Account Description';
    }
    // save the change you made
    update accounts;
}
```

## Execture the static method

Let us execute the method from Anonymous window.

**Test** > **Open Execute Anonymoud Window**

<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-14_at_8.05.31_AM.png" width="50%" />

You can see the output as shown below:

<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-14_at_8.06.02_AM.png" width="100%" />

<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-14_at_8.06.37_AM.png" width="70%" />

## Verify Record Update

If you go back to record detail page of any Account you will notice updated Description

<img src="/salesforcedev/docs/assets/images/Screenshot_2023-03-14_at_8.07.57_AM.png" width="70%" />

**Reference Trailhead** [Apex QuickStart](https://trailhead.salesforce.com/content/learn/projects/quickstart-apex?trailmix_creator_id=banderson136&trailmix_slug=lennar-apex-and-development)