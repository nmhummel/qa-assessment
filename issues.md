I marked by the title which of the issues I fixed with  "********"

ALL FOUND ISSUES, LISTED BY SEVERITY:

# Title: Double Click to Edit Not Working
## Severity: High
## Description:
After adding tasks to list, the ability to double click on item is currently not working.
## Proposed Solution:
Double clicking should treat the text as a form field, allowing user to write in area. Might be an issue with an eventListener.
==================================

# Title: Status Buttons at Bottom Not Working   ***FIXED***
## Severity: Medium
## Description:
'Active' and 'Completed' buttons not working. Unsure if 'All' works; cannot differentiate while other buttons not working.
=> Add 2-3 tasks and push buttons to see error.
## Proposed Solution:
'Active' should only show unchecked items. 'Completed' should only show checked items. 'Completed' should show checked and unchecked items. 
### NOTE: I added a switch case on the app.jsx file to function on line 91. 
1. To test, add 2-3 tasks to list. Ensure that all tasks are shown by default. 
2. Mark one task as complete.
3. Toggle between All, Active, and Completed to ensure correct tasks show up by their status.
==================================

# Title: Clear Completed Not Working
## Severity: Medium
## Description:
User should be able to clear finished tasks when this is clicked.
## Proposed Solution:
When clicked, all items with green checks should be removed from list. There is probably an issue with a clearing function.
==================================

# Title: Status Buttons not hidden
## Severity: Low
## Description:
Bottom row containing buttons should be hidden upon loading. Currently showing.
## Proposed Solution:
Row should only appear once a task has been added to list.
==================================

# Title: Select All Behavior (not sure if this is problem)
## Severity: Low
## Description:
After adding 2-3 tasks to list, the downward arrow in top-left of box currently switched status to opposite. If checked, it becomes unchecked. If unchecked, it becomes checked.
## Proposed Solution:
Not sure what intended behavior is, but usually a select all shouldn't affect items currently selected. Need to make sure the function only selects items that are unchecked.
==================================

# Title: Button Borders Wrong Color     ***FIXED***
## Severity: Low
## Description:
Borders around buttons are wrong color.
## Proposed Solution:
The color should be same brick red as title. 
==================================

# Title: Background Color of List Wrong    ***FIXED***
## Severity: Low
## Description:
Currently, the list is a whiteish color, including the edges of stacked lists that appear to be under top page.
## Proposed Solution:
List background color should be notepad yellow, rgb(254,243,199). 
==================================

# Title: Ruled Lines Wrong Color    ***FIXED***
## Severity: Low
## Description:
Currently, the ruled lines (in between list items) is gray.
## Proposed Solution:
Lines should be blueish color, rgb(175,206,191). Change border color in CSS file for the individual <li>'s 
==================================

# Title: Title "todos" too thick    ***tried to fix; couldn't get it thin enough***
## Severity: Low
## Description:
The title appears to be bold.
## Proposed Solution:
The title shouldn't be bold. Check for <b> tag or font weight in CSS file. 
==================================

# Title: Delete Task 'X' is wrong color     ***tried to fix; couldn't get X thin enough***
## Severity: Low
## Description:
Hovering mouse over a task reveals that the deletion 'X' is currently red that changes shades with hovering.
## Proposed Solution:
The X should be 100% transparent, inside a round gray circle with about 25% transparency.
==================================

# Title: 'All' Button not highlighted as default
## Severity: Low
## Description:
Upon entering first task, the 'All' button is not higlighted as default.
## Proposed Solution:
The 'All' button should be bordered  to show that current view is all tasks. Might be a border issue in the CSS file.
==================================

# Title: Task Selector Circle Incorrect Color
## Severity: Low
## Description:
The circle that you click to select task should be same brick red color as title.
## Proposed Solution:
Check the CSS file for <li> and change the color of circle to the brick red of "todos" title.
==================================