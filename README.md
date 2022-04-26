# How to use Heroku for deploying Your Site
An application for deploying your local project .
`````javascript
`````

## Global for one computer one time.
- - 
* Open a heorku account in the heroku application
* You will get a verification mail in your PC confirm it and log in with that password.
* Download the heroku as per the features of your pc.
* Export the app in your local PC
* Download node in your PC
* Download git in your PC
* Now open the command line with the project you want to deploy the heroku.
* Run heroku log in command and your browser will open the log in page of the heroku app.


## For one time 
- - 
* run [heroku create]
* Make sure you have commited all the last changes of your projects.
* And finally run [git push heroku main]

* Now go to your project in the heroku and open settings on the project and press to reveal-config button

* Copy paste all the key and value from your .env file to heroku key and value line.

* Check the mongodb server that all the ip address connection is ok or not if not make it for all the ip address.
* Now check your heroku URL with your service your want from mongoserver.



## Error  in Heroku
- - 
 __error code=H13 desc="Connection closed without response" method=GET path="/service" host=safe-plateau-81677.herokuapp.com request_id=8433286e-7f1e-49e6-9f79-ccc0b9c66530 fwd="119.157.102.26" dyno=web.1 connect=0ms service=7ms status=503 bytes=0 protocol=https
2022-04-26T10:08:58.502660+00:00 heroku[web.1]: Process exited with status 1
2022-04-26T10:09:28.822277+00:00 heroku[web.1]: State changed from up to crashed :question:__

## Solution
- - 
__:v:__

Check your index.js remove the client.close() line from the code


