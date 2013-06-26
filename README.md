Ignite-UI-2012-POC
==================

Proof of Concept using Ignite UI 2012
-------------------------------------


    git add . ; git commit -m " my comment " ; git push -u origin master
    

IgniteUI(TM) 2012 Volume 2 
========================== 

[http://www.infragistics.com/products/jquery/help](http://www.infragistics.com/products/jquery/help)

Getting Started with JavaScript and CSS
--------------------------------------- 

Copy the 'js' and 'css' folders to your website.	

jQuery, jQuery UI, and Modernizr are required to use igniteUI.

Modernizr needs to be of a custom build with css-boxsizing enabled

if targeting IE7: http://modernizr.com/download/

Once the 'js' and 'css' folders are copied, the following JavaScript and CSS references are recommended in this order:


    <link href="css/themes/infragistics/infragistics.theme.css" rel="stylesheet" type="text/css" />	
    <link href="css/structure/infragistics.css" rel="stylesheet" type="text/css" />
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.js" type="text/javascript"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.8.17/jquery-ui.js" type="text/javascript"></script>
    <script src="http://www.modernizr.com/downloads/modernizr-latest.js" type="text/javascript"></script>  
    <script src="js/infragistics.js" type="text/javascript"></script>



Alternatively Infragistics loader can be used to load only necessary resources.
If that is the choice that is made for your application, instead of placing Infragistics references from above,
only the following are required:


    <head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.js" type="text/javascript"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.8.17/jquery-ui.js" type="text/javascript"></script>
    <script src="http://www.modernizr.com/downloads/modernizr-latest.js" type="text/javascript"></script>
    <script src="js/infragistics.loader.js" type="text/javascript"></script>
    </head>



To request necessary resources, which include CSS and JavaScript files. The following code may be used:


    <script type="text/javascript">
		$.ig.loader({
			scriptPath: './js/',
			cssPath: './css/',
			resources: 'igGrid.Filtering.Sorting,igTree', // This example loads igGrid with Filtering and Sorting features, as well as igTree widgets.
			ready: function () {
				// Initialization code placed here
			}
		});
    </script>
    


**Note:** 
	For more information on using JavaScript and CSS with 
	IgniteUI, see: [http://help.infragistics.com/](http://help.infragistics.com/) 


Copyright 2011-2012 Infragistics, Inc. All rights reserved.