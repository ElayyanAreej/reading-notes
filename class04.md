# Read: 04 - HTML Links, CSS Layout, JS Functions
## HTML Links
Links allow you to move from one web page to another.

Links are created using the ``` <a> ``` element. Users can click on anything between the opening ``` <a> ``` tag and the closing ``` </a> ``` tag. You specify which page you want to link to using the *href* attribute.

![a](https://i0.wp.com/learnwebanalytics.com/wp-content/uploads/2018/12/What-Is-An-Anchor-Tag.png?fit=1211%2C501&ssl=1)

👉
*Notes* 

-An **absolute URL** starts with the domain name for that site, and can be followed by the path to a specific page.

-When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a **relative URL**.

### Directory Structure

On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. *Folders* on a website are sometimes referred to as *directories*.

👉
*Notes* 

-The top-level folder is known as the **root folder**.

-The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called **index.html**.

-If all of the files in your site are in one folder, you simply use the
file name for that page.

-If your site is organized into separate folders (or directories), you need to tell the browser how to get from the page it is currently on to the page that you
are linking to.

-To create a link that starts up the user's **email** program this time the
value of the *href* attribute starts with *mailto:* and is followed by
the email address you want the email to be sent to.

-**target** attribute Specifies where to open the linked document.*_blank*	Opens the linked document in a new window or tab.
```
<a target="_blank|_self|_parent|_top|framename">
```
###  link To A Specific Part Of The Same Page
You can link to a specific part of a page, you need to identify the *points* in the page that the link will go to.You do this using the *id attribute* (which
can be used on every HTML element).

```
<h2 id="C4">Chapter 4</h2>
// Then
<a href="#C4">Jump to Chapter 4</a>
```

###  link To A Specific Part Of Another Page
f you want to link to a specific part of a different page (whether on your own site or a different website) you can use a similar technique.
```
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```

```
<a href="http:/www.htmlandcssbookcom/#bottom">
```
## HTML Layout