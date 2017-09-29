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
