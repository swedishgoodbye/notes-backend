# notes-backend
The front end portion of this project can be found:  
https://github.com/swedishgoodbye/notes-frontend  
**THIS APP IS WORK IN PROGRESS. STABILITY IS NOT ENSURED**
  
## Prerequisite Software:
* [yarn](https://yarnpkg.com/en/)
* [node.js](https://nodejs.org/en/)
* [mongoDB](https://www.mongodb.com/)  
  
## Installation / Starting Server:
* cd into app
* run 'yarn' or 'npm install'
* run 'yarn start' / 'npm start' or 'node server'
  
## API Routes:  
* include 'localhost:5000/' on your request line before these routes  
### DB TEST Route
> /test

### GET Notes  
> /api/f/notes

### GET Note By ID
> /api/f/view/:_\_id_

### POST Note
> /api/c/note  
> The JSON Format for creating a note is as follows:  
> {  
>  **"title":** _"Title as string"_  
>  **"content":** _"Content as string"_  
> }

### PUT Note
> /api/u/:_\_id_  
> Use the same JSON format used by the POST route to update your note

### DELETE Note
> /api/d/:_\_id_  
  
**THERE ARE FILES INCLUDED FOR THE LOGIN/REGISTER SYSTEM. THIS IS A WORK IN PROGRESS FEATURE AND STABILITY IS NOT ENSURED, AND DOES NOT NECESSARILY DO ANYTHING YET.**  
### POST Register
> /api/r/  
> The JSON Format for registering a user is as follows:  
> {  
>  **"username":** _"Username as string"_  
>  **"password":** _"Password as string"_  
> }

### POST Login
> /api/l
