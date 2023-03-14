
---
layout: page
title: Apex Variables
permalink: 
nav_order: 4
parent: Apex
---

Apex is a strongly typed language, supports the following variables

In Apex programming language, every variable and expression must have a specific data type. The data types in Apex include primitives, sObjects, collections, enums, user-defined classes, and null.

Primitives are simple data types like Integer, Double, Long, Date, Datetime, String, ID, or Boolean. sObjects are either generic or specific, such as an Account, Contact, or a custom object. Collections include lists, sets, maps, and enums. User-defined classes and system supplied Apex classes can also be used to create objects. Null is used to assign no value to a variable.

Methods in Apex can return values of any data type listed above or return no value and have a type of Void.

Apex strictly enforces type checking at compile time. For instance, if an object field of type Integer is assigned a value of type String, the parser generates an error. All compile-time exceptions are returned as specific fault codes, along with the line number and column of the error. Debugging Apex provides more information on this topic.

## Primitive data types

Apex uses the same primitive data types as [SOAP API](https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_calls_concepts_core_data_objects.htm), except for higher-precision Decimal type in certain cases. 

All primitive data types are passed by value.
All Apex variables, whether they’re class member variables or method variables, are initialized to null. 

All the variables need to be initialized before using.

### String
Any set of characters surrounded by single quotes. For example,

```java
String s = 'This is a string';
```

There is no upper limit on size of string but is governed by heap size limit.
See 
[Apex Governor Limits](https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_gov_limits.htm) for more details


### Boolean

Boolean is `true`, `false` or `null`.

```java
Boolean isWinner = true;
```

### Date

Date is a primitive datatype, A value that indicates a particular day. Unlike Datetime values, Date values contain no information about time. Always create date values with a system static method.

Some example of Date datatype using `Date.newInstance()` method.

```java
Date myDate = Date.newInstance(1960, 2, 17);
Date newDate = mydate.addDays(2);

```

Create data from today's date and convert to specific format.


```java

DateTime todaysDate = System.today();
String todaysDateStr = todaysDate.format('yyyy-MM-dd');
System.debug(todaysDateStr);


```

### Integer, Long, Double

**Integer**
32 bit number with no decimal

**Long**
64 bit number with no deciment

**Double**
A 64-bit number that includes a decimal point. Doubles have a minimum value of -263 and a maximum value of 263-1. 

Example

```java
Integer i = 0;
Long l = 2147483648L;
Double pi = 3.14159;
```
### Object
Any data type which is supported by Apex


```java
Object object = 100;
// Cast the object to an integer.
Integer i = (Integer)object;
System.assertEquals(100, i);

```


## sObject

An `sObject` represents an object, such as an Account or Contact. For a list of standard objects, see Standard Objects.

Each Salesforce record is represented as an sObject before it is inserted into Salesforce. Likewise, when persisted records are retrieved from Salesforce, they’re stored in an sObject variable.

Standard and custom object records in Salesforce map to their sObject types in Apex. Here are some common sObject type names in Apex used for standard objects.

The  example below creates an sObject of type Account with the name Acme and assigns it to the acct variable.

```java
Account account = new Account(Name='Acme');
```

Reference: [Field Types](https://developer.salesforce.com/docs/atlas.en-us.242.0.object_reference.meta/object_reference/field_types.htm)