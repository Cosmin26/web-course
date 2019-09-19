# Working with form elements

```html
<form>
  <fieldset>
    <legend>Profile</legend>

    <label>First name</label>
    <input type="text" name="firstName" placeholder="Your first name" />

    <label>Last name</label>
    <input type="text" name="lastName" placeholder="Your last name" />

    <label>Email</label>
    <input type="email" name="email" placeholder="Your email" />

    <label>Password</label>
    <input type="password" name="password" placeholder="Your password" />

    <label>Gender</label>
    <select name="gender">
      <option value="male">Male</option>
      <option value="female">Female</option>
    </select>

    <label>Kids</label>
    <input
      type="number"
      name="kids"
      placeholder="How many kids you have?"
      min="0"
    />

    <label>
      <input type="checkbox" name="agreeTerms" /> I agree the Terms & Conditions
    </label>
  </fieldset>

  <fieldset>
    <legend>How you want to be contacted?</legend>
    <label> <input type="radio" value="email" name="contactBy" /> Phone </label>
    <label><input type="radio" value="phone" name="contactBy" /> Email </label>
  </fieldset>

  <fieldset>
    <legend>About yourself</legend>
    <textarea rows="10" cols="100"></textarea>
  </fieldset>
</form>
```

# Homework

Create a form for buying a cinema ticket. The form will have the following sections:

#### In the first `fieldset` with the `legend`: _"Contact details"_ we will have inputs for:

- firstName (text)
- lastName (text)
- email (email)
- phone (phone)

#### In the second `fieldset` with the `legend`: _"Choose a movie"_ we will have inputs for:

- movie (radio). For `movie` use the following `radio` inputs, so the user can choose only one option: `Godzilla`, `Aladin`, `Avengers`, `Rocketman`, `Spider-man`.

#### In the third `fieldset` with the `legend`: _"Choose location"_ we will have a single input:

- location (select). For `location` use a `select` input with `options` for: `Cinema City - Iulius` si `Cinema City - Vivo`.

#### In the fourth `fieldset` with the `legend`: _"Terms and conditions"_ we will have inputs for:

- acceptTerms (checkbox)

At the end of the form put a button with `type="submit"` and text: `Buy tickets`.

**Happy coding!!!** ⌨️
