# Gooey QA Process (Emails)

This document has been produced for all QA testers working at Gooey, and explains what is expected in regards to QA of email builds.

---
## Table of contents
- [Design](#design)
- [Testing](#testing)
- [Standards](#standards)
---

## Design

It is of fundamental importance that the build looks identical to the designs supplied:

- Check each design against the built page looking for any errors or inconsistencies.
- If there is mobile or tablet designs also check these against the build.
- The build should look identical to the designs unless otherwise agreed.

---

## Testing

All emails should be tested using Litmus and a link should be provided by the developer:

- Scroll through each screenshot making sure all is well.
- Check to ensure the developer has not turned any clients off, specifically Outlook 2007, 2010, 2013 and 2013 120dpi.
- If there is any amends to the email, or Litmus issues, ask the developer to resend a revised test link when they have fixed, and repeat process.

---

## Standards

All code released by Gooey should be to a high standard, and semantic:

- Open the email in Dreamweaver and check that it displays correctly on 'Visual View'. This is a good/quick way to see if their is any unclosed tags or errors (multiple classes on a td etc).
- If the email doesn't display there is a code error.
- If the email has tags highlighted in yellow there is an error.
- Check all images have alt tags and the alt tag descriptions are correct.
- If the email uses custom fonts including in the build files, check that the font/s are not available on Google Fonts.
- Check that the email uses the Gooey template:

```
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml"
 xmlns:v="urn:schemas-microsoft-com:vml"
 xmlns:o="urn:schemas-microsoft-com:office:office">
    <head>
        <title>Title</title>
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <style type="text/css">
		#outlook a{padding:0;}
		body{width:100% !important;-webkit-text-size-adjust:none;margin:0; padding:0; background-color:#ffffff}
		.ReadMsgBody{width:100%;}
		.ExternalClass{width:100%;}
		img{border:0; height:auto; line-height:100%; outline:none; text-decoration:none;}
		table, table td {border-collapse:collapse;}
		.ExternalClass * {line-height: 100%}
		@media only screen and (max-width: 479px) {

			.body {min-width:0 !important}
			.wrapper {width:320px !important}
			.panel {width:100% !important; min-width:0px !important}
			.panel-padded {width:95% !important; padding:0 2.5%; min-width:0px !important}
			.image {height:auto !important; max-width:100% !important}
			.hide {display:none!important}

		}

		@media screen {

			* {} /* custom font */

		}
	</style>
        <!--[if gte mso 9]><xml>
         <o:OfficeDocumentSettings>
          <o:AllowPNG/>
          <o:PixelsPerInch>96</o:PixelsPerInch>
         </o:OfficeDocumentSettings>
        </xml><![endif]-->
    </head>
    <body>
    
    	<table class="body" width="100%" style="min-width:600px" bgcolor="#ffffff">
	    <tr>
	        <td class="body" align="center" valign="top" style="min-width:600px">			
                    <table width="100%" align="center" style="min-width:600px" border="0" cellpadding="0" cellspacing="0" class="body">
                        <tr>
                            <td align="center">
                                <table align="center" width="600" border="0" cellpadding="0" cellspacing="0" class="wrapper" bgcolor="#ffffff">

                                    <!-- starts  -->
                                    
                                    <tr>
                                    	<td valign="top">
                                            <table width="100%" border="0" cellpadding="0" cellspacing="0" align="center" style="width:600px" class="panel">
                                                <tr>
                                                    <td valign="top" align="center">
                                                    <img src="image-example.jpg" alt="Alt text" width="308" height="61" style="display:block; max-width:308px; max-height:61px" border="0" />
                                                    </td>
                                                </tr>
                                                <tr>
                                                    <td valign="top" align="center" style="font-family: Georgia, 'Times New Roman', Times, serif; mso-line-height-rule: exactly; font-size:24px; color:#5e3170; text-align:center; line-height:28px">
                                                    This is test
                                                    </td>
                                                </tr>
                                            </table>
                                        </td>
                                    </tr>

                                    <!-- ends -->

                                </table>
                            </td>
                        </tr>
                    </table>
                </td>
            </tr>
        </table>

    </body>
</html>
```

---

-- Produced by James Holloway - Gooey (Last updated 25/01/2018)
