# HTML Contact Form Lab
# HTML Iframe Lab

## Problem Statement

Business and company websites of all types and sizes typically want to provide
multiple ways for their customers or potential customers to contact them.  One
of the most common ways to do this is to provide a _contact form_.
The `iframe` element displays an entire HTML file inside itself, allowing one
HTML page to be contained within another. Before JavaScript became widely used,
_anytime_ a website user clicked on a link, the entire page would refresh. To
provide a better user experience, the `iframe` tag used to reload specific parts
of a page without changing others. For example, when a navigation link was
clicked, from the user's perspective, the navigation would remain the same, and
only the iframe portion of a page would reload.

In this lab, we will practice what we've learned about HTML forms by creating a
contact form similar to those we see on business websites.
With JavaScript, portions of an HTML page can be added and removed
programmatically without needing a refresh. This replaced the need for iframes
in many websites.

Still, there are some specific uses where iframes can be very valuable. One
example: embedded maps.   Embedded maps are a simple option for websites that
need a custom map, and are frequently used in contact pages for businesses. In
this case, an `iframe` can be used to contain an entire, interactive, map page
and place it within our own websites, without the need for writing our own
JavaScript.

In this lab, we will practice what we've learned about HTML iframes by creating
an embedded similar to those we see on business websites.

## Objectives

1. Apply our understanding of HTML forms by building a functional a contact form
1. Create an embedded Google map from scratch
2. Better understand what we've learned about HTML iframes and their attributes

## Deliverables
## Setting Up the Map

To see and test your form in action, run `httpserver` or open `index.html` in a
new browser tab. To test your work, run `learn`.
Before we can get to writing HTML, we need to get a map to embed within an
iframe.

Some basic HTML has been provided for this lab, along with HTML comments on what
is needed.  Follow the provided comments and test messages to see what is needed
when creating the form.  At completion, your form should have:
In your browser, head to
[https://www.google.com/maps](https://www.google.com/maps) and search for a
general location. For instance, `11 Broadway, Manhattan, NY`.

* A _required_ text input for a full name with a placeholder, "Enter Name"
* A _required_ email type input for an email address with a placeholder, "Enter Email"
* A _tel_ type input for a telephone number with a placeholder, "Enter Telephone (optional)"
* A text area for a user to include a message with a placeholder, "Enter Message"
* Labels for each text input
* A checkbox with text of your choosing
* A submit button
Now, click the menu icon located at the top left of the screen and select
**Share or embed map**. Then click the **Embed map** tab.

Google provides the entire iframe tag, but we will add some additional
attributes manually. Highlight the iframe embed code and copy it to your
clipboard. In `index.html` paste the code snippet.

## Deliverables

### The `required` Attribute
We've already got a basic `iframe`, but to pass all the tests, we'll need to add
the following attributes:

The `required` attribute will prevent the browser from submitting the form until
all required inputs are filled in properly. This is functionality is baked into
HTML5 for us automatically, all that is needed is to include the word 'required'
as an attribute, without setting it to any value.
* Add a `width` attribute set to "100%"
* Add a `height` attribute set to "400px"
* Change the `frameborder` attribute to "1"

When an input is required, the `type` attribute (e.g., `text` vs `email`) will
determine what the browser checks, so in the case of an email, the input must
match the format of an email address, including the "@".
Run `learn` to test your work and `learn submit` once you've passed all the
tests.

## Conclusion

Forms are an essential way for users to submit data to a website. Some forms,
like search bars, only contain a single input field, but we can make them as
complex as we need.
The `iframe` element that allows us to load another HTML page, such as this
simple google map page, inside our own HTML page. It is like
looking through a window from our page into another page displaying a Google
Map.

We will only be focused on building out the front end side of this form - it is
typically up to the _backend_ of a website to decide how to handle and store
form data when submitted, which is not within the scope of this lesson.
While iframes have been replaced in many places with JavaScript, they still
prove valuable in specific cases.

<p class='util--hide'>View <a href='https://learn.co/lessons/html-map-contact-form-code-along'>HTML Map Contact Form Code-along</a> on Learn.co and start learning to code for free.</p>
