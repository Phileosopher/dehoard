
[Clean Code Cheat Sheet v2.4](https://www.planetgeek.ch/2014/11/18/clean-code-cheat-sheet-v-2-4/)
(2014) cheat sheet for clean code

[Wojtek Lukaszuk](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)
[Deniz Ozger/clean-code](https://github.com/denizozger/clean-code)
[Jose Angel Barroso/clean-code](https://github.com/jbarroso/clean-code)
[harry830622/clean-code-notes](https://github.com/harry830622/clean-code-notes)
[thebentern/clean-code-study](https://github.com/thebentern/clean-code-study)
[JuanCrg90/Clean-Code-Notes](https://github.com/JuanCrg90/Clean-Code-Notes)
[timkendall/clean-code](https://github.com/timkendall/clean-code)
Some GitHub resources on clean coding practices, mostly based on book 'Clean Code: A Handbook of Agile Software Craftsmanship' by Robert C. Martin

The Art Of Clean Code by [Victor Rentea](https://www.youtube.com/watch?v=J4OIo4T7I_E)
  * Make it more readable even if it makes writing harder : We read 10x more times than we write
  * Boy scout rule : always check in code cleaner than you found it
  * Functions are verbs
  * Boolean names should always answer yes/no
  * Classes are nouns. Avoid meaningless names (OrderInfo, OrderData vs Order)
  * Delete the interfaces : except for Remoting/API client jars and strategy pattern implementation.
  * Names : Make the name speak for itself. Apply Continuous renaming as your learn the application
  * Names : Names should be at least pronounceable. Don't abbreviate ! Unless it's a basic business concept, like VAT
  * Names : should be consistent and unique (synonyms confuse).
  * Names should have meaningful context. eg: order.customerFirstName. But don't repeat yourself (DRY) : Order.~~order~~CreationDate
  * Functions should be small : 5-10 lines, ... or at least should be understandable in 5 sec no more.
  * Functions do one thing
  * Functions have max 2-3 parameters
