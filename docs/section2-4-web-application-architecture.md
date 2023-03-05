# Web Application Fundamdentals

## Web Application Architecture

It is important that you understand how a Web application works before you start building one.

<img src="/docs/assets/images/Screenshot_2023-02-26_at_7.13.50_PM.png" width="70%" />

A Web application is a combination of many small programs, and all these programs work together to serve a purpose.

At the very least, a Web application has a front end, a back end, and a database to store the data.

<img src="/assets/images/Screenshot_2023-02-26_at_7.15.48_PM.png" width="70%" />
<img src="/assets/images/Screenshot_2023-02-26_at_7.17.11_PM.png" width="70%" />


## Illustration

So, here you are, trying to view your favorite video on YouTube or if you are a technical geek like me, then maybe a video on Udemy.

So, you opened up your browser and clicked on a video.

<img src="/assets/images/Screenshot_2023-02-26_at_7.18.18_PM.png" width="70%" />

Now behind the scene, it will send a request to the YouTube application server and it will send your identity like this user is requesting for this particular video.

<img src="/assets/images/Screenshot_2023-02-26_at_7.18.30_PM.png" width="70%" />

Your application server is going to process this request.
It's going to check your identity if you are a genuine user or not, or if you have a subscription or not.
And, then it's going to request for the data from the database server.
So, the database server will have the video files that you may want to view.

<img src="/assets/images/Screenshot_2023-02-26_at_7.17.26_PM.png" width="70%" />

<img src="/assets/images/Screenshot_2023-02-26_at_7.17.57_PM.png" width="70%" />

This database server is going to return the response to your application server back or maybe a link to the video file where the video file is stored, and then your application server is going to send back the response to your browser that, please play this video file from this particular location.

In general, when a user interacts with the application, this layer is called front end.

So, this is the application UI that a user can see and your application server and database server are

called back end, because a user cannot see these servers and how the request is processing there. And, if you remove any of the element from this illustration, so, let's say if I remove my application server, your application will stop working because there is no server to process your request which can identify which video you are requesting and where is it stored.

And, if you remove the database server, then your video file will never be stored and you can never view it.

And, let's say if you remove the front end, then the user will not have any place to interact with your application.

So, all these three elements are essential for an application to work.

So, I hope this clears your mind about what is a front end and what is a back end.

Now, let's try to understand it with the help of an example.

So, here I am on the airbnb website,

and this is how it looks when a user type in "airbnb.co.in" in their browser.

So, the UI has multiple elements which a user can interact with.

Like, I can search for the places to stay, I can search for some of the experiences that I want to explore, maybe I want to do a hitchhiking, then I can search for those experiences here.

I can scroll down and check for all the other services that airbnb provides.

So, this is a front end where a user can interact with the application. Now let's try to search for some places to stay in Hyderabad.

So, I'm going to stay from 16th of May to 17th of May, and let's say we are two adults.

Now, let's click on this search button. So, as soon as you click on the search button, the request is sent to the airbnb application server and the airbnb application server will process your request.

The server will know that you are looking for some places in Hyderabad. Now, this application server is going to make a request to the airbnb database server and it's going to ask about all the places to stay in Hyderabad. The database server will respond back with the data.

Your application server is going to process this data and it's going to pass this data in a form that your front end can understand or your browser can understand.

Then, it's going to return this process response to the browser and here,

## Kitchen Analogy

So, we can say a Web application is like a restaurant where you have a seating area from where a person can read the menu and order for a food item.

This order will be sent to the kitchen, where the order will be prepared. To prepare the order, the chef will need some ingredients which will be stored in a larder and a chef can pick some ingredients based on the order.

Now, again, here we can say the seating area is the client site or a front end from where the user can interact with your application, or in this case, the user can place an order.

<img src="/assets/images/Screenshot_2023-02-26_at_7.29.18_PM.png" width="70%" />

The kitchen is back end or our application server where the request will be processed or the order will be prepared.

And larder is our database where you will keep your ingredients or the user data.

So, this is a classic example to explain how a Web application works and I hope now you understand how these different elements interact with each other to serve a single purpose. In a Web application, a front end is always designed in such a way that it can attract the target audience or the users.

## Front End vs Back end

<img src="/assets/images/Screenshot_2023-02-26_at_7.30.17_PM.png" width="70%" />
<img src="/assets/images/Screenshot_2023-02-26_at_7.30.44_PM.png" width="70%" />

So, this is how a front end looks, where you see the natural beauty and a happy father and his son but, if you want to work on the back end, then this is how it looks.

So, sometimes the back end can be messy and it doesn't look as good as your front end, just wanted to share this with you guys.