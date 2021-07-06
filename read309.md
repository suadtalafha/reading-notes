# Functional Programming Concepts

1-What is functional programming?

 is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared and colocated with methods in objects.

2-What is a pure function and how do we know if something is a pure function?

Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result

It returns the same result if given the same arguments

It does not cause any observable side effects

3-What are the benefits of a pure function?
Referential transparency that you can replace a function call with its resulting value without changing the meaning of the program
4-What is immutability?

mutability is discouraged in functional programming.

5-What is Referential transparency?

Referential Transparency is the property that lets you replace an expression with its value, and not change the results of whatever you were doing.

![image](https://devopedia.org/images/article/21/5929.1491735653.png)


1-What is a module?

that is a component or thing(function, variable,..) that you would to use it outside his original file.

2-What does the word ‘require’ do?

import the file

3-How do we bring another module into the file the we are working in?

first thing module export then in the page we need to use it we should import it by (require )

4-What do we have to do to make a module available?

export it firstly from its original file, then import it to the new file by require.

![image](https://2r4s9p1yi1fa2jd7j43zph8r-wpengine.netdna-ssl.com/files/2018/03/07_loader_vs_es.png)