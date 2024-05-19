High-level overview of what we have to do:
    1) Design the actual language:
        What will tokens look like?
        What will the productions be like?
        What will the language do? 
        
        Is it actually going to be used to program?
        If so, what kind of programs and logic should it have?
        Should it have memory allocation?
        Should it have loops?
        If-else branches?
        Control flow?
        Variables?
        Types? 
        What arithmetic? 
        All that kind of stuff
        I DONT WANNA MAKE CLASSES PELASE PLEASE PLEASE PLEASE PLEAS
        OBJECT ORIENTED PROGRAMMING IS HELL
        
        Do we want it to be LL(1), SLR(1), etc?


        This dictates what compilers, parsers, etc we can make. 
        Tokenizers are always DFAs so we're chilling there.

        I was planning on rewatching the 460 lectures to understand what SLR was again because it was really cool.
    2)  Once we decide on the language (which is honestly the most annoying part) we need to make the tokenizer
        That will be a simple DFA, I think the current 326 classes have an assignment in which you make one.
        Pretty neat stuff, We have to decide on a language, I say C since it's kinda fast.
        WE COULD TRY RUST TBH, IT LOOKS LIKE FUN
    3)  Once the tokenizer is done, we can move onto parsing and building a parse tree.
    4)  Once the parse tree is done, we can implement visitor patterns to check semantic stuff like type checking,
        actual grammar stuff, etc. This part is REALLY cool but it depends on what functionality our language has.
    5)  Profits (put on resume and shmove on)

I'm probably missing stuff but idk and I'm eepy so for now this works