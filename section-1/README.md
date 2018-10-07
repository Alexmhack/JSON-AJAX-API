# jSON & Javascript Objects

**Json** in **Javascript** is in simple string format.

Below is a javascript variable containing key and value pair

```
<script>
	var person = {
		"firstName": "Alex"
	}
</script>
```

If you console log this variable then you will get

```
Object { firstName: "Alex" }
```

If you create a javascript object ```firstName``` and console log it then you will find that it is very identical to the previous results

```
<script>
	var person = {
		firstName: "Alex"
	}
</script>
```

This seems to be json but it isn't. Open [JSLINT](http://jsonlint.com/) and try pasting 
the above both pieces of data only with curly braces like 

```
{
	"firstName": "Alex"
}
```

And hit the **Validate jSON** button and it will show **Valid jSON** but if you try the 
same process with the ```person2``` variable 

```
{
	firstName: "Alex"
}
```

Hit the **Validate jSON** button and it will show errors something like

```
Error: Parse error on line 1:
{	firstName: "Alex"}
--^
Expecting 'STRING', '}', got 'undefined'
```

This tells us what jSON notation actually is and how it is different from javascript 
objects.

**SOURCE CODE IN index.html file**

# jSON Notation
Now that we know how jSON format works we can use it to create and access more data from 
jSON

**index2.html**
```
<script>
	var person = {
			"firstName": "Alex",
			"lastName": "Hopper",
			"age": 19
	}
</script>
```

Then in console use 

```
# command
person.age
# result
19

# command
person.firstName
# result
"Alex"

# command
person.lastName
# result
"Hopper"
```

The dot notation is used here to access the jSON objects in the ```person``` variable
