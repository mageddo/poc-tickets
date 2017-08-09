Tickets is a Prove Of Concept to test a system architecture to solve the problem of a tickets system.

### Project brief
 
The tickets system 
it's a website where the stackholder can access to reserve your ticket to watch a movie, baseball or football match.


### Project features

* Stackholder access the site, choose the wanted room to watch your prefered movie
* At the choose screen he can see seats:
	* In reserve pogress (Silver)
	* Free (Green)
	* Occuped (Red)
* He can choose only the **Free** seats
* When choose a seat then will be redirected to the confirmation and payment screen
	* The payment details will be asked, the system will thank the user and the payment process will occour in background
	* When the payment process complete then the user will be notified the success or error and the seat will be **Occuped** or **Freed** 

### Project issues to be solved
* The seats screen access is very high
* The system primarly uses a relational database and the simultaneos access are more than the database server capacity and
	* Increase the database server capacity is not a option
* The transactional (payment part) and the seats status must to be in relational database 

So the question is:

How to make this system capable of process all this access keeping the 
**ACID** (Atomicity, Consistency, Isolation, Durability) data in relational database ?

# System proposed architecture (at the moment)
![](https://lh3.googleusercontent.com/wuHwn_g_U3aGKSu3MVvw7unh_Pl8shEHOzaZ-BBYRV23mS-dujzT_BFfgTSIO1QvE48nmN3u1wceMSI7-jS_eBUPErQSTkrzAwSuMNrk1cJTsPmhwD0UiE3nlRlWN7bDQpoWZTGvDqk=w1240-h766-no) 