# Problem statement
Students in dormitories need an efficient system for finding handed-out or sharable items like kitchenware, especially during move-in periods, as they often struggle to find available objects, leading to unnecessary purchases.

## Tasks
### Task 1: Find a specific item by filtering
Users can locate a specific item they are looking for by filtering through predefined categories, which gives them a narrowed-down list of items donated.

### Task 2: Creating a sharing quest
Users can create sharing quests for borrowing items they temporarily need but do not possess. They can do this by specifying the item, category, duration, and dates they need an object for, and providing any additional specifications for the requested object.

### Task 3: Answering a sharing quest
Users need to chat with the requester to answer a sharing quest. They can do this by chatting, confirming the agreement and the restitution of the item, leading to the receipt of coins.

## Prototype
### Summary description:
This tool is designed to help students in dormitories efficiently find and share items like kitchenware, particularly during move-in periods when they often struggle to locate available objects. By allowing users to filter through predefined categories to search for donated items, create sharing quests for temporary borrowing, and communicate directly with item owners, the platform simplifies the process of accessing shared resources. The design choices prioritize user convenience and clarity, enabling quick navigation through the items, direct access to open sharing quests, and effective communication between users. This system ultimately reduces the need for unnecessary purchases, creating a culture of sharing and sustainability among students.
**Link to prototype**: https://www.figma.com/proto/Ldg5qkJFMMYuog0y7KFGx4/DROP---App?node-id=40-65&node-type=frame&t=AeoIQS6ZiKrEtYyN-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=40%3A65

### Task 1 Design choices:
To find a specific item the user can either search by entering the item name or filter results using predefined categories. These categories were selected based on the most commonly available items on the platform. If the user wants to set a specific number of coins based on how many the user has, they can set a maximum number of coins they are willing to spend (not implemented for this prototype). The amount of coin the user possesses is always shown on the upper bar, which helps the user be aware of it all the time. The donated item profile contains the donor information, its coin value, the category and a description, which may include additional details provided by the item’s donor. This design ensures that users can easily locate items through intuitive filter features and having only necessary information in item posts make the communication more effective. 

#### Task 1 Instruction:
- Press the filtering button near the search bar to open filter section
- Press the “Uncheck all” text to unclick all categories
- Click only the “Kitchenware” box
- Press the “Filter Items” button to filter the items
- Identify the “Spoon” post and open it by clicking on it
- Scroll the item post to read the description

#### Task 1 Screenshots:
![Filter Section](images/Task1.1.png)
![Donated Item post](images/Task1.2.png)

### Task 2 Design Choices:
We keep the button for adding quests or making donation posts as floating buttons on the right-hand side rather than in-menu buttons on the navigation bar. This helps reduce clutter on the navigation bar, especially when the add button separates into buttons for adding donation items and sharing requests. Furthermore, its prominent position makes it easily viewable and quickly accessible to the user. The create request page uses a form format that is intuitive to users. Most of the elements including category, date, and time are provided through lists or other visual elements like a pop-up calendar or scrollable time selection to reduce errors through keyboard input and speed up the process of input. Additionally, we also provide placeholder texts for all input elements so users can receive instructions on what to input or what format of answer we are expecting.

#### Task 2 Instructions:
- Press the ‘+’ floating button
- Press the button with the icon for ‘share’ to start the creation process
- Add the item name in the ‘Item Name’ textbox
- Select the appropriate category from the ‘Category’ drop-down list.
- Select the date from the calendar in the ‘From’ section to choose the start date of the borrow
- Scroll to find the from time from the list in the ‘From’ section to choose the start time of the borrow
- Select the date from the calendar in the ‘Until’ section to choose the end date of the borrow
- Scroll to find the from time from the list in the ‘Until’ section to choose the end time of the borrow
- Add any specifications for the item in the ‘Description’ box.
- Click the ‘Post’ button to complete the creation of the sharing quest
- The user can now view the updated post on the sharing quest list

#### Task 2 Screenshots:
![Floating buttons to add posts or quests](images/Task2.1.png)
![New sharing quest page](images/Task2.2.png)
![Calender to input date](images/Task2.3.png)
![List to add time](images/Task2.4.png)

### Task 3 Design choices: 
The “Chat” button is positioned on the item page, requiring users to communicate before confirming, which allows them to arrange pick-up details, ask questions, and avoid mismatches with requested items.
As for the “Confirm” button, pressing it removes the request from the list of open quests, ensuring communication before finalizing the agreement and improving the management of the sharing list. After confirmation, the button disappears on the borrower’s side and is replaced by the “Returned” button on the owner’s side to highlight the new state of the agreement. The “Returned” button ensures that all lent items are properly tracked and returned. Once it has been pressed, it changes color to be more evident to the user.
The rating system within the pop-up requires users to rate their experience, ensuring that negative behaviors are recorded for future sharing interactions. 
Chat histories are organized by product, with filters for interaction types such as donation or sharing, allowing users to easily revisit conversations.
A feature that has not been implemented is the notification system. It is planned to ensure prompt responses, with users selecting categories of items they own at sign-up. Only users who select the relevant category will be notified when a matching sharing request is posted. The usability of this feature needs to be validated through a user study, which is why it has not been implemented yet.

#### Task 3 instructions: 
- Press the “Share” button on the bottom bar to view the list of open sharing quests.
- Press the “Cooking pot” sharing quest.
- Press the “Chat” button to chat with the borrower.
- Press the “Message…” bar to type the message.
- Press the keyboard to type your message.
- Press anywhere on the phone screen to see the borrower's response.
- Press the “Message…” bar to type the message.
- Press the keyboard to type your message.
- Press the “Confirm” button to agree on the sharing exchange.
- Press the “Returned” button to indicate that the item has been returned.
- Press the stars in the pop-up to rate the experience with this borrower.
- Press the “X” button in the pop-up to close it.
- Press the “Go back” arrow on the top bar to return to the chat history.

#### Task 3 screenshots:
![Item page with description and “Chat” button ](images/Task3.1.jpg)
![Chat with “Confirm” button](images/Task3.2.jpg)
![Chat with “Returned” button and rating pop-up](images/Task3.3.jpg)
