# CS-230_Operating_Platforms
Summary-
The client for this project was The Gaming Room. A company looking to evolve their existing mobile app,"Draw It or Lose It" into a more accessible web based platform. The main requirements were to transition the game from a device mobile app to a distributed, multi platform system that functions on any modern web browser. The software needed to support multiple teams and players while being sure the data's consistency through a central backend server. 

WHAT DID YOU DO PARTICULARLY WELL IN DEVELOPING THIS DOCUMENT?
I believe I excelled at defining the domain model and structure that was object oriented. I clearly outlined the inheritance relationship between the base Entity class and its subclasses like Game,Team, and Player. I created a "blueprint" that keeps consistent IDs across the system. This helps ensure that any dev joining this system would understand the hierarchy and how data flows throughout this app. 

 WHAT ABOUT THE PROCESS OF WORKING through a design document did you find helpful when developing the code?
 The design process is always essential when identifying logic conflicts before writing even one line of code. EX: Realizing the need for the signleton pattern for GameService was crucial. It helped me understand that a central "Home Base" was necessary to manage different instances and ID counters in one memore location. This will prevent different players from seeing different data. 

 If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
 If i were to revise a section, I would expand the Sysem Architecture View. While the main focus is on the logical domain model, adding a detailed diagram that shows how the Linux server would interact with the clients using TCP/IP would provide a more complete picture of the networks infrastructure. 

 How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?
 The user's primary need is / was a consistent experience no matter the device used. I chose Java for the backend as its a write and run anywhere. This allows the system to keep stable across different server ENV's. Also, considering user needs is important because it dictates the technical constraints. If we don't prioritize the user's need for that "live" feeling, we might not haave a need to implement the iterator pattern to prevent duplicate team names, which would lead to a confusing and broken user experience and UI.

 How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?
 My approach focused on the OOP principles. By using a parent Entity class to reduce repetitive code shows inheritance. We used encapsulation by protecting data by marking attributes as private and using public getters. This prevents accidental changes by other parts of the program. Also, utilizing singltons for service management and iterators for list davigation show design patterns. 
 
In the future I would use and pay more attention to UML Diagrams to visualize any complex relationships and use security by design and ensuring encryption and roles based access are baked into the architecture from day one. 
