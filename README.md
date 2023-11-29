# Login Page

![Image of login page](https://github.com/gabrielrowan/LoginPageFE/assets/86267314/4834fd7a-3263-4431-a860-9158493c634e)

## Responsive Design

Adapatable to desktop and mobile screen sizes

![Image of login page on Galaxy Fold screen size](https://github.com/gabrielrowan/LoginPageFE/assets/86267314/275da9c1-3c15-45b2-8cbb-0c1ac8cc1136)

Responsiveness achieved by redefining font and card padding variables:

```css
:root {
    --fs-header: 36px;
    --fs-medium: 16px;
    --fs-small: 14.5px;
    --pd-card: 30px 40px;
}

@media (max-width: 400px)
{
    :root {

        --fs-header: 32px;
        --fs-medium: 14px;
        --fs-small: 12px;
        --pd-card: 20px 13px;
    }
}
```

## Accessibility

* Colour contrast ratio meets AA and AAA web standard

![Screenshot of colour contrast ratio for login form getting AA and AAA rating](https://github.com/gabrielrowan/LoginPageFE/assets/86267314/f156f507-e5db-42a4-ab3b-273ead73d74c)
  
* Focus styles on all form elements

![Focus background style in effect on email address input field](https://github.com/gabrielrowan/LoginPageFE/assets/86267314/59d6ad56-744c-4ef3-af34-31022e3c61c6)

```css
.login-card .btn:focus {
    background-color: rgb(254,241,251, .9);
    color: black;
    box-shadow: 0 0 10px rgba(163,152,246 .4);
}
```

* `alt` text on icons
* `label` tags used in html instead of placeholder text
* `aria-required=true` used on inputs so that required field is read out to screen readers

```html
 <label for="username">Email address</label>
 <input type="text" id="username" aria-required="true">
 <i class='bx bxs-user' alt="User Icon"></i>
```
  
