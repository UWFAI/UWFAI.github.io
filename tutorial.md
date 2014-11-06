## Editing the Website
### Tutorial for UWF AI Lab Members

The student run UWF Artificial Intelligence Group [website](https://uwfai.github.io) was created to have an aesthetically pleasing web presence, independent of [uwf.edu](uwf.edu), to show off student projects and activities. 

The site is hosted on [Github Pages](https://pages.github.com/), a free hosting site provided by [Github](https://github.com/). Github is the web front of [git](http://git-scm.com/), an open source command line [version control](https://en.wikipedia.org/wiki/Revision_control) tool created by Linus Torvalds.

Version control is how programmers manage discrepencies between files, submit their contributions and scrutinize file histories to find bugs. Version Control is kind of like this:

![Version Control](http://teslamondo.files.wordpress.com/2014/05/http___makeagif-com__media_5-05-2014_8uphvq.gif?w=300)

For _some_ reason... it works.

It's an essential skill that anyone planning to program for a living will need to learn. If it all seems too intimidating however, this tutorial will illustrate several other methods to contribute to the website.

### The Page

[Github Pages](https://pages.github.com/) is a trending service for developer and project pages and offers succinct _urls_, the tech-centric **_io_** top-level domain and the _github_ service name in the rear position. The html, css and javascript are hosted in the user or organization's Github _repository_ (folder), Github Pages then displays that content at the specified _someURL_.github.io

The current site was implemented with [Bootstrap](http://getbootstrap.com/), a mobile first, responsive javascript library. Boostrap adjusts to screensizes so that, regardless of platform, the content looks good. A landing page [template](http://startbootstrap.com/) was used to implement the _modern_, continuous scrolling content style.

To recap: 

* Github houses the code
* The page is displayed on Github Pages (~~~.github.io)
* The page uses the Bootstrap JS library and a Bootstrap template.


### Thats great but how do I change it?

Ways to contribute (_From Social to Technical_) :

 * Make a verbal / written request
 * Browser based editing
 * Command line


#### Verbal Request

Simple as that. Talk to an officer about content you think should be included. Digital media can be submitted via email, dropbox, usb... however you can deliver it. Even if you don't want to dig in to the html, suggestions on structure, content and aesthetics are welcome from all members.

There is a generic Github user **_UWFAIGroup_**, which is the owner of the site repository, this account can serve as a general access user to add, edit and remove content from the site. The access to this user account will also help facilitate transitions between AI Group Officers, as well as give new members permissions to edit the site.

#### Well, maybe a little HTML

Great! All you'll need is your very own github account. All it costs is an email address. If you are still on the fence about creating one, you might want to read about how a lot of companies now think that [Github is your resume](http://anti-pattern.com/github-is-your-resume-now). There is also a pretty neat [student pack](https://education.github.com/pack) of free stuff you can get if you use your _.edu_ email. 

After you've created your account, let an officer know and you can be added as an owner / contributer to the site. Once that has happened, you'll be able to make edits to the code base so that the description of your project is as _flowery_ as you like. 

Webpages use HTML to structure the order and importance of content on a site. CSS is used for controlling the style of the content, such as fonts, sizes and colors. Javascript ties everything together, moves content around to meet the screen size, and makes menus expand and retract.

Unless the group desides to try another template or javascript framework, the majority of contributions will happen in the [index.html](https://github.com/UWFAI/UWFAI.github.io/blob/master/index.html) file.


### Finally the good stuff

The content section of the site features an image and a text description. Each subsequent block swaps from left to right in orientation. These blocks can be extended indefinitely and are a great place to add new content for members projects and studies. The only _finicky_ bit is making sure not to break the left <-> right alteration.

Here is an example of a content block:

```html
    <!-- /.content-section-b -->
    
    <div class="content-section-a">

        <div class="container">

            <div class="row">
                <div class="col-lg-5 col-sm-6">
                    <hr class="section-heading-spacer">
                    <div class="clearfix"></div>
                    <h2 class="section-heading">AI Lab</h2>
                    <p class="lead">The AI Research Group meets and works in the AI & Project Lab in the SSE building 4, room 148.<br>
The lab has 6 highly-capable all-in-one desktops, multiple cabinets for storage, a large overhead monitor for presentations, and several workbenches.  The lab is also furnished with two iRobot Create robots, a LEGO Mindstorms kit, and a number of IntelliBrain-Bot Deluxe robots. </p>
                </div>
                <div class="col-lg-5 col-lg-offset-2 col-sm-6">
                    <img class="img-responsive" src="img/proj_2.jpg" alt="">
                </div>
            </div>

        </div>
        <!-- /.container -->

```

The text content between ```<p class="lead">```  and  ```</p>``` can easily be modified after a copy-paste. To change the image next to the description, you will need to upload it to the **img** folder in the [repository](https://github.com/UWFAI/UWFAI.github.io). Then just insert ```src=img/YOURIMAGENAME.jpg```.  

Easy as **π**.