# Basic Fields

### Creating Common Field Types and Advanced Field Types

[00:00:00](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m00s)
(_Click on these time links to see Youtube video_)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In this tutorial, we will look at creating fields. There are two groups. Easy, plain, or common field types which we will be looking at first, and advanced field types which are primarily your custom field types, which we'll look at only after we had covered the admin views and how you connect fields to views. [00:00:15](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m15s) It's quite important because those custom field types only make sense if you see the relationship between views and fields.

First, we'll look at the more common field types. Not all of them, of course. I'm just going illustrate to you a text field type and a list field type. [00:00:54](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m54s) All the other sort of fields follow the same kind of implementation.

### New field type _Using text field as example_

[00:01:04](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m04s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=64" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

So let's create a new field type. We would select text as our first illustration. It will automatically load the fields here set on the field types default settings we looked at previously. When it comes to this information here you need to have a good background on MySQL to understand what varchar, a text, a medium text, a long text, and so on, exactly means. [00:01:29](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m29s) These are basically the data types in relation to the database. I have now added the feature of you being able to change that because I want to liberate your ability to develop applications that are more advanced than a cookie-cutter kind of component builder. [00:02:04](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m04s) This component builder wants to leave enough room for you to make very advanced choices. So the more I constrain it to a sort of "just click here, there; don't know any code, just go on and build something," the more I am going to frustrate the real developer who wants to design something more advanced and versatile. [00:02:25](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m25s) There are component builders out there that probably have done that, but I want to give you enough tools to be creative which means a little bit more complexity all over. But if you know PHP and have worked with PHP in relation to SQL or any other SQL database connections via Java or any other language, you will know that there is such a thing as a data type.[00:02:59](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m59s)

### Indexes types

[00:03:15](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m15s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=195" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

You will know that it has a length, that you can set some default value to it, and that you can decide whether it's a key or a unique key. Just realize that if you set it as a unique key (as an Index type) it means that specific field will only allow a value once and if that same value is placed in it, it will be an error. [00:03:38](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m38s) You hardly ever use that. You won't even use it for an alias because the alias implementation in Joomla deals with the duplication within the model when it saves the information. It checks whether there is an alias in the database and implements the alias so that it doesn't conflict. So even there you do not need that feature. But it is available and you might see a need to use it, so I added it there.

Then your normal null switch. (Whether the table should be null if it's empty.) [00:04:15](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m15s) Usually you would use one of these default values and then set it to "not null."

### Store method _Default, JSON and other options_

[00:04:28](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m28s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=268" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Now the storing method. Most of the time you will use the default. This is because these other methods require much more knowledge of what you are trying to achieve. If you do have that knowledge, then I would say that JSON would probably be used when you are storing an array of items to the database. [00:04:42](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m42s) Yet when you are using list (which we'll look at just now,) you wouldn't need to use JSON because Joomla's implementation of the list field type deals with arrays. [00:05:09](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m09s) If the list allows for multiple selections then you need to use JSON. [00:05:37](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m37s) If the field type is checkboxes it will be going here and it will add it. If there are multiple selected, it will add it as a JSON option object if the type name is a tag. [00:05:56](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m56s) So if you are using a tag field type it will not go in here no matter what you do. If it's not zero, which is the default, then it will fall back onto this. If it is a checkbox and you haven't selected one of those features.... [00:06:22](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m22s) For example, if you haven't selected one of this JSON or base 64 and it is a checkbox field type, then it will fall back to JSON. [00:06:47](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m47s) That's the default switch. In the switch, it takes what you've set. If you set it to JSON, it will use JSON; if you set it to base, it will use base; if you had done an encryption, it will use that; but if you had set none and it is a checkbox, it will set it to JSON even if you had set the checkbox to default. [00:07:12](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m12s) We are still making sure it's safe as JSON because Joomla doesn't deal with checkboxes correctly. In fact, it tells you as a warning on their pages. The Component Builder knows that and so I coded it so that it will make sure that we're storing it as a JSON object and not just the array itself.

### Compiled info in UI _Explanation of compiled fields_

[00:07:42](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m42s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=462" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This is just looking at the checkboxes and other JSON items for the view and so for most things that we are looking at the UI. [00:07:47](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m47s) If we are not sure how the implementation works, looking at the code is the quickest way to actually understand what would be the way to select. That means if you're not a PHP developer and you cannot figure out where this line or this particular area of code is being addressed, then obviously this is to your own disadvantage. But if you're able to read PHP then the compiler itself leaves in the XML files and other files that you are building. [00:08:20](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m20s) In other models of things that it's building it is showing you in which file it is actually building this part of this group and exactly on what line. So that is the way for you to get in there and see exactly what is being done. [00:08:52](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m52s) It will also help you to determine what you need to change for it to work if it isn't working. There is no way for me to avoid this.

### Store methods support encryption _Encryption of fields supported_

[00:09:12](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m12s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=552" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Going back to just a normal text field. We would just leave it to default. These other options of encryption will be explained in a later video. [00:09:22](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m22s) You would possibly never use these. I had the need for them in a component that I had to develop, and so I added those features in. At this stage, it's really quite difficult to implement. The basic one, which is actually more secure if you would ask certain people, is easy to implement. [00:09:50](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m50s) But the advanced one, which is for other purposes than just your normal encryption, is a bit more advanced and difficult to implement. So for now, if you're not that advanced in your programming skills then you should just avoid these. This base64 is often used where you're storing code into the database. Most of component builder's areas where you can add custom scripting use this base64 as the storing method.

### Example e-mail field _E-mail field and XML fields example_

[00:10:28](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m28s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=628" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

So if we are going to create an email field, we say that it should not be required, change data length\values to 255, leave store method to default, and change the name to email. (We don't usually do uppercase.) [00:10:47](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m47s) That's what is going to be used for the database. So this field all over the system and all the code is going be called by that name: email. Underscore. [00:11:09](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m09s) Here the label is what will be visually seen in the form. There we'll be adding 'Enter Email.' We'll leave the text size the same. Max length is good. I'm not going to use the default field. [00:11:36](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m36s) Default is optional so I can just leave it out. Description: I'm going to say 'Enter Email.' We'll remove those (readonly"false"; disabled"false".) We're going to leave required to 'false' to ensure that it isn't required. Then I'm going to use validate the email and I'm not going to use the field option. [00:12:08](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m08s) The field option is to validate against another field that they both 'equal' each other. We don't need that for this field. Here I'm going to place a demo. I'm going leave those (showon; onchange) out. So there we have an email field. Now this validate option. (There is some custom validating option in Joomla. Email is one of them.) [00:12:42](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m42s) Then there is a way to create your own validation. The way to implement that would be to write PHP up for that. You need to know how to write your own validation and to place it via the custom adding in our files; to place it in the correct location where the Joomla form builder will be able to get that field validation type and add it into your field. [00:13:07](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m07s) So if you know what I'm talking about then you will know where to place it, and you'll later see that in the component itself it has an option to add custom files and how to map it to the correct location. [00:13:31](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m31s) You can then use your own validation figure type there to extend on the validation options. But currently, component builder itself doesn't do extra custom validating options. It only uses Joomla's defaults. That means you can also leave it out and then it doesn't do validation but it will still do filtering. Here is a list of the available filters that Joomla has.

### Target fields with custom CSS/Javascript _Adding custom CSS/javascript to fields, in both edit and list views using Jform and Jquery_
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=850" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[00:14:10](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m10s)

So that's how to create a text field. You can target these text fields with CSS and JavaScript, respectively, in the list and in the single view. The views (plural) is the list view; view (single) is the single view that will be the edit view in the backend. Both of these are targeting the editing view and the list view in relation to its backend display. [00:14:36](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m36s) If you extend the editing view to the front, then it will also load the JavaScript to the front. But you cannot extend the list view to the front. You need to build a custom front which we will eventually get to which is called site views.

So this is primarily targeting your admin area with these scripts. Although you can extend the editing one, which is the single view, to the front, which means it will also extend that to the front. [00:15:10](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m10s) The way to target this field would be: that is the ID plus jform. If you forget that, you could look at any other field and you'd see it says jform_ and then the field name as an ID. [00:15:38](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m38s) I'm just using FireBug to do that. So that means you can just put that in front of the email. Not here though if you want to target it in your Java Script or in your CSS. Let me show you. You'd add #jform_email. [00:16:08](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m08s) Now you can target it with CSS. Maybe color or something. JavaScript is done in the same way. If you use jQuery, add jform_ in front of the field name.

The nice thing about this is that you can add the script to the field and in any view where you use this field this script will follow it. [00:16:54](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m54s) It will go along with it. It will be added to that view dynamically. You don't need to rewrite it everywhere. For example, I have a  script that I'm using for numbers. [00:17:16](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h17m16s) Here is an even better option to demonstrate: I had to create a repeatable field, which we will look at later; it's an advanced field. Inside of that repeatable field, I wanted to add a date field.

### Repeatable field with date _Adding PHP and Javascript in custom script_

[00:17:49](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h17m49s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1069" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Now those of you that work with Joomla will know that you can't currently add a date field to a repeatable field. So what we did (this is probably going to be very impressing) we simply used a text field and added that to it. [00:18:12](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h18m12s) As you can see here we have PHP right in this JavaScript block. The way to add PHP here is to do the open brackets, question mark, PHP, and then again question mark, close. There is a PHP and we are adding the jQuery framework. Now, this script I added to the repeated fields script area, not to the actual text field. [00:18:45](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h18m45s) The reason why I didn't add it to the actual text field is that the text field is going be repeated. So you are going to have ten, twenty, or whatever of that specific text field. But with this code, I'm able to target up to fifty repeats of that field. [00:19:11](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h19m11s) With that field number we set at least fifty, and this JavaScript area is being repeated fifty times. So the course_date_fields_date is an ID I got from after creating the repeated field. I went in and looked at the ID of that field, added a date picker, set the value of the date picker, and basically added it to the field. [00:19:43](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h19m43s) It works very well. So this custom scripting area for JavaScript can also take PHP inside of it (and JavaScript) that will then be added to the view in which this field is going to be used. However, since we are just using it for creating a simple email field, we will click save; or save and close or Save and new. [00:20:17](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h20m17s)

### List field and adding options, static _Setting up a static list_

[00:20:26](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h20m26s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1226" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

So that was looking at creating a text field type. Now we'll do a list field. We click on the list and we see that it has an option 'array' or 'string' there. The options are set with a zero, a pipe, the name, and a coma. [00:20:45](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h20m45s) That basically represents one item in the dropdown. So if you see this drop-down here then each of those items would basically be represented between the comas. [00:21:05](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h21m05s) The (...) makes a separation between the value being stored in the database and the value being show[00:00:15](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m15s)n to the person accessing the form. If that value is the same value (if you want to store in the database the same value as the one that is being displayed) then you simply drop off the pipe with the initial values like that. It will now say option one, option two and option three. [00:21:29](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h21m29s) That is one permitted way to use it. [00:21:50](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h21m50s) You could also say that you want one option to be viewed as having not selected anything yet. So if you want to add another option you would type "select an option." [00:22:15](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h22m15s) By adding a pipe without a value it is being treated as null. So when the drop-down is built, it will be as if nothing is selected. [00:22:57](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h22m57s) Now the other values would be selecting. You can use them as IDs or use a totally different value. It doesn't matter. Just know that it would possibly make everything lowercase if you put it on that side of the (...). [00:23:29](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h23m29s) You can fill in this information based on your requirements. So that's how you set up a list field.

I hope this shows you what is possible, but as you can see this list field isn't dynamic in the way that a custom field possibly can be. [00:23:55](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h23m55s) You see the list field here where you statically set a few values that are unchanging and which should be selected. But with the custom field type, you can have other tables values populate the list for you. So as it's being created your list gets longer dynamically. We will still look at that and it is obviously available, but this is more static "set it once and use it over and over" whereas there is actually also a dynamic list option which I will illustrate later.  

### Radio button example

[00:24:38](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h24m38s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1478" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Let's look at a radio button which is very similar to creating a radio button. There is one point to make here, however. If you create a radio button you'd see that there are only two values. You can add more than two to the list, but I always think of it this way: [00:25:04](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h25m04s) as soon as it becomes a list of values then use a list. A radio button should have four selections at most. (It depends on the length of the text.) As soon as it gets a fifth value, you should look at a list instead. Again, with a radio button, you can just leave it at the default storing method. [00:25:41](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h25m41s) Again the field attributes are very similar to the text attributes except for the 'options array' option here. Then also like the list field type, it is separated by a comma, and the store value and the display value are separated by a pipe. It is important to note that you cannot use quotation marks inside of your values. [00:26:06](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h26m06s) If you want to use quotations inside you need to look up the HTML equivalent of those quotation marks and use that. Then it would work, but if you add a quotation inside, it will break off the string and you would have only one value show up. [00:26:38](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h26m38s)

### Color field example

[00:26:54](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h26m54s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1614" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Let's look at another one. Color is quite straight forward. It has a default value. You need to remember to set the label and the name. The type must not be changed. If you select color here and you do change the type, the component builder will simply ignore what you did. [00:27:16](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h27m16s) The reason for this is because we had set the type itself to be mandatory and unchanging when we had set up the field type. That's why you cannot override it. Everything that you set to mandatory and unchanging will fall back to the setting that you set there in the field type. Even if you change it here, it will not change.

### Show on attributes example

[00:27:46](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h27m46s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1666" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Then there is the description, and if it's required, the showon feature. You can have a list field which has an ID too which should be selected so that this color field should show. So you could say that this field's name is  'view' and 1. [00:28:17](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h28m17s) Only if the option with the value of 1 is selected in the view field will this field show up. [00:28:39](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h28m39s) You can have it if 1 or 4 is selected then it will show up. This implementation is your Joomla default implementation of the showon field. Unfortunately, it cannot target multiple other fields yet, and that's why we have our own implementation in component builder which is far more advanced. [00:29:07](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h29m07s)

### Category field example

[00:29:18](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h29m18s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1758" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Another one that's quite interesting is the category. In Category, you have an extension. If you read it, this extension is the name of the extension for which the category will be retrieved. For example, to list content categories use the value "com_content." [00:29:42](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h29m42s) You can add also target one view, use the value 'com_component.view.' That means that by adding the category field to a view you automatically add a category to your component so you don't need to map the category. In fact, you cannot map it even if you wanted to. [00:30:09](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h30m09s) Joomla already has a category component in place. (You can add your own category view and then use a custom field to link its values to other views.) If you are going to use Joomla's category implementation that integrates with your component, this is the way you do it. You don't write anything for the category area because Joomla does that itself and adds it to your component dynamically. The only thing you need to do is an extension, add your component's name. [00:30:48](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h30m48s) The categories can also be targeting a specific view instead of the whole component itself. So it can be related to just one specific view which means that you can have multiple categories for one component. [00:31:25](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h31m25s) This might be overkill, but it's none the less possible. The way you do that is simple, your component name, and the specific view's name. (The view must be singular. You cannot target a list view; it must be an editable, single view.)

### Editor field example

[00:32:10](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h32m10s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=1930" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The editor is also a common field which is often used. [00:32:11](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h32m11s) The editor is that big block in your Joomla content article manager in which your articles are placed. Here you can add such a block to your component. There are some important things, like buttons. If you read the description we have here it explains to you how it works, including the hide option and what kind of editor you want to load; the preferable or alternative one. [00:32:44](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h32m44s) The button option here: you can read it or hide buttons, based on what you selected. You have a filter option that requires your normal attributes as with other field types in Joomla. Since most of them are extending your base field in Joomla, the type, name, label, and default are also available to all the others.

### Media field example

[00:33:26](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h33m26s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=2006" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Media. Make sure with media that you select the correct directory. If none is set it falls back to images, but you can target a specific directory inside of images. It's mandatory, so you need to set it. You can only target images itself, which is a limitation from Joomla's side. So the directory starts at images. The attribute should be relative to the top-level /images/folder. [00:34:01](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h34m01s) That means that if you want to target a specific folder inside images called 'foo,' then you would add that there. Then preview: if an image has been selected and you want the image to be able to be previewed by hovering over the side of the field, you change it to true. The 'showon' feature is here as well as the other default concepts that we had discussed.

### Notes field example

[00:34:42](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h34m42s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=2082" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Notes come above a field. [00:34:43](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h34m43s) You can add notes around your fields. It has a very nice implementation in the Field Information here that you can read through.

We had now looked at basic field types, or common field types. [00:35:09](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h35m09s) If there are any other field types that you need help with, please look up the Joomla documentation since the implementation is more or less straight forward. We aren't trying to redesign the wheel; we are simply trying to implement Joomla's way of doing it. If there is a field type you need more information on, you can look at Joomla's documentation on that field type. If they don't have documentation then you can go into the field, like I said, libraries. [00:35:41](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h35m41s) There are three places to look in the libraries' folder: CMS, Joomla, and legacy. These are the places where these fields can be found. If you look under the CMS folder, you have captcha field type, chromestyle, content editor. So if you want to know if there are more attributes that can be used in the editor you can open the editor and look through the code and see the attributes that are being implemented across the board. [00:36:06](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h36m06s)

### Translation brief overview

[00:36:31](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h36m31s)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9NO2rKnC6Ug?start=2191" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see that there is an attribute that we are not already targeting you can go to the field type, open it, add the attribute, add the name, add the value, set whether it's mandatory, and set whether it's translatable. [00:36:37](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h36m37s) Whether it is translatable or not, is an important concept. Not all fields are translatable. When a field is translatable, component builder basically translates it for you. If you look at this acronym, for example. I added the label as 'acronym,' then, while the component builder builds this field into your component, it takes that value, [00:37:17](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h37m17s) converts it into a translatable string which adds it to the language file, and then adds that in here so if somebody updates the language file it updates everywhere in the system. This basically means that languages are implemented everywhere in component builder's components. All the components it's building, it translates; as well as everything that you set to be translatable. If we look at a certain field type, like text. [00:37:54](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h37m54s) Any property that you set to translatable means that component builder will dynamically take the hint and translate it into a language string, add it to your language file, and replace the XML with the language string. [00:38:31](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h38m31s)

So that is how you can extend existing field types and create fields with them. I hope that is good enough for you to be able to use. Having fields might still feel very primitive, and so next up we'll be looking at adding those fields to views and basically building your view yourself. [00:38:59](https://www.youtube.com/watch?v=9NO2rKnC6Ug&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h38m59s)