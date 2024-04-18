# Programming Principles
## Software Development Life-Cycle (SDLC)
The SDLC of Help Ticketing System goes through multiple key stages, which are very important for the success of the system.  

The project team will be able to identify the requirements and resources that the system needs during the Planning Phase. This involves harnessing the views of stakeholders such as help desk personnel and users of the system to find out what they actually require and expect (Pressman, 2005). Furthermore, the team estimates the budget, timeline, and the hazards connected with the project. The team sets up a structured plan which is the basis for a functional development process.

The Analysis Stage involves the analysis of the ticketing system on the help desk in order to identify the loads of the system. It regards the knowledge of the ticket creation, resolution and response process within the system, and understanding other functionalities that may be needed to fulfill the users' requirements. The group will receive very detailed information about the system's specifications during the analysis phase, and this will serve as a basis for the following design phase.

At the Design Phase, the design and planning will be made for the program. This comprises of the design of the data structures and algorithms involved in creation, resolution, and response of tickets. Furthermore, the group builds the user interface such that it can be easily navigated by the users. The team takes the first step in designing the system by carefully preparing the system's structure and functioning.

In the implementation phase, the program is coded and tested for debugging. The programmers use Python as the programming language; they turn the design specifications into actual code. During the whole coding process, fault detection is carried out in order to eliminate existing bugs and mistakes (Sommerville, 2016). Through this iterative process, it becomes possible to make the necessary adjustments for the software to operate precisely and effectively.

In Testing Phase, the entire system is put through stringent testing to verify that it satisfies the predefined needs and acts as it is supposed to. This involves both integration and non-functional testing that include unit testing, integration testing, and user acceptance testing. The testing process is always aimed to uncover any discrepancies and problems that are then eliminated, thus making the system quality and reliable.

The application shall be deployed and made accessible to users who are seeking help in the ticketing system. This is done by deploying the software on suitable servers or cloud platforms and tuning the performance settings for maximum success. In addition, the training of the users might be included in order to make sure that they know how to use the system and are able to benefit from the features it provides.

Ultimately, the Maintenance Phase takes the form of continuous support and maintenance operations. This incorporates, but not limited to, the spark of upgrading the software to fix any bugs or security flaws, and also implementing new functionalities or enhancements based on the feedback we receive from our users. Similarly, the help desk team offers technical support to users and resolves all the issues that may arise when putting to operation. The team actively monitors the software for potential glitches and updates that may impact its proper usage. This helps the software to remain operational and relevant to the users.

All along the development cycle, the communication and collaboration among the team members is the key element that need to be done well. The project is kept on track and its objectives are met through constant review and check up points. Through applying a disciplined and planned method to software development, the help desk ticketing system can be rightly built, used, and managed to help users and organizations at large.



# Analytical Comments
The following Python script creates a Ticket System in which users can create tickets, reponse to tickets, reopen closed tickets, and view ticket statistics. Let's provide an analytical commentary on the different components of the script:

1. **TicketData Class**:
- This class, therefore, is a blueprint for a ticket object. It has components, such as the creator name, staff ID, email, description, ticket response, status, and ticket ID.

- It also comprises of attributes that are at the class level i.e. default_response, default_status, starting_number, total_ticket, open_tickets and tickets list.

- Constructor is called with ticket object that has already provided attributes while response and status are assigned default values. In addition, it also manages ticket numbering system and ticket counters at the same time.

- The `show_ticket_statistics()`is a static method to show the ticket statistics for example total tickets created, resolved and open.


2. **Functions for Ticket Operations**:
- `create_ticket()`: Instructs the user to enter ticket information and initializes a new ticket object which will be added to ticket records and counters.

- `reopen_ticket()`: Permits reopening of the ticket by changing the status to "Reopen" if the ticket number matches a closed ticket.</p

- `respond_to_ticket()`: Deals with resolving the issue that a customer has raised via a ticket. If the ticket title is a "password change", it will automatically create a response and will be closed as well. It does so by default, unless a response is provided by the user.

- `display_all_tickets()`: Displays the tickets stored in the system as well.

- `display_ticket_details()`: Shows ticket particulars related to a specific ticket number provided by a user.

- `display_ticket_stats()`: Invokes `show_ticket_statistics()` method to present the ticket statistics.

- `end_program()`: This is to ensure that they know how to exit the program.


3. **Main Functionality**:
- The `main()` function is the starting point and user will be issuing commands from the command line interface which will be like a menu.

- It is a feature, which forces the user to pick up any option until they decide to leave.


4. **Modularity**:
- The script implements simple modularity in that it puts different functions into functions. However, this can be overcome by implementing more modularization which will lead to better readability and maintenance.



# Algorithm/Pseudo Code
1. Start

2. Class TicketData is set up to store ticket data and have methods allowing access to and changes in ticket details.

3. The class contains values for the default ticket status and response and keeps the number of tickets in check as well.

4. The constructor method is used to initialize the values of each object of ticket.

5. Static method, show_ticket_statistics(), is intended to show ticket statistics.

6. The other six ways to raise the ticket are defined : ‘creating a ticket’, ‘reopening a ticket’, ‘responding to a ticket’, ‘displaying all tickets’, ‘displaying ticket details’ and ’displaying ticket statistics.

7. A method for resolving password change requests is added to the Ticket class: 

        i. If the ticket description is "password change": 

        ii. Generate a new password

        iii. The response to the ticket should be as follow: new password

        iv. Update the ticket status to closed

8. The main() function provides an interface where the user can perform operations in the Help-desk Ticket System such as selecting options from a menu.

9. The program ends at the point where the user decides to terminate the system by entering 7 as an option.

10. Stop
