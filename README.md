# Jarkom-Modul-1-IUP5-2021

Group IUP 5 :

Hilmy Hanif         (05111942000005)

Salma Rahma Lailia  (05111942000016)

Khairi Wiryawan     (05111942000023)


# Module 1


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

    
