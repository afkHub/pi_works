# P.I. Works - Geolocation Product Design Engineer Questionnaire

**Question 5**

***Authors***     
Ahmet Fırat Karaoğlu : karaoglu@email.com 

## Abstract
Hello everyone!
<br/>This document is about the user interface specification for the user management screen.

## User Interface
You can see the user management screen view in Figure 1
<p align="center">
<img src="https://lists.office.com/Images/969df1bb-97b6-44ef-9108-dc18a5fd96c2/298428f6-6729-4501-a9de-dcaf554877fe/TDM2S9EALY3MZD42J8KL32SDKC/c2f1cb7e-5022-433a-93a2-1ac0b6ec1015"/>
<br/><em>Figure 1. User Management Screen</em>
</p>

## UI Specification
**User Page(/users)**
* Add "New User" panel at the top of the window. Just one row, side by side "+ New User" button on the far left side of the panel, the "Hide Disable User" checkbox and the "Save User" button on the far right of the panel.
  * When the "+ New User" button is pressed, the "New User" container appears on the right of the window mentioned below.
  * If the "Hide Disable User" box is checked, the hidden users will not be shown in the existing user information table on the left mentioned below.
  * If the entries in the "New User" container on the right are entered correctly on the "Save User" button, the new user is saved and appears in the table on the left. If all the entries in the "New User" container are filled, it becomes active for click.
    * If the inputs are missing or entered incorrectly, Alert is given in the window and it is requested to try again.

* Two tables side by side under the panel. To enter new user information container on the right, showing information table for existing users on the left. Both have the same aspect ratio (equal width and height proportional to the page size). If the data does not fit in the table containing the information of the users, the scrollbar feature becomes active.
  * The table containing the information of current users consists of 4 columns. The information in the 4 columns is "ID", "User Name", "Email", "Enabled". The information in these 4 columns should be bidirectional sortable. The "ID" information is given starting from 1 according to the time the user was added. The information in the other 3 columns is taken from the users.
  * Activated by the "+ New User" button, the "New User" container consists of a header and a form that includes 6 input lines. None of the inputs can be NULL.
    * It writes "New User" in the title.
    * There should be an input box next to the "Username" label on the 1st row. Only English characters, certain special characters and number of characters should be accepted as input.
    * There should be an input box next to the "Display Name" label on the 2nd row. It should be similar to line 1(Username).
    * There should be an input box next to the "Phone" label on the 3rd row. Only valid phone number should be entered. (input type="tel")
    * There should be an input box next to the "Email" label on the 4th row. Only valid email address should be entered. (input type="email")
    * There should be multiple attribute option next to the "User Roles" label on the 5th row. These should be "Guest", "Admin", "SuperAdmin". According to the selection, the feature information is assigned to the user.
    * There should be a checkbox next to the "Enabled" label on the 6th row. If checked, "enabled" is entered as information, if not, "not enabled" is entered.

<br/>
<br/>
<br/>

***Note**: Coloring and theme request can be made by giving color code etc. if expected.*
