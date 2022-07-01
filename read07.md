* [Home page](https://rdball.github.io/reading-notes/)
* [Class 01 learning about markdown](read01)
* [Class 02 the coder's computer](read02)
* [Class 03 git and GitHub](read03)
* [Class 04 HTML review](read04)
* [Class 05 CSS](read05)
* [Class 06 JavaScript](read06)
* [Class 07 Programming with JS](read07)
* [Class 08 Operators and Loops](read08)

# Read: 07 - Programming with Javascript

**reminder to self: there are some aspects of JS that are similar to python. Example, declaring functions, if, then, else statements, operators (most mathematical operators carry over +, *, /, -, **... etc)

A javascript function must first be declared, named and then given parameters of what it should execute when called on (invoked)

Functions are used to “declare” a named set of instructions for javascript to execute when the declared function is called (invoked)

The name of a function should follow camel case if using more than one word to name the function. So if you wanted to name a function for “changing font type” you could enter changeFontType to conform with camel case rather than ChangeFontType or changefonttype

The **optional** parameters *inclosed with ()* after the function name can give your function a parameter to run against the function code. You can have multiple parameters within the () as long as they are separated by a `,` example: (red, green, blue) 

Example of a Javascript function with variables:

    function multiplyNumbers(price, shipping) {
    //Return the sum
        return price*shipping;
    }

    //Call MULTIPLY to multiply the two numbers
    var product=multiplyNumbers(22, 2);

    console.log(product)

This example has a `function` named `multiplyNumbers`. This function contains the parameters `(price, shipping)` and it ends with a `{`

Next we add the code we want the function to execute. For this example we want the code to `return price*shipping;` this will return the value of price multiplied by shipping. This function is then closed with `}` following the code that the function will execute.

Below the function we have a variable that names “product” being equal to our function with the numbers `(22, 2)` Theses numbers will replace the parameters in our named function and will return the sum of 22*2 when we write to the console with `console.log(product)`
Javascript can be linked in the head of your html document with 
    <script src="app.js"></script>

And then a function within your javascript file such as:

    function likeCardio(){  
        let usersChoice = prompt("do you like cardio?");
   
        if (usersChoice.toLowerCase() == "yes"){
            document.write("so you like cardio? perfect, let's train");
    } else{
        document.write("not a fan of cardio? that's alright, feel free to look around and maybe check out strength");
    }
}

Can be called (invoked) with a script in your HTML file where you want the code to display in your HTML page such as:

    <script>likeCardio();</script>