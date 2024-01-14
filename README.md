
# WESTERN GOVERNOR UNIVERSITY 
## D287 – JAVA FRAMEWORKS


C.  Customize the HTML user interface for your customer’s application. The user interface should include the shop name, the product names, and the names of the parts.

File: mainscreen.html
Changes: 13 -> Added stylesheet, 15 -> changed title name, 20 -> added img logo, 31-32 -> changed button color, 69 -> changed button color

File: demo.css
Changes: 1-4 -> Sized img logo.png from container, 6-9 -> Changed font in container, 11-14 -> Changed table margin-bottom and border color, 15-21 -> Changed filter bar border size/style/color

Added logo.png to resources > static > css > logo.png



D.  Add an “About” page to the application to describe your chosen customer’s company to web viewers and include navigation to and from the “About” page and the main screen.

File Name: mainscreen.html
Change: 21 -> Added button to about page

File Name: about.html (created in templates folder)
Changes: 1-21 -> Added template code from mainscreen to match theme and included navigation to mainscreen, 23-32 -> added about section of webpage, 33 -> added happy-scooter.jpg

Change: Added happy-scooter.jpg to resources > static > css > happy-scooter.jpg

Change: Added @AboutController class to Controllers folder

File Name: demo.css 
Change: 31-50 -> added styles to about.html: positioning and color



E.  Add a sample inventory appropriate for your chosen store to the application. You should have five parts and five products in your sample inventory and should not overwrite existing data in the database.

File Name: BootStrapData.java
Changes: 48-99 -> added code for 5 outsourced parts using setters to define them and then saved them to the repo, 106-118 -> added code to create my products and saved them to the product repo, 48 and 107 -> added specifically to only add products or parts when the lists are empty,  120-133 -> created a multi-pack part that searches for duplicates in the outsourced part repo, 134-147 -> created a multi-pack product and a list that finds all products so the products can be iterated through and duplicates can be searched for from the product repo. 



F.  Add a “Buy Now” button to your product list. Your “Buy Now” button must meet each of the following parameters:

File Name: mainscreen.html 
Change: created a "Buy Now" button that links to buyNow() controller with an input of product ID to identify the product inventory to decrement.

File Name: created BuyNowController.java
Changes: 13-30 -> created a controller and getmapping for a buyNow button to decrement inventory by 1 and redirect as a success or failure. 

Files Names: created buynowsuccess.html and buynowfailure.html
Changes: 1-12 -> display a message of success or failure based on the respective redirect from the buyNow() controller.



G.  Modify the parts to track maximum and minimum inventory by doing the following:
•  Add additional fields to the part entity for maximum and minimum inventory.
•  Modify the sample inventory to include the maximum and minimum fields.
•  Add to the InhousePartForm and OutsourcedPartForm forms additional text inputs for the inventory so the user can set the maximum and minimum values.
•  Rename the file the persistent storage is saved to.
•  Modify the code to enforce that the inventory is between or at the minimum and maximum value.

File Name:
Line Number:
Change:




H.  Add validation for between or at the maximum and minimum fields. The validation must include the following:
•  Display error messages for low inventory when adding and updating parts if the inventory is less than the minimum number of parts.
•  Display error messages for low inventory when adding and updating products lowers the part inventory below the minimum.
•  Display error messages when adding and updating parts if the inventory is greater than the maximum.

File Name:
Line Number:
Change:




I.  Add at least two unit tests for the maximum and minimum fields to the PartTest class in the test package.

File Name:
Line Number:
Change:



J.  Remove the class files for any unused validators in order to clean your code.

File Name:
Line Number:
Change:

