[Back to home](index.md)
[Back to projects](projects.md)

# Narratives covered on this page

[Narrative One](#artifact-one-narrative) for the initial enhancements for [CS340-Portfolio-Project-Enhanced](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project-Enhanced)
[Narrative Two](#artifact-two-narrative) for the next step enhancements for [CS340-Portfolio-Project-Enhanced](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project-Enhanced)
[Narrative Three](#artifact-three-narrative) for the thought process behind the creation of [CS-340-Portfolio-Project-Flask-Fork](https://github.com/MadelineJMeyers/CS-340-Portfolio-Project-Flask-Fork)

# Artifact One Narrative

For the enhancements made for category one of the project started in CS 340: Client/Server Development I have taken several steps to move further with a better design and security development for the program.

Originally the only security was set for the CRUD module attached to main file which is used to access the MongoDB database. In this enhancement I have added a basic user authentication which requires the user to enter a username and password to view the dashboard which restricts access to the information in the dashboard until these credentials are entered by the user. I also have taken steps to create more meaningful comments throughout the code to make it easier to develop the code and to understand what each part is for and the reasoning behind these parts. I have also created a download button for the user so they may create a copy of the data if needed. The final enhancement I want to mention in this narrative is the addition of a “dark mode” for the client which darkens the majority of the screen which can make it easier on some users eyes.


# Artifact Two Narrative

The artifact for this category is the dashboard application that was created during CS 340: Client/Server development because to create custom filter options I would need to work to create an algorithm to search a MongoDB database. While I originally created the algorithm to search for specific rescue types I thought it would be helpful to potential clients to also be able to search for specific animal types such as dogs and cats and then to search for specifically younger animals in these categories. So, I created four new search options available in the dropdown to find these types of animals. The algorithm that was created uses not only multiple logical operators to find the animals that fit certain criteria but also includes a logical “or” operator to find animals of different genders without needing to create specific filter options for different genders which reduces the number of potential options by half as many as could have been created.

The skills the creation of these new options shows are the ability to create innovative solutions that use the technology that I am working with to display relevant information to clients and the flexibility of the code if new options need to be created going forward. The code also does not allow for a user to specify any custom input which reduces the amount of potential security flaws by not allowing the user to directly access the database, instead relying on the dashboard to interact with the information in the database.

To aid with the retrieval of information for the dashboard I created two compound indexes which were formatted based on Equality, Sort, and Range guidelines as stated in the MongoDB documentation. These are shown in the following image to show how they were set with each index following the format of the equality index, the sort index, and the range index. The second compound index uses two equality indexes due to the length of the algorithm created in VS Code and what fields were used to create the filters. The creation of these indexes show my skill when it comes to understanding the database that is being used for this project and what can be done on the backend to increase the response time of the resulting searches.
 
<img width="975" height="595" alt="image" src="https://github.com/user-attachments/assets/9ca24302-fd9b-4295-b835-166f45df3b05" />


# Artifact Three Narrative

For this artifact I have chosen a program that was created in CS340: Client Server Development and I have chosen to enhance this project through the method of redeveloping the program using a new framework. The original project was created using MongoDB, Python, Plotly Dash, and Jupyter Notebook to run the program. This enhancement instead uses MongoDB, React.js, Flask, Node.js, and Plotly graphs to create a more scalable version of the program that allows for more modularization of the code and its components. The resulting application is a web dashboard app which shows a breakdown of several metrics while allowing the user to search for specific animals for certain goals. The skills I have shown through this enhancement is my skill to learn new web development frameworks including a new frontend through React.js and a new backend through Flask while also using some familiar technologies such as MongoDB and Plotly’s graphs to visualize information from MongoDB. This aligns with not only the outcome of demonstrating my ability to use well-founded and innovative technologies to create solutions with the goal of delivering value but also the outcome of designing and delivering professional quality communications.
