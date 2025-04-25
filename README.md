# eecs-281---project-3--sillyql-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/eecs-281-project-3-sillyql-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;76496&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS 281&nbsp;-  Project 3- SillyQL Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<h1><a name="_Toc27047"></a>Overview</h1>
A relational database is the most common means of data storage and retrieval in the modern age. A relational database model stores data into one or more tables, where each table has columns and rows. The columns represent a value that can be attributed to an entry (such as “color”, “name”, or “ID”) and the rows represent individual entries or records (such as “Paoletti”, “my cat”, or “BBB 1695”).&nbsp; You may find it helpful to think about <em>rows as</em>​ <em> objects and columns as descriptors for those objects</em>​. For instance, the table pictured to the right has each row corresponding to a car (a data type), and the columns group a car’s vendors, model, etc. such that this information can be easily retrieved. Rows in relational databases are also called records or tuples, but in this project we will use the terminology “row” for consistency. <strong>Rows in Project 3 are not guaranteed</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong> to be unique. </strong>

&nbsp;

However, a database can do much more than simply store information. You must be able to retrieve specific information in an efficient manner. For relational databases, the structured query language

(SQL)&nbsp; is a defined method of retrieving information programmatically. It looks like real English, where a valid command for the above table could be “SELECT Model from Cars marketplace where Price​ &lt; 30000”, which would return a list of models [Corvette, Corvette, Malibu, Malibu, Malibu]. Note that​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the version of SQL used in this project is simplified and modified somewhat from a typical query language.

&nbsp;

For this project, you will write a program to emulate a basic relational database with an interface based on a subset of a standard query language. Your executable will be called silly​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; . You will gain​&nbsp; experience writing code that makes use of multiple interacting data structures. The design portion of this project is significant; spend plenty of time thinking about what data structures you will use and how they will interact.

&nbsp;

&nbsp;

<h1><a name="_Toc27049"></a>Learning Goals</h1>
<ul>
<li>Selecting appropriate data structures for a given problem. Now that you know how to use various abstract data types, it’s important that you are able to evaluate which will be the optimal for a set of tasks.</li>
<li>Evaluating the runtime and storage tradeoffs for storing and accessing data contained in multiple data structures.</li>
<li>Designing a range of algorithms to handle different situations</li>
<li>Evaluating different representations of the same data.</li>
</ul>
<h1><a name="_Toc27050"></a>Project Specification</h1>
<h2><a name="_Toc27051"></a>Program Arguments</h2>
silly​ should accept the following (both optional) command line arguments:

<h5>● -h, –help</h5>
This causes the program to print a helpful message about how to use the program and then immediately ​exit(0)​.

<h5>● -q, –quiet</h5>
This causes the program to run in quiet mode. In quiet mode, your program will run very similarly to normal, except that it will print only numerical summaries of the rows affected by the command, not any of the actual data. Quiet mode exists so that we may stress test your program without overloading the autograder with too much output. This flag only affects the JOIN and PRINT commands and specific instructions for quiet mode output is given for these commands. Otherwise, if there is no mention of quiet mode with respect to a given piece of output, you may assume it is always printed. You can implement this feature last; with a well-built project, adding this functionality should be very simple.

You may find it simpler to check for these flags directly rather than use getopt.

<h2><a name="_Toc27052"></a>User Commands</h2>
On startup, your program should prepare to accept commands from the user. These commands may or may not take the form of redirected input.&nbsp; Your program should print ​”% “​ as a prompt to the user before reading each command.&nbsp; Commands are specified by a command keyword followed by a <em>required</em>​ space character and then the command-specific arguments where applicable. For example, to delete the rows from ​table1 ​where the entries in column ​name​ ​equal ​“John”, one would input:​ DELETE FROM table1 WHERE name = John​.&nbsp; Appendix A contains an example program illustrating the use of these commands.

<h2><a name="_Toc27053"></a>Table Manipulation Commands</h2>
In the following commands, output examples are given.&nbsp; These examples are cumulative throughout the table manipulation command part of the spec (i.e. the table created in the example output for the CREATE command is the same table that DELETE is performed on during the delete command, and so on, so you can follow the state of the table throughout the spec).

<h3><a name="_Toc27054"></a><strong>CREATE – add a new table to the database </strong></h3>
Syntax: ​ ​CREATE &lt;tablename&gt; &lt;N&gt; &lt;coltype1&gt; &lt;coltype2&gt; … &lt;coltypeN&gt; &lt;colname1&gt; &lt;colname2&gt; … &lt;colnameN&gt;

Creates a new table with ​&lt;N&gt;​ columns (where ​N​ &gt; 0). Each column contains data of type ​&lt;coltype&gt; and is accessed with the name ​&lt;colname&gt;​. Table names and column names are guaranteed to be space-free. No two columns in the same table will have the same name (you do not need to check). Valid data types for ​coltype​ are {double, int, bool, string​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​}. This table is initially empty.

Output: Print the following on a single line followed by a newline:

New table &lt;tablename&gt; with column(s) &lt;colname1&gt; &lt;colname2&gt; … &lt;colnameN&gt; created

Possible errors:

<ol>
<li>A table named ​&lt;tablename&gt;​ already exists in the database</li>
</ol>
Given the following as input:

CREATE 281class 3 string string bool emotion person Y/N

The output should be:

New table 281class with column(s) emotion person Y/N created

&nbsp;

<h3><a name="_Toc27055"></a><strong>INSERT INTO – insert new data into table </strong></h3>
Syntax:

INSERT INTO &lt;tablename&gt; &lt;N&gt; ROWS&nbsp; &lt;value11&gt; &lt;value12&gt; … &lt;value1M&gt;

&lt;value21&gt; &lt;value22&gt; … &lt;value2M&gt;

…

&lt;valueN1&gt; &lt;valueN2&gt; … &lt;valueNM&gt;

&nbsp;

Inserts ​&lt;N&gt;​ new rows (where ​N​ &gt; 0) into the table specified by ​&lt;tablename&gt;​.​ The number of values in each line after the first, or M in the example, is guaranteed to be equal to the number of columns in the table. The first value, ​&lt;value11&gt;​, should be inserted into the first column of the table in the first inserted row, the second value, ​&lt;value12&gt;​, into the second column of the table in the first inserted row, and so on.&nbsp; Additionally, the types of the values are guaranteed to be the same as the types of the columns they are inserted into. For example, if the second column of the table contains integers, &lt;value2&gt;​ is guaranteed to be an ​int​. Further, string items are guaranteed to be a single string of whitespace delimited characters (i.e. “​foo bar​” is invalid, but “​foo_bar​” is acceptable).

Output: Print the message shown below, followed by a newline, where ​&lt;N&gt;​ is the number of rows inserted, ​&lt;startN&gt;​ ​is the index of the first row added in the table, and ​&lt;endN&gt;​ ​is the index of the last row added to the table, 0 based. So, if there were ​K​ rows in the table prior to insertion, ​&lt;startN&gt; = K​, and ​&lt;endN&gt; = K + N – 1​.

Added &lt;N&gt; rows to &lt;tablename&gt; from position &lt;startN&gt; to &lt;endN&gt;

Possible errors:

<ol>
<li>&lt;tablename&gt;​ is not the name of a table in the database</li>
</ol>
Given the following as input:

INSERT INTO 281class 8 ROWS happy Darden true stressed students false busy office_hours true stressed students true stressed Paoletti true happy Darden true happy Sith true victorious Sith true

The output should be:

Added 8 rows to 281class from position 0 to 7

&nbsp;

<h3><a name="_Toc27056"></a><strong>DELETE FROM – delete specific data from table </strong></h3>
<h6>Syntax:​ ​DELETE FROM &lt;tablename&gt; WHERE &lt;colname&gt; &lt;OP&gt; &lt;value&gt;</h6>
Deletes all rows from the table specified by ​&lt;tablename&gt;​ where the value of the entry in ​&lt;colname&gt; satisfies the operation ​&lt;OP&gt;​ with the given value ​&lt;value&gt;​.&nbsp; You can assume that ​&lt;value&gt;​ will always be of the same type as ​&lt;colname&gt;​. For example, to delete all rows from ​table1 ​where the entries in column ​name​ ​equal ​“John”​, the command would be: ​DELETE FROM table1 WHERE name = John​.&nbsp; Or, to delete all rows from ​tableSmall​ where the entries in column ​size​ are greater than 15, the command would be: ​DELETE FROM tableSmall WHERE size &gt; 15​.​ For simplicity, ​&lt;OP&gt;​ ​is strictly limited to the set { ​&lt;, &gt; , =​ }.

Output (with example): Print the number of rows deleted from the table as shown below, followed by a newline:

Deleted &lt;N&gt; rows from &lt;tablename&gt;

Possible errors:

<ol>
<li>&lt;tablename&gt;​ is not the name of a table in the database.</li>
<li>&lt;colname&gt;​ is not the name of a column in the table specified by ​&lt;tablename&gt;</li>
</ol>
Given the following as input:

DELETE FROM 281class WHERE person = Darden

The output should be:

Deleted 2 rows from 281class

The search is case sensitive (which makes it easier to code): if we had deleted ​WHERE person = darden​, no rows would have been removed.

&nbsp;

<h3><a name="_Toc27057"></a><strong>GENERATE INDEX – create a search index on the specified column </strong></h3>
<h6>Syntax:​ ​GENERATE FOR &lt;tablename&gt; &lt;indextype&gt; INDEX ON &lt;colname&gt;</h6>
Directs the program to create an index of the type ​&lt;indextype&gt;​ on the column ​&lt;colname&gt;​ ​in the table &lt;tablename&gt;​, where ​&lt;indextype&gt;​ is strictly limited to the set {​hash, bst​}, denoting a hash table index and a binary search tree index respectively.&nbsp; Given the ​&lt;indextype&gt; hash​ on column &lt;colname&gt;​, the program should create a hash table that allows a row in the table to be found rapidly given a particular value in the column ​&lt;colname&gt;​. Given the ​&lt;indextype&gt; bst​ on column ​&lt;colname&gt;​, the program should create an binary search tree that allows rows in the table to be found rapidly given a particular value in the column ​&lt;colname&gt;. ​ ​<strong>Only one user-generated Index may exist per table, at any one time</strong>​. If an index is requested on a table that already has one, discard the old index before building the new one.

When ​bst​ is the specified index type, you should make use of a ​std::map&lt;&gt;​; when ​hash​ is the specified index type, you should utilize a ​std::unordered_map&lt;&gt;​.&nbsp; It is acceptable for both types to <em>exist</em>​ at the same time, but only one (at most) should be in use at any given time (i.e. contain data).

An index is a tool used in databases to speed up future commands. A ​hash​ index creates a hash table, which associates values in a specified column with a collection of rows in the table for which the index was created. Similarly, a ​bst​ index creates a binary search tree which associates values in a specified column with a collection of rows. Both are useful for different types of commands. In order to get the correct output in all cases, you must use an index when it is appropriate.&nbsp; ​<em>Further, you must remember to update your indices upon edits to the table</em>​. ​bst​ indices are ordered by ​operator&lt;​ for the type in the specified column.

Output:&nbsp; Print the message shown below, followed by a newline

Created &lt;indextype&gt; index for table &lt;tablename&gt; on column &lt;colname&gt;

Possible errors:

<ol>
<li>&lt;tablename&gt;​ is not the name of a table in the database.</li>
<li>&lt;colname&gt;​ is not the name of a column in the table specified by ​&lt;tablename&gt;</li>
</ol>
Given the following as input:

GENERATE FOR 281class hash INDEX ON emotion

The output should be:

Created hash index for table 281class on column emotion

Note that in this example, the user program should now have created an index of type hash table that maps from specific emotions of type string to rows in the table ​281class​,​allowing the program to search for all rows where ​emotion = happy​ quickly, among other things.

<strong>&nbsp;</strong>

<h3><a name="_Toc27058"></a><strong>PRINT – print specified rows&nbsp; </strong></h3>
Syntax:​ ​PRINT FROM &lt;tablename&gt; &lt;N&gt; &lt;print_colname1&gt; &lt;print_colname2&gt; … &lt;print_colnameN&gt; [WHERE &lt;colname&gt; &lt;OP&gt; &lt;value&gt; | ALL ]

Directs the program to print the columns specified by ​&lt;print_colname1&gt;, &lt;print_colname2&gt;, … &lt;print_colnameN&gt;​ from some/all rows in ​&lt;tablename&gt;​. If there is no condition (i.e. statement is of the form ​PRINT … ALL​), the matching columns from all rows of the table are printed. If there is a condition (i.e. statement is of the form ​PRINT … WHERE &lt;colname&gt; &lt;OP&gt; &lt;value&gt;​), only rows, whose ​&lt;colname&gt;​ value pass the condition, are printed. The rules for the conditional portion are the same as for the ​DELETE FROM​ statement. It is not guaranteed that the columns in the command are listed in the same order as they exist in the table, nor is it guaranteed that all columns will be listed. <strong>&nbsp;</strong>

<strong>The table must be searched as follows to ensure compatibility with the autograder: </strong>

<ol>
<li>If no index exists or there is a ​hash​ index on the ​<strong>conditional</strong>​ column, the results should be printed in order of insertion into the table.</li>
<li>If a ​bst​ index exists on the ​<strong>conditional</strong>​ column, the results should be printed in the order in the BST (least item to greatest item for ​std::map&lt;&gt;​ constructed with the default ​std::less&lt;&gt; operator), with ties broken by order of insertion into the table.</li>
</ol>
Output : Print the names of the specified columns, followed by the values of each of the specified columns in each row, separated by space.&nbsp; Every line should be followed by a newline.

&lt;print_colname1&gt; &lt;print_colname2&gt; … &lt;print_colnameN&gt;

&lt;value1rowA&gt; &lt;value2rowA&gt; … &lt;valueNrowA&gt; …

&lt;value1rowM&gt; &lt;value2rowM&gt; … &lt;valueNrowM&gt;

Once all the data has been printed, print the following, followed by a newline, where ​&lt;N&gt;​ is the number of rows printed:

Printed &lt;N&gt; matching rows from &lt;tablename&gt;

In quiet mode, do not print the ​&lt;print_colname1&gt;​s or any of the values. Print ​<strong>only</strong>​ the following: Printed &lt;N&gt; matching rows from &lt;tablename&gt;

Possible errors:

<ol>
<li>&lt;tablename&gt;​ is not the name of a table in the database.</li>
<li>&lt;colname&gt;​ is not the name of a column in the table specified by ​&lt;tablename&gt;</li>
<li>One (or more ) of the ​&lt;print_colname&gt;s are not the name of a column in the table specified by​ &lt;tablename&gt;​ (only print the name of the first such column encountered)</li>
</ol>
Given the following as input:

PRINT FROM 281class 2 person emotion WHERE Y/N = true

The output should be:

person emotion office_hours busy students stressed Paoletti stressed

Sith happy

Sith victorious

Printed 5 matching rows from 281class Or in quiet mode:

Printed 5 matching rows from 281class

&nbsp;

&nbsp;

<h3><a name="_Toc27059"></a><strong>JOIN – join two tables and print result </strong></h3>
Syntax:​ ​JOIN &lt;tablename1&gt; AND &lt;tablename2&gt; WHERE &lt;colname1&gt; = &lt;colname2&gt; AND PRINT &lt;N&gt;

&lt;print_colname1&gt; &lt;1|2&gt; &lt;print_colname2&gt; &lt;1|2&gt; … &lt;print_colnameN&gt; &lt;1|2&gt;

Directs the program to print the data in ​&lt;N&gt;​ columns, specified by ​&lt;print_colname1&gt;,

&lt;print_colname2&gt;, …&nbsp; &lt;print_colnameN&gt;​.&nbsp; The ​&lt;print_colname&gt;​s will be the names of columns in either the first table ​&lt;tablename1&gt;​ or the second table ​&lt;tablename2&gt;​, as specified by the &lt;1/2&gt;​ argument directly following each ​&lt;print_colnameN&gt;​.

The JOIN command is unique in that it accesses data from multiple tables. The rules for the conditional portion are the same as for the ​DELETE FROM​ statement except that for the JOIN command, ​<strong>&lt;OP&gt;</strong>​ ​<strong>will be strictly limited to {</strong>​<strong>=</strong>​<strong>} for simplicity.</strong>​&nbsp; It is not guaranteed that the columns are listed in the same order as they exist in the table, nor is it guaranteed that all columns will be listed.

<strong>The JOIN must be accomplished as follows in order to insure compatibility with the autograder: </strong>

<ol>
<li>Iterate through the first table ​&lt;tablename1&gt;​ from beginning to end</li>
<li>For each row’s respective &lt;​ colname1&gt; value in ​ &lt;​ tablename1&gt;, find matching ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &lt;​ colname2&gt; values in &lt;​ tablename2&gt;, if any exist​</li>
<li>For each match found, print the column values in the matching rows in the order specified by the JOIN command</li>
<li>The matching rows from the second table must be selected in the order of insertion into that table.</li>
<li>If no rows in the second table match a row in the first table, that row is ignored from the join.</li>
</ol>
Output : Print the names of the specified columns, followed by the values of each of the specified columns in each row, separated by space.&nbsp; Every line should be followed by a newline.

&lt;print_colname1&gt; &lt;print_colname2&gt; … &lt;print_colnameN&gt;

&lt;value1rowA&gt; &lt;value2rowA&gt; … &lt;valueNrowA&gt; …

&lt;value1rowM&gt; &lt;value2rowM&gt; … &lt;valueNrowM&gt;

Once all the data has been printed, print the following, followed by a newline, where N is the number of rows printed

Printed &lt;N&gt; rows from joining &lt;tablename1&gt; to &lt;tablename2&gt;

In quiet mode, do not print the &lt;​ print_colname1&gt;​s or any of the values. Print <strong>only</strong>​ the following:​ Printed &lt;N&gt; rows from joining &lt;tablename1&gt; to &lt;tablename2&gt;

Possible errors:

<ol>
<li>&lt;tablename&gt; is not the name of a table in the database.​</li>
<li>One (or more ) of the &lt;​ colname&gt;s or ​ &lt;​ print_colname&gt;s are not the name of a column in the​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; table specified by &lt;​ tablename&gt; (only print the name of the first such column encountered)​</li>
</ol>
Given the following&nbsp; as input:

CREATE pets 3 string bool bool Name likes_cats? likes_dogs?

INSERT INTO pets 2 ROWS

Sith true true

Paoletti true false

JOIN pets AND 281class WHERE Name = person AND PRINT 3 Name 1 emotion 2 likes_dogs? 1

&nbsp;

The join specific output should be (Note: the CREATE and INSERT INTO commands will generate their own output, but for simplicity, they are not included in this example):

Name emotion likes_dogs?

Sith happy true

Sith victorious true

Paoletti stressed false

Printed 3 rows from joining pets to 281class Or in quiet mode:

Printed 3 rows from joining pets to 281class

Note that the JOIN is case sensitive and does not create a new table.

<h3><a name="_Toc27060"></a>&nbsp;<strong>REMOVE – remove existing table from the database </strong></h3>
Syntax:

REMOVE &lt;tablename&gt;

Removes the table specified by &lt;​ tablename&gt;​ and all associated data from the database, including any created index.

Output: Print a confirmation of table deletion, followed by a newline, as follows:

Table &lt;tablename&gt; deleted

Possible errors:

<ol>
<li>&lt;tablename&gt; is not the name of a table in the database​</li>
</ol>
Given the following as input:

REMOVE pets

REMOVE 281class

The output should be:

Table pets deleted

Table 281class deleted

&nbsp;

&nbsp;

<h3><a name="_Toc27061"></a><strong>QUIT – exit the program </strong></h3>
Syntax:

QUIT

Cleans up all internal data (i.e. no memory leaks) and exits the program. Note that the program must exit with a return 0​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​ from main()​ .​

Output: Print a goodbye message, followed by a newline.

Thanks for being silly!

Possible errors: None, except for lacking a QUIT​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; command.&nbsp; Every interactive session or redirected input​ file should end with a QUIT​&nbsp;&nbsp;&nbsp;&nbsp; command.​

&nbsp;

&nbsp;

<h3><a name="_Toc27062"></a><strong># – comment / no operation (useful for adding comments to command files) </strong></h3>
Syntax:

<h6># Any text on a line that begins with # is ignored</h6>
Discard any lines beginning with ​#​. This command does not produce any output nor can it generate any errors.

<h1><a name="_Toc27063"></a>Error Checking</h1>
Except for the errors specifically noted above and below, we will not test your error handling. However, we recommend that you implement a robust error handling and reporting mechanism to make your own testing and debugging easier. Normally, you would print error messages to the standard error stream (stderr via ​cerr​), rather than ​cout​. <strong>For this project, however, you must print the specified error</strong>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong> messages to stdout via </strong>​<strong>cout</strong>​<strong> so that they may be tested in conjunction with the rest of the project.&nbsp; DO NOT </strong>​<strong>exit()</strong>​<strong> when one of these errors occurs, display the error and keep running. </strong>

As stated in the Table Manipulation Commands section, there are a few specific errors that your code must check for and print the appropriate output.&nbsp; They are as follows:

<strong>Error 1: </strong>​A table named ​&lt;tablename&gt;​ already exists in the database

<strong>Output:</strong>​ ​Error: Cannot create already existing table &lt;tablename&gt;

&nbsp;

<strong>Error 2:</strong>​ ​&lt;tablename&gt;​ is not the name of a table in the database

<strong>Output:</strong>​ ​Error: &lt;tablename&gt; does not name a table in the database

&nbsp;

<strong>Error 3:</strong>​ ​&lt;colname&gt;​ is not the name of a column in the table specified by ​&lt;tablename&gt;

<strong>Output:</strong>​ ​Error: &lt;colname&gt; does not name a column in &lt;tablename&gt;

&nbsp;

<strong>Error 4:</strong>​ Unrecognized first letter of command (i.e. not one of <u>​<strong>C</strong></u><u>​</u>REATE, ​<strong><u>P</u></strong><u>​</u>RINT, <u>​<strong>R</strong></u><u>​</u>EMOVE, ​<strong><u>#</u></strong><u>​</u>, etc)

<h4><strong>Output:</strong>​ ​Error: unrecognized command</h4>
&nbsp;

For all input errors, you should print the matching response, with the braced variables replaced with the items from the offending command and followed by a newline, clear the rest of the command input, and reprompt the user (​”% “​) as usual. For most commands, clearing the rest of the input line should suffice. If there is an error in the insert command, however, the program should clear as many lines as there are rows to be inserted so that the command is fully flushed. ​<strong>Do not terminate the program</strong>​.

Other than the errors noted above, commands will be well formed. For simplicity, this also holds true when clearing away an erroneous command.

<h1><a name="_Toc27064"></a>Testing and Debugging</h1>
A major part of this project is to prepare a suite of test files that will help expose defects in your program. Each test file should be a text file containing a series of table manipulation commands to run. Your test files will be run against several buggy project solutions. If your test file causes the correct program and an incorrect program to produce different output, the test file is said to expose that bug.

Test files should contain valid SillyQL commands, and should be named

test-n-table-commands.txt​, where ​0 &lt; n ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​≤​ 15​.&nbsp; Make sure that every test file ends in a QUIT command.

Your test files may contain no more than 35 lines in any one file. You may submit up to 15 test files (though it is possible to get full credit with fewer test files). Note that the tests the autograder runs on your solution are ​<strong>NOT</strong>​ limited to 35 lines in a file; your solution should not impose any size limits (as long as sufficient system memory is available).

<h1><a name="_Toc27065"></a>Submitting to the autograder</h1>
Do all of your work (with all needed files, as well as test files) in some directory other than your home directory. This will be your “submit directory”. Before you turn in your code, be sure that:

<ul>
<li>Every source code and header file contains the following project identifier in a comment at the top of the file:</li>
</ul>
<h4>● // Project Identifier: C0F4DFE8B340D81183C208F70F9D2D797908754D</h4>
<ul>
<li>The Makefile must also have this identifier (in the first TODO block).</li>
<li>You have deleted all ​.o​ files and your executable(s). Your Makefile should include a rule or rules that cause ​make clean​ to accomplish this.</li>
<li>Your makefile is called Makefile. To confirm that your Makefile is behaving appropriately, check that “​make -R -r​” builds your code without compiler errors and generates an executable file called ​silly​. (Note that the command line options ​-R​ and ​-r​ disable automatic build rules, which will not work on the autograder).</li>
<li>Your Makefile specifies that you are compiling with the gcc optimization option ​-O3​ (This is the letter “O​​ ,” not the number “0​ ​”). This is extremely important for getting all of the performance points, as ​-O3​ can speed up code by an order of magnitude.</li>
<li>Your test files have names of the form ​test-n-table-commands.txt​, and no other project file names begin with “test.” Up to 15 test files may be submitted.</li>
<li>The total size of your program and test files does not exceed 2MB.</li>
<li>You don’t have any unneeded files in your submit directory.</li>
<li>Your code compiles and runs correctly using version 6.2.0 of the g++ compiler. This is available on the CAEN Linux systems (that you can access via login.engin.umich.edu). Even if everything seems to work on another operating system or with different versions of gcc, the course staff will not support anything other than gcc 6.2.0 running on Linux. To compile with g++ version 6.2.0 on CAEN you ​<strong>must</strong>​ put the following at the top of your ​Makefile​ (or use our provided Makefile​):</li>
</ul>
PATH := /usr/um/gcc-6.2.0/bin:$(PATH)

LD_LIBRARY_PATH := /usr/um/gcc-6.2.0/lib64 LD_RUN_PATH := /usr/um/gcc-6.2.0/lib64

Turn in the following files:

<ul>
<li>All of your .h and .cpp files for the project</li>
<li>Your Makefile</li>
<li>Your test files</li>
</ul>
You must prepare a compressed tar archive (.tar.gz file) of all of your files to submit to the autograder. One way to do this is to have all of your files for submission (and nothing else) in one directory. Go into this directory and run this command:

% dos2unix *; tar cvzf submit.tar.gz *.cpp *.h Makefile test*.txt

to prepare a suitable file in your working directory.

Submit your project files directly to either of the two autograders at: <u>https://g281-1.eecs.umich.edu</u><u>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </u> or<u>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </u> <u>https://g281-2.eecs.umich.edu</u>. Note that when the autograders are turned on and accepting​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; submissions, there will be an announcement on Piazza. The auto graders are identical and your daily submission limit will be shared (and kept track of) between them. You may submit up to two times per calendar day with autograder feedback. For this purpose, days begin and end at midnight (Ann Arbor local time). <strong><u>We will count only your best submission for your grade</u></strong>​&nbsp; .&nbsp; If you would instead like us to<u>​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </u> use your LAST submission, see the autograder FAQ page, or <a href="https://docs.google.com/forms/d/e/1FAIpQLSe8BxRNnZKgRI4o-V7eG5F6LY_GhhWjMyJW8yKcP4XKVm2JrQ/viewform?usp=sf_link">use this for</a>​&nbsp; <a href="https://docs.google.com/forms/d/e/1FAIpQLSe8BxRNnZKgRI4o-V7eG5F6LY_GhhWjMyJW8yKcP4XKVm2JrQ/viewform?usp=sf_link">m</a><a href="https://docs.google.com/forms/d/e/1FAIpQLSe8BxRNnZKgRI4o-V7eG5F6LY_GhhWjMyJW8yKcP4XKVm2JrQ/viewform?usp=sf_link">.</a><u>​</u>

We strongly recommend that you use some form of revision control (ie: SVN, GIT, etc) and that you “commit” your files every time you upload to the autograder so that you can always retrieve an older version of the code as needed. Please refer to your discussion slides and CTools regarding the use of version control.

Please make sure that you read all messages shown at the top section of your autograder results! These messages often help explain some of the issues you are having (such as losing points for having a bad Makefile or why you are segfaulting). Also be sure to note if the autograder shows that one of your own test files exposes a bug in your solution (at the bottom).

<h2><a name="_Toc27066"></a>Libraries and Restrictions</h2>
The use of the C/C++ standard libraries is highly encouraged for this project, especially functions in the &lt;algorithm&gt; header and container data structures. The smart pointer facilities, and thread/atomics​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; libraries are prohibited. As always, the use of libraries not included in the C/C++ standard libraries is​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; forbidden.

<h1><a name="_Toc27067"></a>Grading</h1>
<ul>
<li>80 points — Your grade will be derived from correctness and performance (runtime). Details will be determined by the autograder.</li>
<li>10 points — Test file coverage (effectiveness at exposing buggy solutions).</li>
<li>10 points — No memory leaks. Make sure to run your code under valgrind before each submit. (This is also a good idea because it will let you know if you have undefined behavior, which will cause your code to crash on the autograder.)</li>
</ul>
When you start submitting test files to the autograder, it will tell you (in the section called “Scoring student test files”) how many bugs exist, the number needed to start earning points, and the number needed for full points.&nbsp; It will also tell you how many are needed to start earning an extra submit/day!

&nbsp;

<h2><a name="_Toc27068"></a>Checkpoint</h2>
This project has a few test cases named CP* that represent a checkpoint.&nbsp; The checkpoint involves implementing base functionality for several commands, and you should have it completed within 10 days of receiving the project specification (less in the Spring; about halfway between receiving this document and the final due date).

The checkpoint test cases will only be testing a subset of the functionality of your code. The functionality we will be testing are listed as follows:

<ul>
<li># (comment) Used in all 3 checkpoints</li>
<li>CREATE Used in all 3 checkpoints</li>
<li>INSERT INTO Used in checkpoints 2 and 3</li>
<li>PRINT FROM … ALL Used in checkpoints 2 and 3</li>
<li>REMOVE Used in all 3 checkpoints</li>
<li>QUIT Used in all 3 checkpoints</li>
</ul>
&nbsp;

For example, checkpoint 1 has a comment, a few create and remove commands, and quits.&nbsp; None of the commands produce errors.

<h2><a name="_Toc27069"></a>Test Cases</h2>
All test cases on the autograder test the QUIT command, because all valid input files must end with it. Many include comment(s) so that we know what the test case is doing.&nbsp; Most of the test case names on the autograder are fairly self-explanatory, but here’s a guide:

Appendix: The test case from Appendix A (see below)

CP*: Checkpoint cases (see above)

CREATE*: Primarily tests the CREATE command, but also PRINT and REMOVE

INSERT*: Primarily tests INSERT, but also needs CREATE, PRINT, and REMOVE

DELETE*: Primarily DELETE; also needs CREATE, INSERT; sometimes REMOVE and GENERATE

GENERATE*: Primarily GENERATE, needs CREATE, INSERT, PRINT; sometimes REMOVE,

DELETE

JOIN*: Primarily JOIN, but also needs CREATE, and INSERT; some test REMOVE and GENERATE

PRINT*: Primarily tests PRINT, but also needs CREATE, INSERT, and DELETE

REMOVE*: Primarily tests REMOVE, but also needs CREATE, INSERT, and sometimes GENERATE

&nbsp;

Short*: Tests all commands, “short” only with respect to Medium* and Long*; always run in quiet mode

Medium*: Tests all commands; always run in quiet mode

Long*: Tests all commands; always run in quiet mode

&nbsp;

CP*: Tests the commands listed in the checkpoint section above.

&nbsp;

<h1><a name="_Toc27070"></a>Appendix A: Example from the Spec</h1>
Given the following as input:

#Awesome Spec Example!

CREATE 281class 3 string string bool emotion person Y/N INSERT INTO 281class 8 ROWS happy Darden true stressed students false busy office_hours true stressed students true stressed Paoletti true happy Darden true happy Sith true victorious Sith true

DELETE FROM 281class WHERE person = Darden

GENERATE FOR 281class hash INDEX ON emotion PRINT FROM 281class 2 person emotion WHERE Y/N = true

CREATE pets 3 string bool bool Name likes_cats? likes_dogs?

INSERT INTO pets 2 ROWS

Sith true true

Paoletti true false

JOIN pets AND 281class WHERE Name = person AND PRINT 3 Name 1 emotion 2 likes_dogs? 1

REMOVE pets

REMOVE 281class

QUIT

The output should be: (​ prompt characters and commands not included)

New table 281class with column(s) emotion person Y/N created&nbsp; Added 8 rows to 281class from position 0 to 7

Deleted 2 rows from 281class

Created hash index for table 281class on column emotion person emotion office_hours busy students stressed Paoletti stressed

Sith happy

Sith victorious

Printed 5 matching rows from 281class New table pets with column(s) Name likes_cats? likes_dogs? created Added 2 rows to pets from position 0 to 1

Name emotion likes_dogs?

Sith happy true

Sith victorious true

Paoletti stressed false

Printed 3 rows from joining pets to 281class

Table pets deleted Table 281class deleted

Thanks for being silly!

&nbsp;

<h1><a name="_Toc27071"></a>Appendix B: Variant Types and You</h1>
One of the most difficult parts of implementing an efficient database is handling the problem of heterogenous rows, or the fact that rows in the tables contain multiple types. If you wanted to store your rows as vector&lt;T&gt;​&nbsp;&nbsp; , what would T be? int? string? bool? The answer, in reality, is that you must be​&nbsp;&nbsp;&nbsp;&nbsp; able to store any of the valid types in that row. Unfortunately the current C++ standard does not give us a good way of implementing these types of heterogeneous containers when the types of each column aren’t known at compile time (check out std::tuple&lt;&gt;​&nbsp; for when you do!).​

To remedy this, the course staff has created a special class for you to store in your tables, aptly named

TableEntry. This ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; TableEntry​&nbsp; is an implementation of what is known as a variant type, as it can be​ a variety of different types. While we could modify the TableEntry​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; class to contain arbitrary types, for​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; simplicity we have limited the types that can be represented to the set of those that are valid to appear in this project. Most of how to use the TableEntry​ should be intuitive from the comments in the​ header file. In addition to that, see the below example for further instructions.

The one major downside to our implementation of TableEntry​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; is that it doesn’t play nicely when you​ try to compare two TableEntry​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; objects that contain different types, or try to compare a ​ TableEntry​&nbsp; with a type other than the one it represents internally. To combat that we’ve placed assertions in key locations such that if you do not compile with -​ DNDEBUG (by using ​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; make debug​&nbsp; with the provided​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makefile)​ , these assertions will fire rather than let you have undefined behavior. If you’re getting weird results with this type, try running under debug conditions and see if an assertion fires. We attached a comment to the assertions so that you can see <em>what</em>​&nbsp;&nbsp; ​ the issue is. In order to see <em>where</em>​&nbsp;&nbsp; ​ the issue stems from, you must use a debugger and read the stack trace to find the line of your code that calls the offending method. We suggest against delving into the implementation of this class; it’s pretty complex.

&nbsp;

An example:

#include “TableEntry.h”

#include &lt;unordered_map&gt;

#include &lt;map&gt;

#include &lt;vector&gt; #include &lt;iostream&gt; using namespace std; int main() {&nbsp;&nbsp;&nbsp;&nbsp; unordered_map&lt;TableEntry, int&gt; u_m; // They can be used in unordered_maps&nbsp;&nbsp;&nbsp;&nbsp; map&lt;TableEntry, int&gt; m;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // They can be used in maps&nbsp;&nbsp;&nbsp;&nbsp; vector&lt;TableEntry&gt; v;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;// They can be used in other containers&nbsp;&nbsp;&nbsp;&nbsp; TableEntry tt1{7}, tt2{8};&nbsp;&nbsp;&nbsp;&nbsp; int i = 3;

v.emplace_back(i);&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // .emplace_back() adds a TableEntry(int) to v&nbsp;&nbsp;&nbsp;&nbsp; if (tt1 &gt; tt2 || tt2 &gt; i) // They can be compared w/ each other and their “type”&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;cout &lt;&lt; tt1 &lt;&lt; endl;&nbsp; // They can be sent to an output stream

return 0; } // main()

&nbsp;

<h1><a name="_Toc27072"></a>Appendix C: Project Tips, Tricks, and Things to Avoid</h1>
<h5>Starting the project</h5>
Like the others, this project can be written in stages.&nbsp; Start with the QUIT command, it’s easy and all valid input files must end with it.&nbsp; The # comment is easy.&nbsp; Then work on CREATE, INSERT, and PRINT … ALL; when those three are coded, you can test that your project is starting to work.&nbsp; Don’t worry about indices at the beginning!&nbsp; When you start working on GENERATE and indices, your existing code is still perfectly usable.&nbsp; You’ll just have to add to the existing code, things like “if a useful index exists, do it this way; else do it the old way”, and the “old way” code doesn’t have to change!

&nbsp;

<h5>Video</h5>
Like the others, this project has a video for you: <u>​</u><a href="https://youtu.be/_gbdH5Rm_Xc">https://youtu.be/_gbdH5Rm_Xc</a><u>​</u><a href="https://youtu.be/_gbdH5Rm_Xc">.</a>&nbsp; It should answer a large number of questions about the project, so please watch it.&nbsp; Go back to it again after you’re deeper into coding the project, as some things in it might not make sense at first.

&nbsp;

<h5>Producing Columns of Output</h5>
When you have to produce output, you’ll often have to run a loop to display everything in a given row: column names, table data, etc. separated by spaces.&nbsp; It is easier to code and perfectly acceptable to have a space following the last one.&nbsp; So column names might appear (without quotes) as ​”person emotion “​ (notice the extra space after ​emotion​).

&nbsp;

<h5>Reading and Printing Bools</h5>
For most of the types that can be represented in a table, just reading in and printing as usual will do the trick. That cannot be said for ​bool​, however. Reading and writing ​bool​ as 1s and 0s isn’t the most enjoyable experience. Luckily there’s a fix for that in the form of <u>​</u><a href="http://en.cppreference.com/w/cpp/io/manip/boolalpha">std::boolalpha</a>​. To read in and print variables of type ​bool​ as ​true​ and ​false​, you just need to use this once at the beginning of your ​main()​ and it will persist for the remainder of the program. DO THIS ONLY ONCE, not every time you produce putput!&nbsp; All you’ll need to do is add the following two lines of code to your main file:

int main(…) {

ios_base::sync_with_stdio(false);&nbsp;&nbsp; // you should already have this <strong>&nbsp;&nbsp;&nbsp;&nbsp;cin &gt;&gt; std::boolalpha;&nbsp; // add these two lines&nbsp;&nbsp;&nbsp;&nbsp; cout &lt;&lt; std::boolalpha; </strong>&nbsp;&nbsp;&nbsp;&nbsp;…

// the rest of your program

&nbsp;

<h5>Switches and Enums</h5>
There are many situations in this project where you will find yourself choosing from a finite set of options. The types that are allowed to be in a table is one case; the conditional operators (​&lt;​, ​&gt;​, ​=​) are another. Based on your time in 101/183, you’ll probably be drawn to the traditional conditionals of the form

if … { } else if … { } else { }

There are many cases, however, when what you really want to be using is the <u>​</u><a href="http://www.tutorialspoint.com/cplusplus/cpp_switch_statement.htm">switc</a><a href="http://www.tutorialspoint.com/cplusplus/cpp_switch_statement.htm">h</a><u>​</u><a href="http://www.tutorialspoint.com/cplusplus/cpp_switch_statement.htm"> statement</a><u>​</u><a href="http://www.tutorialspoint.com/cplusplus/cpp_switch_statement.htm">.</a> For reasons that this appendix won’t go into, compilers may be able to optimize ​switch​ statements to be significantly faster than a traditional ​if​/​else​ block. If you think that what you’re doing makes sense as a ​switch​, then you should probably be using one. That being said, don’t contort yourself into using one if it doesn’t make sense. In those situations, it’s not unlikely that the compiler will just turn it into an if​/​else​ anyway. Bear in mind that you can only switch on expressions that can be interpreted as an integer (e.g., ints, chars, and enums).

&nbsp;

These finite set of options should lead you to more than just switches. A very useful construct for this project is the <u>​</u><a href="http://www.learncpp.com/cpp-tutorial/4-5a-enum-classes/">enum class</a>​. These provide the same functionality as ​enum​ with the scoping and type safety of classes. A helpful use of ​enum​ in this project is to represent the different types that can be represented in a table. The following definition may prove useful; it is already coded for you at the top of TableEntry.h​:

enum class EntryType : uint8_t { String, Double, Int, Bool };

You can use this ​enum​ to keep track of what types are stored in each column of a table; for example by creating a vector of this type:

vector&lt;EntryType&gt; types;

&nbsp;

… types.push_back(EntryType::Bool);

You can then later use these stored types in, for example, a switch!&nbsp; You might also want to remember the names of the columns (as strings).&nbsp; The column names and types are called metadata: data about data.&nbsp; They come from the user and need to be saved, but they also describe the other data in your program.

&nbsp;

<h5>Lists Are Not Your Friend</h5>
You will probably at least once while working on the project consider using a ​std::list&lt;&gt;​ for something. There’s a specific application within this project for which using ​std::list&lt;&gt;​ actually kind of makes sense. Unfortunately it only ​<em>kind</em>​ of makes sense. One use case for lists is if you need to remove data from arbitrary locations within the list given that you already know the locations of that element. They’re terrible for almost everything else. They’re absolutely abysmal for iterating over due to their data being not contiguous in memory. This project requires a lot of iterating. Enough said.

&nbsp;

<h5>Making Joins More Efficient</h5>
Doing a join where the second table has an index on the column being joined on is easy and efficient. Unfortunately, when this is not the case, joins can be quite slow and inefficient – given two tables, of sizes ​n​ and ​m​, the complexity of the join is O(n*m), which is quite awful. But can you do better? You can’t use sorting to make this faster, because that would be problematic with regards to the ordering of output. What other tools might you use to solve this problem? This is a problem to discuss with your classmates.

&nbsp;

<h5>unordered_map&lt;&gt; is Your Friend Until It Isn’t​</h5>
The ​std::unordered_map&lt;&gt;​ is a quite useful tool. Many of you are probably learning about hash tables for the first time and thinking “wow, I should use these for everything.” We’ve all been there.

Some of us are still there. The thing with ​unordered_map&lt;&gt;​ is that you’re trading space for time. You get average case ​<em>O</em>​(1) lookup but at the cost of significant memory overhead, possibly even twice as much as you need. The ​std::map&lt;&gt;​ is better in some ways and worse in others. Its memory overhead is constant per element, similar to that of a linked list, but its lookup complexities don’t quite match.

&nbsp;

An important decision in this project is when to make use of these shiny new tools. In one case, with the generation of indices, we’ve created a specific use case for these types. There will likely be other places in the project where you will need to use these types as well. Sadly, it’s not actually the case that unordered_map&lt;&gt;​ is always the best choice in every situation. In many cases a good old vector will do. Spend some time considering what is actually the best container for each individual situation.

&nbsp;

<h5>Basic Templates</h5>
One of the most useful C++ language constructs for this project is probably the template. Templates are one of C++’s main tools for generic programming, or writing code that works the same across many different types. You may remember them from Project 2, in which they allowed us to store any type in a Priority Queue. Let’s say I want to create a method that inserts a new item into a table and so define it as follows:

void insert_into_table(??? item);

But what is the type of ​item​? We don’t want to restrict it to int, bool, double, or even string, since for all of these types the internal code should be the same – stick it in a ​TableEntry​ and insert it into the table. The solution, as you may have guessed, is templates. Use the following definition instead!

template &lt;typename T&gt; void insert_into_table(T item); or

template &lt;typename T&gt;

void insert_into_table(const T&amp; item);

This tells the compiler that ​insert_into_table​ should accept any type and act the same way. This can greatly reduce code duplication in your project. There are more advanced techniques that can be used to tell the compiler to restrict the types allowed to be used with a templated method, but that’s beyond the scope of this course.

&nbsp;

<h5>(unordered_)multimaps, and (unordered_)multisets</h5>
Throughout the course of this project, you will probably at least once find yourself considering one of the ​multi​- containers. Do not use a ​multi​ container.

&nbsp;

The ​multi​- variants of ​map​ and ​set​ are comparable to using a non-​multi​ version with a vector​&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ​ as the mapped-to type. We recommend using a ​map​-plus-​vector​ implementation instead mostly to simplify the interface that you’ll be dealing with. For example, if you were considering writing multimap&lt;Key, Value&gt;​, instead write ​map&lt;Key, vector&lt;Value&gt;&gt;​.

&nbsp;

The ​unordered_multimap​s and ​unordered_multiset​s are even worse. The main problem with using them is a lack of control over the ordering of items with the same key. There are many other performance-related issues with the implementations of these containers, but some of them are based on concepts not covered in this course, so take our word for it and just don’t use them. Instead stick to variations of the ​map​-plus-​vector​ approach described earlier (i.e. ​unordered_map&lt;Key, vector&lt;Value&gt;&gt;​).

&nbsp;

<h5>How <strong>NOT</strong>​ to Use ​ TableEntry​</h5>
As you build your solution you will notice that there are a few key features of ​TableEntry​ that don’t exist or were explicitly disabled. The two most important instances of this are the assignment operator and default constructor.

&nbsp;

The assignment operator is disabled as there’s no reason you ought to be assigning ​TableEntry objects. Once created, a ​TableEntry​ is essentially a constant piece of data. This indirectly disables a few other things, such as calling erase on a vector of ​TableEntry​ objects (i.e.

vector&lt;TableEntry&gt; v; /* put in data */ v.erase(…);​).

You also can’t pass a ​TableEntry​ by value; this is intentional. Copying a ​TableEntry​ is inefficient.

&nbsp;

The default constructor is disabled as a default-constructed ​TableEntry​ doesn’t make much sense. A TableEntry​ exists to represent a cell in a Table whose type isn’t known at compile time. What would the internal type of a default-constructed ​TableEntry​ even be? As with the assignment operator, this indirectly disables a few things, such as calling ​resize​ on a vector of ​TableEntry​ objects. That’s not actually a bad thing, however, since you’re probably better off using ​reserve​ on the vector anyway.

&nbsp;

If you find yourself needing either of these, you might want to reconsider your design rather than trying to contort your solution to get around them.&nbsp; ​<strong>DO NOT MODIFY</strong>​ the ​TableEntry​ files; they will be overwritten when you submit to the autograder.

&nbsp;

<h5>What are vectors</h5>
Vectors, while very useful, are not magic. Many people visualize a vector like this:

&nbsp;

Or basically an array that magically is always big enough to hold the required amount of data. But what does a vector actually look like? Well the code for a vector (without functions) looks something like this:

template&lt;typename T&gt; class vector { private:

size_t size; // how much data I hold right now&nbsp;&nbsp;&nbsp;&nbsp; size_t size_of_alloction; // how much data I ​<em>can</em>​ hold before automatically resizing

T* data; //internal storage of data

};

Knowing this, we really should be visualizing vectors like this:

&nbsp;

Where the small square is the actual vector class object, and Data is the actual data that the vector “contains”, or, in reality, points to.

&nbsp;

Now let’s consider what a vector of vectors looks like:

&nbsp;

Let’s say I declared this as ​vector&lt;vector&lt;type&gt;&gt; v;​ and then inserted my four inner vectors.

Now let’s think about what happens when I want to erase the first inner vector using

v.erase(v.begin())​. You might be thinking, “there’s no need to move the actual data around in memory, we can just move the little squares!” Well you’d be right, and luckily the people who write compilers and the STL noticed this also! So, after calling delete, the only things that get shifted are the little squares:

&nbsp;

Pretty efficient! You shouldn’t be afraid that erasing an inner vector in a vector of vectors moves around all (or any) of the data. Regardless of what happens to the outer vector, even if it gets resized and moved around, the data for the inner vectors (big rectangles) won’t get moved, just the little squares.

&nbsp;

You can think of the data items that vector points to as simply dynamic arrays that vectors manage for you. Normally, you don’t want to touch or look at the data array directly, since as the vector grows, that particular array could get deallocated and reallocated somewhere else. In specific scenarios, however, using it can actually be beneficial. For that reason, vectors actually have a member function that returns a pointer to the internal data, ​vector::data()​. Do with this information what you will. Remember that it’s only safe to use the pointer returned by ​vector::data()​ if the data array will never change size, as when vectors grow, they move stuff around in memory, invalidating pointers.

&nbsp;

<h5>Reading and dealing with input</h5>
The input for this project is very well-formed: at any given time, you know exactly what you’ll need to read next.&nbsp; ​<strong>DON’T</strong>​ read valid input using ​getline()​ and then break it into pieces, just read using ​&gt;&gt;​. Remember though, once you encounter an error you will want to use ​getline()​ to eliminate the invalid portions of input.&nbsp; Also, read what you need; don’t always read a ​string​ and then convert into what you need (an example is coming up next).

&nbsp;

When you’re reading user input, use a ​<a href="https://www.tutorialspoint.com/cplusplus/cpp_do_while_loop.htm">do…while</a><u>​</u> loop.&nbsp; This makes it very easy to prompt the user and read their input at the top of the loop.&nbsp; Don’t prompt the user with ​cout &lt;&lt; “% “​ inside of every command processing function!&nbsp; Do it ​<strong>once</strong>​ inside the top of the loop.

&nbsp;

Learn the difference between ​.push_back()​ and ​.emplace_back()​.&nbsp; Using ​.push_back()​ takes what you give it, and adds a ​<strong>copy</strong>​ of it into the vector.&nbsp; The ​.emplace_back()​ member function calls a constructor to convert from what it’s given to what needs to be stored into the vector.&nbsp; For example, if you have a vector of ​TableEntry​ objects, and call ​.push_back()​ with a ​TableEntry​ object, you get a compiler error because the ​TableEntry​ type cannot be copied!&nbsp; However if you

.emplace_back()​ an ​int​, it will automatically call the ​TableEntry​ constructor that accepts an int​, and add a ​TableEntry​ containing an ​int​ to the end of the vector!&nbsp; For example, when you’re processing the INSERT INTO command, and the next column that you need to process contains an int​, read directly into an ​int​ variable using ​&gt;&gt;​, then ​.emplace_back()​ that ​int​ into the vector (which should be the correct row of your 2D table of data).

&nbsp;

Don’t write the same code 12 times!&nbsp; For example, when doing DELETE or PRINT…WHERE you might feel that you need to do a ​switch​ for a 4-way split of type, (​int​, ​double​, ​bool​, ​string​), then inside each of those do a 3-way split for comparison (​&lt;​, ​&gt;​, ​=​).&nbsp; Instead, in each part of the 4-way split, create a ​TableEntry​ containing the desired type, and pass it to another function that does a 3-way split on the comparison.&nbsp; Better yet, just call the other function and pass it an anonymous ​TableEntry variable!&nbsp; Better still, have the second function create one of three different functor types (one functor type for each comparison type), and call a third function, passing it the functor as a templated type.
