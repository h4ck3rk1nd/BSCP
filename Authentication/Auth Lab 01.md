#### The page appears to be a blog post site:
![image](https://github.com/user-attachments/assets/c74afe74-c1e1-4ee3-81cb-472463eb32bf)

#### At the top right corner of the site, there's a my account section:
![image](https://github.com/user-attachments/assets/3d785d3b-b134-4e9e-aceb-5309b8e677f3)

#### On visiting the _My account_ section, it greets with a login page as:
![image](https://github.com/user-attachments/assets/7cd0c7c9-7f66-4bb6-a61a-155a2c3bb85b)

#### Try to enter any random username and password, to see the response of the site as:
![image](https://github.com/user-attachments/assets/0cd442f0-ba41-4ef4-b9a9-29cca5b34697)

#### Upon entering the credentials hit the _Log in_ button to see the reaction of the site as:
![image](https://github.com/user-attachments/assets/413db14e-dad3-42fb-9638-a01513c55d2b)

#### It can be seen that even though the credentials were wrong, yet the site only responded for the wrong uername.
#### This simply means that the username can be enumerated.
#### Fire up Burp Suite and Intercept the Login request from the site as:
![image](https://github.com/user-attachments/assets/3471fc4e-9860-43c0-96cb-46d336b5f03c)

#### Next send this request to Intruder tab for enumerating the username as:
![image](https://github.com/user-attachments/assets/a98511ed-3ccb-4ff1-a314-c00e101d3ce2)

#### Configure the payload to run the brute force for the username placeholder as:
![image](https://github.com/user-attachments/assets/8f437aa8-7396-44a3-be3f-9add224a6dbd)

#### Select the _Sniper attack_ as the attack and under the Payloads section select the _Simple list_ and from the given username list copy and paste the usernames, to enumerate the same.
#### Once the payload has been configured, hit the _Start attack_ button at the top as:
![image](https://github.com/user-attachments/assets/12d9e13e-c04d-4c62-905d-00d90d9050a1)

#### It should start the attack, notice the response length to see a different response length, meaning it should show this time for the _Invalid Password_ as:
![image](https://github.com/user-attachments/assets/491c7ff1-52a9-470e-96af-7c424eb20361)

#### It did show for the username: _adam_ that the password was invalid, stop the attack and now configure the same payload with the password list to run against the username: _adam_ as:
![image](https://github.com/user-attachments/assets/6c90825a-5831-47b2-9fca-ecdbdb158f5d)

#### Once the payload has been configured, hit the _Start attack_ button to start the brute-force attack against the username:_adam_ as:
![image](https://github.com/user-attachments/assets/8f21a8e4-b98e-489c-b822-536ab25acc87)

#### At the password:_pass_ it gives a redirect, meaning the credential combination is correct.
#### Try to login using the same credentials as:
![image](https://github.com/user-attachments/assets/e6262005-636a-4507-b904-4b2ec3711dd6)

![image](https://github.com/user-attachments/assets/3c3824ee-03f3-4628-95e5-de2167bcf5d3)

#### The user _adam_ is hacked with kindness !!!

