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

Copy and paste this code:

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

- Switch the "include" code with the paragraph to move the image from left to right