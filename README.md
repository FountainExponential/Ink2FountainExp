# Ink2FountainExp
A tool that converts stories written in Ink by Inkle to Fountain Exponential.

Fountain Exponential and Ink are very similar, but where Ink focuses on programming power, Fountain Exponential focuses on readability. This means that Ink messes things together for briefness. This is specifically so with text generation. Fountain Exponential will separate thing out so it will be easier to see where things start and end.

## Technical approach
The conversion will probably entail the following steps:
1. Asses the Ink by Inkle project.
2. A parser for Ink by Inkle will be created based on the sources available on Github. Unfortunatly Ink does margenaly follow those rules and the project needs rafactoring. A common set of components in a compiler is:
    * Lexer - break the program up into words.    
    * Parser - check that the syntax of the sentences are correct.    
    * Semantic Analysis - check that the sentences make sense.    
    * Optimizer - edit the sentences for brevity.    
    * Code generator - output something with equivalent semantic meaning using another vocabulary. 
2. After the story has become a parse tree in memory, we match the elements with those in Fountain Exponential.
3. Then we might do some optimizing and beautifying on the converted parse tree.
4. At last we flush the Fountain Exponential parse tree to a file.
