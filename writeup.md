-> First off, because previously we learned that we can use `sudo -i -u user2 bash {bash script}` to run commands as user2 (who has superuser permissions at least to some    
    extent), I used the same idea to create a bash script to read the `/root/id_rsa` file to see if I could ssh into the root user with the id_rsa key and no password:
<br><br>
<img width="929" alt="Screenshot 2024-11-23 at 5 09 42 PM" src="https://github.com/user-attachments/assets/ee422087-12c2-4c70-8ee2-fabee9a46605">
<br><br>
-> I was able to read the `/root/id_rsa` file, so I copied it and pasted it into a file called id_rsa on my machine, and then used `chmod 600 id_rsa` to change the permissions on     the file so ssh would not refuse a login request:
<br><br>
<img width="929" alt="Screenshot 2024-11-23 at 5 10 51 PM" src="https://github.com/user-attachments/assets/1ab6ce44-cac0-4cbe-9fe8-0ab5d32df6e3">
<br><br>
<img width="929" alt="Screenshot 2024-11-23 at 5 15 36 PM" src="https://github.com/user-attachments/assets/8c44828c-068e-41b2-b493-d5288c571b35">
<br><br>
<img width="929" alt="Screenshot 2024-11-23 at 5 19 01 PM" src="https://github.com/user-attachments/assets/f1ad6b63-0180-442e-96aa-8fb392c85856">
<br><br>
-> Now I am able to login as root through SSH and read the root flag file:
<br><br>
<img width="929" alt="Screenshot 2024-11-23 at 5 21 47 PM" src="https://github.com/user-attachments/assets/df77003d-30f5-40fe-9623-68d7d38bce5b">
