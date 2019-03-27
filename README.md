Task 1

1.	Download and install docker.
2.	Run command ‘ docker run jboss/keycloak’ on cmd 
3.	 Open Kitematic.exe
4.	Select running Keycloak container
5.	Go to settings and click General Tab
6.	Add a user name for KEY_CLOAK user 
7.	Add a password for KEY_CLOAK user
8.	Now click Hostname/Ports tab
9.	Add 8080 as a port ahead of ip ‘192.168.99.100’
10.	Access KeyCloak by URL ‘192.168.99.100 :8080’ by using the username and password set at steps 6 and 7.
11.	Create a realm using Name as ‘TestProjectKeyCloak’
12.	Create a Client  with id ‘test-app’ and set Valid redirect URI ‘http://localhost :8080’
13.	Create a role with name ‘user’
14.	Create a user with name ‘user1’. Set credentials of user to ‘password’. Go to role mapping TAB and map ‘user’ role to the user 
15.	Run spring application and access a url ‘http://localhost :8080/getSecuredProjects’
16.	You will be prompted to give username and password. Add the credentials username = user1, password = password (the user created on keycloak)
17.	You will see the predefined Projects in db.


TASK 2
1.	A page is also created on  Angular 6 which shows lists of project by calling api from spring boot. 
(So you need the spring project running on localhost :8080 and also peroform the keycloak setup explained in Task1)
2.	After running angular app (use npm install and the ng serve to run the app )you will see list of projects and above it . Asumming that you do have angular setup with you. if not then take this as refference https://angular.io/guide/quickstart
