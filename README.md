# Personal Blog Web

https://serene-everglades-37897.herokuapp.com/
## CSS
The css frame work is the part I most like because use bootstrap it's so easy to get the beautiful layout.
One problem is because the footer position is absoulte
so if I make the class card has the margin-left and margin-right
the footer will move to right and left side has lots of white space
so the class can not have the margin-left and margin-right

One tips i found out is if we want a space between the two class
we can add one calss that has property like margin top: 5 % and we can reuse this div class in lots of place.
such as give some white space between 2 col
![personalb2](https://user-images.githubusercontent.com/79159894/186612811-918ce150-6ea4-4e9d-b99d-1d43f0fba9b8.png)


## Connect with MongoDB and Heroku

This project took me 72 hours no sleep to complete. The part of ejs code and css just took one day and last 2 day all spend on connect with mongoDB and heroku.
I build a full stack project before, name to-do list web, so I know how to connect to mongodb.
I did this before and it connect with mongodb successfully.

go to the project file and 
mongo "mongodb+srv://cluster0.jnxzx3s.mongodb.net/blogDB" --apiVersion 1 --username 123

but it appear error that say mongo shall has been superseded by mongosh.
But I am confused mongo shall and mongsoh isn't they are the same thing? And the solution told me that they are not same thing and mogo will be replace by mongosh.

![mongodb](https://user-images.githubusercontent.com/79159894/186591806-7477a78b-e051-4de3-a521-45cd9b9b91d5.png)

So the solution of this problem is 
1. downolad the mongosh from mongodb web
2. move the mongosh to mongodb bin file
3. enter the connection string : 27017

![image](https://user-images.githubusercontent.com/79159894/186603301-b1ae124f-1552-476d-8ecf-5f1a065e7424.png)
3. Then use the same command in the blog file
![image](https://user-images.githubusercontent.com/79159894/186603786-4f441ffc-1d91-4ccf-827a-19888d2f7297.png)
mongosh "mongodb+srv://cluster0.jnxzx3s.mongodb.net/blogDB" --apiVersion 1 --username 123

then we can successfully connected with mongodb!


After that, we can start connect with heroku application to let the website release at the internet.
At the project file
1. git init
2. git add * (start add numerous node module files)
3. git commit -m "first initial"
4. heroku login (the login web pop out)
5. heroku create
6. touch Procfile
7. modify Procfile by vs code
![image](https://user-images.githubusercontent.com/79159894/186606063-b5fbfbbd-3b35-42d4-959a-9c2e3b726301.png)


9. node --version(check node version and modify json file node version)
10. git add *
11. git commit -m "update"
![image](https://user-images.githubusercontent.com/79159894/186606276-4996f1d3-a9b1-4717-bd4a-1b85e5c562ba.png)

13. git push heroku master
14. Then web been deploy on the heroku app
![image](https://user-images.githubusercontent.com/79159894/186608379-7f59922a-c86f-4cd5-b776-44081e3c54cf.png)


## Update the heroku app
If we modify the code we need to update the heroku, and the process be lik
1. git add * 
2. git commit -m "update"
3. git push heroku
4. done update


And because I add the my blog proget in the github respositary
So i need to update the repositary, but I encounter some probelem that first I push the project to master but now I want project been push to main
so I need to
git fetch orign
git merge origin main
otherwise it will appear error said fail to push some refer to https://github.com/52147/<repository name>/git.
![image](https://user-images.githubusercontent.com/79159894/186609145-fdb72c7c-95f3-47e6-b013-0122edfaf214.png)

