! IMPORTANT NOTICE: json does not allow commenting in files!
! This is why I'm doing the commenting in this README

[Example Theme](2016-04-07-162132_1366x768_scrot.png)

```
{
	//specify version
	"version":"1.0",
	/* specify the template format from chrome you are using.
	 * pretty sure it does not work with other versions */
	"manifest_version":2,
	// Name the theme if you'd wish"
	"name":"My Theme",
	// start the actual theme
	"theme":{
		// images section
		"images":{
			/* this sets the main frame where the close button
			 * usually is */
			"theme_frame":"dark-square-design-wide-i.png",
			// where the forward back and refresh buttons are
			"theme_toolbar":"dark-square-design-wide-i.png",
			// inactive tabs
			"theme_tab_background":"dark-square-design-wide-i.png",
			// sets new tab background
			"theme_ntp_background":"some_image.png",
			// if you have a graphical signature, you can add it
			"theme_ntp_attribution":"some_other_image.png"
		},

		"colors":{
			/* the color values range from 0 to 255 the
			 * names are also pretty self explanatory */
			"ntp_link":[130,174,164],
			"ntp_text":[221,221,221],
			"ntp_section_link":[221,221,221],
			"ntp_section_text":[0,104,111],
			"ntp_background":[0,12,21],
			"frame":[0,104,111],
			"toolbar":[0,104,111],
			"tab_text":[221,221,221],
			"tab_background_text":[0,104,111],
			"bookmark_text":[221,221,221]
		},
		"tints":{
			/* this is for the back, forward and refresh buttons
			 * the values range from zero to one. */
			"buttons":[0.33,0.5,0.47]
		}

		"properties":{
			"ntp_background_alignment":"bottom",
			"ntp_background_repeat":"no-repeat"
		}
	}
}
```

To load this theme into your browser:
* Go to chrome://extensions/,
* Check the developer mode button on the top right,
* Click Load unpacked extenstion...
* load the directory with your .json file
