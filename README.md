# jQuery Gender Field

A jQuery plugin for transgender friendly gender form fields. Collect semi-structured data from your forms.
You're probably already storing gender as a string, so why not allow your users to tell you more?

A dropdown box gives many options like a select field, for ease of use. But by utilizing a text field, genderField can provide suggestions as the user types, as well as enable the user to type their gender as they wish.

[Try it on jsfiddle!](http://jsfiddle.net/Lda8yvsc/)

## Usage

Add jquery.genderField.js and jquery.genderField.css to your server, add the following lines to your HTML:

```
<script src="jquery.genderField.js"></script>
<link rel="stylesheet" href="jquery.genderField.css">
```

Then add the following code in `<script>` tags or in a .js file, replacing #gender with the id or selector for your input text field:

```javascript
$(document).ready(function() {
	$("#gender").genderField();
});
```
	
And that's it!

## Styling

`.genderField-dropdown` and `.genderField-dropdown span` can easily be styled using additional CSS.

## Default Genders

This is by no means a complete list of all genders, but captures many common genders.

* Agender
* Androgyne
* Androgynous
* Bigender
* Cis Female
* Cis Feminine
* Cis Male
* Cis Masculine
* Cis Woman
* Demigirl
* Demiguy
* Female
* Feminine
* Femme
* Genderqueer
* Genderweird
* Gender Fluid
* Intergender
* Intersex
* Male
* Man
* Masculine
* Neutrois
* Nonbinary
* Other
* Pangender
* Trans Female
* Trans Male
* Trans Man
* Trans Feminine
* Trans Femme
* Trans Woman
* Woman

## Additional Genders

Pass an object into `$(selector).genderField()` to add additional genders or turn off the background arrow image.
e.g.

```javascript
$(selector).genderField({showArrow:false, additionalGenders: ['third gender','none']});
```

## Options

* `additionalGenders (String[])`: Adds additional genders to the default list.
* `genders (String[])`: Sets the dropdown list of genders to the provided array.
* `lowercase (Boolean)`: Sets the gender list to have all lowercase genders. Default is `true`.
* `showArrow (Boolean)`: Sets the design of the box to show a dropdown arrow or not. Default is `true`.
* `allowPreferNotToDisclose (Boolean)`: Sets the dropdown to have a "Prefer not to disclose" option or not. Default is `true`.

