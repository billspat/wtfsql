## What They Forgot to teach you about SQL

***The real and practical guide to using databases with your data science, academic or research project* **

SQL has been around for a long time, and databases are everywhere.  There is one in your phone.   There are many many good tutorials on the SQL language, and the SQL language is not hard to learn.  If that's true, then why don't we see more adoption of SQL in academia or for research data?  I believe it's not the fault of SQL but because the following  are **not** clearly explained if even discussed:

-   how to model data using the linked tables (the relational model)
-   understanding what a data server is and how to maintain one for your work group for collaboration
-   if the data is not from an instrument or must be edited manually (as some portion of most of our data is), how to get the data in to the database or even harder, a standard data entry process.

Most books and sites that attempt to teach you the SQL language[^1] do not talk about these practical considerations. In addition the tutorials cover many of the database engines but not all and they don't put them in great context.

Note: I totally stole the idea for this name from Dr. Jenny Bryan's book "What They Forgot to Teach You About R" hosted on  https://rstats.wtf

### Building

This is built using [Quarto](https://quarto.org), a mark-down based literate programming system.   It uses the [Quarto 'book'](https://quarto.org/docs/books/) system (see `_quarto.yml` ) which compiles the qmd files into the `_book` folder and makes basic HTML.  


For more information, the Quarto documentation. the code blocks use mostly R, as this currently is the only supported way that Quarto can run straight SQL in code blocks.   
 
 
 ### install using R
 
 this project uses [renv](https://rstudio.github.io/renv/articles/renv.html) to manage packages, which can be used to install 
 
 ```R
 install.packages('renv')
 renv::restore()
 ```
 
 ### Build using R 
 
 really, the quarto docs are a better place to learn about this, but I hear this is what you do: 
 
 ```R
 quarto::render()
 ```

to build the book, which runs the code in the code blocks.   




[^1]: Ok, I know that saying SQL Language is saying "Structured Query Language Language" so sue me.  the word SQL is used also for the database server that can interpret SQL, sometimes the database instance and the box it runs on, and in the product SQL Server &trade;   So SQL Language is to clarify the L and not the server.   Feel free to use a greasemonkey script to correct that as you read.   
