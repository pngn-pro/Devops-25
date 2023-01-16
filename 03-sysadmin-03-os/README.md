1. chdir("/tmp")
2. openat(AT_FDCWD, "/usr/share/misc/magic.mgc", O_RDONLY) = 3 (strace -f file)

3. lsof -p 12664 <br>
bash 12664 alexander   2r      REG                0,1     6122   2079 /var/log/test-delete.log (deleted)
<br>
echo '' > /proc/12664/fd/2
4. Зомби-процессы освобождают ресурсы
5. В федоре не заработало никак, запускал через vagrant/ubuntu.
openat(AT_FDCWD, "/etc/ld.so.cache", O_RDONLY|O_CLOEXEC) = 3
<br>
openat(AT_FDCWD, "/usr/lib/x86_64-linux-gnu/libmagic.so.1", O_RDONLY|O_CLOEXEC) = 3
<br>
openat(AT_FDCWD, "/usr/lib/x86_64-linux-gnu/libmagic.so.1", O_RDONLY|O_CLOEXEC) = 3

6.    Part of the utsname information is also accessible  via  /proc/sys/ker‐
       nel/{ostype, hostname, osrelease, version, domainname}.
   7.  ; - Это разделитель команд,
       && - Логический оператор
   Т.е. В примере с ; будет выполнены перечисленные команды, когда с && Вторая команда будет выполнена в случае успеха первой.
   <br>
   **Set -e** - немедленный выход, если выходное состояние команды ненулевое.
   Нет смысла использовать, так как команда завершится.
8. <br> 
**-e** - останавливает выполение команды при ошибке.<br>
**-u** - Незаданные параметры считаются ошибкой, без выхода интерактивной оболочки<br>
**-x** - Трассировка ошибок<br>
**-o** - Запись текущих настроек в стандартный вывод.<br>
9. S/Ss/Ssl/I< <br>
Вторые-третьи символы это характеристики процесса. Высокий/низкий приотритет, многопоточность.