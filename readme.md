Tabbed Search for WorldCat Local / Discovery
============================================

To use:  upload search.html and style.css onto a web server.  Replace all search form action URLs with the URL of your WorldCat Local / Discovery instance.  Update databaseList, format/subformat, and scope input parameters with the parameters you want to be searched.

![Basic Search Box](https://raw.githubusercontent.com/lpmagnuson/discovery-tabbed-search/master/images/search1.png)

####With Dropdown menus for scope selection
Use the files in the dropdown folder to give your users a choice of your local library scope(s) or "Libraries Worldwide".

![Search box with dropdowns](https://raw.githubusercontent.com/lpmagnuson/discovery-tabbed-search/master/images/dropdown.png)

####Hosting with LibGuides
If you don't have a web server, you can use the combined.html file.  Edit form action URLs, search parameters, and CSS as desired.  In LibGuides Admin, go to Content > Assets.  Upload combined.html as a Document.  Note the ID of the document, and construct a URL that looks like this:

http://yourschool.libguides.com/ld.php?content_id=22044474   

Use this URL to construct your embed code (see below).

NOTE: If you need to use https (e.g., you are embedding your search box in a page that requires or loads https by default, which is always recommended), you can only use https if your LibGuides domain uses libguides.com.  If you have a custom LibGuides domain (e.g., libguides.yourschool.edu), you cannot use https with these URLs and thus your search box cannot be embedded into secure web pages.  If you are in this situation, you may wish to seek out a low-cost web host or a host that offers free hosting for non-profits.  More information about the use of https with LibGuides custom domains is available from [SpringShare help](http://guidefaq.com/a.php?qid=43801).  

####Embedding a search box
Once the code is on a server somewhere, you can create an iframe for use embedding in LibGuides or other web pages, for example:
```
<p style="text-align:center"><iframe frameborder="0" height="250" scrolling="no" seamless="" src="
http://www.example.com/search.html" width="450"></iframe></p>
```
Just replace http://www.example.com/search.html with the location of the search.html page on your server.

Be sure to include a height parameter of at least 250px (especially in LibGuides) for responsive optimization.

####Interested in Data Visualization?
This search box code is released open source and is free to use, but consider supporting its author (me) by buying a copy of the [LITA Guide to Data Visualization](https://www.amazon.com/Data-Visualization-Visual-Storytelling-Libraries/dp/1442271108).  Thanks!

####License
GNU GPL Open Source License.  &copy; PALNI 2015.


