# Jarkom-Modul-1-IUP5-2021

Hilmy Hanif         (05111942000005)
Salma Rahma Lailia  (05111942000016)
Khairi Wiryawan     (05111942000023)

# Module 1

11. Filter so that wireshark only picks up packets coming from port 80!

    ``tcp.port == 80``
    
    ![image](https://user-images.githubusercontent.com/73702347/134342478-9b623040-e4d9-4901-b455-ac4ebe92341d.png)

12. Filter so that wireshark only picks up packets coming from port 21!

     ``tcp.port == 21``
     
     ![image](https://user-images.githubusercontent.com/73702347/134342599-1676b27c-73a4-4f29-a10a-de5e145124ab.png)
     
13. Filter so that wireshark only picks up packets coming from port 443!

     ``tcp.port == 443``

    ![image](https://user-images.githubusercontent.com/73702347/134342708-78a83abc-13d4-4cfa-bd3b-ca7e33f267f4.png)

14. Filter so that wireshark only picks up packets going to kemenag.go.id!

     ``tcp.port == kemenag.go.id``
     
     ![image](https://user-images.githubusercontent.com/73702347/134342907-c953a02c-2742-4f88-8de6-a99665d17bd8.png)
     
15. Filter so that wireshark only picks up packets coming from your local ip address!

    Open cmd then type ipconfig, after that you will get your ip address. For searching your originated packets, we use src host means initial host.

    ``ip.src == 192.168.1.4``
    
    ![image](https://user-images.githubusercontent.com/73702347/134342990-77b59523-eefb-4ec7-ab10-d1944bcbba1f.png)
    
