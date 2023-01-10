# Animated Mail Button
A simple, animated mail button built using HTML and CSS. The button features an envelope icon that animates and transforms into a "check" icon when clicked, indicating that the mail has been sent successfully.

## HTML
This code creates an animated mail button using HTML and CSS. The HTML structure consists of a container element with a class of "letter-image", which contains several child elements that make up the different parts of the mail button.

```HTML
  <div class="letter-image">
    <div class="animated-mail">
      <div class="back-fold"></div>
      <div class="letter">
        <div class="letter-border"></div>
        <div class="letter-title"></div>
        <div class="letter-context"></div>
        <div class="letter-stamp">
          <div class="letter-stamp-inner"></div>
        </div>
      </div>
      <div class="top-fold"></div>
      <div class="body"></div>
      <div class="left-fold"></div>
    </div>
    <div class="shadow"></div>
  </div>
```

## CSS
The CSS code styles these elements to create the animation. The animated-mail class is used to style the overall button, and several other classes are used to style the individual parts of the button (e.g. `body`, `top-fold`, `back-fold`, etc.). The `-webkit-transition`, `-moz-transition`, and `transition` properties are used to create the animation effect when the button is hovered over, by transitioning the transform property of several elements.

You could add an on hover effect, that makes the button appear like it's being pressed and then released.

```CSS
.letter-image:hover .animated-mail {
  -webkit-transform: rotateX(90deg);
  -moz-transform: rotateX(90deg);
  transform: rotateX(90deg);
  -webkit-transition-duration: 0.5s;
  -moz-transition-duration: 0.5s;
  transition-duration: 0.5s;
}
```

It's worth noting that this button's design is meant to look like a folded piece of mail and this animation is for demonstration purposes only, As the design and functionality of the button, need to be adjusted to fit the desired context.

It could also be helpful to add some JavaScript functionality, to create a link when the button is clicked that would take you to your email client, or a mailto link.

## Usage
To use this button, simply copy and paste the HTML and CSS into your project.

Please let me know if you need any further modifications.

## Preview
<img width="957" alt="Screenshot_20230110_195125" src="https://user-images.githubusercontent.com/59678435/211579428-860f4f36-b305-45c7-be22-12e00d519f65.png">
