#### The page appears to be a blog site:
![image](https://github.com/user-attachments/assets/ee3018be-aabd-4d95-9a91-364cb4580f89)

#### At the top right corner, there's _My account_ section:
![image](https://github.com/user-attachments/assets/88226f5c-8d05-442f-ba44-13eaa52a58cf)

#### Heading over to the _My account_ page, the page greets with a _Login_ page as:
![image](https://github.com/user-attachments/assets/7b593912-eee8-4ad3-b6d6-1239dcd6d013)

#### As per the lab, it can be assumed that, the user _wiener_ can be successfully logged in, and so can the user _carlos_, the issue is that we do not have access to the _carlos's_ 2FA verification code.
#### We can log in via _wiener's_ account, let's log in via the user _wiener's_ credentials:
![image](https://github.com/user-attachments/assets/6fab3ac7-65bf-4f13-ae80-8f1fd60e6ac4)

#### Once we hit the _Log in_ button, we are prompted to enter the 4-digit verification code as:
![image](https://github.com/user-attachments/assets/83082903-5704-4ecb-adaf-f378add617ec)

#### Let's access the Email of the user _wiener_ and try to enter the 4 digit verification code as:
![image](https://github.com/user-attachments/assets/4e5a4fa2-c384-4c88-8761-bf9cefd5faab)

![image](https://github.com/user-attachments/assets/f33e1ce2-1bba-4dee-8e99-414183cb0a2a)

#### Once we login successfully we have full access to the user _wiener's_ account, we can see that we have hit the _my-account_ endpoint, meaning this endpoint is accessed after the 2-step verification is performed.
![image](https://github.com/user-attachments/assets/8efe5018-59fb-4284-8139-bc1d637920f4)

#### There are two methods now, to bypass this 2-step verification 2FA and gain access to _carlos's_ account.
#### The first method is that since we know that the length of the verification code is 4, we can try to brute force the verification code and gain access to the _carlos's_ account, or we can try to check if the server is enforcing the validation of the endpoint _my-account_.
#### Let's go ahead and logout from the user _wiener_ and try to login via the user _carlos_ and drop the request for the 2-step verification request, that the application makes to sever and change the URL manually to the endpoint of _my-account_ as was for the user _wiener_ earlier, meaning we are skipping the 2-step verification code generation as:
![image](https://github.com/user-attachments/assets/b95bf97e-280c-4abd-b848-b64c660503a8)

#### After dropping this 2-step verification code generation request, we will change the endpoint in the URL to _my-account_
![image](https://github.com/user-attachments/assets/219eacc9-79d2-44ec-9e98-22f175b13c29)

#### Once the endpoint is hit, we should be able to bypass the 2FA for the user carlos and gain access to his login page as:
![image](https://github.com/user-attachments/assets/a91f96af-8b17-439e-8d99-0c6ba2b807aa)

#### Thus, the user _carlos_ is hacked with kindness !!!
