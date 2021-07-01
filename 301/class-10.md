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
# JavaScript error messages && debugging

1- What is a ‘refrence error’?

        is wrong with your code is the (in)famous error message 

2- What is a ‘syntax error’?

        This is as simple as when you try to use a variable that is
         not yet declared you get this type os errors.


3- What is a ‘range error’?

        Try to manipulate an object with some kind of length and
         give it an invalid length and this kind of errors will show 
        up.

4- What is a ‘tyep error’?

        Like the name indicates, this types of errors show up when 
        the types (number, string and so on) you are trying to use 
        or access are incompatible, like accessing a property in an
         undefined type of variable.


5- What is a breakpoint?

        tools to testing a CODE step by step and show how running


6- What does the word ‘debugger’ do in your code?

        To debug your JS code