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

1. Use "include" code to include images: `{% include feature/image-float.html objectid="trice_015" float="start" width="50" %}`
2. Replace values for `objectid`, `float`, and `width`:
    - `objectid`: Any objectid that corresponds to an item in the exhibit (refer to metadata spreadsheet: <https://docs.google.com/spreadsheets/d/14yu7vqfoq3Ti15D4EWcGOeBtc1Q_As88Vcan5qpo4mA/edit?usp=sharing>)
    - `float`: Float the image left or right. Options: `start` = left; `end` = right
    - `width`: Set the width of the image. Options: `25`, `50`, `75`, `100`