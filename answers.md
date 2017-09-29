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
