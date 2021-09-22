# Jarkom-Modul-1-IUP5-2021

Hilmy Hanif         (05111942000005)
Salma Rahma Lailia  (05111942000016)
Khairi Wiryawan     (05111942000023)

# Module 1

11. Filter so that wireshark only picks up packets coming from port 80!

    ``tcp.port == 80``
    
13. Filter so that wireshark only picks up packets coming from port 21!

     ``tcp.port == 21``
     
15. Filter so that wireshark only picks up packets coming from port 443!

     ``tcp.port == 443``
     
17. Filter so that wireshark only picks up packets going to kemenag.go.id!

     ``tcp.port == kemenag.go.id``
     
19. Filter so that wireshark only picks up packets coming from your local ip address!

Open cmd then type ipconfig, after that you will get your ip address. For searching your originated packets, we use src host means initial host.

    ``ip.src == 192.168.1.4``
