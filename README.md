# Frontend Mentor - Newsletter sign-up form with success message solution

This is a solution to the [Newsletter sign-up form with success message challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/newsletter-signup-form-with-success-message-3FC1AZbNrv). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- Add their email and submit the form
- See a success message with their email after successfully submitting the form
- See form validation messages if:
  - The field is left empty
  - The email address is not formatted correctly
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Links

- Solution URL: [Add solution URL here](https://olubabadee.github.io/Newsletter-signup-form/index.html)
- Live Site URL: [Add live site URL here](https://olubabadee.github.io/Newsletter-signup-form/index.html)

## My process

### Built with

- Semantic HTML5 markup
- CSS3
- CSS Grid
- Flex
- Media Query for the different display widths

### What I learned

Well I am already knowledgeable on HTML and CSS
But it has been a while I really practiced so this was more like a revision for me.
I also got to test out using AI (Chat GPT) to aid the building of my website which was quite helpful.
Plus my JavaScript code is not the best so Utilize AI (Chat GPT) in getting my JavaScript code for the form dynamism

### Some Code I am Proud of

```js
 // Check if the email is empty or not valid
          if (
            emailInput.value.trim() === "" ||
            !isValidEmail(emailInput.value)
          ) {
            // Show error message and apply error styling
            labelError.classList.remove("hidden");
            emailInput.style.backgroundColor = "var(--lighttomato)";
            emailInput.style.color = "var(--tomato)";
            emailInput.style.border = "2px solid var(--tomato)";
            emailInput.style.placeholderColor.textcontent = "var(--dark)";
          } else {
            // Email is valid
            labelError.classList.add("hidden"); // Hide the error message

            // Reset the styling to default
            emailInput.style.border = "solid var(--grey) 1px";
            emailInput.style.color = "var(--black)";
            emailInput.style.backgroundColor = "var(--white)";

            // Store the email address (you can use localStorage, cookies, or send it to a server)
            const storedEmail = emailInput.value;

            // Redirect to the success page
            window.location.href = `success.html?email=${encodeURIComponent(
              storedEmail
            )}`;
          }
        });

```

### Continued development

Well I would like to master the form and submit action, for instance I found it difficult storing the email address in the first page and using it in the success page.

### Useful resources

Well I got all my solutions from Chat GPT, the thing is you would neeed to know how to ask the AI the right questions so as to get the right answers. Sometimes sharing a snippet of your code will help the AI recognize what your intentions are.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Olubabadee)
- Twitter - [@yourusername](https://twitter.com/babaspecial1)
