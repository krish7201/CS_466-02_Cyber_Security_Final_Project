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
![image](https://github.com/user-attachments/assets/4cb885ff-20b4-4d7b-8816-e259d5898adf)

### Project Flowchart
![image](https://github.com/user-attachments/assets/0abdc0c7-6f7b-4be8-a106-158336fe135c)

### Data Acquisition
The data we will be using to encrypt and decrypt, will be all forms of historical texts of the United States of America such as: the Emancipation Proclamation, Gettysburg Address, Star-Spangled Banner, Pledge of Allegiance and the Declaration of Independence.

### User Documentation 
Our development environment for this project was between MacOS and Windows 10/11, it was developed in Java, we used the IDE IntelliJ for development and GUI layout; the only things that weren’t default about our file path setup were that we put the test files in the “src” folder and some test files outside the source folder on the root of the project, everything else was default as it’d be set up in IntelliJ.

When you download our project, it’ll sit in your downloads like this:
![image](https://github.com/user-attachments/assets/9d73824c-25a5-4da2-a822-1759281723b8)

When you open the project you’ll see a jar file, that’s all you need to run the program (provided you’re creating your own test files). Double click on the jar file and the program will start.
![image](https://github.com/user-attachments/assets/3f2035aa-dc3c-46fc-a390-d9fa4b19d7da)

The username and password is: CoolKid99 and something (to access the user mode: get the username and password incorrect three times).
![image](https://github.com/user-attachments/assets/2b969983-042c-43e1-bda8-607508c1a3df)

If you’ve launched the JAR file outside of the project folder, the browse button will default to the documents folder on your Windows computer, not sure about Mac. You can feed the program any text file (file with a .txt file extension), no other files will be accepted (the program will remain on the browse section if fed a file that doesn’t have a .txt file extension).
![image](https://github.com/user-attachments/assets/5c13a262-bc62-4890-956f-8272593f14ea)

![image](https://github.com/user-attachments/assets/fb15f4ac-6243-41ab-9e48-d3936ce909ca)
Figure 1: Login page

![image](https://github.com/user-attachments/assets/309afabf-41f0-418c-9ad1-0f3ba8496b04)
Figure 2: Window displays red text when invalid Username or Password is entered

![image](https://github.com/user-attachments/assets/c085a749-e4cc-4fd6-b488-43d9960583d5)
Figure 3: Window when admin has logged in (Admin view)

![image](https://github.com/user-attachments/assets/e7323b86-8d00-41f5-8ca4-fae8485aa661)
Figure 4: Window once non admin user has logged in (non-admin view)

![image](https://github.com/user-attachments/assets/121dc6e6-53e1-4374-979e-99c165b67fbb)
Figure 5: Displayed window once user clicks ‘Browse’ to view text files (Admin view)

![image](https://github.com/user-attachments/assets/b7e7f47f-476d-4e55-955c-84bb14938c6c)
Figure 6: Text file has been chosen (becomes grayed out); user enters a key for encryption (Admin view)

![image](https://github.com/user-attachments/assets/7bf57fd3-7c50-47fb-8d18-965e91d259b2)
Figure 7: ‘Encrypt’ has been pressed and ciphertext is displayed (non-admin view)

![image](https://github.com/user-attachments/assets/51c4a8e1-5377-44c0-a8d5-cc597182ff0b)
Figure 8: ‘Decrypt’ has been pressed and output is displayed (non-admin view)

![image](https://github.com/user-attachments/assets/e8b114f5-7008-420e-8203-722fe9b37e8a)
Figure 9: User entered a key and pressed ‘Encrypt” button which displays a portion of the ciphertext (encryption portion gets grayed out) (Admin view)

![image](https://github.com/user-attachments/assets/1cab4682-6225-4821-bd0d-8bb240bd191c)
Figure 10: User clicks ‘Decrypt’ which displays a brute force method of all possible decrypted plaintext and a percentage that describes how likely a certain key and its plaintext is related to solving the ciphertext. 

Discussions
Sokhanndara – A few problems I had with the java implementation was figuring out how to shift the letters. At first, I thought I could shift the letters normally using the key but got answers that didn’t match what I was expecting. For instance, when I shifted ‘Z’ five letters forward I got ‘e’ or I somehow ended up symbols instead of characters. Then I looked up other codes to see how they figured it out and noticed that they incorporated the numbers 65 and 97. Initially, I did not know what or where those numbers came from, then I realized that they were the decimal number for the letters ‘A’ and ‘a’ in the ASCII table. I ended up importing the Caesar Cipher Shift Algorithm from GeeksforGeeks and modified it to my understanding. Then, with the encouragement from my partner, Kris, I created my own implementation of the Casear Cipher Shift Algorithm using an alphabet array. 

Kris – Leading up to the end I was really having troubles implementing the recursive binary search for looking up the words in the dictionary. I was implementing similar functionality to .compareTo and I didn’t realize it immediately. I couldn’t tell if implementing photos was possible to be done properly without a lot of work. I tried one method and I couldn’t get high resolution photos into the program because I couldn’t scale them down. I didn’t end up implementing the manual decrypt. I hashed the username too, I thought that’d be important.


