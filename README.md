# Topics Cyber Security CS 466-02 - Final Project
This is a project that me and my group mate Sokkhandara created for our cyber security class final project.

Everything was developed in IntelliJ Idea, using the Java programming language. This is a caesar cipher encryption/decryption program, with an added brute force dictionary decryptor.

### Instructions:
- Have latest JDK installed (https://www.oracle.com/ae/java/technologies/downloads/)
- Download project zip (https://github.com/krish7201/CS_466-02_Cyber_Security_Final_Project/archive/refs/heads/main.zip)
- Extract files
- Run .jar file

### Project Description
Our project uses a GUI (implemented in Java) to demonstrate how the Caesar Cipher Cryptographic System works through two different instances (admin and non-admin). In both cases, the program should work the same, but the admin is allowed more freedom to do certain tasks that the non-admin is restricted from. 

### Related Works
The GeeksforGeeks article contained information about the historical name, mathematical equations for encryption and decryption, images explaining the shifting, examples, step-by-step procedure; and code implementations in the languages C++, Java, Python3, C#, PHP, and JavaScript.1 
Used the website, Cryptii.com, to help us prove that our encryption/decryption algorithm was working properly. 

### Significance
Our project we have designed is intended to help us improve our abilities programming with Java and give us an understanding of encryption and decryption algorithms. Also, it exposes us to potential work field experiences where problems or new ideas may become apparent, and we would have to fix those issues the best way possible. 
Project Specification and Design 

Allows the user the ability to login and access the GUI that contains all the necessary components needed for the Caesar Cipher Cryptographic System such as: allowing the user to encrypt a plaintext into a ciphertext, decryption of the ciphertext and a display of potential plaintexts after decryption.

Our UML diagram is split into 5 different classes:
- Login class takes in the user’s username and password 
- Authentication class takes the input that the user has entered and compares it to the true username and true password. If the user’s input matches the true username and true password, then the user is verified as an ‘admin’. Otherwise, they’re considered a ‘non-admin’
- GUI class contains all of the buttons 
- Encryption class takes in a .txt file and an integer (key for the Caesar Cipher Shift) and encrypts the .txt file. Our program also uses the Encryption class to perform the ‘Brute Force’ attack. 
- StringTokensInDictionary class that allows the program to check if the words in the decrypted message matches to actual English words

### Project UML diagram:
![image](https://github.com/user-attachments/assets/9193e7dd-f580-48d7-8591-22ba2c795c74)

![image](https://github.com/user-attachments/assets/0abdc0c7-6f7b-4be8-a106-158336fe135c)

![image](https://github.com/user-attachments/assets/4cb885ff-20b4-4d7b-8816-e259d5898adf)

