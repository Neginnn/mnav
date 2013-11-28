#Mobile Navigation (Mnav)

Author: Karl Castillo<br/>
License: MIT

##Instructions
```html

  // Include jQuery
  <script type="text/javascript" src="js/jquery-1.10.2.min.js"></script>
  
  // Include Mnav
  <script type="text/javascript" src="js/mnav.js"></script>
  
  // Include the CSS
  <link rel="stylesheet" type="text/css" href="css/mnav.css"/>
```
```javascript
  // Call Mnav
  $(function() {
    $('selector').Mnav();
  });
  
  // or
  
  $(function() {
    $('selector').Mnav({
      // options
    });
  }
```


##Options
| Option Name     | Default | Description                    |
| --------------- |:-------:| ------------------------------ |
| `mainMenuSpeed` | 200     | Speed when the main menu opens |
| `subMenuSpeed`  | 200     | Speed when the sub menu opens  |

##Events
- `mnav.open` - Opens the main menu (same as if you clicked the main menu button)

##TODO
- [ ] Implement theming
- [ ] Implement Choice of whether to put the main menu button on the left or right side

##Notes
You are free to modify the CSS and JS files to fit what you need to do. This is just a skeleton for you produce awesome apps in the future!

Happy Coding!
