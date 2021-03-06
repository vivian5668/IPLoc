# ASCIImage
###  - Convert Your Image to ASCII
<img width="481" alt="readme_pic" src="https://user-images.githubusercontent.com/35155255/36921325-cdfbb1aa-1e18-11e8-8ffe-2c64ea469747.png">


## Introduction
Looking for a modern way to re-create images? Try ASCIIamge! Simply upload a picture, and you will get back the ASCII image in text format. Try it [here](https://asciiamge.herokuapp.com/).

## Supported Browsers

- Chrome Version 63.0 and higher

- Firefox Version 58.0 and higher

## Wireframes
### Web Version
>For the best user experience, the web version uses a consistent centered layout with a navigation bar on the top. The navigation bar is dynamic based on if there is a user currently logged in.

- Main page
<img src="https://user-images.githubusercontent.com/35155255/36921109-f713b6ce-1e17-11e8-8029-21f8b723e82b.png" height="250">

- Image upload page
<img src="https://user-images.githubusercontent.com/35155255/36921102-ef25012a-1e17-11e8-8477-8d3499aca05b.png" width="380">

- Gallery page
<img src="https://user-images.githubusercontent.com/35155255/36921115-f9f4ce46-1e17-11e8-89c7-e69091d1b35e.png" width="300">

### Mobile Version
>The mobile version resembles the web version mostly with minor modification to fit contents on smaller screens. The navigation bar collapses and slides out from the left of the screen once you click on the hamburger icon. The gallery page also changes column layout on mobile version.
<img src="https://user-images.githubusercontent.com/35155255/36921116-fc7ad3a4-1e17-11e8-9dd4-9887c9ae6f8b.png">

## Routes
| Verb          | Path          | Action | Usage        |
| ------------- |---------------| -------|--------------|
| GET     		| /				| index  |	Homepage	|
| GET     		| /auth/signup	| new  	 |	Display form to create a new profile	|
| POST     		| /auth/signup  | create |	Create user account	|
| GET     		| /auth/login	| show   |	Display form to enter login info	|
| POST    		| /auth/login	| show   |	Authenticates user login info	|
| GET     		| /auth/logout	| index  |	Logs user out of the application	|
| GET     		| /gallery		| show   |Display the gallery page	|
| GET     		| /instructions	| show   |	Display instructions for this app	|
| GET     		| /profile		| redirect|	Display the user's projects if user is logged in	|
| GET     		| /projects		| index  |	Show all user's projects	|
| GET     		| /projects/new	| show   |	Display form to allow the user to create a new project	|
| POST    		| /projects/new	| create |	Create a new project	|
| GET     		| /projects/:id	| show   |	Display the project identified by project_id	|
| GET     		| /projects/:id/edit| show  |	Display the form that allows the user to modify project information	|
| PUT     		| /projects/:id	| update  |	Change project information	|
| DELETE     	| /projects/:id/destroy	| delete  |	Delete a project	|


## Models & Sample Data
|id| name          | email          | password |
|--|------------- |---------------| -------|
| 2| Happy    		| happy@gmail.com			| $2a$10$Cnu/3QHw2WCaMo4xTfq5K.MTL9W2N4PDlA9t/0UOrj6I3A8c9GD7a  |	

|id| project_name  | description   | cloudinary_url | ascii_url     | userId        |
| -|----------- |---------------| ---------------| ------------- |---------------|
| 1| Sydney Colors | School Project| http://res.cloudinary.com/dxc.. |<span>djiendjncjd... | 2 |

## Technology / Library Used

- Javascript

- jQuery

- Materialize CSS
- Sequelize
- Node.js
- Relational databse

## Next Steps

- Add a loading page for long API calls

- Allow users to login user Facebook / Github / Google login, etc.

## Resources

- Google GIF / image search

- Materialize CSS documentation
- [Firestack API](https://blog.filestack.com/api/an-api-to-convert-any-image-into-ascii/) Transforms images to ASCII
- [Cloudinary API](https://cloudinary.com/) Stores and manages images on the cloud




