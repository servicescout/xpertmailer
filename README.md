# xpertmailer
Minimally modified fork of xpertmailer to support loading via composer.

# Download

Since we are not currently registered with packageist, need to provide the repo info:

Composer:

	"repositories": [
		{
			"type": "vcs",
			"url": "https://github.com/servicescout/xpertmailer"
		}
	],

	"require": {
		"servicescout/xpertmailer": "dev-master",
	},

# Changes from original

Constants for controlling error logging were converted to public static variables
on the `ServiceScout\XPertMailer\FUNC5`:

	FUNC5::$display_xpm4_errors
	FUNC5::$log_xpm4_errors

Usage is the same as the corresponding constants as originally documented:
http://www.xpertmailer.com/documentation/

except `$log_xpm4_errors` is just an array, instead of a serialized array, and 
display is turned off by default.
