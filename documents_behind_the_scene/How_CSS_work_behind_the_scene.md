# Load HTML #

- Parse HTML
- Document Object Model (DOM)


# Load CSS #

- Parse CSS
	+ Resolve conflicts CSS delcarations
	+ Process final CSS values
- CSS Object Model (CSSOM) 


# Website Rendering #

- Render tree
- the Visual Formating
- Final rendered Website


----------------------------

# CASCADE #

Source stylesheets
- Author CSS (put it the last if rely on 3rd-party stylesheets)
- User CSS
- Browser CSS (User Agent)

ORDER:
**IMPORTANCE > SPECIFICTY (If same IMPORTANCE) > SOURCE ORDER (If same SPECIFICTY)**

## 1st IMPORTANCE ##

- `!important`
- Author delcarations
- User delcarations
- Default browser delcarations


## 2nd SPECIFICTY ##

**Inline > IDs > Classess > Elements**

1. Inline styles ((Need Example))
2. IDs 

```css
/* The element with id="demo" */
#demo {
  border: red 2px solid;
}
```

3. Classess

```css
/* Classess: ".button" */
/* pseudo-class: ":hover" */
#nav a.button:hover {
	background-color: yellow;
}
```

4. Elements

```css
p {
  text-align: center;
  color: red;
}
```


## last SOURCE ORDER ##

The last delcaration in the code will override all other delcarations.

Means: The last delcarations will be applied.

