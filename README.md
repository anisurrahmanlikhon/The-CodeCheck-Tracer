# The-CodeCheck-Tracer

The CodeCheck Tracer lets you author tracing exercises. You decide what the student should see: code fragments, variables, objects, arrays, and so on. You can make the program run up to an interesting point, then ask students to predict the next line, update a variable, draw a pointer, or choose among higher-level tasks (such as “move left/move right” in a binary tree).

You first map out the exercise in your mind, perhaps after studying some examples. Then you write the code for the “puppet master”. In each step, you either ask the student or update the program state yourself.

That code is written in JavaScript, but have no fear. If you know Java, C++, or Python, you can quickly pick up the few JavaScript constructs that you need. The students do not see any JavaScript (unless, of course, you happen to teach them JavaScript).

The CodeCheck tracer API takes advantage of advanced JavaScript features (generators, proxies) that greatly simpilfy authoring. To wait for student input, you simply use a yield expression. When you change the value of a path such as myObj.myField, the visual representation is automatically updated.

You put the code inside a web page, together with your instructions. Students simply work through your web page. Or you can use the CodeCheck service to publish the page and enable scoring. If you like, the scores can end up in your learning management system. Read on for the details!

I developed the tracer from interactive elements for my Big Java/Big C++/Python for Everyone books. Those books have different exercise types for tracing variables, objects, and algorithms. The CodeCheck tracer combines them all. And it is driven by JavaScript code instead three different ad-hoc markup languages.



