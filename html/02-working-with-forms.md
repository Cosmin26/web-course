# Working with form elements

```html
<form>
  <fieldset>
    <legend>Profile</legend>

    <label for="firstName">First name</label>
    <input
      type="text"
      id="firstName"
      name="firstName"
      placeholder="Your first name"
    />

    <label for="lastName">Last name</label>
    <input
      type="text"
      id="lastName"
      name="lastName"
      placeholder="Your last name"
    />

    <label for="email">Email</label>
    <input type="email" name="email" id="email" placeholder="Your email" />

    <label for="password">Password</label>
    <input
      type="password"
      name="password"
      id="password"
      placeholder="Your password"
    />

    <label for="favoriteColor">Favorite color</label>
    <input type="color" name="favoriteColor" id="favoriteColor" />

    <label for="avatar">Avatar picture</label>
    <input type="file" name="avatar" id="avatar" />

    <label for="income">Monthly income</label>
    <input type="range" id="income" name="income" min="0" max="10000" />

    <label for="gender">Gender</label>
    <select name="gender" id="gender">
      <option value="male">Male</option>
      <option value="female">Female</option>
      <option value="other">Other</option>
    </select>

    <label for="kids">Kids</label>
    <input
      type="number"
      name="kids"
      id="kids"
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
    <label for="bio">Short bio</label>
    <textarea name="bio" id="bio" rows="10" cols="100"></textarea>
  </fieldset>
</form>
```

### Code together

Implement a form for sending emails, having the following inputs: `fromName`, `toEmail`, `subject`, `message`.
The form's action should be the following url: `https://18z9lalk4f.execute-api.us-east-1.amazonaws.com/dev/email/send`.

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
