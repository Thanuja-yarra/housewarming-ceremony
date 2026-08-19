first commit
second commit

GRUHA PRAVESHAM — INVITATION WEBSITE
======================================

WHAT'S IN THIS FOLDER
----------------------
index.html            The invitation page (home page)
error.html             Custom "page not found" page
readme.txt              This file
images/
  kalasham-entrance.png   Decorated entrance with kalasham, marigold garlands & rangoli
  marigold-toran.png      Marigold flower toran/garland reference
  pearl-toran.png         Pearl & marigold bunting reference

EVENT DETAILS USED ON THE PAGE
-------------------------------
Headline:  Gruha Pravesham (గృహ ప్రవేశం)
Date:      15th October
Venue:     Tiruvuru
Time:      Placeholder of 10:30 AM was used since no exact muhurtham
           time was given — open index.html and search for "10:30 AM"
           to update it, and add the year and full address once
           confirmed (search for "Tiruvuru" and "15th October").

HOW TO VIEW IT LOCALLY
------------------------
Just double-click index.html — it opens directly in any browser,
no server or installation needed.

HOW TO PUBLISH IT (STATIC HOSTING)
-------------------------------------
This is a plain static site (HTML + CSS + images, no build step),
so it works on any static host. A few free, easy options:

1) Netlify Drop (fastest, no account needed for a quick preview)
   - Go to https://app.netlify.com/drop
   - Drag this whole folder onto the page
   - You'll get a live link in seconds (create a free account to
     keep it permanently and set a custom URL)

2) GitHub Pages (good if you already use GitHub)
   - Create a new repository and upload all the files in this
     folder (keep the images/ folder structure as-is)
   - Go to Settings > Pages > set the source branch to "main"
     and the folder to "/ (root)"
   - Your site will be live at
     https://<your-username>.github.io/<repo-name>/

3) Vercel
   - Go to https://vercel.com/new
   - Import/upload this folder as a project
   - Deploy — no configuration is needed for a static site like this

4) Any traditional web host (cPanel, GoDaddy, etc.)
   - Upload the whole folder's contents into the public_html
     (or www) directory via FTP or the file manager
   - Make sure index.html sits at the root of that directory

ERROR PAGE (404)
------------------
error.html is a styled "page not found" screen matching the
invitation's design. Most hosts let you set it as the custom
404 page:
  - Netlify: rename it to 404.html and place it at the site root
    (Netlify auto-serves 404.html for missing pages)
  - GitHub Pages: also looks for a file named 404.html at the root
  - cPanel/Apache hosts: point the "ErrorDocument 404" directive
    (in .htaccess) to /error.html, e.g.
       ErrorDocument 404 /error.html

If you'd like, you can simply duplicate error.html and save a copy
as 404.html so it works automatically on Netlify/GitHub Pages
without any extra configuration.

CUSTOMIZING
------------
- Text and details: open index.html in any text editor and edit
  the wording directly — it's plain, readable HTML.
- Colors and fonts: all defined near the top of the <style> block
  in index.html under ":root" — change the hex values there to
  restyle the whole page at once.
- Images: swap the files inside images/ (keep the same filenames,
  or update the "src" paths in index.html to match new filenames).

That's it — the whole site is self-contained in this one folder.
