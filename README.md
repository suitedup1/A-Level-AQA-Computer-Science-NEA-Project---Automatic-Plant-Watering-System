# A-Level-AQA-Computer-Science-NEA-Project---Automatic-Plant-Watering-System

Problem Statement
People who want to get into gardening or botany may struggle with remembering when to water their plants, knowing how much water the plants need and dealing with taking care of their plants for an extended period of time.
The way this can be solved is with an automatic plant growth management system.
It does this via data collection with sensors [humidity, moisture sensors etc.] connected to a Raspberry PI. The sensors and pump will interact with the Raspberry Pi’s GPIO [General Purpose Input/Output] pins. This data is stored and interpreted by an algorithm and at the user’s discretion either automatically keeps the plant hydrated [small-sized pumps that are controlled by the system] or simply reminds them to do it themselves. It also will have an interface that presents data on weather conditions like humidity, wind speed, temperature, and anything else that the plant requires. The user will be able to select from a range of plants that may require different optimal growth conditions.

1. Educate and guide the user on taking care of their plant
  Store a source of information to be displayed to the user at appropriate times
  Display basic guidance on plant watering upon setting up a plant
  Include multiple plant profiles for the user to create
  Warn the user if they are placing the plant in suboptimal conditions
2. Be able to water the plant without user intervention if preferred
  A function triggered upon initially a basic water threshold  or a more sophisticated algorithm
  Use a motor driver to switch on the pump when necessary
  Be able to run completely autonomously if desired
3. Log sensor and actuator data on the Raspberry Pi
  Input data periodically through GPIO input pins
  Store in an SQLite based file
  Communicate this data effectively with the client side device
4. Display environment data in a clear format
  Use an appropriate python GUI to present the data to the user
  Link this with the plant profile
  Include comments on trends
5. A rule based decision-making algorithm implemented 
  Receive the data input from the sensors
  Push these into a function that outputs a score
  Use this score to make a decision on what to do for the plant and store it as well
