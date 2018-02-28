# PROJECT SYNOPSIS
  
## Project Name
Movie App / IMDB App  
  
## Project Description
This application allows users to add movie information and preview the same. Adding a new movie takes the following input parameters:  
Movie Name, Movie Rating, Movie Release Date, Movie Description & Movie Image URL.  
  
## App Usage/Flow of App
On running the app for the first time & accessing the home page, the following can be noticed:  
  
### Home Page (http://localhost:4200/movieHome):  
1. IMDB Icon: Present constantly on all pages of the app. Clicking this form anywhere will navigate user to home page.  
2. "Add a movie" button: Clicking on this, will navigate the user to a page(http://localhost:4200/addMovie) where new movie information can be entered and added.  
3. A jumbotron stating "No Movie Data Available".  
4. A search bar with a "Search Movies" placeholder.  
  
### Adding a Movie (http://localhost:4200/addMovie):  
1. This page can be accessed from home page on clicking the red "Add a movie" button.  
2. User can enter movie details here, the following being mandatory fields:  
Movie Name(text), Movie Rating(drop-down) & Movie Release Date(date).  
Movie Decription(text-area) & Movie Image URL(text) fields are optional.  
3. If the user skips a mandatory field for some reason, a warning is shown and the corresponding field border turns red. If the validation passes for a field, the field border would become green.  
4. Please note that the "Add to Movie Database" button is disabled until all fields pass validation.  
5. Once all details are filled in, clicking on "Add to Movie Database" button takes us to the home page where the movie just entered is displayed.  
  
### Viewing the added movie - back to home page
1. In the home page, user would notice that the previously displayed "No Movie Data Available" message has now been replaced by the movie added. More precisely, the image from the URL they provided is shown, below which stars depicting the rating is displayed.  
2. If no image URL is provided, a default one is displayed that says "NO POSTER FOUND".
3. A rating given between 1 & 2 displays RED star(s), between 3 & 4 displays YELLOW stars and a rating of 5 shows 5 GREEN stars.  
4. Hovering over this image highlights its border with a color same as the one used to display the star rating. Hovering also shows the movie name.  
5. Adding more movies adds subsequent image movie icons to this list.  
6. Clicking on any icon takes user to a page showing its corresponding details.  

### Searching for a movie
This feature is again available in the home page itself. User can type in a movie name and the results displayed would be based on matching this string of letters with the initial characters of movie names in the list. 
  
### Viewing a movie's details
1. In the home page, clicking on any movie image icon navigates user to its corresponding details page (http://localhost:4200/movieDetail/:id).  
2. Here, user can see the representational movie image, movie name & rating (as heading), below which is displayed the release date. Further below the movie description can be seen, if user has provided the same. Otherwise, "N/A" is displayed.  
  
### Typed an invalid URL?
If a user types an invalid URL in the address bar, he/she would be navigated to a page that notifies the user saying "Oops! Page not found :(". User can then navigate back to home page by either clicking on the IMDB icon or the "Go Home" button.
