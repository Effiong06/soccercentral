***SOCCER CENTRAL***


***OVERVIEW***
_______________________________________________

Soccer Central is simply a site designed to provide users with imformation and stats regarding professional association football games. The user would input the match the want to learn about and they would be shown the stats regarding the teams and players involved

It is a basic website simply displaying information about the user's desired match and additional details. Unfortunately, as shown in the demo, issues with the API did not allow for the proper development of the website
  
 ***DEMO***
 ______________________________________________
 {A link to a demo video (explaining and displaying the contents of the website)} :- [https://drive.google.com/file/d/1Cw2H1KV_yT3OaqwVAqRbwfu8lV1cIBrA/view?usp=sharing](url)
 
 Open this link to access Soccer Central :- [https://www.ueff.tech/](url)
 
 ***TECHNOLOGY USED***
 ______________________________________________
 - Frontend :-
      -HTML: for structuring a webpage
      -CSS: for styling
      -JavaScripts: for page interactivity
- API Interactions :-
     - FootApi from [https://rapidapi.com/fluis.lacasse/api/footapi7](url)
- Deployment :-
    Deployed on nginx and haproxy for load balancing

***API INTERACTION***
______________________________________________
The application imports the latest data about to professional football matches and players. It will then display the requested match or player with  the necessary information pertaining to them.

API Documententation: via this link to access the documentation [https://rapidapi.com/fluis.lacasse/api/footapi7](url)

***LOCAL DEVELOPMENT SETUP***
_____________________________________________

 ***Step 1*** :- 
  Clone this repo: soccercentral .
   by: git clone [https://github.com/Effiong06/soccercentral.git](url)
   then move inside it by: cd soccercentral 
 ***Step 2*** :-
   OPEN THE PROJECT:
     You can open the index.html file in your browser as this is just a front-end application

***DEPLOYMENT***
_____________________________________________
***PREREQUISITES***

Two web servers :-
"Web-01" and "Web-02" (where nginx is installed, and I configured /etc/nginx/sites_available/default, I put my index.html file ( I opted to use only one file) that was used for this project, placed in the directory - /var/www/html - so that it can be accessed by visiting the IP_Address)
    
Load balancer :-
  Through "lb-01" (where "haproxy" is installed to distribute the requests through those two servers. And those were done through configuring an haproxy config file ( /etc/haproxy/haproxy.cfg ), So you can access it through linking up to the IP_address of this lb-01)
  
***The DOMAIN NAME***
The domain I used, was created from DotTech domain which I used to link up with the IP_Address so if you vist my domain you will get the same by visiting via IP_Address.
    
***SSL CERTIFICATE***
From lb-01 , I created a certificate using 'certbot', issued and signed by Letsencrypt.
    
***CHALLENGES and SOLUTIONS***
_______________________________________________

     Challenge: I could not connect to the API server .
     solution: Working on it lol

***CREDITS and ACKNOWLEDGEMENT***
_______________________________________________

API USED: FootAPI from RapidAPI :-
  [https://rapidapi.com/fluis.lacasse/api/footapi7](url)
Visit the link above for its documentation.
    
