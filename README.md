# Login Page

![Image of login page](https://github.com/gabrielrowan/LoginPageFE/assets/86267314/4834fd7a-3263-4431-a860-9158493c634e)

## Responsive Design

Adapatable to desktop and mobile screen sizes

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
* Focus styles on all form elements

```css
.login-card .btn:focus {
    background-color: rgb(254,241,251, .9);
    color: black;
    box-shadow: 0 0 10px rgba(163,152,246 .4);
}
```

* `alt` text on icons
* `Labels` used in html instead of placeholder text
* `aria-required=true` used on inputs so that required field is read out to screen readers

```html
 <label for="username">Email address</label>
 <input type="text" id="username" aria-required="true">
 <i class='bx bxs-user' alt="User Icon"></i>
```
  
