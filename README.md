# Ionic Starwars

## Project Des cription: 
The objective is to bulid a simple StarWars app using SWAPI(Starwars API) that will display Star Wars characters in a list, allow searching, and provide a details page to display additional info about the characters. 

The project should have two pages and one provider (service). More information below:

##Main page - list.html and list.ts 
This is the main page of the app. It should have the title of 'Star Wars'. It should display the first 10 star wars characters' names by calling the getAll method from swapi-service.ts. It will have a search bar across the top that filters the reults as users types. When users click on a name, it should navigate to the details page by passing the corresponding character ID. 

## Detail page - list-detail.html and list-detail.ts
This is the details page for Star Wars characters. It should accept a character ID from the route, and display the name, gender, mass, and height of the character by calling the getOne method in swapi-service.ts. There is no requirement on the style except that it looks decent on a mobile device. The page title should be the name of the Star Wars character and there should also be a back button that lets users go back to the main page. 

## StarWars Service - swapi-service.ts
This purpose of this service is to make http calls to the Star Wars API (SWAPI) and return a promise. It should have the two methods - getOne and getAll. getOne takes a parameter of id will issue an http GET to http://swapi.co/api/people/{id}. getAll takes no parameters and will issue a GET to http://swapi.co/api/people. 

## Acceptance Criteria
1. When the app loads, it should display the names of the first 10 star wars characters in a list. 
2. The list can be filtered by entering a search criteria. 
3. By clicking  / tapping on a name, it should go to the details page, where the name, gender, mass, and height of the character are displayed. 

## Submission criteria: 
Once the application works correctly and meets all the criteria above, it should be deployed to a public git repository. 

## Resources: 
1. [Angular1 and Angular2 comparison](https://angular.io/docs/ts/latest/cookbook/a1-a2-quick-reference.html)
2. [Introduction to Ionic2](http://www.joshmorony.com/beginners-guide-to-getting-started-with-ionic-2/)
3. [Setting up Ionic2](http://ionicframework.com/docs/v2/getting-started/)
4. [Sample ionic2 project for pokemon](https://github.com/dmackerman/ionic2-pokedex)

The last one is a similar app built using the Pokemon API. Feel free to use it for reference. Although you won't be able to run the project, as it was built using an older version of ionic, some things haven't changed much. You can look at https://github.com/dmackerman/ionic2-pokedex/tree/master/www/app/components/