# Cars App Assignment

## What is happening
This is a full-stack web application that allows users to manage a list of cars. The front end is built with HTML, CSS, and Vanilla JavaScript, and the back end is powered by a Node.js server using Express. Users can view a table of cars, add new cars, delete existing records, and update car details. The front end communicates with the back end API using `fetch` requests.

## How I solved the problem
To handle the core requirements, I modified the `index.html` file to properly fetch and display the data from the `/api/cars` endpoints. 

The trickiest part was figuring out how to handle the **Update** logic. To solve this, I repurposed the existing "Add a Car" form:
1. When a user clicks the `[update]` button on a specific row, a `GET` request fetches that car's data.
2. That data is used to automatically fill in the form fields, and the form switches into "edit mode" (saving the specific car's ID).
3. When the user submits the form, instead of sending a `POST` request to create a new car, the app sends a `PUT` request to update the existing record. The table then refreshes to show the new data.

## Screenshots

*(Drag and drop your screenshot of the app here)*

*(Drag and drop a screenshot of adding/updating a car here)*
