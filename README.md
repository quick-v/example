# Form Validation Example with Quickv

In this repository, we explore various form validation examples using Quickv. [Quickv](https://github.com/quick-v/quickv) is a powerful tool that allows you to quickly set up validation rules for your form fields, ensuring the integrity of user-submitted data.

## Installation

To get started, you can follow the official Quickv tutorial for a more detailed installation guide: [https://quickv.vercel.app/docs/tutorial](https://quickv.vercel.app/docs/tutorial).

You can clone the form validation examples repository with Quickv from this repository.

## Validation Examples

In this repository, you will find different examples of form validation using Quickv. Each example is designed to illustrate a specific validation rule and can be used as a starting point for your own projects.

Here are some examples of using Quickv to validate different types of form fields:

### Name Field

```html
<div class="form-group">
  <label for="name">Name</label>
  <input type="text" id="name" name="name" data-qv-rules="required|only:string|startWithUpper|between:2,32" />
  <div data-qv-feedback="name"></div>
</div>
```

This code validates a name field by applying the following rules:
- `required`: the field is required and cannot be empty.
- `only:string`: the name should only contain letters.
- `startWithUpper`: the name should start with an uppercase letter.
- `between:2,32`: the length of the name should be between 2 and 32 characters.

### Email Address Field

```html
<div class="form-group">
  <label for="email">Email Address</label>
  <input type="email" id="email" name="email" data-qv-rules="required|email" />
  <div data-qv-feedback="email"></div>
</div>
```

This code validates an email address field using the following rules:
- `required`: the field is required and cannot be empty.
- `email`: the email address must be in a valid format.

### Password Field

```html
<div class="form-group">
  <label for="password">Password</label>
  <input type="password" id="password" name="password" data-qv-rules="required|min:8" />
  <div data-qv-feedback="password"></div>
</div>
```

This code validates a password field by applying the following rules:
- `required`: the field is required and cannot be empty.
- `min:8`: the minimum length of the password should be 8 characters.

These examples are just a glimpse of the possibilities offered by Quickv. You can explore further validation rules available in the official Quickv documentation: [https://quickv.vercel.app/docs/validation/rules](https://quickv.vercel.app/docs/validation/rules).

Feel free to experiment with these examples and adapt them to your specific needs. With Quickv, form validation becomes simple and efficient!