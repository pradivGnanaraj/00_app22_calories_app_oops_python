# Calorie Calculator

The Calorie Calculator is a simple web application built using Flask that helps users estimate their optimal daily calorie intake based on various factors such as weight, height, age, and local temperature. The application utilizes data from external sources to provide accurate calorie calculations.

## Features

- Calculate optimal calorie intake based on weight, height, age, and local temperature.
- Provides temperature data from TimeAndDate.com using a web scraper.
- User-friendly web interface for input and result display.
- Interactive and responsive design.

## Components

- **app.py:** Main application file responsible for setting up the Flask app and defining routes.
- **calorie.py:** Contains the `Calorie` class, which calculates the optimal calorie intake based on user inputs and temperature.
- **temperature.py:** Includes the `Temperature` class, which scrapes temperature data from TimeAndDate.com using XPath.
- **temperature.yaml:** YAML configuration file defining the XPath for temperature extraction.
- **static/main.css:** Stylesheet for customizing the frontend interface.
- **templates/:** Folder containing HTML templates for different pages.
- **requirements.txt:** Lists the required dependencies for the application.

## How to Use

1. Clone the repository and navigate to the project directory.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the application using `python app.py`.
4. Open a web browser and access the application at `http://localhost:5000`.
5. Enter your weight, height, age, country, and city, then click "Calculate" to get the estimated calorie intake.

## External Dependencies

- Flask: Web framework for handling requests and routing.
- WTForms: For creating and handling input forms.
- Selectorlib: Web scraping library used to extract temperature data.
- Requests: Library for making HTTP requests.
- Jinja2: Template engine for rendering HTML templates.

## Design Considerations

- The application follows the MVC (Model-View-Controller) pattern.
- Input validation is important to ensure accurate calculations and data integrity.
- The web scraper in the `temperature.py` module extracts temperature data from TimeAndDate.com using a predefined XPath in the `temperature.yaml` configuration file.
- The frontend uses responsive design to ensure a consistent experience across different devices.

## Deployment

You can deploy the application on a web server or cloud platform of your choice. Make sure to update the `app.run()` statement in the `app.py` file for production deployment.

## Future Enhancements

- User accounts and history tracking for personalized experiences.
- Integration with external APIs for more accurate temperature data.
- Improved error handling and feedback for users.
- Enhanced UI/UX design for a more visually appealing interface.

## Credits

This application is developed by [Your Name] as part of a coding project.

---
