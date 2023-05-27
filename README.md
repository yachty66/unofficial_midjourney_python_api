# unofficial_midjourney_python_api

## welcome to the unofficial midjourney api  💭🛳️🌅

follow the steps to make it run on your computer:

1. git clone https://github.com/yachty66/unofficial_midjourney_python_api.git

2. install requirements from requirements.txt

2. if you have a folder structure like and you want to use the api in a file called main.py:

```markdown 
project_directory
│   main.py
│
└───unofficial_midjourney_python_api
    │   midjourney_api.py
```

you need to import the api with:

`from unofficial_midjourney_python_api.midjourney_api import MidjourneyApi`

4. if you dont have a subscription to midjourney yet go and make one

5. in the same discord account where you described to midjourney create a new server (name doesnt matter) and add the midjourney bot from midjourney to this server

6. go to https://discord.com/developers/applications and create a new bot. 

7. go to oAuth2 - url generator and under permisson click bot and administrator in the checkboxes which show up after that. 

8. copy and paste the generated url in your browser and add the bot to the server you just created

9. Next you need to get all the information to call the api appropriately - prompt, application_id, guild_id, channel_id, version, id, authorization. 

10. go to your your discord server and open your developer console (on mac with fn+f12) and open the network tab. 

11. trigger the midjourney bot with the slash command `/imagine` and some arbitrary prompt and click after that click on the name `interactions`.  

12. first go the `Headers` tab and save the your `Authorization` key and than go to the `payload` window and save application_id, guild_id, channel_id, version, id, and authorizatio from the json. 

13. create a folder called `images`in the root of the project (the image created by the api will land there)

13. call the api as following `midjourney = MidjourneyApi(prompt="Yoda", application_id="application_id", guild_id="guild_id", channel_id="channel_id", version="version", id="id", authorization="authorization")`



## Example projects which are build with the api 

https://twitter.com/celebritydiff 

DM me your project at https://twitter.com/MaxHager66