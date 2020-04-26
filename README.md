# s14-mp9, Locker Logbook
## Team Members:
* Lapan, Jessamyn Kristi
* Chen, Ysabelle Chloe Tan


**Heroku Link**: https://stormy-caverns-88085.herokuapp.com/home
# How to Use This Web Application

## Setting Up the Application
Before actually using the application, the user is required to do the following:
1. Install NPM/Node Packaging Manager and its Frameworks
2. Install Database Tools.
3. Add certain data to MongoDB Atlas

### Install NPM/Node Packaging Manager and its Framework
1. Access the directory of the application by
Using this command on cmd or git-bash.
```
cd ___________
```

or


Directly entering cmd on the File Explorer folder of your directory.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/cmd.png)

2. Initialize NPM.
```
npm init
```

You can enter without modifying values as you install until you reach this question:
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/cmd3.png)

Type in "yes", and your packages are installed.

3. The following should be installed:
    * express
    * express-session
    * http
    * body-parser
    * cookie-parser
    * mongoose
    * mongodb
    * path
    * handlebars
    * express-handlebars
    * express-validators
    * bcrypt
    * url
    * bootstrap
    * connect-flash

The format to install the frameworks in cmd or git-bash:
```
npm install _____
```

Example:
```
npm install express
```

### Installing Database Tools
1. Install Robo 3T through this link: https://robomongo.org/download
2. Log in or register an acccount for MongoDB Atlas
3. Create an account for your MongoDB Atlas project
4. Connect Robo 3T with MongoDB Atlas

**Create a new project in MongoDB Atlas.**
Of course, name your project.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas.png)

Then add your groupmates' addresses to the MongoDB Atlas Project
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas2.png)

**Create a new cluster in MongoDB Atlas.**
Click on the 'Build a Cluster' button.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas3.png)

Choose the free Shared Clusters
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas4.png)

Choose a region to host your cluster, or don't do anything at all.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas5.png)

Wait for the cluster to be fully created.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/atlas6.png)

**Connect to the cluster**
Connect to the cluster
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/connect.png)

Connect to your application. In this case, Robo3T
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/connect2.png)

Copy the link of the connection string, and then replace the "<password>" segment with your own. 
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/connect3.png)

**Create or use an existing connection in Robo 3T.**
Set type to Replica Set.
Name the database anything.
Paste the link to the From SRV text field below, and then click the From SRV button. The clusters will then show up.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/robo.png)

Check personal authentication.
Databse should be named "admin"
Enter your Database username and password.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/robo2.png)

Authentication Method is "Use CA Certificate"
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/robo3.png)

## Using and Exploring the Application
After initializing the necessary tools to run the application, you can now use the application itself. 

### User Mode
The typical person using the application. Only has control of viewing, reserving, and abandoning a locker and viewing and editing their profile.

### Login and Register
For the users' conveniency, both the log in and register features are in the same page. 

Login
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web1.png)
The login page can now check for incorrect passwords or nonexistent accounts.


Register
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web2.png)
Registration can now check if the user missed some forms or typed in a password with less than 6 characters.

#### Home
The main page of the logged in user.

User Home
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web3.png)

#### View Current Locker
This page is a quick view of the user's current locker, whether reserved, owned, or abandoned. The user can also cancel their reservation or abandon their locker.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web4.png)

If the user does not own a locker, the user is given a quick button to the View Lockers page to find a locker to reserve.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web17.png)

Otherwise, the current locker of the user and its details like its locker code and address are shown.

#### View Lockers and Reserve One
The user can view a catalog of lockers from a selected location to seek one to reserve. 
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web5.png)

Unless already reserved, owned, or the user already owns/reserves/abandons a locker, the user can reserve a locker in a location of their choice. 

After reserving the locker, the user either had the option to reserve or cancel the reservation. 
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web18.png)

#### Search Lockers
The search function for the lockers can now perform advanced search function, alongside the locker number and location only search functions.

Location Results
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web7.png)

Locker Results
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web8.png)

Advanced Search Results
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web33.png)
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web31.png)
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web32.png)

#### Profile
The profile shows the credentials of the user such as their full name, ID number, degree program, e-mail address, and mobile number. 
Everything except for the ID number can be edited in Edit Profile. The profile pages also shows the user's locker and other way to cancel a reservation or abandon a locker.

Profile
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web9.png)

Edit Profile
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web10.png)

### Admin Mode
The admin has the control on locker management. Not only they can add, edit, and delete lockers, but also set the start and end dates for locker reservation. The admin is the very first user registered in the application, as previously demonstrated.
The admin may be a user, but unlike a regular one, the admin does not have a profile of their own. However, they cannot meddle with reserved or occupied lockers.

#### Managing lockers
The admin can do the following when managing lockers:
1. Add Locker
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web19.png)
The locker code should either have 3 or 4 digits, going with the number of digits a real life padlock has.

2. Delete A Locker
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web26.png)
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web27.png)
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web28.png)

3. Editing A Locker by clicking directly on it
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web24.png)

4. Adding New Locations
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web22.png)

5. Deletng Locations
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web23.png)
Only locations without any reserved, owned, or abandoned lockers may be deleted.

6. Setting the Term Dates to mark the span allowed to reserve a locker.
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web25.png)
Although actually deleting the reservations and ownerships during a specific does not work now, thisr reminds the user the span of the reservation or ownership period.

Locker Manager
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web13.png)

Date Manager
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web14.png)

#### Managing Pending Locker Reservations
This page shows users' reservation and abandonment requests and views all the currently owned lockers. To organize the tables more neatly, two dividers for the tables of reserved lockers and owned and abandoned lockers. The reservation table is separated from the owned and abandoned tables, which are grouped together.

Two buttons for accepting and rejecting requests are in the reservation and abandonment tables.

Reserved Locker Requests
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web15.png)
Picks reservations to accept or reject.

View Owned Lockers and Abandon Locker Requests
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web16.png)
Shows all the currently owned lockers. Also picks abandoment requests to accept or reject.


### Others
#### About Page
Shows the NPM packages and other tools such as database applications. Also lists a few details about the machine project group
![alt-text](https://github.com/unisse-courses/s14-mp9/blob/master/readme-images/web30.png)
