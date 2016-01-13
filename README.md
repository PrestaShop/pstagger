# jQuery Prestagify Plugin

A simple jQuery plugin in order to create tags input bars, this is still a beta so play around with it but we do not recommend to use it in production at the moment.

Do not hesitate to make PR for improvement or bug fixes !

[Get it from Github](https://github.com/PrestaShop/Prestagify)

Lastest version: 0.1.0 (beta)


## Instructions

Add mandatory files

	<script src="jquery.prestagify.js"></script>
	<link rel="stylesheet" type="text/css" href="jquery.prestagify.css" />

Once that done, create an input like you would do in any other case:

	<input id="input-tags" />

Then, simply call the tagsInput function on any field that should be treated as
a list of tags.
Then, make a call to Prestagify plugin on all desired input to be 'Prestagified'

	$('#input-tags').Prestagify();

## Options

	$(selector).Prestagify({
		/* CSS custom */
        wrapperClassAdditional: 'myClass',
        tagsWrapperClassAdditional: 'myClass',
        tagClassAdditional: 'myClass',
        closingCrossClassAdditionnal: 'myClass',
        clearAllIconClassAdditional: 'myClass',
        clearAllSpanClassAdditional: 'myClass',
        tagInputWrapperClassAdditional: 'myClass',
        tagInputClassAdditional: 'myClass',
        /* Global configuration */
        delimiter: ' ',
        inputPlaceholder: 'Add tag ...',
        closingCross: true,
        context: null,
        clearAllBtn: false,
        /* Callbacks */
        onTagsChanged: null,
        onResetTags: null,
	});

## API

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Default</th>
      <th>Note</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td> wrapperClassAdditional </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>
      </td>
    </tr>

    <tr>
      <td> tagsWrapperClassAdditional </td>
     <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>    </tr>

    <tr>
      <td> tagClassAdditional </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>
    </tr>

    <tr>
      <td> closingCrossClassAdditionnal </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>
    </tr>

    <tr>
      <td> tagInputWrapperClassAdditional </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>
    </tr>

    <tr>
      <td>tagInputClassAdditional </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>
    </tr>

    <tr>
      <td>clearAllIconClassAdditional </td>
      <td>String</td>
      <td>''</td>
      <td>Add custom CSS to the plugin</a>    
    </tr>

    <tr>
      <td>delimiter </td>
      <td>String</td>
      <td>' '</td>
      <td>Determine on which character the plugin has to explode the full string</td>
    </tr>

    <tr>
      <td>inputPlaceholder</td>
      <td>String</td>
      <td>'Add a tag ...'</td>
      <td>Simply replace input placeholder by the one you choose</td>
    </tr>

    <tr>
      <td>closingCross</td>
      <td>Boolean</td>
      <td>true</td>
      <td>Whether we have to display a "closing cross" on each tag generated in order to remove them</td>
    </tr>

    <tr>
      <td>context</td>
      <td>Object</td>
      <td>null</td>
      <td>You may want to specify a specific context on your callback, just give that context here (e.g: this)</td>
    </tr>

    <tr>
      <td> clearAllBtn </td>
      <td>Boolean</td>
      <td>false</td>
      <td>Determine if the global reset input button has to be displayed
      </td>
    </tr>

    <tr>
      <td>onTagsChanged</td>
      <td>Callback</td>
      <td>none</td>
      <td>Callback called everytime input tag has changed, it will receive an array representing each tag available in the input
      </td>
    </tr>

    <tr>
      <td> onResetTags </td>
      <td>Callback</td>
      <td>none</td>
      <td>Callback called whenever the reset button is clicked and input emptied
      </td>
    </tr>

  </tbody>
</table>
