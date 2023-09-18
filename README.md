# TITLE TBD
## Elevator Pitch
Zork. The Hitchhiker's Guide to the Galaxy. Dungeon Man. These games shaped all modern rpgs (Except maybe Dungeon Man.) But text based adventure games are not dead! As web apps become increasingly popular, and users become increasingly used to typing on their phones, a space opens up for narratively driven games that are easily controlled on from a mobile device. Most high paced games are difficult or impossible to control from a phone, but the deliberate, puzzle-driven pacing of a text based adventure game allows for an experience just as good on mobile as you'd get on any other device. And with modern technology, the limits of a text based adventure game can be pushed. The background and text color may grow dim in a dark cavern, the text may shake or even collapse under an earthquake, images can be easily embedded, and a method of leaving messages for other players can allow for hints and tips to collaboratively work towards the end goal. 

### Design

![Mock](voterMockUI.jpg)

Here is a sequence diagram that shows how to people would interact with the backend to vote.

![Voting sequence diagram](votingSequenceDiagram.png)

### Key features

- Secure login over HTTPS
- Progress stored persistently
- Manual save button, logout button, etc. 
- Real time "canned" messaging system, with room information available
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
