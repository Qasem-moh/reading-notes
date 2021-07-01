# The JavaScript Call Stack - What It Is and Why It's Necessary



1- What is a ‘call’?

        The call stack is primarily used for function invocation (call)

2- How many ‘calls’ can happen at once?

         steps 3
3- What does LIFO mean?

        LIFO: When we say that the call stack, operates by the data 
        structure principle of Last In, First Out, it means that the
        last function that gets pushed into the stack is the first
        to be pop out, when the function returns.



4- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

        function firstFunction(){

            throw new Error('Stack Trace Error');
        }

        function secondFunction(){
            firstFunction();
        }

        function thirdFunction(){
         secondFunction();
        }

        thirdFunction();

5- What causes a Stack Overflow?

        A stack overflow occurs when there is a recursive function 
        (a function that calls itself) without an exit point. The 
        browser (hosting environment) has a maximum stack call that 
        it can accomodate before throwing a stack error.



***