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
  
  // Include the Theme
  <link rel="stylesheet" type="text/css" href="css/mnav-theme.css"/>
```

###HTML Structure
```html
  <nav id="navigation">
    <ul>
      <li><a href="#">Link 1</a></li> <!-- No submenu -->
      <li><a href="#">Link 2</a> <!-- Has Submenu -->
        <ul>
          <li><a href="#">Sub Link 1</a></li>
          <li><a href="#">Sub Link 2</a></li>
        </ul>
      </li>
    </ul>
  </nav>
```

###Calling
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

###CSS Structure
```css
#ID_OF_CONTAINER {
  display: inline-block;
  position: relative;
  width: 100%;
}

/*Inside the media-query*/
#ID_OF_CONTAINER {
  padding-top: 40px;/* Height of your mobile button */
}
```
**Important:**
For the navigation to look its best, make all `anchor` tags be the same height as the buttons.

##Options
| Option Name       | Default      | Description                                      |
| ---------------   |:------------:| ------------------------------------------------ |
| `theme`           | 'mnav-theme' | The theme to be used for the menu (class name)   |
| `mainMenuSpeed`   | 200          | Speed when the main menu opens                   |
| `subMenuSpeed`    | 200          | Speed when the sub menu opens                    |
| `delayClose`      | 250          | Delay before the submenu closes after hover      |
| `mobileButtonPos` | 'right'      | Position the mobile button left, center or right |
| `subMenuOpen`     | false        | Open submenu by default (hides the arrow)        |

##Events
- `mnav.open` - Opens the main menu (same as if you clicked the mobile menu button)

##TODO
- [x] Implement theming
- [x] Implement Choice of whether to put the main menu button on the left or right side
- [ ] Add more themes (more icons?)

##Notes
You are free to modify the CSS and JS files to fit what you need to do. This is just a skeleton for you produce awesome apps in the future!

Happy Coding!

##Version History:
 - `1.1` - Fixed public event `mnav.open` bug, and restructured how hover and click events are handled
 - `1.2` - Added an example on how to use `mnav.open` event in `index.html`, and added some pretty styling
