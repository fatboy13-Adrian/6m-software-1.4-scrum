## Assignment

### Brief

Write your answers for each question:

Question 1:
Imagine you are hired by a startup company for a school to implement their IT infrastructure as their IT consultant. n your own words (300 words or less), describe how could implementing Scrum help their IT team improve their productivity.

By implementing scrum, it can enhance productivity of the IT team in a startup school by fostering better collaboration, set clear goals and adaptability. 
This will help the school's IT team to operate more efficiently, deliver solution faster and adapt to changing of needs, which is critical in our fast paced and evolving field of education.

Below are how I will implement scrum to help the IT team to improve on their productivity:

Foster better collaboration
- Scrum encourages daily stand - up meetings whereby teammates discuss their work progress, challenges faced and plans for the day.
- Such open communication ensures the IT team is aligned to avoid misunderstanding and foster team work within the organization.

Set clear goals
- Through sprint planning, IT team can breakdown large projects into smaller, and managable tasks such as setting up of school network or deployment of e-learning webpages.
- Clarity will help the team to prioritize their tasks and focus on delivering value on an incremental basis.

Adaptability
- By using scrum's iterative approach, it allows IT team to regularly review and adjust their plans so that they can respond effectively to new requirements or challenges like a sudden need to setup an online learning platform.

Continuous improvement (CI)
- Sprint retrospective at end of each iteration allows the IT team to reflect on what was done well and what can be improve upon.
- This would provide constant feedback loops that promotes learning and enhancing efficiency over time.

Customer - centric approach
- Scrum emphasizes on delivering functional increments on a regular basis, which ensures that all stakeholders receive usable outputs and provide feedback.
- It will help IT team to focus on meeting the actual needs within the project.

References
- https://www.scrum.org/learning-series/what-is-scrum/


Question 2:
Write ten (10) user stories for a book-borrowing website for a library. Write it in the format: `As a ____, I want to ____, so that _____`.
1. As a library user, I want to find books available in all library branches, so that I can find the book I need at a library branch that is near my home.
2. As a library user, I want to reserve books online, so that I can collect the book in my free time from the library branch that is near to my home.
3. As a library user, I want to receive notifications / updates on book's availability, so that I can make plans to collect them.
4. As a library user, I want books / audiobooks online, so that I can access them anytime without visiting the library.
5. As a library user, I want to be able to renew my borrowed books online, so that I can extend the loan period without visiting the library.
6. As a library user, I want to filter the search results by availability, genre and language, so that I can find the books that meet my preference.
7. As a library user, I want to be able to view my borrowing history, so that I can track my book reading records and avoid borrowing duplicates.
8. As a library user, I want to be able to access book recommendations based on my borrowing history / habits, so that I can discover new books that interest me.
9. As a library administrator, I want to generate reports on borrowing trends and book popularity, so that I can make informed decisions about the library collections.
10. As a parent, I want to find books that are suitable for children, so that I can help my kids to develop good reading habits.


References:
- https://www.nlb.gov.sg/main/services/faqs/eresources
- https://www.nlb.gov.sg/main/services/faqs/NLB-Mobile/get-started-with-libby
- https://www.nlb.gov.sg/main/services/faqs/NLB-Mobile/Getting-started
- https://nlb.overdrive.com/
- https://www.nlb.gov.sg/main/services
- https://www.nlb.gov.sg/main/services/Loans-and-Reservations
- https://www.nlb.gov.sg/main/site/discovereads/children
- https://www.nlb.gov.sg/main/site/discovereads/MTL/Chinese/reading-recommendations

Question 3: 
Define [Acceptance Criteria](https://resources.scrumalliance.org/Article/need-know-acceptance-criteria) for 3 to 5 user stories out of the 10 user stories you have defined.
1. As a library user, I want to find books available in all library branches, so that I can find the book I need at a library branch that is near my home.
Find for a book that is available in 1 branch:
    - Given that the user is on book search page
    - When user enter title or author
    - Then system to display branch where book is available

Find a book that is not available:
    - Given that user is on book search page
    - When user find a book that is unavailable in any branch
    - Then system should display message "Book is unavailble"

Filter by branch
    - Given that user is on book search page
    - When user select a specific library branch filter
    - Then system should display only books available in that branch

2. As a library user, I want to reserve books online, so that I can collect the book in my free time from the library branch that is near to my home.
Reserve a book successfully
    - Given that user had logged into their user account
    - And book is available for user to make Reservation
    - When user click on reserve button and select a branch
    - Then system should confirm reservation and display pickup date and branch

Attempt to reserve a book that is already being reserved
    - Given that user is viewing book details
    - And book is already reserved by another user
    - When user attepmts to reserve book
    - Then system should display message "Book is reserved by another user"

Reserve a book without select branch
    - Given that user had logged into their user account
    - When user tries to reserve a book without branch selection
    - System should display message "Please select a branch"

3. As a library user, I want to receive notifications / updates on book's availability, so that I can make plans to collect them.
Opt into receiving availability notifications
    - Given that user is logged into their user account
    - When user attempts to search for a book that is unavailble
    - Then system should provide options for user to subscribe to book availability notification

Received book notification when book is available
    - Given that user had subscribed to availability notification for a specific book
    - And book becomes available
    - When system sends book available notification
    - Then user should receive notification by email or SMS with instructions for pickup

Unsubscribe notification availability
    - Given that user had subscribed to availability notification for a book
    - When user choose to unsubscribe availability notification
    - Then system should stop sending availability notification and confirm cancellation with user

4. As a library user, I want to be able to renew my borrowed books online, so that I can extend the loan period without visiting the library.
Renew loan successfully
    - Given that user had logged into their user account
    - And book borrowed is eligible for early renewal
    - When user navigate to "my borrowed books" section and click renew button for a book
    - Then system should extend loan period by the allowed duration and display new due date

Attempt to renew overdue book
    - Given that user is logged into their user account
    - And loan period had expired
    - When user tries to renew an overdue book
    - Then system should display message "This book cannot be renewed as it is overdue. Please contact library"

Renew book without remaining renewals
    - Given that user is logged into their user account
    - And book had reached its maximum number of renewals allowed
    - When user tries to click on renew button
    - Then system shoud display message "Renewal limit had been reached. Please return book"

5. As a library user, I want to be able to view my borrowing history, so that I can track my book reading records and avoid borrowing duplicates.
View history
    - Given that user had logged into their user account
    - When user navigate to browsing history section
    - Then system should show the browsing history of previously borrowned books with details such as author, borrowed / return dates and title

Find book within borrowing history
    - Given that user had logged into their user account
    - When user enter a keyword in search branch
    - Then system should filter and display information that matches the keyword on search branch

View borrowing history statistics
    - Given that user is on borrowing history page
    - When user access their borrowing history
    - Then system should optionally provide a summary of borrowing patterns

Export browsing history
    - Given that user is on browsing history page
    - When user click export button
    - Then system should generate a CSV/PDF file containing the browsing history

Question 4
Define story points based on the ACs.
1. As a library user, I want to find books available in all library branches, so that I can find the book I need at a library branch that is near my home.
    Find for a book that is available in 1 branch: 5 points
    Find a book that is not available: 2 points
    Filter by branch: 5 points

2. As a library user, I want to reserve books online, so that I can collect the book in my free time from the library branch that is near to my home.
    Reserve a book successfully: 5 points
    Attempt to reserve a book that is already being reserved: 3 points
    Reserve a book without select branch: 2 points

3. As a library user, I want to receive notifications / updates on book's availability, so that I can make plans to collect them.
    Opt into receiving availability notifications: 5 points
    Received book notification when book is available: 6 points
    Unsubscribe notification availability: 2 points

4. As a library user, I want to be able to renew my borrowed books online, so that I can extend the loan period without visiting the library.
    Renew loan successfully: 5 points
    Attempt to renew overdue book: 3 points
    Renew book without remaining renewals: 3 points

5. As a library user, I want to be able to view my borrowing history, so that I can track my book reading records and avoid borrowing duplicates.
    View history: 5 points
    Find book within borrowing history: 2 points
    View borrowing history statistics: 4 points
    Export browsing history: 8 points

### Submission 

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL. 


### References

_Example of Referencing Classmate_

Referenced the code block below from Terence.
```js
    function printMe()
    {
        console.log("I am a reference example");
    }
```

_Example of Referencing Online Resources_

- https://developer.mozilla.org/en-US/
- https://www.w3schools.com/html/
- https://stackoverflow.com/questions/14494747/how-to-add-images-to-readme-md-on-github

