# KF-Server-Crack (Windows + Linux)
Full actual server crack + autorestart with logs.

Don't forget to open all Steam ports.

The following list of default ports need to be open for a server to run successfully:

    7707 UDP/IP (Game Port) - для подключения в игре.
    7708 UDP/IP (Query Port) - для отображения инфо о сервере в игре.
    7717 UDP/IP (Steam Query Port).
    28852 TCP/IP and UDP (Allows your Server to Connect to the Master Server Browser).
    8075 TCP/IP (Port set via ListenPort that your WebAdmin will run on).
    20560 UDP/IP (Steam Port).

Since the game is running with the Steam backend, if you are running more than 1 server per IP, you will need to make sure that you have some additional ports open beyond the default KF ports. If you change the default Game Port from 7707, this change will be reflected in the Master Server Port (28852) and the Steam Port (20560) as well.

You must also change OldQueryPortNumber=7717 under [IpDrv.UdpGamespyQuery] in the KillingFloor.ini to match the increase of the 7707 port. So if you change 7707 to 7807, then 7717 would change to 7817. If this is not done, the server will crash when starting. 

Если у Вас нестандартный порт (7707), а например 9507, то необходимо изменить 2 стимовских порта по следующей формуле:

28852 - 7707 = 21145

21145 + 9507 = 30652

Далее аналогично с портом 20560

Для Steam Query Port прибавляем +10 к основному порту. То есть 9507 + 10 = 9517. Это и будет Steam Query Port.

Для отображения инфо о сервере после смены порта прибавляем +1 к основному порту. То есть 9507 + 1 = 9508

![изображение](https://github.com/user-attachments/assets/8b82206c-3152-4aaf-900a-2ccad06f15dd)

![изображение](https://github.com/user-attachments/assets/d6a61fbf-0a28-49b7-877d-791a1119e0dc)
