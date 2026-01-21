I found the default Blogger fonts hard to read, so I switched to a more readable font that fits my preferences which is Google San Flex. This method is also works for other fonts as well.

1. Pick your font at https://fonts.google.com/selection
2. Click **<> Get embeded code**
3. Copy the line similar to this one:
```
<link href="https://fonts.googleapis.com/css2?family=Google+Sans+Flex:opsz,wght@6..144,1..1000&display=swap" rel="stylesheet">
```
4. Add `amp;` after the ampersand `&` and add slash `/` just before the right bracket `>`. You will get
```
<link href='https://fonts.googleapis.com/css2?family=Google+Sans+Flex:opsz,wght@6..144,1..1000&amp;display=swap' rel='stylesheet'/>
```
5. In the theme's HTML of blogger, look for `<head>`. Then add the code in step 4 just beneath `<head>`
6. Searh for `]]></b:skin>` using `Ctrl + F`, add the following code block above it.
```
body, p, .post-body, h1, h2, h3, h4 {
    /* Switch to Google Sans Flex */
    font-family: 'Google Sans Flex', sans-serif !important;
    
    /* 'wght' 420: Slightly thicker than normal for better digital legibility */
    /* 'opsz' 14: Adjusts letter shapes for standard paragraph reading */
    font-variation-settings: 'wght' 420, 'opsz' 14 !important;
    
    /* Optional: ensures a clean line height for the body text */
    line-height: 1.6;
}

/* Specific adjustment for Headers to make them stand out */
h1, h2, h3, h4 {
    font-variation-settings: 'wght' 700, 'opsz' 36 !important;
    margin-top: 20px;
}
```
