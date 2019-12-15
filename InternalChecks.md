#Internal Checks

## Purpose
This file documents the internal checks that occur within the code of the population model project in order to ensure that it functions correctly.

##User Inputs
Within this model the user is asked to input values for six variables:

            * num_of_sheep 
            * num_of_wolves 
            * neighbourhood 
            * num_of_iterations 
            * wolf_threshold 
            * sheep_threshold 
            
These variables MUST be positive integers for the program to function correctly. This data is validated internally via a try/except error capturing structure. In the event one of these variables is found not be a positive integer a message box is displayed asking the user to reenter these values.         
