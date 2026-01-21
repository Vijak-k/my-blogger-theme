The page margins are too close to the body text. We can adjust it using the following step
1. Go yo HTML of the theme
2. Search for `]]></b:skin>` using `Ctrl + F`
3. Paste the following code above it
```
/* Add 20px margins to the Header and Main Content */
header, 
.header-outer, 
.main-inner, 
.post-body, 
.content-inner {
    padding-left: 20px !important;
    padding-right: 20px !important;
    box-sizing: border-box;
}

/* Ensure the background stays full width if applicable */
.content-outer, .header-outer {
    max-width: 100%;
}
```
4. Save it.
