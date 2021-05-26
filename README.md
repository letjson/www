## letjson

The cost of parsing JSON

Because the JSON grammar is much simpler than JavaScript’s grammar, JSON can be parsed more efficiently than JavaScript. 
This knowledge can be applied to improve start-up performance for web apps that ship large JSON-like configuration object literals (such as inline Redux stores). Instead of inlining the data as a JavaScript object literal.

As long as the JSON string is only evaluated once, the JSON.parse approach is much faster compared to the JavaScript object literal, especially for cold loads. A good rule of thumb is to apply this technique for objects of 10 kB or larger — but as always with performance advice, measure the actual impact before making any changes.

## Getting Started

  
    let_json()
