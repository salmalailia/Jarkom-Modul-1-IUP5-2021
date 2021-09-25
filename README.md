# Jarkom-Modul-1-IUP5-2021

Group IUP 5 :

Hilmy Hanif Ibrahim (05111942000005)

Salma Rahma Lailia  (05111942000016)

Khairi Wiryawan     (05111942000023)


# Module 1

1. What web server is used on "ichimarumaru.tech"!


```http.host == ichimarumaru.tech``` and then follow TCP


![Screenshot (349)](https://user-images.githubusercontent.com/73766131/134770713-74ab74e3-4e0f-467b-b839-0a39571a2150.png)


2. Find the packets from the web that use the basic authentication method!


```http.authbasic```


![Screenshot (359)](https://user-images.githubusercontent.com/73766131/134770729-abaf6526-3bd2-4893-a4f5-3245925d7a3f.png)


3. Follow the instructions at basic.ichimarumaru.tech! Username and password can be obtained from the .pcapng file!


```http.host == basic.ichimarumaru.tech```


![Screenshot (357)](https://user-images.githubusercontent.com/73766131/134770752-5a9405ac-4cae-44c1-a66f-31da75d55758.png)
Credentials: kuncimenujulautan:tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN

![Screenshot (356)](https://user-images.githubusercontent.com/73766131/134770764-39a18896-8956-4915-a42a-cfe8b91e47c9.png)


4. Find the mysql packets that contain the select query command!


```mysql.query matches "select"```



![Screenshot (351)](https://user-images.githubusercontent.com/73766131/134770789-ead0bf92-a4a1-4684-a221-e175668597b7.png)

5. Login to portal.ichimarumaru.tech then follow the instructions! The username and password can be obtained from the insert query in the users table from the .pcap file!



```mysql.query matches "insert"```



 ![Screenshot (353)](https://user-images.githubusercontent.com/73766131/134770863-e35aef21-64a2-441d-9971-5fef6da9a75b.png)

![Screenshot (352)](https://user-images.githubusercontent.com/73766131/134770869-9c45c56e-79c3-4df1-bd0c-6a0f10a661cb.png)



6.  Find username and password when logging into FTP Server!
    
    ``ftp.request.command == USER || ftp.request.command == PASS``
    
    ![image](https://user-images.githubusercontent.com/73651220/134756443-621611cb-4715-4f93-a223-b001f3ed7fa5.png)

7. There are 500 zip files saved to FTP Server with names 0.zip, 1.zip, 2.zip, ..., 499.zip. Save and Open the pdf file. (Hint = the name of the pdf is "Real.pdf")

    ``ftp-data contains "Real.pdf"``
    
    ![image](https://user-images.githubusercontent.com/73651220/134769365-931c561d-4749-4446-9664-0204271c93e5.png)
    
    ![image](https://user-images.githubusercontent.com/73651220/134756487-50ab3f31-db88-4938-9856-6b61d0b40b03.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756492-2fdb5872-0cc3-4c5b-8a6b-5726a597bff1.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756960-8a4abe08-38ec-4f33-a373-e817613bab9c.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756517-c13a9c70-662f-4c11-9573-71f9075e60be.png)

8. Look for the packets that show the retrieval of files from the FTP!

    ``ftp.request.command == RETR``
    
    ![image](https://user-images.githubusercontent.com/73651220/134756593-c187c301-5760-44cc-9ccc-69bb933e55b0.png)

9. From the packets going to FTP, there are indications of storing some files. One of them is a file containing confidential data with the name "secret.zip". Save and open the file!

    ``ftp-data.command == "STOR secret.zip"``
    
    ![image](https://user-images.githubusercontent.com/73651220/134756647-8ad74b6b-702c-4d81-a934-2bbc4d9c0208.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756651-6fc58c74-58f2-4fe4-9e4d-501cab2a7f3e.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756659-6c0d06b3-8f91-499b-a15e-9bab8cbd318d.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756687-d8188a4d-fc96-4f54-a846-61169b83a2e1.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756731-35135baa-230b-4fc3-a6be-79e499a95cdc.png)

10. Also there is "history.txt" which probably contains the history of the bash server! Use the contents of "history.txt" to find the password to open the secret file in "secret.zip"!

    ``ftp-data.command == "STOR history.txt"``
    
    ![image](https://user-images.githubusercontent.com/73651220/134756817-a6bdad89-a9d8-4688-8190-db40f21b9e7d.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756836-6eb34787-f46b-4b0c-9491-678ade1cfa44.png)

    ``ftp-data.command == "STOR bukanapaapa.txt"``
    
    ![image](https://user-images.githubusercontent.com/73651220/134756847-de13880f-c736-48b8-b35e-3560ac5ffea4.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756863-5363955e-934b-4f5e-9d51-70dceb4deb14.png)
    
    ![image](https://user-images.githubusercontent.com/73651220/134756903-40468e75-f223-46c6-a2f8-88f234746fb3.png)

    ![image](https://user-images.githubusercontent.com/73651220/134756909-6eadb4d3-7580-46f1-83b7-e9b05663af8e.png)

11. Filter so that wireshark only picks up packets coming from port 80!

    ``tcp src port 80``
    
    ![image](https://user-images.githubusercontent.com/73702347/134542323-7dc6bdd8-cb73-40bd-a41b-36fd0022fb77.png)

    ![image](https://user-images.githubusercontent.com/73702347/134542432-ea7730cb-4724-42f5-b176-5b71dcdfeb0f.png)

12. Filter so that wireshark only picks up packets coming from port 21!

     ``tcp src port 21``
     
     ![image](https://user-images.githubusercontent.com/73702347/134542766-cc3d1045-3a42-4f3e-92be-e54617dede05.png)
     
     ![image](https://user-images.githubusercontent.com/73702347/134542869-05f48479-4a0e-40a0-afef-30a701fd436c.png)

13. Filter so that wireshark only picks up packets coming from port 443!

     ``tcp src port 443``

    ![image](https://user-images.githubusercontent.com/73702347/134542966-6c8f542b-792f-4d03-a623-463e19d288c2.png)
    
    ![image](https://user-images.githubusercontent.com/73702347/134543000-3594efd1-4537-4a78-9513-4f5454ffe332.png)

14. Filter so that wireshark only picks up packets going to kemenag.go.id!

     ``dst kemenag.go.id``
     
     ![image](https://user-images.githubusercontent.com/73702347/134543239-2ed092d6-a4b2-488b-83b6-b1053a566ebe.png)
     
     ![image](https://user-images.githubusercontent.com/73702347/134543337-c22bc23c-dd10-4e79-a7a7-df8580b17be8.png)
     
15. Filter so that wireshark only picks up packets coming from your local ip address!

    Open cmd then type ipconfig, after that you will get your ip address. For searching your originated packets, we use src host means initial host.

    ``src host 192.168.1.4``
    
    ![image](https://user-images.githubusercontent.com/73702347/134543511-f6362835-40ff-45f2-b49e-619e4b8fb485.png)
    
    ![image](https://user-images.githubusercontent.com/73702347/134543531-146953c4-6861-4103-a514-46928d3dac03.png)

    
