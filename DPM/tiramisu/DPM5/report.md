# Split-n’-share
## CS473 Introduction to Social Computing - 2024 Fall  
**Project 5: Showcase and Final Report**  
Nghiem Xuan Son  
Thuy Trang Nguyen  
Mai Nguyen  

---

### Representative Screenshots

1. Browse Products Page

The Browse Products Page is the first screen users see after logging in. This page serves as the starting point for discovering group-buying opportunities. Users can:

- Search for Products using the search bar for quick navigation.
- Filter by Categories to narrow results based on product type or pick-up location (e.g., KAIST dormitories).

![[./images/UI-1.png]]
![[./images/UI-2.png]]

2. Creating a Joint-Purchase Posting

The Create Posting feature enables users to initiate group-buying opportunities. Users fill out key details such as:

- Title & Image: Add a descriptive title and optional image for better visibility.
- End Date & Category: Specify the duration of the offer and select an appropriate category.
- Pickup Location & Price: Choose a pick-up location from a dropdown list and share the total cost, which will be divided among participants.
- Product Description: Include essential details about the product and any special instructions.

![[./images/UI-3.png]]

#### Product Detail Page


​​The Product Detail Page presents all the information entered during the posting process. Depending on the user’s role:


- If the User is the Host:
  - Access the Open Group Chat feature to manage co-buyers and facilitate communication.
- If the User is Not the Host:
  - Use Chat with Host to initiate direct communication before joining.
  - Click Request to Join to send a participation request to the host and wait for their approval. 
  - Once a request is sent, the Request to Join button changes to Cancel Request, allowing co-buyers to withdraw their request if they decide not to join.

![[./images/UI-4.png]]
![[./images/UI-5.png]]
![[./images/UI-6.png]]

4. Posting Management Page

The My Postings Page is where the host can manage their postings and oversee group-buying activity. Key features include:
- Post Information: View details such as the date a post was created, product information, price, and category.
- Pending Co-buyers & Approved Co-buyers:
  - Pending requests from co-buyers are queued here. The host is notified whenever a new request is received.
  - Hosts can approve or decline requests, and approved co-buyers are automatically added to the Approved Co-buyers list.
- Actions:
  - Delete Posting: Remove a posting from the platform.
  - Open Group Chat: Start a group chat with approved co-buyers to facilitate communication for the deal.


![[./images/UI-7.png]]

#### User Page


The User Page showcases a user’s profile and activity, including:


- Public Information: View reviews given to and received from other users.
- Review Functionality: Post reviews for hosts after completing a deal, offering text feedback and star ratings.
- Post History: Explore the user’s current and past postings for credibility.


![[./images/UI-8.png]]
![[./images/UI-9.png]]

#### Settings Page

The Settings Page allows users to update their personal information, such as a brief description, dormitory, department, phone number, and profile picture. Users can make changes and save them by clicking the Update Settings button. This page ensures profiles stay up-to-date and personalized.



![[./images/UI-10.png]]


---

### Quality Arguments

Split-n'-Share simplifies group purchasing for KAIST students by offering an intuitive platform to share bulk purchases, access discounts, and foster collaboration within a trusted community. The interface is designed to be efficient, user-friendly, and socially engaging.


Our feature set supports creating, joining, and managing joint purchases with tools tailored to user needs. The **filtering system** includes two key criteria: category and pick-up location. Filtering by pick-up location minimizes walking distance for users, while the **search bar** allows users to quickly find relevant posts by scanning for keywords across all postings.


The **Chat with Host** option, accessible directly from a post, enables seamless communication for users seeking more information before joining a deal. Our standout feature is the **request-approve-join group chat** system. Interested users can request to join a deal, which the host can approve or reject. Upon approval, a dedicated group chat is automatically created for the host and co-buyers. This real-time chat streamlines discussions about payment, pick-up arrangements, and updates, ensuring transparency and accuracy.


To enhance trust and safety, Split-n'-Share includes a **review system**. After completing a purchase, users can leave reviews on the host’s profile, helping others assess credibility and fostering a secure community environment.


The visual design adheres to the standards of e-commerce platforms, making it highly intuitive, even for first-time users. Features like dropdown menus, clear icons, and logical workflows ensure a smooth experience across all functionalities.


By combining these features, Split-n'-Share delivers a robust, well-designed platform that meets KAIST students’ specific needs for group purchasing while encouraging social interactions and trust within the community.

---

### Deployment Summary

The deployment of Split-n'-Share was conducted on the Render platform with MongoDB Atlas as the database. Ten KAIST students participated in the user testing, split between pre-presentation (5 users) and after presentation day (5 users)


Due to the limitation with the database server, our website was not able to handle a large amount of posting, hence we had no choice but to delete some users’ posting and left behind only 8 postings. 

#### Testing Procedure

1. **Organic Testing:** Users freely explored the platform for 5 minutes without guidance.
2. **Structured Evaluations:** Users performed tasks including creating accounts, postings, browsing the product feed, using filters, exploring deals, chatting with the host, requesting to join a deal, and leaving reviews. Help was provided only when necessary.

#### Results

After the user testing procedure, the users were asked to fill in the user experience evaluation form (https://forms.gle/LAJ6rSkwRVrPHmzF8). 


The results of the survey are as follows:

![[./images/UT1.png]]
![[./images/UT2.png]]
![[./images/UT3.png]]
![[./images/UT4.png]]
![[./images/UT5.png]]
![[./images/UT6.png]]
![[./images/UT7.png]]
![[./images/UT8.png]]
![[./images/UT9.png]]

To summarize, user feedback for Split-n'-Share was overwhelmingly positive, with 90% of users rating ease of navigation, overall satisfaction, visual design, and usability as 4 or 5. The Pick-up Location Filter and Request to Join features were most valued, while the Request-Approve Group Chat System was deemed intuitive by 90% of respondents. The Review System significantly influenced trust, with 90% rating its impact as high.


Additionally, users suggested improving the app's loading speed when browsing the feed or opening chats with the host. They also recommended features like tailored product suggestions based on user interests and enhanced chat functionalities, such as message pinning or multimedia support. We will take into consideration these feedback for better improvement later on.

---

### Discussion

Split-n’-Share addresses key aspects such as incentives, quality control, communication, and moderation. The financial savings offered by collaborative bulk purchases are a primary driver for user participation. By splitting costs among multiple participants, users save money on items that would otherwise require significant upfront investment or result in surplus burdens. Beyond monetary benefits, the app fosters **community trust**, an intangible reward. The exclusivity of the platform for KAIST students creates a shared sense of belonging, encouraging participation and collaboration. This dual incentive structure—**tangible (financial savings)** and **intangible (community trust)**—motivates users to engage actively in group-buying opportunities.


The app prioritizes **trust-building** within a verified community. To register, users must use their KAIST email, which is verified through an email-based system. This exclusivity reduces the risk of fraudulent accounts or malicious users. The **transparent review system** further enhances trust, allowing both hosts and co-buyers to evaluate participants based on past reviews and performance. This system promotes **accountability** and encourages **reliable user behavior**—key components of quality control.


The concept of **social translucence** is integrated into the app’s design, providing users with the visibility needed to make informed decisions. For instance, participants can view details about current co-purchase members, the number of participants, and detailed deal information before deciding to join. To combat **dissociative anonymity**, the app makes certain user information (e.g., name, major, residence location) publicly visible on profiles. This approach avoids hiding real identities, fostering accountability and reducing the likelihood of irresponsible or antisocial behavior.


The app employs a **community-focused moderation system** rather than relying on centralized oversight. Key features include: (1) A **review system** that provides transparency into user reliability. (2) **Host control**, which grants hosts the authority to accept or reject participants based on profile reviews and past activities. (3) Public profiles displaying user reviews and past participation records. Implicit **norms** govern user behavior within the app. Users are expected to take responsibility for managing logistics—such as shipping, payment, and delivery—within their groups once formed. These norms encourage independence and self-management, reducing the platform’s operational burden.


Another layer of **quality control** is provided through host permissions. Potential buyers cannot automatically join a deal; they must send a request, which the host can approve or reject. This allows hosts to screen participants based on profile reviews or past behavior, maintaining high group standards. Such control minimizes issues like non-payment or miscommunication and protects the host’s privacy.


The app supports **real-time synchronous communication** through group chats and host-participant messaging. These tools establish **common ground** among users, enabling them to clarify misunderstandings, share information, and coordinate logistics effectively. This functionality enhances collaboration and strengthens social ties, addressing a core aspect of social computing—supporting social interaction.


Despite its strengths, the app has limitations. The absence of a **centralized moderation team** or automated oversight system means platform-wide behavior or content isn’t actively managed. This reliance on community-driven mechanisms could pose scalability risks as the platform grows beyond its current user base. 




---

### Individual Reflections

#### Thuy Trang Nguyen

I worked on the backend of Split-n'-Share, where I focused on designing and structuring database schemas in MongoDB to represent core elements like products, group purchases, and user profiles. Alongside that, I created RESTful API endpoints to handle essential features like adding and managing products, creating and updating group purchase deals, retrieving user data, and managing participant lists.


One of the biggest challenges was integrating the backend with the frontend. This required a lot of testing and debugging to ensure the APIs worked smoothly with the frontend. A recurring issue was mismatched data formats between what the frontend needed and what the backend provided, which sometimes caused problems in the interface. I had to refine the API responses and work closely with the frontend team to align everything, making sure the user experience was seamless in the end.
On the teamwork side, one advantage was that we already knew each other, so scheduling and communicating were relatively easy. However, we struggled with having structured discussions, which sometimes led to confusion about tasks and progress. Going forward, I’ve learned how important regular and organized team check-ins are to keep everyone on the same page.


This was my first time working on a website, so I learned a lot. I now know how to design efficient database schemas, build and test APIs, and handle data consistency when multiple users interact with the platform. I also got better at debugging issues between the backend and frontend and collaborating with a team, which has prepared me for tackling more complex projects in the future.

#### Mai Nguyen

My primary contribution was developing the website’s front end based on the foundational setup by my teammate Son. I focused on implementing UI functionalities for the product page, including posting and displaying group-buying deals from both the host’s and co-buyers perspectives, enabling purchase requests, and adding filtering options. After completing Design Project 4, I proposed new features to enhance the user experience, such as host management for postings and purchase requests, and a group chat feature for communication. I collaborated with Son to implement these improvements, ensuring smoother functionality for both hosts and co-buyers. For user testing, I worked with Trang to recruit participants and collect feedback.

One of my biggest challenges was learning React and front-end development due to my limited prior experience, which made teamwork initially difficult as our skills were not aligned. We really struggled with integrating the front end with the back end, as many functions and components were built separately by different team members, and we had our own assumptions. When it came to integration, it turned out there was a lot of miscommunication, so we had to make many adjustments during integration and deployment. One good thing about teamwork is that I could see us all growing together and helping each other solve problems, which made progress much faster compared to if I had worked on my own.

Through this project, I developed crucial front-end skills, including reading and applying library documentation to integrate and customize third-party libraries. I gained experience in collaborative software development, using tools like Git for version control. Additionally, the user testing process was insightful. While some user concerns aligned with ours, others offered fresh perspectives on service improvement. This feedback not only enhanced our project but also helped me understand how to build more user-centered products in the future.


#### Son Nghiem Xuan

I focused on developing the user-facing side of our web application, starting with laying the groundwork of the project and setting the stage so my teammates can collaborate seamlessly. My key responsibilities included implementing the user profile and login pages where I developed the authentication logic and features for managing one’s postings and account details. In addition, I also worked on the real-time chat functionality between group-buying participants, and closely cooperated with Mai to deliver the product browsing page.

Our team worked well together. Everyone was punctual and did their parts excellently. It was easy for everyone to decide on meeting times, and we had a lot of quality discussion and developed a shared mental model of our project. However, a substantial hurdle for me was inadequate coordination between the backend and the front-facing side of our app. API endpoints and data schemas were defined differently in the frontend and backend, leading to many bugs that were time-consuming to fix. We were able to overcome this problem by closely communicating with each other our requirements. In future projects, I will first define a shared requirements specification so that both sides are able to develop independently and frictionlessly.

I learned a lot throughout this project. I learned how to design a clean and usable user interface, how to implement real-time chat systems, and costs and benefits of different design choices when building a social computing platform. I also learned a lot about how to communicate and work efficiently in a team, how to perform needfinding, and how to extract valuable insights from users' feedbacks and improve upon the design.
