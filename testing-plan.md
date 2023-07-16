# Phase 5: Delivery Plan

## *Types of Testing*
### Manual Acceptance Testing: 
- User Interface/Navigation:
  -  Test Navigation flow in website to ensure that users can switch between different tabs 
  - Ensure and verify that all buttons and links are functional and accurate
  - Text, font, color, and headings are consistent and easy to read. 
- Game Functionality:
  - Ensure that the game allows users to drag and drop items in the recycling bin
  - Test items with different scenarios (waste, compost, recycle) to ensure that it will be sorted in the correct bin 
  - Ensure that the game provides proper feedback to correct and incorrect drops. 
  - Ensure that any items dropped outside of the bin will return back to its starting position.
- Information Sections:
  - Ensure that the statistics sections displays accurate information and data
  - Test readability of content: font sizes, color, and format
  - Should be clear and concise when it comes to explanations and recycling practices.
- Special Recycling Cases:
  - Test the accuracy of the information that is given for each item, which also includes the reasons as to why they can not be recycle
  - Make sure external resources such as phone numbers and links direct users to the correct source and is accurate
- Accessibility:
  - All images are screen reader friendly and have proper tags 
- multi-browser:
  - Test the application on different web browsers such as Chrome, Safari, and Firefox to ensure website renders and functions correctly


## *Testing Process*
### Who will test:
- Developers will test after each issue is completed
  - They will work to implement feedback on product design and fix any issues along the way
-  Product Designers test after each milestone
### When will we test:
- Developers will run tests on their computer after each issue has been completed, then they will merge the code with the main git branch
- Product designers will then rerun tests after each milestone is complete to ensure that all tests pass. Checking to make sure it is also supported on different browsers such as Chrome, Safari, and Firefox.

## *Test Environments*
- Browsers required for this testing: 
  - Google, Safari, Firefox
- Devices required for this testing:
  - Laptop/computer
- When code for each issue is completed, developers will perform code testing on their own computer before deploying.
- After hitting a milestone, all code should be deployed to production to allow for testing by the product designers.



## *Defect management*
1. If the tester finds a defect during testing at any time, they will document it right away by providing information and screenshots of the defect 
2. Tester will inform the project manager, so the issue can be prioritized to having it fixed.
3. After the defect is reported to the project manager, we will then discuss as a team to review the defect’s impact and priority. We will discuss the solutions to fix the error. 
4. When the defect is triaged, it will be assigned to a developer, so they can begin fixing the defect. Assignment will be distributed based on the development team members’ expertise and comfort level. 
5. When the bug is fixed, developers will check and ensure that there are no new errors.
6. The developer will then inform the tester and team to look at the issue again after it has been fixed.
7. The tester will look at the fixed defect to ensure that the issue has been resolved.

## *User acceptance testing script*
<h3 align="center">
  <strong>Test navbar feature:</strong>
</h3>

- Context: User opens happy recycling website and is on the homepage
- Action: User clicks on “Learn” item in navigation bar 
  - Expect: Website should change pages to the learn page and the learn item in the nav bar should be underlined (Requirement N1b & N1c)
- Action: User clicks on “Game” item in navigation bar
  - Expect: Website should change pages to the Game page and the Game item in the nav bar should be underlined (Requirement N1b & N1c)
- Action: User clicks on “Special cases” item in navigation bar
  - Expect: Website should change pages to the Special cases page and the Special cases item in the nav bar should be underlined (Requirement N1b & N1c)
- Action: User clicks on “Home” item in navigation bar
  - Expect: Website should change pages to the Home page and the Home item in the nav bar should be underlined (Requirement N1b & N1c)

<h3 align="center">
  <strong>Test Game feature Context 1:</strong>
</h3>

- Context: User opens a happy recycling website and is on the game page. The current draggable item is a “pizza box”
- Action: User drags “pizza box” to the recycle bin 
  - Expect: Overlays the “incorrect” header (Requirement G3c.1)
  - Expect: The draggable item/element (pizza box) returns back to its starting position (Requirement G3c.2)
  - Expect: The recycle bin will no longer accept any drops and “incorrect” header message will remain until the user clicks on the “new item” button (Requirement G3c.3)
- Action: User drags “pizza box” to the trash bin 
  - Expect: Overlay the “correct” header and displays description as to why the user is correct (Requirement G3b.1)
  - The current draggable item/element (pizza box) will stay until user has click “new item” button (Requirement G3b.2)
  - The brand mascot and “great job” message will appear and be displayed on screen  (Requirement G3b.3)
- Action: User drags “pizza box” to the compost bin 
  - Expect: Overlays the “incorrect” header (Requirement G3c.1)
  - Expect: The draggable item/element (pizza box) returns back to its starting position (Requirement G3c.2)
  - Expect: The compost bin will no longer accept any drops and “incorrect” header message will remain until the user clicks on the “new item” button (Requirement G3c.3)
- Action: User clicks on “New item” button
  - Expect: The draggable item changes to a “toothbrush”, which is the next active game item (Requirement G2b)

<h3 align="center">
  <strong>Test Game feature Context 2:</strong>
</h3> 

- Context: User opens a happy recycling website and is on the game page. The draggable item is a “pizza box”. User clicks on the “new item” button. The current draggable item is now a “toothbrush”
- Action: User drags “toothbrush” item to the recycle bin 
  - Expect: Overlay the “correct” header and displays description as to why the user is correct (Requirement G3b.1)
  - The current draggable item/element (toothbrush) will stay until user has click “new item” button (Requirement G3b.2)
  - The brand mascot and “great job” message will appear and be displayed on screen  (Requirement G3b.3)
- Action: User drags “toothbrush” item to the trash bin 
  - Expect: Overlays the “incorrect” header (Requirement G3c.1)
  - Expect: The draggable item/element (toothbrush) returns back to its starting position (Requirement G3c.2)
  - Expect: The trash bin will no longer accept any drops and “incorrect” header message will remain until the user clicks on the “new item” button (Requirement G3c.3)
- Action: User drags “toothbrush” item to the compost bin 
  - Expect: Overlays the “incorrect” header (Requirement G3c.1)
  - Expect: The draggable item/element (toothbrush) returns back to its starting position (Requirement G3c.2)
  - Expect: The compost bin will no longer accept any drops and “incorrect” header message will remain until the user clicks on the “new item” button (Requirement G3c.3)
- Action: User clicks on “New item” button
  - Expect: The draggable item card changes to a “Egg Shells”, which is the next active game item (Requirement G2b)


<h3 align="center">
  <strong>Test Game feature Context 3:</strong>
</h3>


- Context: User is on a new game item for the compost bin, such as egg shells just after clicking “new item”
- Action: User drags “Egg Shells” to the compost bin
  - Expect: Overlay the “correct” header and displays description as to why the user is correct (Requirement G3b.1)
  - The current draggable item/element (egg shells) will stay until user has click “new item” button (Requirement G3b.2)
  - The brand mascot and “great job” message will appear and be displayed on screen  (Requirement G3b.3)


<h3 align="center">
  <strong>Test links in footer:</strong>
</h3>

- Context: User opens happy recycling website and is on any of the pages
- Action: User clicks on “Contact Us” item at the bottom of the page 
  - Expect: Email client will open a new email composition window with the recipient email addresses pre-populated.  (Requirement F1b)


<h3 align="center">
  <strong>Test links and phone-numbers in Special Cases Page:</strong>
</h3>

- Context: User opens happy recycling website and is on the special cases page 
- Action: User clicks on “info@lightrecycle.org” 
  - Expect: Email client will open a new email composition window with the recipient email addresses pre-populated. (Requirement S2e)
- Action: User clicks on “1-800-RECYCLE” 
  - Expect: The user’s laptop will ask the user to confirm the action before starting the call. (Requirement S2e)

<h3 align="center">
  <strong>Test links and phone-numbers in Special Cases Page:</strong>Test button on home page</h3>
  
- Context: User opens happy recycling website and is on the home page
- Action: User clicks on “Learn more” button
  -Expect: User will be redirected to the Learn Page. (Require ent )

