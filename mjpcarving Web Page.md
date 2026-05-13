# mjpcarving.art Web Page


The domain mjpcarving.art was purchased for 5 years from [godaddy.com](http://godaddy.com) mid 2025\. Since at this time there are no plans for this to be a commercial site it was a goal to put this together as cheaply as possible. I found free hosting at “[infinityfree.com](http://infinityfree.com)”. Username is [mark@penniman.net](mailto:mark@penniman.net), password is On2Narnia. URL is: [https://dash.infinityfree.com/accounts/if0\_36794951](https://dash.infinityfree.com/accounts/if0_36794951) . Log in with the username and password. In the center of the resulting web page ‘mjpcarving.art’ is listed. Select ‘Manage’. Every 3 months or so it is necessary to create and install a new free SSL certificate from “Let’s Encrypt”. When a new SSL is created it takes a while to process. 
Click on ‘File Manager’. The various files used are:   

htdocs/index.php \= initial web page, links to thumbnails  
\<\!-- index.php →  
\<\!doctype html\>  
\<html\>  
\<head\>  
\<link rel="stylesheet" href="style.css"\>  
\</head\>  
\<title\>Wood Carvings\</title\>  
\<center\>  
\<h1\>Marco's Woodcarvings\</h1\>  
\<image src="Carving Logo.jpg" width="410" height="540"\>\<br\>  
\<?php  
print "While still in high school Mark (Marco) got his first commercial woodcarving job. It was probably a referral through the art store where he worked. At that time he worked in trade for carving tools. The split between his own designs and following a design are about 50/50. Here and there he has done a few commercial jobs but for the most part woodcarving has been a source of recreation for him, as it is now in 2024\. (NOTE: this rudimentary website was created the same way Marco likes to do his carvings. By hand. The old fashioned way. No motorized tools)\<br\> \<br\> Exodus 31:3-5  
\\"I have filled him with the Spirit of God, with ability and intelligence, with knowledge and all craftsmanship, to devise artistic designs, to work in gold, silver, and bronze, in cutting stones for setting, and in \<b\>carving wood\</b\>, to work in every craft.\\" ";  
 	 ?\>  
 \<h1\>  
    \<p\>  
 \<a href="samples2.html"\>Samples\</a\>  
    \</p\>  
    \</h1\>  
\</body\>  
\</html\>

htdocs/samples2.html \= links to thumbnail pictures of carvings  
	Example:  
	\<\!-- sample2.html →  
\<\!doctype html\>  
\<html\>  
    \<head\>  
          \<link rel="stylesheet" href="style.css"\>  
    \</head\>  
\<body\>  
\<title\>Wood Carvings\</title\>  
\<center\>  
\<h1\>Marco's Woodcarvings\</h1\>  
   \<h3\>Woodcarvings over the years\</h3\>  
     \<a href="Carvings/ChurchSign.html"\>  
        \<img src="Carvings/1969-ChurchSign.jpg" alt="Freedom Church 1969" width="200" height="70" class="ImageBorder" /\>  
     \</a\>  
…  
      \<a href="Carvings/LIONSHEAD.html"\>  
         \<img src="Carvings/2025-LambLion.jpg"  alt="Lamb with Lion in its eye 2025" width="100" height="70" class="ImageBorder" /\>  
     \</a\>  
\</body\>  
\</html\>

htdocs/carvings/yyyy-name.jpg (or jpeg) \= image file, picture of the carving  
htdocs/carvings/name.html \= links to image file and has description:   
Example:  
\<\!-- Bellows2.html →  
\<\!doctype html\>  
\<html\>  
    \<head\>  
        \<link rel="stylesheet" href="../style.css"\>  
    \</head\>  
\<body\>  
   \<title\>Wood Carvings\</title\>  
   \<center\>  
       \<img src="2000-Bellows2.jpg"  alt="Bellows with Family Crest 2000" height="70%"\>  
       		      \<br\>  
     	\<figcaption\>  
   	    2000-Bellows2.jpg rendition of the Penniman family crest. Executed in Philippine mahogany.  
	\</figcaption\>  
 	   \</figure\>  
\</body\>  
\</html\>  
htdocs/style css \= style document that effects whole webpage  
body {   
    color: brown;  
    background-color: tan;   
   }  
h1 h3 {   
    color:\#381c07ff;   
    }  
p {  
    color: brown;   
  }  
img.ImageBorder {  
    border: 5px solid \#555;  
    padding: 1px;  
    /\* border-style: solid black;  
 	  border-width: 3px; \*/  
}

A new woodcarving was added to the website but the change didn't show. Here is the resulting Grok dialog:   
The most common reasons for a new image not showing up on Infinity Free (while others do) are straightforward and fixable. Here are the likely culprits, in order of probability:  
1\. Case Sensitivity (Very Common on Infinity Free)  
Linux-based servers (like Infinity Free) are case-sensitive.  
photo.jpg is not the same as Photo.JPG, photo.JPG, or PHOTO.jpg.  
Same for folder names: images/ vs Images/.  
Fix:  
Check the exact filename and folder name in your File Manager or FTP.  
Update the \<img src="..."\> in your HTML to match exactly.  
Or rename everything to lowercase (e.g., new-carving.jpg and images/) for simplicity.  
2\. File Upload Location or Path Issue  
All web files must be inside the htdocs folder (or a subfolder of it).  
If you uploaded the new image to the root or a different folder, it won't work.  
Relative paths in your HTML must be correct.  
Fixes to try:  
Confirm the image is in the same folder structure as the working thumbnails (e.g., if thumbnails are in htdocs/images/, put the new one there too).  
In your HTML, use a relative path like:  
\<img src="images/new-carving.jpg" alt="Wood carving"\>  
(Adjust based on your actual structure. Use ../ if it's one folder up.)  
Test the direct image URL in a new browser tab (e.g., https://your-site.infinityfreeapp.com/images/new-carving.jpg). If you get 404/Not Found, the path or upload is wrong.  
3\. Browser Cache  
Your browser may be showing an old cached version of the page without the new image.  
Quick fix: Hard refresh with Ctrl \+ F5 (or Cmd \+ Shift \+ R on Mac). Or open the page in an incognito/private window.  
4\. Filename Problems  
Spaces, special characters, or very long names can cause issues.  
Very large files might exceed limits or fail to upload properly.  
Recommendation: Rename to something simple like carving-01.jpg (lowercase, no spaces, short).  
5\. Other Quick Checks  
File actually uploaded? Double-check in the Infinity Free File Manager that the file is there and has a reasonable size (not 0 KB).  
Image format: Try saving as .jpg or .png (ensure the extension matches your HTML).  
HTML code: Make sure the \<img\> tag is correct and not missing quotes or has typos. Example:  
\<img src="images/new-carving.jpg" alt="Description of carving" width="200"\>  
Permissions: Usually not an issue, but in File Manager, the file should be readable (e.g., 644).  
Debugging Steps  
Open your page, right-click the broken image area → Inspect (or Inspect Element).  
Look at the \<img\> tag and the Network tab for errors (404, 403, etc.).  
Test the full image URL directly.  
If you share:  
Your site URL (if public)  
The exact \<img src="..."\> line for the new image  
The folder structure (e.g., where the HTML is and where the image is)  
I can give more specific advice. These issues are extremely common on Infinity Free, and one of the above almost always solves it. Let me know what you find\!

5/11/2026 MJP attempted to add another item to the web page and found it didn't work. Ugh. Much digging and trial and error revealed that the were 2 samples2.html files, one in htdocs and one in htdocs/Carvings. The one in htdocs was bogus, but the one in htdocs/Carvings had entries that pointed to the wrong place for the *.html and *jpg files. MJP made the corrections, tested the site and was satisfied. The changed were put in git. 
