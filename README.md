# AI Dog
The AI (Artificial Intelligence) Dog project is a team submission for the Microsoft Azure U.S. Hack for Acessibility on Devpost.

# What is Does
AI Dog helps a user find an accessible route from point A to point B on campus. We were inspired to make navigating more accessible after we learned first hand how difficult it is to get around campus with a leg injury.

# How it Works
AI Dog collects geo location data on campus using the Google Streetview API which we then pass to the Azure Computer Vision API to analyze the returned Google Streetview API images to determine if the location is accessible or not.

Some things we look for in the analyzed images may be sidewalks, crosswalks, ramps, lack of stairs, etc.

We store the results of our campus evaluation in an Azure Cosmos database for use in our web app.

The AI Dog interface is an accessible website where a user can easily find an accessible route to where they need to go on campus.

By choosing the campus they are on, and entering their current and destination location they will get accessible directions. Upon hitting the submit button a request is made to an Azure Function API we developed to analyze the info stored in our Azure Cosmos database and return an accessible route to the user.

# Suggested Search Data
Here are some suggested locations of 3 campuses that you can test with if you are not familiar with the campuses.

Georgia Tech
- 266 4th St NW, Atlanta, GA 30313 (Starbucks), 801 Atlantic Dr, Atlanta, GA 30332 (Institute for Robotics and Intelligent Machines)

Massachusets Institute of Technology
- 150 Nassau St, New York, NY 10038 (Brooklyn Chop House), City Hall Park, New York, NY 10007 (New York City Hall)

Pace University
- 190 Massachusetts Ave, Cambridge, MA 02139 (Flour Bakery), 405 Memorial Dr, Cambridge, MA 02139 (Pi Beta Phi)
