# Coder!
An example code blog site with a static HTML page generator based on [editor.js](https://editorjs.io/). The purpose of this site is to show off how you can create a "static site generator" with a static site!

Essentially new pages can be created on the site itself, then you just upload those new pages to your host, and you're good to go!

## Creating new pages

When you head to `/create-a-page` there is a tool that will let you input data, once you add some content, you can hit the button to export an HTML file with the content you added to the editor.

Functionally this just builds a string, then uses [filesaverJS](https://github.com/eligrey/FileSaver.js) to then export that string to a file. The process is relatively fragile, it requires you to leave the first heading block (since that becomes the filename), and there's probably other bugs, but the foundation is there to prove the point. 
