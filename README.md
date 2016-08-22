#urlbar-notification-button
Use this with your Firefox add-on to place buttons in the url bar! Buttons are
sdk objects, so panels can be attached to them, just like standard sdk toggle
buttons.

# To use in your Firefox add-on
In the add-on directory:
```bash
$ npm install urlbar-notification-button --save
```

In your add-on code, import the class:
```
const { Button } = require('url-bar-notification-button');
```

You can then construct a button as follows:
```
const settings = {
  id,
  className,
  message, // message that button will display
  styleLocation, // place within data/ of your add-on directory
  iconLocation, // place within data/ of your add-on directory,
};

new Button(FirefoxWindow, onClickCallbackFn, settings);
```

Methods:
`destroy()`
Call to completely remove button

`show()`

`hide()`

`addClassToButton(class)`

`removeClassFromButton(class)`

# License
This add-on is licensed under the MPLv2. See the `LICENSE` file for details.
