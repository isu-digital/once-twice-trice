# Add content to exhibit pages

## Create a GitHub account

1. Go to <https://github.com>
2. Click the "Sign up" button
3. Enter your email and create a username and password to complete the sign up process
4. Send your username to Olivia, she'll add you to the repository

## Edit page text

1. Find and open exhibit pages in the "pages" folder (example: `introduction.md`)
2. Review Markdown basics: <https://evanwill.github.io/markdown-everywhere/content/3-md-reference.html>
3. Dilineate sections using headings

## Add images

### To wrap text around images:

1. Copy and paste the "include" code to include images: `{% include feature/image-float.html objectid="trice_015" float="start" width="50" %}`
2. Replace values for `objectid`, `float`, and `width`:
    - `objectid`: Any objectid that corresponds to an item in the exhibit (refer to metadata spreadsheet: <https://docs.google.com/spreadsheets/d/14yu7vqfoq3Ti15D4EWcGOeBtc1Q_As88Vcan5qpo4mA/edit?usp=sharing>)
    - `float`: Float the image left or right. Options: `start` = left; `end` = right
    - `width`: Set the width of the image. Options: `25`, `50`, `75`, `100`

### To place images and text side by side:

For image to show up on the **left**, copy and paste this code:

```
<div class="row pt-3">
<div class="col-md-5" markdown="1">

{% include feature/image.html objectid="trice_029" %}

</div>
<div class="col-md-7" markdown="1">

Phasellus id finibus diam, sit amet mollis velit. Phasellus pretium vulputate orci, id fermentum neque congue eu. Nulla mollis, felis ut interdum tempor, purus tortor ullamcorper massa, lobortis aliquam odio urna eget purus. Nulla feugiat enim magna, quis condimentum metus rhoncus et. Duis nec dui eu nibh consequat vestibulum non sit amet urna. Pellentesque at nulla quis orci aliquet placerat ut ut urna. Integer sed placerat ex. Sed volutpat elementum enim, ac accumsan eros aliquam et. Nam eu ante in ante ullamcorper rutrum. Etiam leo lorem, posuere vitae sem non, vestibulum volutpat massa. Fusce eu commodo mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Praesent a enim ac enim fringilla lobortis et vel justo. Phasellus ut venenatis purus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer vel diam porta, interdum neque sit amet, scelerisque massa. Cras ut placerat eros. Fusce scelerisque, eros et scelerisque suscipit, lacus purus blandit orci, id pulvinar tellus diam sit amet dui. Vivamus a elit tristique, efficitur nisi eu, suscipit lorem. Suspendisse a sapien aliquam, ultrices magna sed, accumsan massa. Etiam vitae tempor tortor. Cras pharetra a ipsum sit amet porttitor. Suspendisse potenti.

</div>
</div>
```

- In the image include, replace values for `objectid`. Add or edit the value for `width` if needed:
    - `objectid`: Any objectid that corresponds to an item in the exhibit (refer to metadata spreadsheet: <https://docs.google.com/spreadsheets/d/14yu7vqfoq3Ti15D4EWcGOeBtc1Q_As88Vcan5qpo4mA/edit?usp=sharing>)
    - `width`: Set the width of the image. Options: `25`, `50`, `75`, `100`

For an image that shows up on the **right**, copy and paste this code:

```
<div class="row pt-3">
<div class="col-md-5" markdown="1">

Phasellus id finibus diam, sit amet mollis velit. Phasellus pretium vulputate orci, id fermentum neque congue eu. Nulla mollis, felis ut interdum tempor, purus tortor ullamcorper massa, lobortis aliquam odio urna eget purus. Nulla feugiat enim magna, quis condimentum metus rhoncus et. Duis nec dui eu nibh consequat vestibulum non sit amet urna. Pellentesque at nulla quis orci aliquet placerat ut ut urna. Integer sed placerat ex. Sed volutpat elementum enim, ac accumsan eros aliquam et. Nam eu ante in ante ullamcorper rutrum. Etiam leo lorem, posuere vitae sem non, vestibulum volutpat massa. Fusce eu commodo mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Praesent a enim ac enim fringilla lobortis et vel justo. Phasellus ut venenatis purus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer vel diam porta, interdum neque sit amet, scelerisque massa. Cras ut placerat eros. Fusce scelerisque, eros et scelerisque suscipit, lacus purus blandit orci, id pulvinar tellus diam sit amet dui. Vivamus a elit tristique, efficitur nisi eu, suscipit lorem. Suspendisse a sapien aliquam, ultrices magna sed, accumsan massa. Etiam vitae tempor tortor. Cras pharetra a ipsum sit amet porttitor. Suspendisse potenti.

</div>
<div class="col-md-7" markdown="1">

{% include feature/image.html objectid="trice_029" %}

</div>
</div>
```

- In the image include, replace values for `objectid`. Add or edit the value for `width` if needed:
    - `objectid`: Any objectid that corresponds to an item in the exhibit (refer to metadata spreadsheet: <https://docs.google.com/spreadsheets/d/14yu7vqfoq3Ti15D4EWcGOeBtc1Q_As88Vcan5qpo4mA/edit?usp=sharing>)
    - `width`: Set the width of the image. Options: `25`, `50`, `75`, `100`

## Include multiple images on the same line:

Use code block below. Add multiple objectid values to the `objectid` variable, separated by a semicolon (ex. `objectid="trice_002;trice_003"`):

```
<div class="row pt-3">
<div class="col-md-5" markdown="1">

{% include feature/image.html objectid="trice_002;trice_003" %}

</div>
<div class="col-md-7" markdown="1">

Phasellus id finibus diam, sit amet mollis velit. Phasellus pretium vulputate orci, id fermentum neque congue eu. Nulla mollis, felis ut interdum tempor, purus tortor ullamcorper massa, lobortis aliquam odio urna eget purus. Nulla feugiat enim magna, quis condimentum metus rhoncus et. Duis nec dui eu nibh consequat vestibulum non sit amet urna. Pellentesque at nulla quis orci aliquet placerat ut ut urna. Integer sed placerat ex. Sed volutpat elementum enim, ac accumsan eros aliquam et. Nam eu ante in ante ullamcorper rutrum. Etiam leo lorem, posuere vitae sem non, vestibulum volutpat massa. Fusce eu commodo mi. Interdum et malesuada fames ac ante ipsum primis in faucibus. Praesent a enim ac enim fringilla lobortis et vel justo. Phasellus ut venenatis purus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer vel diam porta, interdum neque sit amet, scelerisque massa. Cras ut placerat eros. Fusce scelerisque, eros et scelerisque suscipit, lacus purus blandit orci, id pulvinar tellus diam sit amet dui. Vivamus a elit tristique, efficitur nisi eu, suscipit lorem. Suspendisse a sapien aliquam, ultrices magna sed, accumsan massa. Etiam vitae tempor tortor. Cras pharetra a ipsum sit amet porttitor. Suspendisse potenti.

</div>
</div>
```

## Update Navigation Menu

1. In selected page (ex. `theme1.md`) edit the value for `title` on line 2.
2. Edit the value for `permalink` on line 4 to reflect the new permalink for your page (will show up in URL). Example: `once.html`
3. Locate and open the `config-nav.csv` file within the `_data` folder.
4. Locate the page name you want to change (ex. `Theme 1` -> `Once`), and insert your new page name in its place.
5. Locate the corresponding permalink you want to change (ex. `theme1.html` -> `once.html`), and insert your new permalink in its place.
6. The edited `config-nav.csv` now might look something like this:

```
display_name,stub,dropdown_parent
Introduction,/,
Once,/once.html,
Theme 2,/theme2.html,
Theme 3,/theme3.html,
Theme 4,/theme4.html,
Theme 5,/theme5.html,
```