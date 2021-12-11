# 21

Moulinette https://moulinette.msk.21-school.ru/

Last Of Olds http://jcorwin.ru/

FAQ Школы 21 для новичков и не очень https://github.com/daniiomir/faq_for_school_21

amatilda's memory_leaks_manual https://github.com/daniiomir/faq_for_school_21/blob/master/docs/memory_leaks_amatilda.pdf

GNU make https://www.gnu.org/software/make/manual/make.html

42-exam-rank-02 https://github.com/Glagan/42-exam-rank-02

42-exam-rank-03 https://github.com/Glagan/42-exam-rank-03

my 42-exam-rank-04 https://github.com/lelderbe/exam04 

examrank-02-03-04-05-06 https://github.com/markveligod/examrank-02-03-04-05-06

Что нужно и чего не нужно делать во время Code Review: https://apptractor.ru/info/articles/chto-nuzhno-i-chego-ne-nuzhno-delat-vo-vremya-code-review.html

# Лайфхаки

```bash
# Удалили руками .brew и теперь не удаётся поставить? Пишем в терминал и запускаем:
$ curl -fsSL https://rawgit.com/kube/42homebrew/master/install.sh | zsh

# Разбивка аргументов типа "1 2 3 4" на части в zsh:
$ setopt sh_wordsplit

# Проверка на утечки перед выходом из программы:
$ leaks --atExit -- ./a.out
    
# Для Visual Studio Code есть расширение, позволяющее работать по SSH с файлами на другом хосте:
# https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack
```

# Проекты и ресурсы по ним

[libft](#libft) | [get_next_line](#get_next_line) | [ft_printf](#ft_printf) | [minitalk](#minitalk) | [ft_server](#ft_server) | [minishell](#minishell) | [ft_services](#ft_services) | [cub3d](#cub3d) | [libasm](#libasm) | [push_swap](#push_swap) | [Philosophers](#Philosophers) | [C++](#c) | [Inception](#Inception)

Лекции без спойлеров: #coding_wiki https://www.notion.so/coding_wiki-1d8b8bc675f5426db90a02dd22324ac8

Чеклисты: school21-checklists https://github.com/mharriso/school21-checklists https://github.com/caecitasminimus/school21-checklists https://github.com/brazhenko/school21-checklists

## Inception

Установка docker на ubuntu: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-ru


## C++

Столяров со стр. 93 "10. Язык C++": https://disk.yandex.ru/i/9bylKcEGPWJlyw

Intra: https://elearning.intra.42.fr/tags/38/notions

C++ Reference: http://www.cplusplus.com/reference/

Google C++ Style Guide: https://google.github.io/styleguide/cppguide.html

### cpp00 - basics

### cpp01 - new, delete, references, filestreams, Karen

How can I convert a std::string to int? [Самый простой способ преобразовать int в string в C++](https://coderoad.ru/5590381/%D0%A1%D0%B0%D0%BC%D1%8B%D0%B9-%D0%BF%D1%80%D0%BE%D1%81%D1%82%D0%BE%D0%B9-%D1%81%D0%BF%D0%BE%D1%81%D0%BE%D0%B1-%D0%BF%D1%80%D0%B5%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D1%8C-int-%D0%B2-string-%D0%B2-C) https://stackoverflow.com/questions/7663709/how-can-i-convert-a-stdstring-to-int https://stackoverflow.com/a/6154614

Объект stringstream не обновляет значение: https://stackoverflow.com/questions/13891856/cannot-overwrite-stringstream-variable-with-a-new-value

Array of functions http://www.cplusplus.com/forum/beginner/4639/

### cpp02 - function overloading, operator overload, canonical form

Orthodox canonical class form: https://www.francescmm.com/orthodox-canonical-class-form/

### cpp03 - inheritance, diamond inheritance

Multiple Inheritance in C++ https://www.geeksforgeeks.org/multiple-inheritance-in-c/

### cpp04 - sub-typing polymorphism (RTTI), abstract classes, interfaces, deep object copying

### cpp05 - nested classes, exceptions

### cpp06 - C++ casts - преобразования типов через static_cast, dynamic_cast и т.п.

### cpp07 - шаблоны функций (template<T>)

### cpp08 - использование STL

C++: “undefined reference to” templated class function: https://stackoverflow.com/questions/10632251/undefined-reference-to-template-function https://bytefreaks.net/programming-2/c/c-undefined-reference-to-templated-class-function

## Philosophers

    Цель проекта: научиться взаимодействовать из нескольких параллельных потоков (философы)
    с общими разделяемыми ресурсами (вилки, печать) избегая дедлоков.

🔥 Unix Threads in C: https://www.youtube.com/playlist?list=PLfqABt5AS4FmuQf70psXrsMLEDQXNkLq2

Столяров со стр. 529 "7. Параллельные программы и разделяемые данные" https://disk.yandex.ru/i/UOfHiR8f1AgVWA

Без спойлеров: https://www.notion.so/Philosophers-4a4982d5c1aa4e2db3a8cfd2df7bd1cd

    Отображение всех потоков процесса (Linux):
    ps -T -p <pid>
    
    Должны жить:
    3 310 100 100
    3 310 100 80
    3 310 80 100
    
    Никто не должен умереть:
    3 310 100 100 1
    3 310 100 300 1
    
    Должна завершиться работа после смерти без задержки:
    3 310 200 10000
    3 310 20000 100

## push_swap

    Цель проекта: реализовать алгоритм сортировки стека с как можно меньшим количеством операций
    в условиях ограниченного набора команд и с возможностью использования второго стека.
    
    Для последовательности из 3 чисел: должно быть не больше 3 инструкций
    Для последовательности из 5 чисел: должно быть не больше 12 инструкций
    Для последовательности из 100 чисел: <700 инструкций на 5 баллов
    Для последовательности из 500 чисел: <5500 инструкций на 5 баллов

С чего начать?
1. Конечно же с Makefile!
2. Создать структуру, которая будет содержать стеки (двунаправленные списки или массивы) и прочие служебные поля.
3. Реализовать операции со стеками (pa, ra, sb и т.д.) в виде функций, которые будем просто вызывать, а они уже сами сделают необходимые действия со стеками и напечатают выполненную операцию на экран.
4. Реализовать типичные операции для просмотра элементов в стеке - мы ведь имеем возможность видеть и анализировать всё содержимое стека. Так что, прежде чем выполнять какие-нибудь операции, можно просчитать, что будет лучше. И чтобы было проще, оформим это всё в отдельных функциях, например, таких как: получить значение элемента по индексу, получить индекс элемента по значению, проверить наличие элемента в стеке, получить позицию в противоположном стеке, куда следует вставить этот элемент, поднять минимальный элемент (прокрутить стек) на самый верх и т.п.
5. Также понадобится очередная реализация atoi под этот конкретный проект (входные числа вида "1a" здесь не подойдут). Плюс любые вспомогательные функции (сравнение строк, минимум двух чисел и т.п.).
6. Реализовать алгоритмы сортировки 2х и 3х чисел. На них проверить, как всё работает. Порадоваться :)

Каркас готов, до этого момента был просто внимательный кодинг вспомогательных функций. Осталось добавить алгоритм сортировки для большего количества входных данных. Здесь достаточно чего-нибудь простого, главное реализовать без ошибок (я три дня не мог продвинуться с проектом, пока не обнаружил ошибку в логике работы - а уже начал думать, что я безнадёжен).

За основу я брал алгоритм сортировки вставками (Insertion sort). Идея: перебирать элементы и вставлять в нужное место в результирующем стеке. В итоге получился вот такой простой план действий:
<details>
  <summary>Спойлер: алгоритм</summary>

1. Перекидываем все элементы в стек B, чтобы стек A оказался пуст. Теперь в стек A будем переносить элементы в отсортированном порядке (но не обязательно начинать с наименьшего элемента).
    
2. Для этого просчитываем для каждого элемента в стеке B стоимость его переноса в стек A, т.е. сколько операций необходимо будет произвести с обоими стеками, чтобы вставить элемент в нужную позицию. Выбираем элемент с наименьшей стоимостью и производим действия, необходимые для его переноса (прокрутка стеков, push a).

3. Повторять пункт 2, пока стек B не станет пуст)

Этого алгоритма ПОЧТИ достаточно, чтобы сдать на отлично. Выдаст ~6000 для 500 чисел (с улучшениями 4200 - 4500), и ~630 для 100 чисел.

Как можно улучшить: комбинировать операции прокрутки стеков (например: одновременные операции ra и rb заменять на rr), на шаге 1 перебрасывать в массив B с минимальной сортировкой (точнее, группировкой).

</details>

В процессе выполнения проекта познакомился с radix sort - интересная поразрядная сортировка, которой вообще ничего не нужно знать об элементах стека, просто над каждым элементом необходимо произвести нужные действия. С radix можно сдать проект на среднюю оценку и при этом написать по минимуму логики.

----

Варианты алгоритмов:

от VBrazhnik: https://github.com/VBrazhnik/Push_swap/wiki/Algorithm

от asipes: https://vk.com/@forum42intra-push-swap

от Jamie Dawson: https://medium.com/@jamierobertdawson/push-swap-the-least-amount-of-moves-with-two-stacks-d1e76a71789a

от Leo Fu - radix sort: https://medium.com/nerd-for-tech/push-swap-tutorial-fa746e6aba1e

Визуализатор процесса сортировки: https://github.com/o-reo/push_swap_visualizer

Ещё один текстовый визуализатор и пара видео под ним: https://github.com/rizky/42-push_swap

```bash
# чтобы zsh разбивал строку на элементы, как bash
$ setopt sh_wordsplit
    
# количество операций
$ ARG="4 67 3 87 23"; ./push_swap $ARG | wc -l
$ ARG=`ruby -e "puts (1..5).to_a.shuffle.join(' ')"`; echo $ARG ; ./push_swap $ARG | wc -l
    
# проверка чекером
$ ARG="4 67 3 87 23"; ./push_swap $ARG | ./checker_Mac $ARG
$ ARG=`ruby -e "puts (1..5).to_a.shuffle.join(' ')"`; echo $ARG ; ./push_swap $ARG | ./checker_Mac $ARG
    
# запуск визуализатора
$ ./pyviz.py `ruby -e "puts (1..100).to_a.shuffle.join(' ')"`
    
# проверка на утечки перед выходом
$ leaks --atExit -- ./push_swap 1 5 2 4 3
```

## minishell

Без спойлеров: https://www.notion.so/minishell-imicah-a341793fc312485b90020fe950f6d5df

Без спойлеров termcap: https://www.notion.so/minishell-termcap-sgertrud-dcc3fcbae6d14d24bb3fb50e1b5a04b9

42Docs: https://harm-smits.github.io/42docs/projects/minishell

🔥 Unix Processes in C: https://www.youtube.com/playlist?list=PLfqABt5AS4FkW5mOn2Tn9ZZLLDwA3kZUY

🔥 Столяров со стр. 336 "5.3 Процессы" https://disk.yandex.ru/i/UOfHiR8f1AgVWA

Дэвид Гриффитс, Дон Гриффитс Изучаем программирование на C - стр. 434 "Процессы и системные вызовы" https://disk.yandex.ru/i/UeZRu-JJqSqeqA

Bash Reference Manual - https://www.gnu.org/software/bash/manual/bash.html

https://pubs.opengroup.org/onlinepubs/009695399/utilities/xcu_chap02.html

```bash
# Проверка не закрытых fd-шников:
$ lsof -c minishell

# Интересные кейсы:
$ yes | yes | head
$ cat | ls

# запустить minishell без переменных окружения
$ env -i ./minishell

# запустить ls без "./"
$ unset PATH
$ cd /bin
$ ls

# замена переменной окружения на значение
$ export AA="1       444        5"
$ echo $AA
1 444 5

$ export $FOLDER="/bin no_such_dir"
$ cd $FOLDER
```

## ft_services

<details>
  <summary>Project deprecated</summary>

    Самый простой и быстрый путь к полностью функционирующему кластеру
    Kubernetes – использовать инструмент Minikube. Minikube – это инструмент,
    который настраивает одноузловой кластер. Такой кластер отлично подходит
    как для тестирования системы Kubernetes, так и для разработки приложений
    локально.
    
    Minikube запускает Kubernetes внутри виртуальной машины, запущенной через VirtualBox,
    поэтому, прежде чем вы сможете запустить кластер Minikube, вам также нужно установить VirtualBox.
    
    Взаимодействие с кластером через: kubectl.

Важное:

    Если ошибки с DNS в VirtualBox - использовать alpine:3.12

    // указать в zsh minikube использовать /goinfre. Не забыть после команды перезапустить терминал!
    echo "export MINIKUBE_HOME=/goinfre/$USER" >> ~/.zshrc

Без спойлеров: https://www.notion.so/ft_services-e0700a527d0d45039388f65087c23b21

🔥 От Докера к K8s: https://m.habr.com/ru/company/ruvds/blog/438982/ https://m.habr.com/ru/company/ruvds/blog/438984/

Что такое Kubernetes (оф.сайт): https://kubernetes.io/ru/docs/concepts/overview/what-is-kubernetes/

🔥 Kubernetes в действии (книга на русском): https://disk.yandex.ru/i/d2oWpYUiDCCi-w

☝️ Настройка Minikube HOME folder: https://stackoverflow.com/questions/45947551/minikube-home-folder https://minikube.sigs.k8s.io/docs/handbook/config/#exclusive-environment-tunings

Зачем eval $(minikube docker-env): https://stackoverflow.com/questions/42564058/how-to-use-local-docker-images-with-minikube

Группа в ТГ: https://t.me/joinchat/VgygI_iu76nosxxn

Minikube documentation: https://minikube.sigs.k8s.io/docs/

42Docs: https://harm-smits.github.io/42docs/projects/ft_services

Путеводитель по Kubernetes для детей. В картинках: https://www.itsumma.ru/press/kinder-kubernetes

A visual guide on troubleshooting Kubernetes deployments: https://habr.com/ru/company/flant/blog/484954/ https://learnk8s.io/troubleshooting-deployments

Dockerized nginx is not starting https://stackoverflow.com/questions/24241292/dockerized-nginx-is-not-starting

Run multiple services in a container: https://docs.docker.com/config/containers/multi-service_container/

Kubernetes Tutorial for Beginners [FULL COURSE in 4 Hours]: https://www.youtube.com/watch?v=X48VuDVv0do&ab_channel=TechWorldwithNana

Examples: https://github.com/container-examples

Example: Deploying WordPress and MySQL with Persistent Volumes: https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume/

Kubernetes CheatSheet: https://github.com/dennyzhang/cheatsheet-kubernetes-A4

    brew install minikube
    minukube version
    minikube addons list
    
    kubectl version                     // are you there?
    kubectl cluster-info                // информация о кластере
    kubectl get nodes                   // общая информация о нодах
    kubectl describe node minikube      // подробная информация о конкретной ноде
    kubectl get all                     // информация сразу по подам/сервисам/деплоям
    kubectl delete deployment <name>    // удалить развёртывание (по аналогии - и остальное)
    kubectl exec -it <pod> -- sh        // зайти внутрь пода через консоль
    
    //Volumes
    kubectl get pv                      // show PersistentVolumes (не актуально для minikube)
    kubectl get pvc                     // show PersistentVolumeClaims 

#mysql

    > SHOW VARIABLES LIKE 'skip_networking';
    should be OFF for network connections

#influxdb

    Есть в репозитории, установить, создать файл конфигурации, подключить том PVC
    apk add influxdb

</details>
    
## libasm

    Цель проекта: переписать несколько функций, которые писали в либе на Си, но теперь
    на более низкоуровневом языке. Понять, как всё работает, почувствовать разницу :)

Важное:

    В 64-битных программах первые шесть аргументов передаются через регистры: rdi, rsi, rdx, rcx, r8, r9.
    В 32-битных - аргументы передаются через стек.
    
    Возвращаемое значение из функции передаётся через rax и, если потребуется, также через rdx.
    
    Следующие регистры обязательно нужно сохранять (push) и восстановливать их значения (pop)
    перед выходом из функции: rbp, rbx, r12, r13, r14, r15.

Памятка: https://www.notion.so/LibASM-ddd4ac8ffb834c19a9e85ee1b1ca685b#78266914c2614a29897ed769b8a35b59

MacOS syscalls (0x2000000 + код из таблицы): https://opensource.apple.com/source/xnu/xnu-1504.3.12/bsd/kern/syscalls.master

_ _ _error errno explanation: http://www.za.freebsd.org/doc/en_US.ISO8859-1/books/developers-handbook/x86-return-values.html

System call error handling http://osr600doc.xinuos.com/en/SDK_sysprog/SCL_SysCallErrHdl.html http://cs.wellesley.edu/~cs249/Lectures/System-Calls-Error-Handling/system-calls-error-handling.html

x86 Assembly Crash Course (вводное видео) https://www.youtube.com/watch?v=75gBFiFtAb8

NASM Tutorial https://cs.lmu.edu/~ray/notes/nasmtutorial/

NASM doc https://www.nasm.us/xdoc/2.15.05/nasmdoc.pdf

x86_64 NASM Assembly Quick Reference ("Cheat Sheet") https://www.cs.uaf.edu/2017/fall/cs301/reference/x86_64.html

x86 Assembly Guide https://www.cs.virginia.edu/~evans/cs216/guides/x86.html

Debug: lldb + Voltron https://github.com/snare/voltron

    $ lldb a.out
    r               ; run
    b _ft_strlen    ; set breakpoint to function
    n               ; next instruction
    
    в другом окне:
    voltron view d  ; show code
    voltron view r  ; show registers
    etc..
    
    ~/.zshenv
    export PATH="/Users/$USER/Library/Python/3.7/bin:$PATH"

Чекер (если он вам всё же нужен): https://github.com/cacharle/libasm_test (нужен python3: brew install python3)

42Docs: https://harm-smits.github.io/42docs/projects/libasm.html

Группа в ТГ: https://t.me/joinchat/SLHcFZEh4lZMKPi0

## cub3d

Без спойлеров: https://www.notion.so/Cub3D-fd79729951a84906807af2b252f1d0bc

42 Docs MiniLibX https://harm-smits.github.io/42docs/libs/minilibx

wolf3d https://github.com/qst0/ft_libgfx#wolf3d

Game engine BLACK BOOK Wolfenstein 3D https://disk.yandex.ru/i/6CfkIoCfjahmtg

MiniLibX - Simple Graphical Interface Library for students https://qst0.github.io/ft_libgfx/man_mlx.html

Зачем нужны синусы и косинусы? https://www.youtube.com/watch?v=hwpWTkdh-BA

Bits to Bitmaps: A simple walkthrough of BMP Image Format https://medium.com/sysf/bits-to-bitmaps-a-simple-walkthrough-of-bmp-image-format-765dc6857393

Raycasting engine rendering creating slight distortion increasing towards edges of screen (выравниваем стены) https://stackoverflow.com/a/24206301

Как сделать 3D Игру на Python с Нуля [ Pygame ] https://www.youtube.com/watch?v=SmKBsArp2dI&list=PLzuEVvwBnAsZGeSVhOXpnW-ULsGYpNyQe

For Coderz - RAYCASTING - сделай себе немного DOOM'a. Алгоритм трассировки 3D лабиринта как в игре WOLF. https://zxpress.ru/article.php?id=8482

Рейкастинг для самых маленьких https://proglib.io/p/raycasting-for-the-smallest

ONLINE IMAGE COLOR PICKER https://pinetools.com/image-color-picker

## ft_server

<details>
  <summary>Project deprecated</summary>

    Цель проекта: познакомиться с системным администрированием и контейнеризацией,
    как альтернативой полноценным виртуальным машинам.
    Попотеть над настройкой разных сервисов(

Основы Docker. Большой практический выпуск https://www.youtube.com/watch?v=QF4ZF857m44

Docker самый простой и понятный туториал. Изучаем докер, так, если бы он был игровой приставкой https://badcode.ru/docker-tutorial-dlia-novichkov-rassmatrivaiem-docker-tak-iesli-by-on-byl-ighrovoi-pristavkoi/

Get started with Docker Machine and a local VM https://eternalhost.net/blog/razrabotka/chto-takoe-docker

Docker Tutorial For Beginners: https://www.youtube.com/watch?v=o5af1LBgAFw&ab_channel=Simplilearn

--

Start containers automatically: https://docs.docker.com/config/containers/start-containers-automatically/

    Mac sed:
    sed -i '' 's/old_text/new_text/' $FILENAME

</details>

## minitalk

    Цель проекта: передать от процесса-клиента на процесс-сервер строку текста, используя только сигналы.
    
    PS нет, строку текста, как она есть, никак не передать с помощью сигналов - надо что-то придумать.

Столяров - 5.3 Процессы (стр. 338)  https://disk.yandex.ru/i/UOfHiR8f1AgVWA

Code Vault: https://www.youtube.com/watch?v=5We_HtLlAbs&list=PLfqABt5AS4FkW5mOn2Tn9ZZLLDwA3kZUY&index=16

Спойлер: Передача файла сигналами - https://habr.com/ru/post/122823/

## ft_printf

Без спойлеров: https://www.notion.so/ft_printf-3e358ed673d14164b88de9eb428f3c6a

Чекеры: https://github.com/gavinfielder/pft https://github.com/Mazoise/42TESTERS-PRINTF https://github.com/charMstr/printf_lover_v2 https://github.com/cacharle/ft_printf_test

## get_next_line

Без спойлеров: https://www.notion.so/get_next_line-59fb1381311b4867b4cfaeec5b94c193

Чекеры: https://github.com/Mazoise/42TESTERS-GNL https://github.com/charMstr/GNL_lover

## libft

    Цель проекта: написать требуемые функции и собрать их в библиотеку,
    которую можно будет использовать в последующих проектах.
    
Makefile: видео в Интре с бассейна

Makefile от saugustu: https://www.notion.so/Makefile-6c182588c3064bfd8b72d97f66be708c

Чекеры: https://github.com/jtoty/Libftest https://github.com/ska42/libft-war-machine https://github.com/alelievr/libft-unit-test

# Книги

Brian_Kernighan_Dennis_Ritchie-The_C_Programming_Language-RU: https://disk.yandex.ru/i/IsiG-LyAD4x0tg

Стандарт Си: https://disk.yandex.ru/i/u20PseJbNLYMNw

Столяров 1: https://disk.yandex.ru/i/sKUkM3D_BqfSrw 2: https://disk.yandex.ru/i/UOfHiR8f1AgVWA 3: https://disk.yandex.ru/i/9bylKcEGPWJlyw

Дэвид Гриффитс, Дон Гриффитс Изучаем программирование на C: https://disk.yandex.ru/i/UeZRu-JJqSqeqA
