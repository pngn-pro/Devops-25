2.CPU: 2
memory: 1024
3. Дописать конфигурацию, что бы выглядело так:
Vagrant.configure("2") do |config|
        config.vm.box = "bento/ubuntu-20.04"
        config.vm.provider "virtualbox"  do |v|
                v.memory = 2048
                v.cpus = 2
end
end

Это нам даст 2 CPU, и 2048 Мб памяти.

4. 
![](/home/alexander/Изображения/Снимки экрана/vagrant-2.png)
5. 
5.1 history-size. 30 строка (man bash | less -N)
5.2 Значение ignoredups приводит к тому, что строки, соответствующие предыдущей записи истории, не сохраняются.
Значение ignoreboth является сокращением для ignorespace и ignoredups.
6. 412 Строка. "Когда увеличивается позиционный параметр, состоящий более чем из одной цифры, он должен быть заключен в фигурные скобки"
7. 
touch ./file{1..100000}
7.2 Создать 300000 файлов не получится. "bash: /usr/bin/touch: Слишком длинный список аргументов"

8. Это сокращение программы test. В данном примере проверяется существует ли файл и является он каталогом.

9. 
![](/home/alexander/Изображения/Снимки экрана/9.png)
#mkdir -p /tmp/new_path_directory/

#cp /bin/bash /tmp/new_path_directory/

#export PATH=

#export PATH="/tmp/new_path_directory/:/root/miniconda3/bin:/root/miniconda3/condabin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin"

10. Команда at -- используется для запуска заданий в заданное время.

batch	указывает системе запускать задание только в указанное время

11. Virtualbox установил, ubuntu поставил, но выполнял всё на домашней машине :)
