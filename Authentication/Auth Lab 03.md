#### The page appears to be a blog site:
![image](https://github.com/user-attachments/assets/fa0dfba3-de13-49f4-856c-35da7ebccc0e)

#### At the top right corner of the blog site, there's a _My account_ section:
![image](https://github.com/user-attachments/assets/7177c1f7-5353-481c-a64e-8df5136e70c1)

#### Let's access the _My account_ page and try to login as the user _wiener_:
![image](https://github.com/user-attachments/assets/e312a3b9-83bc-481f-8963-8f0aa0702719)

#### We should be able to login as the user _wiener_:
![image](https://github.com/user-attachments/assets/2d557e98-9844-4892-b0de-4f24874250ae)

#### Let's try to reset the password of the user _wiener_ as:
![image](https://github.com/user-attachments/assets/45398c67-40bb-45cc-99e2-775ed83abf5d)

#### After entering the username, let's hit the _submit_ button and then head over to the _password reset_ link and set the new password for the user _wiener_ as:
![image](https://github.com/user-attachments/assets/0dde3040-ba6a-42c3-89f0-a426df510371)

![image](https://github.com/user-attachments/assets/4c60f00b-29b1-42be-9cf2-fdd8ea7c8e2a)

#### Now after we hit the submit button, we should be able to login via the user _wiener_ with the new password:
![image](https://github.com/user-attachments/assets/36404935-83ed-41a1-b330-8b25cca29a09)

![image](https://github.com/user-attachments/assets/46e0a8ff-a927-406b-ab1a-cd125d9fc3a2)

#### Now let's repeat this process, after having seen how the password reset logic works, let's see the request that the application makes while sending the password reset request:
![image](https://github.com/user-attachments/assets/1405a378-07b9-47a5-916d-79505ba46fe6)

#### The application makes a request to the _forgot-password_ endpoint and at the bottom we have the _username=wiener_ let's forward this request.
#### Let's click on the password reset link and enter the new password, and capture the request as:
![image](https://github.com/user-attachments/assets/92f9c8f3-d02e-4373-b49d-ecc12b5d3582)

#### If we observe closely, there's a _temp-forgot-password-token_ that appears twice in the request, meaning this particular token is for the user _wiener_ let's send this request to the repeater's tab as:
![image](https://github.com/user-attachments/assets/93d0bec1-60ee-4091-9a6b-f70f4ff23dac)

#### If the application does not really care for the _temp-forgot-password-token_ and the username, meaning we can change the token value and username in the request and should be able to change the password for the user _carlos_ as:
![image](https://github.com/user-attachments/assets/a35c25d1-4952-4a83-8a2b-53916888d886)

#### After having changed the token value and the username, let's send this request and notice the response as:
![image](https://github.com/user-attachments/assets/8f8963ac-60e6-4aae-85a3-7657234ef8af)

#### We are getting a redirect, following the redirect we get a **200 OK** response, that means we have been able to change the password for the user _carlos_ successfully.
![image](https://github.com/user-attachments/assets/e918f551-ae06-49b8-9667-3f072e0e311e)

#### Let's try to login via the user _carlos_ as:
![image](https://github.com/user-attachments/assets/1c4a5dbb-7ab0-42c5-bd55-d7b397273f99)

#### We should be able to login successfully as:
![image](https://github.com/user-attachments/assets/bcfd5aa1-51c1-4f67-a8ac-63372d8e4ae8)

#### Thus, carlos was hacked with kindness !!!





