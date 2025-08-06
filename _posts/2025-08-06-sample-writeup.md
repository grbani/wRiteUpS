---
# This is the "Front Matter" for the post.
# It contains metadata that Jekyll uses to build the page.

# Specifies that this post should use the 'post' layout we created.
layout: post

# The title of your writeup. This will be displayed at the top of the page.
title:  "Sample Writeup: The First Challenge"

# The date of publication.
date:   2025-08-06 19:45:00 +0000

# Tags help organize your posts. You can use them to filter content later.
tags: [ctf, web, beginner]
---

## Introduction to the Challenge

This is a sample writeup to demonstrate how posts are structured. The challenge was a simple web-based task where the goal was to find a hidden flag in the page's source code.

### Step 1: Analyzing the Web Page

The first step was to load the webpage and look for anything out of the ordinary. I used my browser's developer tools (`F12`) to inspect the HTML.

```html
<!-- I found this interesting comment hidden at the bottom of the body tag -->
<!-- The flag is not here, but you are getting warmer. Try checking the /assets/js/main.js file. -->
```

### Step 2: Finding the Flag

Following the hint from the comment, I navigated to the `main.js` file and found the flag encoded in Base64.

```javascript
// The flag is encoded to keep it safe from prying eyes ;)
var encodedFlag = "Q1RGe2p1c3RfZDFtbDBfMW5nX3RoM19zdHJ1Y3R1cmV9";

// To decode it, you can use a simple online tool or your terminal.
```

After decoding the string, I got the flag.

**Flag:** `CTF{just_d1m0_1n_th3_structure}`

This concludes the sample writeup! You can now create your own by following this format.
