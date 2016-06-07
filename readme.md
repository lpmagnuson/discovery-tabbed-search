Tabbed Search for WorldCat Local / Discovery
============================================

To use:  upload search.html and style.css onto a web server.  Replace all search form action URLs with the URL of your WorldCat Local / Discovery instance.  Update databaseList, format/subformat, and scope input parameters with the parameters you want to be searched.

![Basic Search Box](https://raw.githubusercontent.com/lpmagnuson/discovery-tabbed-search/master/images/search1.png)

####With Dropdown menus for scope selection
Use the files in the dropdown folder to give your users a choice of your local library scope(s) or "Libraries Worldwide".

![Search box with dropdowns](https://raw.githubusercontent.com/lpmagnuson/discovery-tabbed-search/master/images/dropdown.png)

####Hosting with LibGuides
If you don't have a web server, you can use the combined.html file.  Edit form action URLs, search parameters, and CSS as desired.  In LibGuides Admin, go to Content > Assets.  Upload combined.html as a Document.  Note the ID of the document, and construct a URL that looks like this:

http://libguides.yourschool.edu/ld.php?content_id=22044474   

Use this URL to construct your embed code (see below).

####Embedding a search box
Once the code is on a server somewhere, you can create an iframe for use embedding in LibGuides or other web pages, for example:
```
<p style="text-align:center"><iframe frameborder="0" height="250" scrolling="no" seamless="" src="
http://www.example.com/search.html" width="450"></iframe></p>
```
Just replace http://www.example.com/search.html with the location of the search.html page on your server.

####License
GNU GPL Open Source License.  &copy; PALNI 2015.
