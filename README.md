# javascript-interview-questions

Output of following code snippet 
var myObject = { 
    foo: "bar",    
    func: function() {    
        var self = this;    
        console.log("outer func:  this.foo = " + this.foo);    
        console.log("outer func:  self.foo = " + self.foo);    
        (function() {    
            console.log("inner func:  this.foo = " + this.foo);   
            console.log("inner func:  self.foo = " + self.foo); 
        }());    
    }    
};    
myObject.func();

Output is - 
outer func:  this.foo = bar 
outer func:  self.foo = bar
inner func:  this.foo = undefined
inner func:  self.foo = bar

scope and scope chaining in javascript
