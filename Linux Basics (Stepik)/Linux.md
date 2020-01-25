-------------------------------------------------------------------------------
# LINUX

<!-- MarkdownTOC levels="2,3" autolink="true" uri_encoding="false" markdown_preview="github" -->

- [I. Терминал](#i-%D1%82%D0%B5%D1%80%D0%BC%D0%B8%D0%BD%D0%B0%D0%BB)
  - [Основные комманды:](#%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D0%BD%D1%8B%D0%B5-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B0%D0%BD%D0%B4%D1%8B)
  - [Ввод/вывод:](#%D0%B2%D0%B2%D0%BE%D0%B4%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4)
  - [Работа с программами:](#%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%D0%BC%D0%B8)
- [II. Работа на сервере](#ii-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D0%BD%D0%B0-%D1%81%D0%B5%D1%80%D0%B2%D0%B5%D1%80%D0%B5)
  - [Скачивание файлов:](#%D1%81%D0%BA%D0%B0%D1%87%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2)
- [III. Работа с программами](#iii-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0%D0%BC%D0%B8)
  - [Информация о системе:](#%D0%B8%D0%BD%D1%84%D0%BE%D1%80%D0%BC%D0%B0%D1%86%D0%B8%D1%8F-%D0%BE-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B5)
  - [Работа с архивами:](#%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D0%B0%D1%80%D1%85%D0%B8%D0%B2%D0%B0%D0%BC%D0%B8)
  - [Поиск файлов и слов:](#%D0%BF%D0%BE%D0%B8%D1%81%D0%BA-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2-%D0%B8-%D1%81%D0%BB%D0%BE%D0%B2)
- [IV. Скрипты на bash](#iv-%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D1%8B-%D0%BD%D0%B0-bash)
  - [Переменные:](#%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D0%B5)
  - [Аргументы скрипта:](#%D0%B0%D1%80%D0%B3%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%B0)
  - [Условные конструкции:](#%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%BD%D1%8B%D0%B5-%D0%BA%D0%BE%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%86%D0%B8%D0%B8)
  - [Циклы и функции:](#%D1%86%D0%B8%D0%BA%D0%BB%D1%8B-%D0%B8-%D1%84%D1%83%D0%BD%D0%BA%D1%86%D0%B8%D0%B8)
- [V. Настройка системы](#v-%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D1%8B)
  - [Права доступа:](#%D0%BF%D1%80%D0%B0%D0%B2%D0%B0-%D0%B4%D0%BE%D1%81%D1%82%D1%83%D0%BF%D0%B0)
  - [Удобная история команд](#%D1%83%D0%B4%D0%BE%D0%B1%D0%BD%D0%B0%D1%8F-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%8F-%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4)
  - [Virtual Box:](#virtual-box)
  - [Переменные окружения:](#%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D0%B5-%D0%BE%D0%BA%D1%80%D1%83%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F)
  - [Установка с USB:](#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-%D1%81-usb)

<!-- /MarkdownTOC -->

-------------------------------------------------------------------------------
## I. Терминал

```
<user>@<computer_name> <path>
<command> <options> <arguments>

ctrl + shift + C    : копировать
ctrl + shift + V    : вставить
ctrl + A            : начало строки
ctrl + E            : конец строки
ctrl + W            : удалить слово слева
ctrl + R            : поиск по введённым командам
alt + B             : назад на слово
alt + F             : вперёд на слово
Tab                 : автодополнение

ctrl + shift + T    : открыть новую вкладку в терминале
ctrl + shift + W    : закрыть текущую вкладку терминала
alt + <#>           : перейти в указанную вкладку терминала

Ubuntu:
super + A           : show all applications
super + L           : lock screen
super + S           : show overview
super + ↑/↓         : maximize/restore window
super + ←/→         : toggle window to left/right
```

### Основные комманды:

```
man <command>       : справка (или <command> --help или info <command>)
clear               : очистить экран терминала (ctrl + L)
reset               : реинициировать терминал
exit                : закрыть терминал
pwd                 : напечатать рабочую директорию
ls <path>           : список папок (-h удобный размер,-l списком,-a все ф и п)
tree                : отобразить структуру подпапок и файлов
cd <path>           : сменить директорию
mkdir <path>        : создать директорию (~/dir{1..5}.txt, ~/{dir1,dir2}.txt)
touch <path>        : создать файл (~/file{1..5}.txt, ~/{file1,file2}.txt)
rm <path>           : удалить файл/директорию (-r дир.,-rf дир. без вопросов)
cp <path1> <path2>  : скопировать файл/директорию (-r дир.)
mv <path1> <path2>  : переместить файл/директорию
mc                  : файловый менеджер midnight commander
shutdown            : выключение
reboot              : перезагрузка

~                   : /home/user
/                   : / (root)
..                  : на уровень выше
.                   : текущая директория
-                   : назад
*                   : любое кол-во любых символов
?                   : один любой символ

root directory:
/bin                : standard executables
/sbin               : important system executables
/etc                : system configuration files
/var                : frequently updated files like logs
/root               : home directory of the administrator account
/home               : a user account home directories (/Users on a Mac)
/opt                : package-manager installed files
/tmp                : temporary files; usually wiped between boots
/usr                : user applications and utilities
```

### Ввод/вывод:

```
cat <file>          : вывести содержимое файла на экран
less <file>         : открыть для чтения (q выход, / поиск, g/G начало/конец)
nano <file>         : открыть для редактирования (ctrl + x — выход)

Standart Input  -->  PROGRAM  -->  Standart Output
(keybord/files)         I          (screen by def)
                        V                         
                   Standart Error                 
                  (screen by def)                 

<program> <   <file>: брать stdin из файла
<program> >   <file>: выводить stdout в файл
<program> >>  <file>: выводить stdout в файл с дозаписью
<program> 2>  <file>: выводить stderr в файл
<program> 2>> <file>: выводить stderr в файл с дозаписью
(/dev/null переправление в никуда)
```

### Работа с программами:

```
chmod +x <program>            : сделать программу исполняемой (executable)
<prog1>|...|<progN>           : конвеер(pipe) (stdout[i] = stdin[i+1])
./<file>                      : запустить (в текущей директории)
<program> <filepath>          : запустить (файл программы)
<program> &                   : запустить программу в фоновом режиме (bg)
sh <filepath>                 : запустить (файл shell)

sudo apt-get install <prog>   : установить программу (--only-upgrade)
             remove  <prog>   : удалить программу
             update           : обновить ссылки на пакеты
             upgrade          : обновить все программы
```

-------------------------------------------------------------------------------
## II. Работа на сервере

```
IP (internet protocol) адреса — приватные и публичные (IPv4 и IPv6).
приватные: 10.x.x.x, 172.16.x.x-172.31.x.x, 192.168.x.x

curl ifconfig.me                               : узнать свой публичный IP
ip a (или hostname -I | awk '{print $1}')      : узнать свой приватный IP
ssh <login>@<server_address> -p <port>         : войти на сервер (exit: выйти)
(Чтобы каждый раз не вводить пароль используют ключи авторизации)

scp -P <port> <login>@<server>:<path1> <path2> : копировать сервер → клиент
scp -P <port> <path1> <login>@<server>:<path2> : копировать клиент → сервер
(Также можно исп-ть файловые менеджеры, например, filezilla)
```

### Скачивание файлов:

```
wget <link>         : скачать файл в текущюю директорию

options:
-P <path>           : сохранить в указанной директории
-O <path>           : сохранить под указанным именем
-i <file.txt>       : скачать файлы по ссылкам из текстового файла
--spider            : проверить доступность файла
-r -l <depth>       : рекурсивное скачивание с заданно глубиной
-A <type1>,...      : список разрешённых расширений
-R <type1>,...      : список запрещённых расширений
```

-------------------------------------------------------------------------------
## III. Работа с программами

```
ctrl + C            : прервать программу
ctrl + Z            : приостановить программу (далее fg или bg)

jobs                : посмотреть запущенные программы
fg <#>              : продолжить выполнение программы
bg <#>              : продолжить выполнение программы в фон.реж. (или <prog> &)
history             : посмотреть историю команд (-c очистить)
ps                  : посмотреть запущенные процессы (-aux)
top                 : смотреть процессы в реальном времени (-u <user> польз-ля)
kill <#>            : завершить процесс (-9 "убить" процесс)
```

### Информация о системе:

```
uname -a            : общая системная информация
lsb_release -a      : инфо о версии ОС
ip addr             : инфо о состоянии сети
free -h             : оперативная память
nproc               : число ядер
lscpu               : инфо о процессоре
df -h               : инфо о жёстком диске (du -cksh для папки) (--max-depth 1)
```

### Работа с архивами:

```
unzip <arc.zip>               : распаковать архив .zip
gunzip <arc.gz>               : распаковать архив .gz и удалить (-c без удал.)
tar -xvf <arc.tar>            : распаковать архив .tar
tar -xzvf <arc.tar.gz>        : распаковать архив .tar.gz
zip <arc.zip> <file1>...      : архивировать файлы/папки в .zip
gzip <arc.gz> <file>          : архивировать файл в .gz и удал. (-c без удал.)
tar -cvf <arc.tar> <file1>... : архивировать файлы/папки в .tar (-zcvf и в .gz)

bzip2 <file>                  : tar -cjvf <arc.tar.bz2> <file>
bunzip2 <arc.bz2>             : tar -xjvf <arc.tar.bz2>
```

### Поиск файлов и слов:

```
find -name <file>   : найти файл (можно в дир. если <path> перед -name)
grep <line> <file>  : найти строку в файле (-с N раз?, -r найти в файлах папки)
wc <opt> <path>     : посчитать <opt> в файле (-l строки -w слова -c символы)
diff <path1> <path2>: сравнить файлы/директории
```

-------------------------------------------------------------------------------
## IV. Скрипты на bash

**Shell** (оболочка) — интерпретатор команд, может выполнять скрипты (sh, bash,...).

Создание скрипта:
1. `touch script.sh`
2. `gedit script.sh &`

```
#!/bin/bash (путь до интерпретатора)
echo "Hello, World!"
# comments (except first line)
```
3. `chmod +x script.sh`
4. `./script.sh или bash script.sh`

### Переменные:

```
<name> = <value>    : запись значения переменной
$<name> or ${<name>}: чтение значения переменной

Напр:
1. path1 = ~/Docs
   path2 = $path1/file.txt    # path2 = ~/Docs/file.txt
   echo "Path is $path2"      # Path is ~/Docs/file.txt
   echo "Path is ${path1}"    # Path is ~/Docs

2. #!/bin/bash
   d_path = ~/downloads
   f_path = $d_path/file.txt
   echo "Creating file $f_path"
   touch $f_path
   echo "Checking content of dir $d_path"
   ls $d_path

3. let "value = a + b"        # *,/,+,-,%,**,+=,-=,...
```

### Аргументы скрипта:

```
Передача аргументов скрипту : ./script.sh <arg1> ... <argN>
Обработка внутри скрипта    : $1,...,$N  аргументы 1,...,N
                              $0         имя скрипта
                              $#         кол-во аргументов

Напр:
1. var = "First argument is $1"
   echo "There are $# arguments"

2. #!/bin/bash
   var1 = $1
   var2 = $2
   echo "Arguments are $var1 and $var2"
```

### Условные конструкции:

```
1.  if   [[ <cond1> ]]              -z <line> : строка пуста?       
    then                            -h <line> : строка не пуста?    
        <comm1>                                                     
    elif [[ <cond2> ]]              !,&&,||   : NOT,AND,OR          
    then                            == (-eq)  != (-ne)              
        <comm2>                     <  (-lt)  >  (-gt)              
    else                               (-le)     (-ge)              
        <comm3>                     (... для строк  (...) для чисел)
    fi                                                              
                                    -e <path> : путь сущ-ет?        
2.  case <var> in                   -f <path> : это файл?           
    <val1>) #[val1-val2] для диап.  -d <path> : это директория?     
        <comm1>                     -s <path> : размер файла > 0?   
        ;;                          -x <path> : файл исполняемый?   
    ...                                                             
    <valN>)                                                         
        <commN>                                                     
        ;;                                                          
    *)                                                              
        <commN+1>                                                   
    esac                                                            
```

### Циклы и функции:

```
1.  for <var> in <values_list>      # <values_list> через пробелы              
    do                              # break, continue                          
        <comm1>                     # read <var> : записать введённок польз-ем 
    done                            #              значение в переменную       

2.  while [[ <cond> ]]
    do
        <comm2>
    done

3.  <function> ()                   # вызов: <function> <arg1> .... <argN>     
    {                               # глобальные и локальные переменные:       
        <comm. with $1,...,$N>      # {... var_global = ...                    
    }                               #  ... local var_local = ...}              
```

-------------------------------------------------------------------------------
## V. Настройка системы

### Права доступа:

```
users               : узнать, кто в системе
adduser <new_user>  : добавить нового пользователя (и passwd <new_user>)
userdel -r <user>   : удалить пользователя и его домашний каталог
less /etc/passwd    : узнать всех пользователей <user>:x:<id>
                      (id>1000: наст.польз. id<1000: сист.службы)
groups <user>       : узнать группы пользователя
sudo <command>      : выполнить комманду от имени пользователя root
ls -l <path/file>   : узнать права доступа файлов

Вывод   : drwxrwxr-x N <user> <group> size date file, где:

d/-     : папка или файл
rwx/--- : чтение, запись, доступ/исполнение для пользователя, группы, остальных
N       : число хард связи (дополнительное имя файла)
<user>  : владелец папки или файла
<group> : группа владельца папки или файла
size    : размер папки или файла
date    : дата и время последнего изменения
file    : имя папки или файла

chmod ### <file>    : установить права доступа (### — 3 числа)
```

| Восьмеричное | Двоичное |
|:------------:|:--------:|
|      0       |    ---   |
|      1       |    --x   |
|      2       |    -x-   |
|      3       |    -xx   |
|      4       |    x--   |
|      5       |    x-x   |
|      6       |    xx-   |
|      7       |    xxx   |

```
chmod [ugoa][+-=][rwx] <path> : изменить права доступа, где:

ugoa                : user, group, other, all
+-                  : добавить или забрать права
rwx                 : read, write, execute

Примеры:
u+x                 : право выполнения владельцу
ug=rw,o=r           : владельцу и группе — чтение/запись, остальным — чтение
a-x                 : все лишаются права выполнения
g=u                 : группе назначаются такие же права, что и владельцу
```

### Удобная история команд

1. Открыть `~/.inputrc`
2. Вставить следующее:
```
"\e[A": history-search-backward
"\e[B": history-search-forward
"\e[C": forward-char
"\e[D": backward-char
```
3. Теперь при вводе пары символов и нажатии кнопки вверх команды перебираются не в хронологическом порядке, а в порядке релевантности.

### Virtual Box:

**ВАЖНО**:
Чтобы эмулировать 64 битные системы, нужно включить в биосе VT-d и Intel Virtual Technology.

```
Полноэкранный режим : Устройства - Образ гост.ОС - ... (или sh ...)
Общие папки         : 1. автоподключение (yes)
                      2. sudo adduser <user> vboxsf
                      3. reboot/relogin
```

### Переменные окружения:

```
alias rm='rm -i'    : изменить или задать комманды для текущего окна терминала
(без пробелов)        (напр: подтверждение удаления rm)
echo $<var>         : вывести <var> (локальны для каждой вкладки терминала)
env                 : вывести все текущие переменные
export <var> = '...': задать значение переменной (export PATH='$PATH:<dir>')
                      (напр: PATH дир.зап-ых файлов, HOME дом.дир.)
unset <var>         : вернуть значение <var> по умолчанию (или export <var>= )

Чтобы изменить постоянно:
~/.profile (переменные окружения)
~/.bashrc  (алиасы)
~/.inputrc

PowerShell          : Get-Alias
```

### Установка с USB:

1. Скачать iso файл.
2. Записать его на флешку с помощью rufus.
3. Поменять в BIOS настройки запуска.
4. Загрузится и установить систему.
