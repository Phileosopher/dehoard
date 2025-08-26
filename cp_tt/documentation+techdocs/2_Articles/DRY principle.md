
Suppose we have a specification that lists the columns in a database table. We'll then have a separate set of SQL commands to create the actual table in the database, and probably some kind of programming language record structure to hold the contents of a row in the table. The same information is repeated three times. Change any one of these three sources, and the other two are immediately out of date. This is a clear violation of the DRY principle. To correct this problem, we need to choose the authoritative source of information. This may be the specification, it may be a database schema tool, or it may be some third source altogether. Let's choose the specification document as the source. It's now our model for this process. We then need to find a way to export the information it contains as different views-a database schema and a high-level language record, for example.

[Nicolò Pignatelli](https://hackernoon.com/this-is-not-the-dry-you-are-looking-for-a316ed3f445f)
(2018) This is not the DRY you are looking for

[Jamie Wong](http://jamie-wong.com/2013/07/12/grep-test/)
(2013) Too DRY - The Grep Test
