<!--  PART 1  -->

<!-- 1)
Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead. -->

var profileImage = document.querySelector(".profile-image")
profileImage
profileImage.setAttribute("src", "https://placebear.com/400/400")


<!-- 1)
Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

var portfolioImage = document.querySelector(".photography")
portfolioImage
portfolioImage.setAttribute("src", "https://dummyimage.com/325x225/000/00ccff")


<!-- 2)
Select the heading that says "Panda the Bear" and change it to your own name. -->

var title = document.querySelector("h1", ".highlight")
title
title.innerText
title.innerText = "Kaiser Chan"


<!-- 3)
Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

var employmentSubtitle = document.querySelector("#employment h3")
employmentSubtitle
employmentSubtitle.innerText = "History of Excellence"


<!-- 4)
Change the colour of the body -->

document.body.style.backgroundColor = "darkblue";


<!-- 5)
Change the colour of each element using the highlight class. Use a for loop to do this. -->

var highlight = document.querySelectorAll(".highlight")
highlight
for (var i = 0; i < highlight.length; i++) {
    highlight[i].style.color = "yellow";
}


<!-- 6)
Change the font family of the h1 to 'monospace'. -->

var title = document.querySelector("h1")
title
title.style.fontFamily = 'monospace'


<!-- 7)
Find a way to select the round icons in the sidebar and then change their colour. -->

var actionIcon = document.querySelectorAll(".action-icon-bg")
actionIcon
for (var i = 0; i < actionIcon.length; i++) {
    actionIcon[i].style.backgroundColor = "red";
}


<!-- 8)
Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

var nameField = document.querySelector("#name");
nameField
nameField.setAttribute('placeholder', "Identify Yourself")


<!-- 9)
Change the placeholder attribute of the message field to "state your business". -->

var messageField = document.querySelector("#message")
messageField
messageField.setAttribute("placeholder", "State your business")


<!-- 10)
Give the name field a "value" attribute of "your nemesis". -->

var nameField = document.querySelector("#name");
nameField
var attribute = document.createAttribute("value");
attribute.value = "Your nemesis";
nameField.setAttributeNode(attribute);


<!-- 11)
Change the value attribute of the email field to "koalathebear@gmail.com". -->

var emailField = document.querySelector('#email');
emailField
var attribute = document.createAttribute("value");
attribute.value = 'koalathebear@gmail.com';
emailField.setAttributeNode(attribute);


<!-- 12)
Change the value of the submit button on the contact form to "En garde!". -->

var submitButton = document.querySelector('#submit');
submitButton
submitButton.setAttribute('value', 'En garde!');


<!-- 13)
We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

var submitButton = document.querySelector('#submit');
submitButton
var disable = document.createAttribute('disabled');
submitButton.setAttributeNode(disable);

<!-- 14)
We should help Panda protect their privacy by erasing their personal details from the sidebar. -->

var bioInfoValue = document.querySelectorAll('.bio-info-value');
bioInfoValue
for (var i = 0; i < bioInfoValue.length; i++) {
    bioInfoValue[i].innerText = null;
}



<!--  PART 2  -->

<!-- Removing Elements from DOM  -->
<!-- 1)
Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element) -->

var timeTravel = document.querySelector('#time-travel');
timeTravel.parentNode.removeChild(timeTravel);
