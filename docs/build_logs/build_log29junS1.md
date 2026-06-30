- Date: 29 June 2026 (Session 1)
Duration: 2hours 35 mins 
Goad():
Implement the command parser module for redislite to convert raw user input to structured commands.

What I did():
1. I created the initial command parser class which will be for parsing the user given commands 

2. Then I designed the parser in such a way that it can accept and tokenize the commands into individuals 

3.Implemented whitespace-based tokenization to split commands such as:
SET key value
GET key
DEL key
EXISTS key
4. Added validation to ignore empty inputs and handle multiple spaces between tokens.
5. Established a structure for identifying the command name separately from its arguments.
Also integrated the parser with the CLI so that every user command is processed through the parser before execution.
Organized the project by separating parser declarations and implementations into dedicated header and source files.

Problems():
Inconsistent user input 