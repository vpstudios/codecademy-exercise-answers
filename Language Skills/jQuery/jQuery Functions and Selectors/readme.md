##[1. Functions, Part I: $(document).ready] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Functions are the basic unit of action in jQuery.
```script.js
$(document).ready(function() {
    $('div').hide();    
});
```
##[2. Functions, Part II: Functions Explained] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* A function is made up of three parts: the function keyword, any inputs that function takes (they go between the ()s and are separated by commas if there are more than one), and whatever actions the function should perform (these go between the {}s).
```script.js
$(document).ready(function() {
    $('div').click(function() {
        $('div').fadeOut('slow');
    });
});
```
##[3. Variables] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Variables are a place for us to store information for use at a later time. Variables can hold any type of information you work with, so just think of them as containers.
```script.js
$(document).ready(function() {
var $target=$('li:last-child');
$target.fadeOut('fast');
});
```
##[4. $p vs $('p')] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
```script.js
var $div = $('div');
```
##[5. Using Functions to Select HTML Elements] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
```script.js
$(document).ready(function() {
    $('div').fadeIn('slow');
});
```
##[6. Selecting by Class] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* We don't have to limit ourselves to selecting HTML elements.
```script.js
$(document).ready(function() {
    $('button').click(function() {
        $('.vanish').fadeOut('slow');
    });
});
```
##[7. Selecting by ID] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* If we can select by class, it follows that we can also select by ID.
```script.js
$(document).ready(function() {
    $('button').click(function() {
        $('#blue').fadeOut('slow');
    });
});
```
##[8. Flexible Selections] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Anything you can target with CSS, you can modify with jQuery.
```script.js
$(document).ready(function() {
    $('.pink, .red').fadeTo('slow',0);    
});
```
##[9. 'this' is important!] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
```script.js
$(document).ready(function() {
    $('div').click(function() {
        $(this).fadeOut('slow');
    });
});
```
##[10. Ready?] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* All right! Time to use our new jQuery knowledge to add another interactive component to our website: a sliding panel that moves up and down when clicked.
```script.js
$(document).ready(function() {
    $(this).click();    
});
```
##[11. Click and Pull] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Good! Now we want to trigger an event when the "Slide Up/Down" tab is clicked (that tab's class is .pull-me).
```script.js
$(document).ready(function() {
    $('.pull-me').click();    
});
```
##[12. Toggling Our Panel] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Perfect! Just one more step: we need to tell .click() what to do. In this case, when our pull tab is clicked, we want our sliding panel (with the class .panel) to open or close.
```script.js
$(document).ready(function() {
    $('.pull-me').click(function() {
        $('.panel').slideToggle('slow');    
    });    
});
```
##[13. Well Done!] (https://github.com/vpstudios/Codecademy-Exercise-Answers/blob/master/Language%20Skills/jQuery/jQuery%20Functions%20and%20Selectors/script.js)
* Great work! See how easy this is? With a little jQuery magic, you can make your websites do all kinds of amazing things.
```script.js
$(document).ready(function() {
    $('.pull-me').click(function() {
        $('.panel').slideToggle('slow');    
    });    
});
```