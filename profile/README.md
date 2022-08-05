# Lali-Ho Reviews

### The purpose

The website aims to provide a hub for Final Fantasy XIV players to find Free Companies that match their interests, as well as be able to post or read reviews from previous and current members.

In this context, a “Free Company” (FC) in Final Fantasy XIV (FFXIV) is analogous to a guild or clan in any other game, in that it is essentially a social club for like minded members.

### Target audience

The target audience of this site would be primarily made up of players of the relevant game, but from that group could include users looking to join a FC, FC looking to voice their opinions, and even FC Leaders looking for feedback.

## Deployed site (coming soon)

Lali-ho Reviews [Coming Soon ]()

Github Repos:
[Ruby API](https://github.com/Lali-ho-Reviews/Lali-ho-React) | 
[React Frontend](https://github.com/Lali-ho-Reviews/Lali-ho-API)

### Features

- Search Free Companies by:
- Name
- Category
- Ranking
- View Free Company details, reviews and ratings
- Post reviews of Free Companies
- Search all existing Free Companies via the FFXIV API
- Optional sign up/log in for users - maybe by using the Loadstone
- At least a basic admin view for moderation

#### Sprinkles (features we would like to implement if time)

- User profile view to see the entire post history
- “Like” reviews
- Admin to ban users

### Tech stack

- Ruby/Ruby On Rails
- React
- HTML/CSS
- Bootstrap CSS
- Tailwind CSS
- PostgreSQL
- Github, Heroku
- AWS for image storage

## Dataflow Diagram

![Dataflow Diagram](/docs/Guilds_data_flow.drawio.png)

## Application Architecture Diagram

![ArchitectureDiagram](/docs/ArchitectureDiagram.png)

# Stories

### User Stories(Global)

- As a User I would like to see a list of FC’s.
- As a User I would like to search for a specific FC by name.
- As a User I would like to filter FC’s by tags/categories.
- As a User I would like to view more information about an FC.
- As a User I would like to read reviews about an FC.
- As a User I would like to view another User's profile, including their reviews.
- As a User I would like to be able to sign up for an account using my email.
- As a User I would like to log into my account using my email.
- As a User I would like to be able to recover my account by resetting my password.

### Admin Stories

- As Admin I would need to be able to view submissions for new FC’s.
- As Admin I would need to be able to approve or reject FC submissions.
- As Admin I would need to be able to edit and delete other Users reviews.
- As Admin I would like to be able to ban Users.
- As Admin I would like to be able to see all reviews, for easier moderation.

### Anonymous Stories

- As an Anonymous User I would like to be able to post a review.

### Logged in User Stories

- As a Logged in User I need to be able to sign out of my account.
- As a Logged in User I would like to view my own profile.
- As a Logged in User I would like to change my details, including my password.
- As a Logged in User I would like to be able to delete or edit my own reviews.
- As a Logged in User I would like to be able to delete my own account.
- As a Logged in User I would like to be able to set my own profile picture.
- As a Logged in User I would like to be able to “like” reviews.

# Wireframes

![Wireframes Homepage](/docs/home%20.png)

### Landing page

#### High priority

- Sign up/ Log in
- Search bar
- List of Free Companies

These are all high priorities as they are needed to make the landing page functional without them the Global user wouldn't be able to interact with the site. The category links are a second as the user can still use the site without them.

![Wireframes Fc list ](/docs/FC-list.png)

### FC list page

#### High priority

- Nav bar
- List of FC’s
- Sort by

These are the highest priority on the FC list page without them the Global user specifically ‘ Would like to see a list of Fc’s” would not be possible. The same goes for the sort button without that the global user would not be able to change how they view the list of the FC - whether they would like to do it with the lowest rating or by how many views.

The FC list page is an overview of all FC’s on the site if a user wants to see more information or wants to leave a review for the particular FC they can click the component and it will take them to the FC page.

![Wireframes Fc Profile page](/docs/FC-profile.png)

### FC page

#### High priority

- Nav bar
- Reviews
- Like / Flag

These are the highest priority on the FC page as they connect to the Global user stories with being able to view a particular FC page and to be able to read the reviews. The like and flag button connects to the Logged in user stories of being able to 'like' another reivew and the flag it to bring it to an Admins attention.

To get to this page a User must first have either searched for it via the search options on the site (landing page and nav bar) or find it from the FC list page.

![Wireframes Form layouts](/docs/Basic-formlayout.png)

### Forms

The form pages are to help with continuity within the site, making sure all forms follow the same layout however context will change inside depending on what form is shown.

![Wireframes Admin profile](/docs/Admin-profile.png)

### Admin profile

#### High priority

- Password changing
- Delete account
- Email/username field

These are the highest priority on the Admin profile tab as this connects to the Global user stories of being able to change their information on the site eg password, email, and username.

To get to an Admin page you first need to be added as an Admin then you will have access to the Admin panel via nav bar.

### Admin Reviews

#### High priority

- Shows your reviews
- Edit and delete button for reviews

These are highest priority on the review tab as it connects to the Logged in User stories of being able to see your own reviews and being able to edit or even delete them.

### Admin Flagged

#### High priority

- Shows the flagged reviews
- Allow and delete button for flagged reviews

These are highest priority on the Flagged tab as it connects to the Admin User Stories of being able to manage reviews that people flag as inappropriate.

The admin user has a menu component to the left of the screen with the clickable options for: Profile, Reviews, Flagged. When one of the buttons are pressed the component on the right will change to display the corresponding information.

![Wireframes Auth user profile](/docs/Authenitcated-user-profile%20.png)
### Authenticated user profile 
#### High priority 
- Password changing 
- Delete account
- Ban account
- Email/username field

These are the highest priority on the Authenticated profile tab as this connects to the Global user stories of being able to change their information on the site eg password, email, and username. The ban button can only be seen by an Admin with the rights to ban a user if needed. 

To get access to the user profile a user must first sign up to the site then they will have access to these pages via nav bar. 


### Authenticated user reviews 
#### High priority 
- Shows your reviews 
- Edit and  delete button for reviews

These are the highest priority on the Authenticated user review tab as it connects to the Logged in User stories of being able to see your own reviews and being able to edit or even delete them. 

The Authenticated user also has the same menu option in their profile as well, to keep styling consistent throughout the site. 


# Task Allocation & Tracking

Tasks for the development of Lali-Ho Reviews are tracked using a Trello board [found here](https://trello.com/b/uveGyFVr/t3a2-part-ab)

- Planned Features list- tasks that have yet to be started and are essential
- Styling list- To keep track of what needs to be styled
- Documentation Requirements list- make sure we meet the requirements of the assignment
- To Do list- Track what has to be done
- Personalized lists- to keep track of who is working on what
- Reviewed lists- Make sure we are reviewing each others work and if we are stuck can add it to the teachers trello.
- Testing list - to see what has been tested and what needs to be tested.
- Ready- Is ready to be implemented
- Done and deployed- is on the site and is running the way we want it to.
- Bugs list - keep track of bugs and if we have found solutions

![Trello images](/docs/T3A2_Trello1.png)
![Trello images](/docs/trello2.png)


# Manual Testing 

We created a document for manual testing as a user and also as a deveoloper.  The Manual testing was mainly done on the front end and had three stages of testing.  The first test was when it was first implimented, there was a second test when it had been a few days and other branches had been merged. The final test was done the day before this assignment was due as a final check over before submission

![testing image](/docs/manual.png)

# Rspec Testing

- React Router - React Router was the library in which server-side routing was implemented.  It allows the creation of single-page web or mobile applications that dont have to refresh the page each time it is used. 
For the Rails side, we opted to utilise Rspec for a series of automated tests. These tests focused on our 3 major models: Users, Companies and Reviews. These tests include checking the creation parameters of the models, particularly users and reviews as they will be more often interacted with by the end user, routing tests to ensure that routes are set up properly and a suite of request tests, that cover all the expected and unexpected CRUD requests.

# Libraries used

### React

- Flowbite & Tailwind -  Tailwind was the main styling library used with the help of Flowbite which is based on Tailwind.  These Libraries were used for all things to do with styling from implementing custom font size and colours and using what the framework provides at the same time. It made styling components inline easy and fast 

- Axious - Anxious was the library which created HTTP requests from internal API's as well as getting support for request and response interception, conversion of data into JSON format, and transforming it into usable data for the application.


### Rails

The gems we utilised on Rails outside of the default ones included: 
- Knock - Handled JWT and authentication, and was probably a poor choice considering it's out of date.
- pg_search - My beloved pg_search makes implementing search functions on Rails such a breeze.
- Rspec - Main automated test suite
- Database Cleaner - Assisted Rspec for testing
- FactoryBot - Assisted Rspec for testing
