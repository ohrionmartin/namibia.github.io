# New Placeholders Feature

 So we have a new feature in JCB version 2.9. 14 It's the latest release if you look at the release notes Added the new placeholder area for Global And component level placeholders now Those of you did know did know that JCB already has a few placeholders [00:00:26](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m26s) Which you can use across The System If I have to show you those in the code They are as follow So once I've set of Place holders is the word component and this HHH is Basically It is the same as 3 of those and then again on this side Three of those [00:00:53](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m53s) So three opening angle brackets and three closing angle brackets That's what the hh the sorry no that's what the bbb And a ddd stands for Where is the hhh stands for hashes one two three of those the side And Three of those This side [00:01:18](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m18s) So those are placeholders that you know Should know about already and gives you the The possibility to Add component name lower case all Uppercase First Letter All uppercase And then with hashes as well as with Opening angle [00:01:38](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m38s) Brackets enclosing angle brackets So That's the first set of placeholders which You should know about already If not Then it's possibly The truth that you haven't watched Previous tutorials Which I would encourage you to do the other set is basically the view Placeholder [00:02:02](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m02s) The view has a few variations and it's not always available in every area depending on What the Area is So for example in the backend the admin area It has view and views For the list And again you have this hashes and you have the open Square Braces Bracket And they closing Square brackets And [00:02:31](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m31s) Again all lowercase then one uppercase and then all uppercase So it's variations of View Now the reason why you have the s at times is because there is A list View name And then there is the View name As the edit View Single View name [00:02:53](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m53s) And so These place holders are also available but just when you are busy working In the admin Admin View area So With regards to the site View area There is also a placeholder Let me see if I can quickly find that here Ok here it is So it has a capital S in front or a lower s [00:03:21](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m21s) So Again It's because we don't have a Different site view doesn't have a list view it can actually be a listview or it can be A Single View Based on the dynamic get So that's why there isn't really a difference So So we working with S View [00:03:41](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m41s) Uppercase and lowercase all uppercase again with hashes and with braces again We have this function to add the list option but you see It is actually the exact same Code so If there by some reason is a List Implementation somewhere It's really just replacing with With the same code So those are the custom Place holders or [00:04:11](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m11s) What's the word the core place holders That already exist in the system And They already were taking JCB to a place where We could achieve a lot of dynamic reusability Of use of Fields and all sorts of Other implementations But then came along The idea [00:04:36](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m36s) To actually be able to set our own place holders in the gooey Of JCB And to reuse them wherever we would like to Just like custom code with behave accept It's a string and not A code snippet so That's the major difference And it also doesn't come with an IDE Roundabout Editing [00:05:03](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m03s) Feature as custom code snippets do It's just a in place replacement behaviour So Let's go back to the IDE to show you that I mean Not the ID the the gooey JCB itself So in JCB there is now a place called Place holders And You can open that up [00:05:29](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m29s) And if you have imported some of my components you might have some values in here already If not it might have no values So we still having these 3 Open Square Brackets and closing Square brackets Surrounding our place holders if I was to create a new place holder And type in any word It it automatically adds The [00:05:56](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m56s) Brackets around the word An immediately starts a surge all across JCB To see if it's being used anywhere If not obviously it tells you it's not being used Now any word in this case I can add any type of string on this side So as long as it is a one-liner string it can really be anything It can have Dollar sign in it it can have brackets in it It can have multiple brackets in it It can have [00:06:31](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m31s) Even braces in it and again brackets and braces And it can have dollar signs in well It's supposed to If you find something and it breaks stuff Let me know in GitHub tell me about it it's a bug it's supposed to be able to To handle any type of string now I've said all that now let's see if it actually does like clicking save here Oh yeah So it kept it exactly that way [00:07:01](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m01s) Now That means where ever in my program I am you all let me just for safety add this as comment So it's basically a comment string It could have been a variable name it could have been another string now you might say why not just Type that string In that area Well You see JCB we are starting to embark upon A idea With I'm not sure how far it will go [00:07:32](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m32s) Or how wide or broad it will expand But it is the possibility of reusing code From your custom code area in different components In different views This often requires That certain little strings Be different But There is a place where passing a string at from every component becomes very tedious Because yes custom codes has this feature [00:08:03](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m03s) Where you can pass this string To the Code and then it updates that string in the code But There was this idea that we really don't want to be passing any string And yet have a Automated Updating string behaviour in custom code So This is where placeholders come in [00:08:26](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m26s) So if I save and close out of this I now have this new place holder any word And I can now Go to A component And let's say I'm gonna take this anthropometry component as an example And I'm going to just add this place holder here like that And [00:08:49](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m49s) Save and close this is in the helper class So I just added it to anthropometry now I'm also gonna add it to this Medical aid one Again the same place order like that save and close Now I know for this implementation what I'm showing you right now It might not be that exciting But I'm telling you if You start to sort of Think about the [00:09:17](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m17s) Greater implication For example if we were to Go to the dynamic code And for example get method get member This get member function oh wait I'm on the wrong place I'm talking custom code Now let's say which one I think I have This little dot trick which is just a little JavaScript That sort of runs and [00:09:47](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m47s) Populates a little dot Tick tick tick tick tick showing like there's a progress Just a little snippet Now It's being used quite a few places and I might want to use like for example Let's say Member profile I might be using member profile in more than one component And [00:10:16](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m16s) Now That means this specific Site view the specific site view is being used in different components Now If I want to have the code be different when used in One component Then used in another that's where placeholders really come in it's full strength So if I was to place that snippet here any word As an example And save and close this [00:10:47](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m47s) I now have in this little Nice little dot trick I have a placeholder which will Be replaced with This value But let's say I instead want to Have it be different in one of the components that uses that little dot Code snippet I can go to that specific [00:11:14](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m14s) Component And I can add That place holder here And Say not Like The other and now for this component This place holder will be Basically not like the other So now you have a placeholder with within this component behaves differently [00:11:39](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m39s) Then it does within other components And that's really where placeholders So let's compile this and see what happens I have a few here so we got medical aid I'm gonna compile that let's see I don't have it installed So I've have to first do coral This is a project Which we are planning to launch quite soon I'm quite excited about this project It's gonna be one of our proprietary projects Ok so what's happened here oh yeah [00:12:13](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m13s) We haven't set up the The path ok just Put it in Now so we gonna have to backup folder path setup now I can do anthropometry And have it Compile it's actually updating and placing all those Placeholders and stuff Ok so we gonna see the difference And then I'm also going to add the medical aid one Which is the one that doesn't have that overwrite [00:12:43](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m43s) So it should use the global Implementation Ok so now with basically added These two Components to our Joomla website And We have used placeholders That actually Target A specific any word [00:13:06](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m06s) And we've placed that In those components helper classes And also within 1 Custom codes snippet Called Little nice little dot trick Now to see in which of those components where there's little nice little dog trick is going to appear It's basically gonna be in the member profile of Corel So Yeah that means we'll go look and see what it did [00:13:37](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m37s) So first I'm going to open the helper class Of coral It's this one here And then Scroll down to that where that snippet should have been added So in the anthropometry component it set not like the other because we added the overwrite Then in the medical aid component it added those That's very strange string A typed out And in the coral component Nice little dot trick [00:14:08](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m08s) It also added that little Snippet Now to show you how easy it is to overwrite this again on a component level Let me open this up Let me go to the components And to Coral An add a that snippet in here And That [00:14:33](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m33s) Easy Save and close And then we compile that one again Now we open the IDE again And that easy So That is the power of placeholders it really replaces only from where the placeholder starts to where it ends. It means you have the ability to change that little text to have the ability to Change You know [00:15:09](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m09s) This Yes you actually able to Change even the little dot You add a space Or I'm not sure about the Space one That might be over eager but The reality is it's really powerful you're able to anywhere add a dynamic string Which you then can overwrite on a component level [00:15:32](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m32s) So yes I hope you find it very useful Because I am finding it at this stage I have components that Actually Run together or How can I say And all these components build on top of coral Coral Itself is a Sort of Central [00:15:55](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m55s) Integration hub if you will Where all these components you know connect into Coral And create Exciting kind of Interface So that means I often need to rename certain values differently just based On The actual component [00:16:17](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m17s) And This way I'm able to have that kind of placeholder Power And replacing it and have the same code snippet Across these components but just because it's now in this component is actually being updated differently Then it would in for example this one And yeah they are even more Implementations But I think this would be enough to get you going and help you understand Why we added placeholders [00:16:48](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m48s) And where we think it will be able to Take the JCB community With More creative abilities Right inside The The graphic interface Of JCB Well again As always thank you for watching [00:17:08](https://www.youtube.com/watch?v=USVLYu4ZLCc&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h17m08s) Let me know if you have any questions either in the comments or on the Forum You're most welcome.