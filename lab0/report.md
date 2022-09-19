<!-- # Отчет по лабораторной работе №1 -->
#### «Национальный исследовательский университет ИТМО»
### Основы профессиональной деятельности
## Лабораторная работа 1
## Вариант 368982
### Хабнер Георгий, P3131
###  2022

###1. Первое задание
Команды:
>
    mkdir lab0
    cd lab0
    touch cherrim3
    echo Тип диеты Phototroph > cherrim3
    mkdir hydreigon6
    cd hydreigon6
    touch venusaur
    echo "Тип диеты Omnivore
    Phototroph"> venusaur
    touch golem
    echo Тип покемона ROCK GROUND > golem
    mkdir togekiss
    mkdir mienshao
    touch tyrogue
    echo "Живет Mountain
    Urban" > tyrogue
    mkdir lanturn8
    cd lanturn8
    mkdir raichu
    mkdir diglett
    touch scyther
    echo "Способности Leer Quick Attack Focus Energy Pursuit
    False Swipe Agility Wing Attack Fury Cutter Slash Razor Wind Double
    Team X-Scissor Night Slash Double Hit Air Slash Swords Dance
    Feint" > scyther
    touch bastiodon
    echo Тип покемона ROCK STEEL > bastiodon
    mkdir tympole
    touch tangela
    echo "Возможности
    Overland=6 Surface=2 Jump=2 Power=2 Intelligence=4
    Reach=0" > tangela
    cd ..
    touch sentret9
    echo "weight=13.2 height=31.0 atk=5
    def=3" > sentret9
    touch spearow8
    echo Развитые способности Sniper > spearow8
    mkdir vileplume2
    cd vileplume2
    mkdir budew
    touch cofagrigus
    echo "Возможности
    Overland=7 Surface=7 Sky=7 Jump=3 Power3=0 Intelligence=4 Phasing=0
    Invisibility=0" > cofagrigus
    mkdir porygon2
Вывод папки lab0
>[s368982@helios ~/lab0]$ ls
cherrim3        lanturn8        spearow8
hydreigon6      sentret9        vileplume2

Вывод папки hydreigon6
>[s368982@helios ~/lab0/hydreigon6]$ ls
golem           togekiss        venusaur
mienshao        tyrogue


Вывод папки lanturn8
>[s368982@helios ~/lab0/lanturn8]$ ls
bastiodon       raichu          tangela
diglett         scyther         tympole


Вывод папки vileplume2
>[s368982@helios ~/lab0/vileplume2]$ ls
budew           cofagrigus      porygon2
###2. Второе задание
>
        chmod u=r,g=,o=r ./lab0/cherrim3
        chmod u=rx,g=w,o=r ./lab0/hydreigon6

        chmod u=rw,g=,o= ./lab0/hydreigon6/venusaur
        chmod 600 ./lab0/hydreigon6/golem
        chmod u=wx,g=rw,o=x ./lab0/hydreigon6/togekiss
        chmod u=rw,g=w,o=r ./lab0/hydreigon6/tyrogue
        chmod u=rx,g=rw,o=x ./lab0/hydreigon6/mienshao

        chmod u=rx,g=wx,o=rwx ./lab0/lanturn8
        chmod 755 ./lab0/lanturn8/raichu
        chmod u=wx,g=wx,o=rx ./lab0/lanturn8/diglett
        chmod u=,g=r,o=r ./lab0/lanturn8/scyther
        chmod u=r,g=,o= ./lab0/lanturn8/bastiodon
        chmod u=rwx,g=rx,o=w ./lab0/lanturn8/tympole
        chmod u=,g=r,o=r ./lab0/lanturn8/tangela

        chmod 064 ./lab0/sentret9

        chmod u=rw,g=w,o= ./lab0/spearow8

        chmod 337 ./lab0/vileplume2
        chmod u=rwx,g=rx,o=wx ./lab0/vileplume2/budew
        chmod u=rw,g=w,o= ./lab0/vileplume2/cofagrigus
        chmod u=wx,g=x,o=w ./lab0/vileplume2/porygon2

Права содержимого lab0
>[s368982@helios ~/lab0]$ ls -l
total 19
-r-----r--  1 s368982  studs  29 17 сент. 20:41 cherrim3
dr-x-w-r--  4 s368982  studs   7 17 сент. 20:41 hydreigon6
dr-x-wxrwx  5 s368982  studs   8 17 сент. 20:41 lanturn8
----rw-r--  1 s368982  studs  36 17 сент. 20:41 sentret9
-rw--w----  1 s368982  studs  47 17 сент. 20:41 spearow8
d-wx-wxrwx  4 s368982  studs   5 17 сент. 20:41 vileplume2 

Права содержимого hydreigon6
>[s368982@helios ~/lab0/hydreigon6]$ ls -l
total 3
-rw-------  1 s368982  studs  36 17 сент. 20:41 golem
dr-xrw---x  2 s368982  studs   2 17 сент. 20:41 mienshao
d-wxrw---x  2 s368982  studs   2 17 сент. 20:41 togekiss
-rw--w-r--  1 s368982  studs  26 17 сент. 20:41 tyrogue
-rw-------  1 s368982  studs  39 17 сент. 20:41 venusaur

Права содержимого lanturn8
>[s368982@helios ~/lab0]$ cd lanturn8;ls -l
total 7
-r--------  1 s368982  studs   35 17 сент. 20:41 bastiodon
d-wx-wxr-x  2 s368982  studs    2 17 сент. 20:41 diglett
drwxr-xr-x  2 s368982  studs    2 17 сент. 20:41 raichu
----r--r--  1 s368982  studs  198 17 сент. 20:41 scyther
----r--r--  1 s368982  studs   83 17 сент. 20:41 tangela
drwxr-x-w-  2 s368982  studs    2 17 сент. 20:41 tympole


###3. Третье задание
>
    chmod -R 777 ./lab0
    #скопировать содержимое файла sentret9 в новый файл lab0/vileplume2/cofagrigussentret
    cp ./lab0/sentret9 ./lab0/vileplume2/cofagrigussentret

    #скопировать рекурсивно директорию lanturn8 в директорию lab0/lanturn8/diglett
    cp -r ./lab0/lanturn8 ./lab0/lanturn8/diglett

    #объеденить содержимое файлов lab0/lanturn8/bastiodon, lab0/vileplume2/cat ./lab0/lanturn8/bastiodon ./lab0/vileplume2/cofagrigus > ./lab0/sentret9_44

    #создать символическую ссылку c именем Copy_82 на директорию hydreigon6 в каталоге lab0
    ln -s ./lab0/hydreigon6 ./lab0/Copy_82

    #cоздать символическую ссылку для файла sentret9 с именем lab0/hydreigon6/golemsentret
    ln -s ./lab0/sentret9 ./lab0/hydreigon6/golemsentret

    #скопировать файл sentret9 в директорию lab0/hydreigon6/mienshao
    cp ./lab0/sentret9 ./lab0/hydreigon6/mienshao

    #cоздать жесткую ссылку для файла cherrim3 с именем lab0/hydreigon6/venusaurcherrim
    ln ./lab0/cherrim3 ./lab0/hydreigon6/venusaurcherrim

Вывод содержимого cofagrigussentret 
>[s368982@helios ~/lab0/vileplume2]$ cat cofagrigussentret
weight=13.2 height=31.0 atk=5
def=3

Вывод содержимого diglett
>[s368982@helios ~/lab0/lanturn8/diglett/lanturn8]$ ls
bastiodon       scyther
diglett         tangela

Вывод содержимого sentret9_44
>[s368982@helios ~/lab0]$ cat sentret9_44
Тип покемона ROCK STEEL
Возможности
Overland=7 Surface=7 Sky=7 Jump=3 Power3=0 Intelligence=4 Phasing=0
Invisibility=0

Символическая ссылка  Copy_82
>[s368982@helios ~/lab0]$ ls -l
total 32
-rwxrwxrwx  2 s368982  studs   29 17 сент. 20:41 cherrim3
lrwxr-xr-x  1 s368982  studs   17 17 сент. 21:33 Copy_82 -> ./lab0/hydreigon6

Символическая ссылка lab0/hydreigon6/golemsentret
>[s368982@helios ~/lab0/hydreigon6]$ ls -l
total 4
-rwxrwxrwx  1 s368982  studs  36 17 сент. 20:41 golem
lrwxr-xr-x  1 s368982  studs  15 17 сент. 21:33 golemsentret -> ./lab0/sentret9

sentret9 в lab0/hydreigon6/mienshao
>[s368982@helios ~/lab0/hydreigon6/mienshao]$ ls sentret9

>[s368982@helios ~/lab0/hydreigon6]$ cat venusaurcherrim
Тип диеты Phototroph

###4. Четвертое задание
>
    #Подсчитать количество символов содержимого файлов в директории lanturn8, результат записать в файл в директории /tmp, ошибки доступа перенаправить в файл в директории /tmp
    wc -m ./lab0/lanturn8/* &>> /tmp/s368982_log

    #Вывести четыре первых элемента рекурсивного списка имен и атрибутов файлов в директории lab0, начинающихся на символ 's', список отсортировать по убыванию даты модификации файла, ошибки доступа не подавлять и не перенаправлять
    grep -rl . | grep /s 2>&1 | xargs ls -lt | head -4

    #Вывести содержимое файлов с номерами строк в директории lanturn8, исключить строки, содержащие "ble", регистр символов игнорировать, ошибки доступа перенаправить в файл в директории /tmp
    cat -n ./lab0/lanturn8/*  2>> /tmp/s368982_log | grep -vi ble 

    #Подсчитать количество символов содержимого файлов: golem, tyrogue, отсортировать вывод по уменьшению количества, подавить вывод ошибок доступа
    wc -m ./lab0/hydreigon6/golem ./lab0/hydreigon6/tyrogue | head -2 | sort -r 2>/dev/null

    #Вывести рекурсивно список имен и атрибутов файлов в директории lanturn8, список отсортировать по имени z->a, ошибки доступа не подавлять и не перенаправлять
    ls -R ./lab0/lanturn8 | sort -r | grep "."

    #Вывести список имен и атрибутов файлов в директории vileplume2, список отсортировать по возрастанию даты доступа к файлу, добавить вывод ошибок доступа в стандартный поток вывода
    chmod u=rx ./lab0/vileplume2
    ls -lcr ./lab0/vileplume2 2>&1

1 задание
>[s368982@helios ~]$ cat /tmp/s368982_log
wc: ./lab0/lanturn8/diglett: open: Permission denied
wc: ./lab0/lanturn8/raichu: read: Is a directory
wc: ./lab0/lanturn8/scyther: open: Permission denied
wc: ./lab0/lanturn8/tangela: open: Permission denied
wc: ./lab0/lanturn8/tympole: read: Is a directory
      24 ./lab0/lanturn8/bastiodon
      24 total

2 задание
>grep: ./lab0/hydreigon6/golemsentret: No such file or directory
grep: ./lab0/hydreigon6/togekiss: Permission denied
grep: ./lab0/Copy_82: No such file or directory
grep: ./lab0/vileplume2: Permission denied
grep: ./lab0/lanturn8/diglett: Permission denied
grep: ./lab0/lanturn8/scyther: Permission denied
grep: ./lab0/lanturn8/tangela: Permission denied
grep: ./lab0/sentret9: Permission denied
-rwxr-xr-x  1 s368982  studs   36 18 сент. 01:15 ./lab0/hydreigon6/mienshao/sentret9
-rw-r--r--  1 s368982  studs  142 18 сент. 01:15 ./lab0/sentret9_44
-rw--w----  1 s368982  studs   47 18 сент. 01:15 ./lab0/spearow8

3 задание
>[s368982@helios ~]$ cat -n ./lab0/lanturn8/*  2>/tmp/s368982_log
     1  Тип покемона ROCK STEEL

4 задание
>
      25 ./lab0/hydreigon6/golem
      21 ./lab0/hydreigon6/tyrogue

5 задание
>ls: ./lab0/lanturn8/diglett: Permission denied
tympole
tangela
scyther
raichu
diglett
bastiodon
./lab0/lanturn8/tympole:
./lab0/lanturn8/raichu:
./lab0/lanturn8/diglett:

6 задание
>total 6
drwxr-x-wx  2 s368982  studs    2 18 сент. 01:15 budew
-rw--w----  1 s368982  studs  107 18 сент. 01:15 cofagrigus
d-wx--x-w-  2 s368982  studs    2 18 сент. 01:15 porygon2
-rwxr-xr-x  1 s368982  studs   36 18 сент. 01:15 cofagrigussentret

###5. Пятое задание
>
    chmod -R 777 ./lab0
    #Удалить файл spearow8
    rm ./lab0/spearow8

    #Удалить файл lab0/lanturn8/bastiodon
    rm ./lab0/lanturn8/bastiodon

    #удалить символические ссылки Copy_*
    rm ./lab0/Copy_*

    #удалить жесткие ссылки lab0/hydreigon6/venusaurcherr*
    rm ./lab0/hydreigon6/venusaurcherr*

    #Удалить директорию vileplume2
    chmod -R u=rwx ./lab0/vileplume2
    rm -r ./lab0/vileplume2

    #Удалить директорию lab0/hydreigon6/mienshao
    chmod -R u=rwx ./lab0/hydreigon6/mienshao
    rm -r ./lab0/hydreigon6/mienshao

##Вывод
В ходе работы я познакомился с основными linux-командами

![alt text](aefd3a2b1457cc9188af97ca70440499--computer-humor-tech-humor.jpg)