# Blog enabled Jekyll Based Personal Webpage
 
This is a personal webpage based on Jekyll and Liquid inspired from the [Barry Clarks Jekyll-Now](https://github.com/barryclark/jekyll-now) Repository.

<img src="https://user-images.githubusercontent.com/29497016/120059989-ad3a0e80-c072-11eb-886d-710ea1f6783d.png" alt="Home Page Preview" width="500"/>

---

### Key Feature
All the personal information including projects and other activities go into the YAML files in the _data_ directory and _config.yml_ file making the web page very easy to customize.

There are five YAML files in _data_ directory and _config.yml_ file in the root folder and their content are as follows:

* _`config.yml`_ : Contains basic information of the user, email, and social media handles.

* _`navigation.yml`_ : The list in this file defines the navigation pane of the website. Currently there are 5 tabs availaible in the list. Any of the tabs can be disabled by commenting or deleting the entry corresponding to that tab. To add another tab, an entry corresponding to the name of the tab and associated webpage address needs to be made. 
![NavigationPane_NewEntry](https://user-images.githubusercontent.com/29497016/120059947-56343980-c072-11eb-867e-ae2ad85a6955.PNG)


* _`home.yml`_ : The content for the homepage is stored on this page. Content of the _- Intro_ entry takes in raw HTML code for the description to be shown on the home page and can easily be modified to give personal style to the description.

* _`projects.yml`_ : This file has three sections corresponding to Research Projects, Technical Project, and Miscellaneous Projects. New entries corresponding to the projects is to be made in _sub_ directory of respective section. Options availaible for project entries in different sections are shown in the sample project entries. Kindly note that sequence of projects is important and project that appears first in the list will appear first on the webpage.

* _`publications.yml`_ : This data file is similar in structure to the _projects.yml_ file however the _sub_ directory is under the _year_ entry to display the list in chronological order on the webpage. Entries for a specific year are to be made in _sub_ directory of that year. Options availaible corresponding to different sections are shown in their respective examples.

![PublicationPage_Entries](https://user-images.githubusercontent.com/29497016/120059952-5d5b4780-c072-11eb-831f-fb2185353498.PNG)


* _`extras.yml`_ : The page enlists the hobbies and other experiences and can be customized using the options availaible in the sample entries.

---

The structure of the webpage is quite intuitive and adaptable and can easily be modified to suit ones preferences. Descriptions of the folders and files are as follows:

* _`_data`_ : As explained above, it contains most of the personal data content displayed on the webpage.
* _`_drafts`_ : Drafts of blog post.
* _`_posts`_ : Published posts with format as yyyy-mm-dd-Title.md
* _`_includes`_ : This folder contains files with HTML codes (correspinding to metadata, navigation pane, and footer) that are used on every page.
* _`_layouts`_ : Contains layout files which define the structure of the webpage by placing codes from _includes_ folder at appropriate locations on the page.
* _`_sass`_ : Stores all the css code in .scss format which is compiled using _styles.css_ file in _/assets/css_ folder.
* _`_assets`_ : Contains css, images, and other files used on the webpage.

Structure in which content from the YAML files in _data_ folder is displayed is defined in corresponding HTML files in the root directory.

---

I would love to hear suggestion and improvements, kindly reach out to me on my [email](@mailto:Apoorv9600@gmail.com) or raise an issue.

Thank You.







