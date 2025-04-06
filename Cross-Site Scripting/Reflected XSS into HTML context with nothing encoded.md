#### The page appears to be a blog site:
![image](https://github.com/user-attachments/assets/40222d71-45d4-41e4-947d-9d3975bd144f)

#### At the very first glance, there is an input field at the top of the blog site, that says, _Search the blog..._
#### The next step would be to check if the site is vulnerable to XSS.
#### Try to input a random text in the search tab as:
![image](https://github.com/user-attachments/assets/23206589-02e6-44ba-9049-199c356c3072)

#### After entering a random text, click on the Search button to see the results of the search as:
![image](https://github.com/user-attachments/assets/5c6f6f00-e36d-4e4d-94c0-0eeada02c547)

#### There’s no blog post with the name h4ck3rk1nd but the site does use the user input to render the search result, meaning the site is vulnerable to **Reflected-XSS**.
#### Try to input an inline script in the search tab as the payload to trigger the Reflected-XSS, when the search result gets rendered as:
![image](https://github.com/user-attachments/assets/7861e7b4-504f-47a4-9dca-dda664f30247)

#### Once the payload is entered, click on the Search button and the Reflected-XSS should trigger as:
![image](https://github.com/user-attachments/assets/56c762e3-ac1a-4c74-af6d-29f2723aad0a)

#### Thus, the challenge is solved with kindness
![image](https://github.com/user-attachments/assets/b19f3631-6b9f-45ad-81b2-c8adef4d784c)
