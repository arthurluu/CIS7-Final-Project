# CIS7-Final-Project
Spring 23 final project
Documentation (Eric, Joseph, Arthur):

This program was designed and created to calculate the different travel options for a sales team from four different cities. In the program, it will calculate and display different route options based on user selection. Depending on the options the user selects, the program will calculate and display different routes, alternative paths, and/or the cheapest roundtrip route in order let the user travel efficiently. In our program, it solves the problem of determining optimal travel routes for the sales team (the user) and ensures that the sales team makes informed decisions in order to maximize their travel efficiency. The program utilizes various functions to achieve desired output. The program also implements a switch case based menu in order to obtain desired user output based on what the user selects. There are three different “main” functions where we store user choices, calculate route destinations, and calculate the shortest route. The calculations in this program mainly involve determining the shortest and cheapest route in order to maximize travel efficiency. We also implemented a struct for adjacent cities that serves as a data structure for holding the variables and is used to calculate different travel options. The current limitations of the program is that it may not easily be adaptable to accommodate additional cities. To improve the program we could have added an adjacency matrix in order to handle dynamic changes in cities and routes. If were to scale the program up, I think we would add additional functionality to where the user is allowed to input custom routes or integrate “real-time” traffic information to see which route is most efficient.


Psuedocode Rough Draft
// Struct to hold adjacent cities
struct AdjacentCities
    int city, adj1, adj2, adj3

// Function to display user choices
void UserChoices()
    Display main menu choices

// Function to display route destinations
void RouteDestinations()
    Display destination cities

// Function to display the shortest route
void ShortestRoute()
    Display the shortest and cheapest route

// Function for choice 1: Route Choices
void Choice1()
    Display a list of possible routes

// Function for choice 2: Adjacent Roads
void Choice2()
    Display a list of adjacent roads

// Function for choice 3: Cheapest Roundtrip Route
void Choice3()
    Call ShortestRoute() function

// Function for choice 4: Distance Between Cities
void Choice4()
    Calculate and display distance between cities

// Main function
int main()
    Display welcome message “Welcome to Sleepy Joe’s Solar Sales GPS :”
    Call RouteDestinations() function
    Display main menu
    Read user input

    WHILE Loop until user chooses to turn off GPS
        If user chooses option 1
            Call Choice1() function to list possible routes the user may take
        Else if user chooses option 2
            Call Choice2() function to list adjacent roads
        Else if user chooses option 3
            Call Choice3() function to find the cheapest roundtrip route
        Else if user chooses option 4
            Call Choice4() function to find the distance between cities
        Else if user chooses option 5
            Display GPS off message
            Exit the program
        Else
            Display error message “Error. Please select from the 4 options or Turn off GPS,” for invalid input
	  End WHILE LOOP if n != 5

    Exit Program

