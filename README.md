# exercise-1-modularity-rashmi2383
exercise-1-modularity-rashmi2383 created by GitHub Classroom

Required Python/3.6.0 or up

To run:
$python main_app.py

Main_app integrates all the modules and works as expected.

For Exercise-1, which tackles aysnchronous APIs in the modules, our architecture employs a queue based approach. The system takes input from the sensors and queues them up. Which provides data to the real time data processor for further processing. And once the data is processed, it is given to the display unit for displaying various statistics to the user. It also stores the data to the database with the current date and timestamp so that whenever further analysis needs to be done, at that point in time, the data is readily available.

We used queue based approach which has its own advantages and dis-advantages. 

Advantages:
Using queues, we figuered out that it was easier to write code. We restricted the memory usage to a fix number of queue size and hence we could save memory space. If we wanted we could have even set up the priorities of the task like which values to process first, using queue. 

Disadvantages:
The challenges we faced using queue was that we have to take care of underflow and overflow situations. If the queue is empty, the data processor starves and if the queue is full then we end up loosing lot of sensitive data.

We could have explored the option of using callback functions which was event driven and could have been more useful. 
