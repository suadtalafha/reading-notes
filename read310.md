# Understanding the JavaScript Call Stack

1-What is a ‘call’?

When a function is invoked, call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation .

2-How many ‘calls’ can happen at once?

one at a time excuted

3-What does LIFO mean?

When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

4-Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.?

`function firstFunction(){ console.log(“Hello from firstFunction”); }

function secondFunction(){ firstFunction(); console.log(“The end from secondFunction”); }

secondFunction();

5-What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

`function callMyself(){ callMyself(); }

callMyself();`

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQncU4ZAfnACbHNps7qjVDRGY2fMcCUKMwqyA&usqp=CAU.jpg)

# JavaScript error messages

1-What is a ‘refrence error’?

This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
2-What is a ‘syntax error’?

when you have something that cannot be parsed in terms of syntax and This can be solved by just fixing the syntax

3-What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

4-What is a ‘tyep error’?

when the types (number, string and so on) you are trying to use or access are incompatible

5-What is a breakpoint?

can also be achieved by putting a debugger statement in your code in the line you want to break and this is awesome for when you want to debug huge cycles for specific values

6-What does the word ‘debugger’ do in your code?

 to identify JavaScript errors and we can use it for example to debug huge cycles for specific values.

 
 ![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQEIehZ9agMc0NA8rVsybmwTh4vnrn-ybRWHA&usqp=CAU.jpg)