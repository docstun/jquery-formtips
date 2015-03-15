# jquery-formtips

## What?

jQuery Formtips is a plugin for the popular javascript library jQuery. It enables a form to draw default values or messages into input/textarea elements. The text is fetched from the title-attribute of the element.

## How can I use this plugin?

Of course, at first you need a current version of the jQuery library. Go to the jQuery website and get yourself a copy.

Next, insert the form tips plugin as shown below:

    <script type="text/javascript" src="jquery.formtips.js"></script>

Now, attach the plugin code to some elements. In our example below we did the following:

    $(document).ready(function() {
      $('form input.help, form textarea.help').formtips({
        tippedClass: 'tipped'
      });
    });

Finally, give your css-class a certain style (mabye lighten it up a little) to show the user that the "tipped" version provides some help-text. Put the default text into the title-attribute of the elements you selected to be tipped.
