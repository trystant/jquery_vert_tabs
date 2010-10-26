JQuery Vert Tabs
=================

This is a copy of the jquery-vert-tabs plugin, a [jQuery](http://jquery.com) plugin for impementing vertical tab navigation on a web site. This is based on the [jquery-vert-tabs](http://code.google.com/p/jquery-vert-tabs/) plugin by Seth Lenzi, with some additional logging for debugging purposes as well as a change that sets the method for making AJAX requests to GET from POST.

Installing jQuery Vert Tabs                                                                                
===========================
Currently, "Installing" the plugin involves copying over the JavaScript and CSS file from the jQuery Vertical Tabs repository to the #{RAILS_ROOT}/public/javascripts and #{RAILS_ROOT}/public/stylesheets directories.
TODO: Create Rake task to "automatically" install the plugin in a Rails project.

Major modifications to plugin
=============================

A few changes have been made to the jquery-vert-tabs plugin in order to work with this project. They are as follows:

* A new option, "ajaxHttpMethod" that allows you to set the HTTP method of the AJAX request. Defaults to POST if no method is selected.

* The criteria for selecting the 'open' tab has been changed. It initially was the first tab, but for this engagement, the last tab needed to be open. The logic was specific to the project TODO: change the criteria for making an open tab configurable, if possible. This is on line 123 of jquery-jvery-tabs.js
                                                                                                                                                                                            
* A lot of 'console.log' statements have been added to the code for debugging purposes. TODO: Remove the console.log statements and possibly implement JavaScript Debug http://benalman.com/code/projects/javascript-debug/
 

