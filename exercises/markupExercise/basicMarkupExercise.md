# Web Publishing Exercise 

## Overview & Goals

In today's exercise, you'll use your IDE of choice (Adobe Brackets, Visual Studio Code, etc.) to create some web pages. Much of the HTML I'm asking you to create was already covered in the HTML Essential Training tutorial, so this should primarily be review.

## Setting Up Your Folders and Files

On your computer (or on a USB drive) create a folder called RIT Web. Inside that folder, create a folder called www. Inside of the www folder, create a folder called igme110. And inside of the igme110 folder, create a folder called media. The www folder represents your www directory on 'banjo.rit.edu'. The igme110 folder is where all of your exercises and projects for this class will be stored. 

![Example File Structure](110homepage-folderstructure.png)


## Creating Your Class Home Page

Using VS Code (or your HTML editor of choice), create a new HTML file in the igme110 folder called index.html. 

In the head of the document, add this content to the title element (using your name, of course): `<title>Elizabeth Lawley's IGME 110 Page</title>`

In the body of the document, add a level 1 heading element containing your name. Below that, add a paragraph element that that includes a few lines about yourself. Save the file. 

Open a web browser, and in the browser use the File-->Open command to locate and display the index.html file you just created. (Or, if you have previewing capability in your editor, you can use that.) It should look something like this:

![Screenshot of index.html page](110homepage-1.png) 

## Adding an Image

Find a Creative Commons-licensed image on the web, or an image that you own the rights to, that you’d like to include on your page. Save it in your igme110 folder. 

You’re going to add code to your HTML to display the image properly on the page. In Komodo edit, put your cursor after the heading with your name, but before the first paragraph of text. (If there’s not a blank line there already, you can add one, to make the code easier to read.) Type in `<img src="" alt="">` (or, use the Emmet shortcut by typing `img` and pressing tab). 

Between the quote marks following src, you're going to add the *relative* path to the image you downloaded. Because the image is in the same directory as your html file, the relative path is just the file name--if you don’t provide any other information besides a file name, the browser will assume that the image is in the same directory as the HTML file it’s displaying. My image file is called dog.jpg, so my tag would now look like this:
```<img src="dog.jpg" alt="" />```

Between the quote marks following alt, you’re going to add text that will display if the browser is unable to display images. My tag now looks like this:
```<img src="dog.jpg" alt="Morgan the dog” />```

Save your file, go back to the browser window that you used to view it in the last section, and reload the file. It should now look something like this:

![index.html with image added](110homepage-2.png) 

Add a paragraph of text after the title, describing the image. Include information about where you got the image--including a link back to the source if it's not an image you took yourself.
 
If your image isn’t showing up properly, ask for help now! (If it’s much too big to display properly on the page, try finding and downloading a smaller image from the web. )

## Relative References to Other Directories

As your web site gets bigger, keeping all your files in the same directory makes it harder to keep them organized. Web developers typically have different directories for different parts of their site, and also often  keep images in a separate directory. You created a media folder in your www directory, and that’s where we’re going to put the images you use on your site. 

On your computer, open the igme110 folder you created. Move your image file from igme110 into the media folder. Your structure should look like this:

![index.html with image added](110homepage-filestructure.png) 

Now try reloading your page in the browser again.  If you followed the directions properly, the image won’t load now. The browser is still looking for it in the same directory as the HTML file, but it’s not there. We need to tell the browser how to find the image, using a relative path. 

In your html file, change the img tag so that it looks like this (using your image information, of course):
   ```<img src="media/dog.jpg" alt="Morgan the dog" />```

This tells the browser to look in the media folder that’s inside the igme110 folder. Reload the page in the browser to see if it worked. The image should show up again. (If not, ask for help!)

## Creating and Linking to a Second Page

Using your HTML editor, create a new HTML 5 file. Save it with the name page2.html. Give it a title of “Your Name’s Second Page.” (Put that in the title tag, as well as in a level 1 heading on the page.) 

Add an image to this page, as well, and a paragraph of text with whatever content you'd like. 

Add a second paragraph with a link back to your index.html page. Because we’re using relative links, and because the file is in the same igme110 directory, you only have to specify the file name, like this:
   ```<p><a href="index.html">My First Page</a></p>```

Go back to your index.html file, and add a link at the end of that page to your new HTML file, like this:
```<p><a href="page2.html">My Second Page</a></p>```

Here's an example:

![Screenshot of Example Page 2](110homepage-3.png)

In your web browser, reload your index.html page, and make sure the links between your pages work properly. If they don’t, ask for help! 


## Due Date
You must have this exercise completed by next class on Thursday, September 10th. Upload your files, in a zip folder to the dropbox  `Exercise - HTML` and making sure that the files are present and include the requested components. 
