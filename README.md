# ProblemsIT_lab2
Современные проблемы информатики и вычислительной техники. Лабораторная №2
Для утилиты lftp создать профиль apparmor, позволяющий ей исправно функционировать в рамках минимально необходимых и достаточных ограничений в операционной системе

Выполнение:
 1. Устанавливаю недостающие пакеты для работы с apparmor путем команды apt-get istall apparmor-utils.
 2. При создании профиля, выяснилось, что отсутсвует программа lftp, устанавливаем ее.
 далее создаем профиль:переходим в каталог /etc/apparmor.d/ 
 aa-autodep lftp /etc/apparmor.d/usr.bin.lftp
 3. Запускаем утилиту профилировки: aa-genprof lftp Далее запускаем программу lftp в новом терминале.
 
