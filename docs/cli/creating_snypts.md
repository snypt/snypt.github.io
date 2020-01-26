# Creating Snypts

Now that your Snypt CLI project has been configured properly it's time to start creating some snypts.

To recap Snypt CLI will look through all files listed in snypt.json for snypts to save. 

To create snypts in code we add simple annotations around the code we want to save. 

Take the following example:

Let's say we want to save this method:

```javascript
    function doStuff(){
        let answer = 1 + 1;
        console.log(answer);
    }
```

We would add a comment at the beginning and the end as such 

```javascript
    //@@code @note {my sample function} @tags {code, sample, for-later}
  function doStuff(){
        let answer = 1 + 1;
        console.log(answer);
    }
    //@end
```

Because these examples are javascript comments are added with __//__. This can be done 
in any language using the appropriate syntax. 

The first part of our comments should include the type of snypt we are adding.
Currently only ``@@code`` and ``@@colors`` are supported.

The second two value are optional ``@note`` and ``@tags``. 

Other full examples

```javascript
    //@@code @note {my sample function} @tags {code, sample, for-later}
  function doStuff(){
        let answer = 1 + 1;
        console.log(answer);
    }
    //@end
```

```css
/* @@colors @note {gradient for home page} @tags {css, colors}*/
.alt{
    background: #ED213A;  /* fallback for old browsers */
    background:-webkit-linear-gradient(to right, #93291E, #ED213A);
    background:linear-gradient(to right, #93291E, #ED213A); 
}
/* @end */
```
