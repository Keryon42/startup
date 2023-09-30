# TITLE TBD
## Elevator Pitch
Zork. The Hitchhiker's Guide to the Galaxy. Dungeon Man. These games shaped all modern rpgs (Except maybe Dungeon Man.) But text based adventure games are not dead! As web apps become increasingly popular, and users become increasingly used to typing on their phones, a space opens up for narratively driven games that are easily controlled on from a mobile device. Most high paced games are difficult or impossible to control from a phone, but the deliberate, puzzle-driven pacing of a text based adventure game allows for an experience just as good on mobile as you'd get on any other device. And with modern technology, the limits of a text based adventure game can be pushed. The background and text color may grow dim in a dark cavern, the text may shake or even collapse under an earthquake, images can be easily embedded, and a method of leaving messages for other players can allow for hints and tips to collaboratively work towards the end goal. 

### Design

![Login Screen](https://github.com/Keryon42/startup/blob/main/Images/Login%20mockup.PNG?raw=true)
![Game](https://github.com/Keryon42/startup/blob/main/Images/Game%20mockup.PNG?raw=true)
![Chat](https://github.com/Keryon42/startup/blob/main/Images/Chat%20mockup.PNG?raw=true)


### Key features

- Secure login over HTTPS
- Progress stored persistently
- Manual save button, logout button, etc. 
- Real time "canned" messaging system
- Page that displays username and number of commands used to win

### Technologies

I am going to use the required technologies in the following ways.

- **HTML** - Uses correct HTML structure for application. Most of application will be text driven, and therefore will require large amounts of HTML. 
- **CSS** - General styling, simpler text modifications, like changing colors to represent environment or certain actions.
- **JavaScript** - Provides login, buttons for accessing canned chat, some of the fancier effects like words shaking or collapsing
- **Service** - Backend service with endpoints for:
  - login
  - retrieving save data
  - retrieving list of winners
- **DB** - Store users, save data, list of winners
- **Login** - Register and login users. Credentials securely stored in database. Without logging in no progress can be saved.
- **WebSocket** - Canned chat allows real time limited communication between users, in lieu of any form of moderation. 
- **React** - Application ported to use the React web framework.

## HTML deliverable

For this deliverable I built out the structure of my application using HTML.

- **HTML pages** - Four html pages, a home/login page, an about page, a page listing those who have cleared the game, and the page where you play the game
- **Links** - A directory at the top lets you navigate to any of the four pages. The about page has links to various inspirations for the game. 
- **Text** - A brief description of the game on the about page, and some placeholder introductory text on the game page. 
- **Images** - Placeholder image placed on about page, will eventually replace with some sort of logo
- **Login** - Input box and submit button for login, for now submit button just links to play page. 
- **Database** - List of victors will be pulled from database.
- **WebSocket** - Message button will open up messages left in local area and allow users to write their own. 
