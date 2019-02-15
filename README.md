# Description
  @description Customize SharePoint 2013/2016/O365 classic forms
  @type jQuery
  @name HillbillyTemplate
  @category Plugins/HillbillyTemplate
  @author Mark Rackley / http://www.markrackley.net / mrackley@paitgroup.com, editer by Jeff ANGAMA https://twitter/jeffangama

 #OBjective 
* Customize new form / edit / view form easily. Add bootstrap, jquery to it.
* When using that project vs jslink ? When you want to set field value or customize a form to be prettier

 # Installation 
 1. git clone https://github.com/seaSide974/gulpsynchLocalToRemote to get a gulp task that push html css js to style library. Configure it. Create a folder in src : style library and a subfolder "yourappname". 
 2. git clone this project, rename myapp to your app name. **
 3. Copy paste myapp folder renamed, to your project (created in step 1)
 3. Set a content editor in new form / edit form / view form of your list, set the link to the html 
 4. Replace the value "myapp" in HillBillyTemplate.html" to your app name, should be the same as your folder name in style library

 # Usage: 
    
    There is an example configured in 
     jQuery(document).ready(function($) {
   
         $().HillbillyTemplate({
             genericAlert: false, // true/false - show a generic error alert if SharePoint Form error happens on submission
             moveSaveCancel: false, // true/false - Are you also moving the save and cancel butttons?
             alertErrorText: "<message>" // - What message do you want to display to the users if there is a SharePoint form error on submit
         });
 		
    }); 
 
 # Additional Documentation for version 2:
   
    Template span for save button
    <span class="hillbillyFormSave"></span>
  
    Template span for cancel button
    <span class="hillbillyFormCancel"></span>
 
  
 /

 #V3 By Jeff ANGAMA
* Scroll to errors area. remove popup alert
* Use internalName instead of displayName for the html template
* Grab the field description, avoiding typing in the template the fields names
* Support redeployment and javascript every day, user will not have to do CTRL + F5. thank to rev=date..
* Separate html from JS
* JQUERY / Bootstrap / multiple JS FIle
