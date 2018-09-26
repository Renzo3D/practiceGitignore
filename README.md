# practiceGitignore

This is a simple practice that helps me understand how .env and .gitignore work together.

I learned that the write syntax for .env is capital letter and separated by a underscore, as well as quote are not needed after equals.

  ex:
    @ .env file
    MY_SECRET_PASSWORD = inHereCanGoAnyAPIKey-or-AnyInformationThatDoesnt-need-to-be-Expose.

in order to invoke our secret password in our js file, We have to put in the top of our file the follow. require('dotenv').config()
we have to also isntall npm i -u dotenv for that requirement to work.
once installed we can make the calls.

ex call:

@ js file (index.js)

console.log(process.env.MY_SECRET_PASSWORD)

Finally, before pushing into github we have to hide .env and that when .gitignore come handy.

we create a file call .gitignore and insde that file we simply type the files that need to be hide./ .env contains our
sensitive information so we need to hide it.

ex :

@ .gitignore 

    .env
    
EXTRA INFORMATION THAT I NEED TO FIND OUT IF IT IS TRUE OR IT IS JUST LIKE THAT FOR USING WINDOWS.

I was trying to implement the .env inside the .gitignore using the command line (for hours) and didnt work, .env was still showing up. 
EX:

created .env like this.
    touch .env
created .gitignore and add .env to it.
  echo '.env' > .gitignore
  
 everything looked find. But when pushing in github it will still show my env file. I tried multiple times in different ways.
 The only way that it worked was if I create the files and implement them individually and manually from VSCode. 

