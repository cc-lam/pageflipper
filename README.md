pageflipper
=======

A jquery plugin for creating a panel of pages the user can flip trough using either touch events or mouse events. It feels as smooth and responsive as flipping pages in a native touch app. It is especially designed for the iPad.

## Usage
Load the necessary javascript and css files:

```html
<script type="text/javascript" src="path/to/jquery.pageflipper.js"></script>
<link rel="stylesheet" type="text/css" href="path/to/pageflipper.css"> 
```

Initialize the pageflipper on the wanted dom element:

```javascript
$(document).ready(function() {

   $( '#pageflipper' ).pageflipper( );

   $( '#page1' ).focus( function( ) {
      console.log( '#page1 in focus' );
      //Do ajax or whatever
   });

   $( '#page2' ).focus( function( ) {
      console.log( '#page2 in focus' );
      //Do ajax or whatever
   });

   $( '#page3' ).focus( function( ) {
      console.log( '#page3 in focus' );
      //Do ajax or whatever
   } ;

});
```

The pageflipper needs a ul with a li pr page to work:

```html
<div id='pageflipper'>
   <ul>
      <li id='page1'>
         <p>Page 1</p>
      </li>
      <li id='page2'>
         <p>Page 2</p>
      </li>
      <li id='page3'>
         <p>Page 3</p>
      </li>
   </ul>
</div>
```


Credits
------
Inspiration and idea based on Christian Laverton's panelslider.
Thanks to wtw software for opensourcing the plugin.