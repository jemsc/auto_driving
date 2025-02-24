# auto_driving

improvements made:
1. Preventing duplicate names for car. 
2. Preventing entry of car position on existing car positions. 
3. Preventing entry of car position out of field bounds
4. lowercase is accepted for direction & commands. 
5. Simulation is able to detect the collision of a third car onto collisions that have already happened. 
6. Simulation results displays collision report and final position & status of all cars. 

    ## Example Usage with Collision

    1. Start the program:
        ```
        Welcome to Auto Driving Car Simulation!
        ```

    2. Enter the field dimensions:
        ```
        Please enter the width and height of the simulation field in x y format: 5 5
        ```

    3. Add the first car:
        ```
        Please choose from the following options:
        [1] Add a car to field
        [2] Run simulation
        1
        Please enter the name of the car: Car1
        Please enter initial position of car Car1 in x y Direction format: 1 2 N
        Enter commands (L, R, F only): LFLFLFLFF
        ```

    4. Add the second car:
        ```
        Please choose from the following options:
        [1] Add a car to field
        [2] Run simulation
        1
        Please enter the name of the car: Car2
        Please enter initial position of car Car2 in x y Direction format: 1 3 N
        Enter commands (L, R, F only): F
        ```

    5. Add the third car:
        ```
        Please choose from the following options:
        [1] Add a car to field
        [2] Run simulation
        1
        Please enter the name of the car: Car3
        Please enter initial position of car Car3 in x y Direction format: 3 3 E
        Enter commands (L, R, F only): FFRFFRFRRF
        ```

    6. Run the simulation:
        ```
        Please choose from the following options:
        [1] Add a car to field
        [2] Run simulation
        2
        ```

    7. View the results:
        ```
        Your current list of cars are:
        - Car1, (1,2) N, LFLFLFLFFF
        - Car2, (1,3) N, F
        - Car3, (3,3) E, FFRFFRFRRF

        After simulation, the result is:
        - Car1, collides with Car2 at (1, 3) at step 10
        - Car1, (1,3) N (collided)
        - Car2, (1,3) N (collided)
        - Car3, (5,1) E
        ```

    8. Choose to start over or exit:
        ```
        Please choose from the following options:
        [1] Start over
        [2] Exit
        ```
