# City Cards CRUD Application

## Overview

This project is a simple web application that allows users to create, read, update, and delete (CRUD) information about various cities. The application is built using HTML, CSS, and JavaScript, with Bootstrap for styling.

## Features

- **Add City**: Users can add new cities to the list by providing the city name, image URL, description, ranking, and air quality.
- **Edit City**: Users can edit the details of existing cities.
- **Delete City**: Users can delete cities from the list.
- **Persistent Data**: The city data is stored in the browser's local storage, ensuring that it persists across page reloads.

## File Structure

```
index.html
```

## Code Explanation

### HTML

The HTML file sets up the structure of the application:

- **Head Section**: Includes meta tags, the page title, and links to Bootstrap CSS.
- **Body Section**: Contains a container div with the ID `app` where the city cards will be dynamically rendered. It also includes scripts for Bootstrap JS, jQuery, and the main JavaScript code.

### CSS

Custom styles are included within the `<style>` tag in the `<head>` section to style the city cards:

- `.card`: Styles for the city card container.
- `.card img`: Styles for the city image.
- Other classes (`.card-title`, `.card-description`, `.card-ranking`, `.card-air`, `.card-actions`) for the content inside the card.

### JavaScript

The JavaScript code handles the CRUD operations and rendering:

- **City Data**: The initial city data is loaded from `localStorage` or uses default values if none exist.
- **saveCities()**: Saves the current city data to `localStorage`.
- **renderCities()**: Renders the city cards based on the current city data. It also includes an "Add City" button.
- **addCity()**: Prompts the user for city details and adds a new city to the list.
- **editCity(index)**: Prompts the user to edit the details of the city at the specified index.
- **deleteCity(index)**: Confirms and deletes the city at the specified index.

## How to Use

1. **Open the Application**: Load the `index.html` file in a web browser.
2. **Add a City**: Click the "Add City" button and fill in the prompted details.
3. **Edit a City**: Click the "Edit" button on a city card and modify the details as prompted.
4. **Delete a City**: Click the "Delete" button on a city card to remove it.

## Example Usage

Upon loading the application, the user will see a list of cities with their respective details. Users can add new cities, edit existing ones, and delete cities as needed. The changes will be saved in the browser's local storage, ensuring persistence across sessions.

## Technologies Used

- **HTML**: For the structure of the application.
- **CSS**: For styling the application.
- **JavaScript**: For the application logic and interactivity.
- **Bootstrap**: For responsive and modern UI components.
- **Local Storage**: For persistent data storage.

## License

This project is licensed under the MIT License. Feel free to use and modify the code as needed.

---

This README file provides a comprehensive overview of the project, explaining its features, code structure, and usage instructions.