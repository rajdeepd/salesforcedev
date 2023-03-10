
# Declarative tools in Salesforce

Apex is not the only technology in Salesforce which can access your data or manipulate it. Apart from Apex, there are multiple declarative tools available in Salesforce which can read your data  or manipulate it. These declarative tools are also called the point and click tools because you do not have to write any code to use these.

However, you need your problem solving ability to write your logic in these tools.


## Workflow Rule

Now, let's have a look at these declarative tools one by one. The first one is Workflow Rule and Workflow Rule has been part of the Salesforce platform for many many years and it's one of the most mature tools available on the Salesforce platform right now.

If you go back 10 years, then Workflow Rule was the only available automation tool at that time.

These Workflow Rules can have multiple actions, like send an e-mail or sending an outbound message or creating a task or updating the self record where the workflow Rule is executing or the parent record but it doesn't allow the child the record update.

That means if your Workflow Rule is executing on a parent object, you can not update the related child record on that parent record.

These are the limitation in Workflow Rule.

Workflow rule has been deprecated to Flow and Flow Builder.

## Process builder
Later, Salesforce introduced one more declarative tool, which is called Process Builder. It supports many types of actions, like all the actions in workflow rule except the outbound message, it cannot send outbound message, but it can send an email. 
It can create a task or any type of object record for that matter.

So, you can create any type of record using Process Builder.

It can also update the record, the parent record or the child record So, Process Builder supports all types of record update, but these records should be related to each other.

So, either this record that you want to update should be the self record where the process builder is executing, or it should be the parent record, or it can be the child record.

The Process Builder also can execute your Apex class. So, you can have your logic in your Apex class and can directly call it from the Process Builder.

A Process Builder can have multiple steps unlike Workflow Rule. So, in one single Process Builder, you can have your entire logic using different if-else conditions or using different steps
However, the Process Builder does not support deleting of a record.

So, if you want to delete a record, the Process Builder is not the right tool for you.

If you want to update the unrelated records, this means if you have two different objects, which do not share any kind of relationship and you

have a Process Builder on one of the objects, then you can not update the records of the other object from the Process Builder.

## Flowbuilder
This is a new tool replacing process builder which we will exoplain below.


## Visual Flow
The last and the most powerful declarative tool available in Salesforce is the Visual Flow.

Visual Workflow is a feature in Salesforce that allows users to automate business processes by creating flows using the Cloud Flow Designer. Flows can execute logic, interact with the database, call Apex classes, and collect data from users. Autolaunched flows can be launched without user interaction, and Visual Workflow has three different aspects: design, manage, and run. Users can build flows using combinations of elements, connectors, and resources. Visual Workflow is available in several Salesforce editions and can be used for various purposes, such as scripting calls for customer support or generating real-time quotes for a sales organization. It is different from Workflow and has limitations and considerations to keep in mind when designing, managing, and running flows.




A Visual Flow can do so much more than what a Workflow Rule or a Process Builder can do. And, it can execute Apex classes, it can execute lightning components as well, you can design your screens using Visual Flow, you can almost write all types of logic in Visual Flow, so, it's very similar to how Apex is written.

<figure>
<img src="/salesforcedev/docs/assets/images/Screenshot 2023-03-09 at 9.29.08 PM.png" width="100%" />
 <figcaption>Fig.- List of flows in setup</figcaption>
</figure>

You can also declare certain methods that you can call from Visual Flow.

But, it comes with its own cost. The execution of a Visual Flow is slower than Apex.
<figure>
<img src="/salesforcedev/docs/assets/images/Screenshot 2023-03-09 at 9.28.30 PM.png" width="100%" />
 <figcaption>Fig.- Creating a new flow</figcaption>
</figure>



<figure>
<img src="/salesforcedev/docs/assets/images/Screenshot 2023-03-09 at 9.29.02 PM.png" width="100%" />
 <figcaption>Fig.- Flow builder</figcaption>
</figure>


So, let's say if you have similar logic in your Visual Flow and in Apex class, then your Apex class will execute faster than the Visual Flow.

The debugging of Visual Flow can be challenging sometimes, and it's not that easy to debug the errors in your Visual Flow.

Visual Flow is not a pure a declarative tool, but a low code development tool where you don't have to write that much amount of code that you write in your Apex class.

Visual Flow is by far the most powerful declarative tool and you can do almost everything in the Visual Flow but still, it cannot match the power of Apex code. For some complex requirements, implementing a Visual Flow can be very challenging compared to writing an Apex code.

To summarize, these are the declarative tools available in Salesforce. In this course, our main focus would be to learn Apex and write Apex code.

So, we will not be implementing any of these declarative tools.