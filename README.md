базовые команды.
ssh pi@turtlebro(номер).local


ls - чекнуть что внутри папки
sd ~/(путь) - перейти в папку
rostopic list/ rostopic echo /bat(пример)

ПИТОН СКАЧАТЬ
sudo apt install python3-psutil
sudo apt install python3-tqdm

cat /etc/*-release Я НЕ ПОМНЮ ЗАЧЕМ ЭТО

КОРОЧЕ 1 ДЕНЬ

А И Б БЛОК

А блок
приёмка, ну тут сами разберёмся, нет драйвера двигателя.
ПЕРЕХОДИМ К КОМАНДАМ

ПО ТАБЛИЦЕ 1-4
1.ИМЯ КАК В СЕТИ
2.АЙПИ ЧЕРЕЗ ifcongif на роботе
3.частоту через iwconfig
4.......
ПО ТАБЛИЦЕ 5-15
5. lsb_release -a
6. lsb_release -a
7. python3 --version
8. rosversion rospy
9. rosversion turtlebro
10. - rosservice call /board_info "request: {}"
11. - rosservice call /board_info "request: {}"
12. free -- kilo
13. timedatectl
14. cat /etc/os-release если не работает cat /proc/cpuinfo | grep Serial
Серийный номер расбери пай (цифры после нулей)
15. rostopic list
ПО ТАБЛИЦЕ 16-20
16. rostopic echo /bat
17. v412-ctl--list-formats-ext
18. rostopic echo /bat
19. мультиметром измеряем
20. Разница 18 и 19
ПО ТАБЛИЦЕ 21-29
21. На сайте по айпи чекаем IP:8080
22. rostopic echo /odom
23. rostopic echo /odom
24. rostopic echo /imu
25. rostopic echo /scan
26. aplay -l
27. кнопки нажимаем и проверяем
28. Проверить на плате физически
29. ну по идеи если ростопик работает, то это тоже

НУ И ВСЁ

Б блок

ВНАЧАЛЕ СЕРВИС ПАКЕТЫ
 
https://github.com/voltbro/ profi _service_pkg_1
https://github.com/voltbro/ profi _service_pkg_2

Делаем по инструкции качаем 1 всё делаем, переходим ко второму

по инструкции, git log доходим до отката, коммита коппируем его
пишем git checkout и хеш коммита (ЦИФЕРКИ)
далее git pull origin master
дальше к иструкции компилиция catkin_make
и запуск roslaunch profi_service_pkg_2 start_configure.launch








ЭТО НЕ ДО КОНЦА СДЕЛАНО

Rqt команда для вызова ПО по анализу bat файла
перед этим на компе запускаем ядро ROS roscore
