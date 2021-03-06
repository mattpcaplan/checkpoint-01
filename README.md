# Checkpoint 01

## Instructions

1. Fork this repo.
2. Clone your fork.
3. Follow the instructions.
4. Make one commit for each question.
5. Open a pull request to this repo.

If you finish early, try tackling the [Moonrise Kingdom exercise](https://github.com/ga-wdi-exercises/moonrise_kingdom/blob/master/sam_registration.jpg).

--------------

## HTML

### #1

Open up `index.html` in a text editor and browser. Link to the provided stylesheet.

<link rel='stylesheet' href='styles.css' type="text/css">

### #2

Identify one non-semantic tag and replace it with a semantic one.

ORIGINAL:
<div class='main'>
  <h2>The Main Content</h2>

Semantic version:
<header class='main'>
  <h2>The Main Content</h2>


### #3

Something about the image tag is incorrect. Fix the error.

ORIGINAL:
<img src='https://jesse.sh/img/me.jpg'>

Update:
<img src="https://jesse.sh/img/me.jpg" alt="Jesse Playing guitar">

### #4

Change the title of the page. Specifically, change what shows in the tab of the page (i.e., at the top of the browser).

ORIGINAL:
<head>
  <link rel='stylesheet' href='styles.css' type="text/css">
</head>

Update:
<head>
  <link rel='stylesheet' href='styles.css' type="text/css">
  <title>Jesse's Page</title>
</head>

### #5

Set the margin to 0 for each direct child of:

- `header`
- `footer`
- `.main`
- `aside`

header > * footer > * .main > * aside > * {
margin:0;  
}

### #6

If you inspect the `.left` and `.right` elements, you will see that they have `width: 50%;` and `float: left`. However, they are not sitting next to each other.

Fix this issue without modifying any of `.left` and `.right`'s `padding`, `border`, or `width`.

> Commit

### #7

When the page is fewer than 600px wide, the background of `.main` turns red.

Instead of making `.main` red, reorder the elements to...

@media(max-width:600px){
  header{
    order:1;
  }
  .main{
    order:2;
  }
  aside{
    order:3;
  }
  aside{
    order:4;
  }
  footer{
    order:5;
  }
}

Do this using only CSS -- do not rearrange the HTML.


### #8

Open up `workflow.txt`

Rearrange the lines to identify the correct workflow for submitting a pull request on a non-master branch.

Remove the lines that are not required in this workflow.

> Commit
