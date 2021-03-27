# 21

Moulinette https://moulinette.msk.21-school.ru/

Last Of Olds http://jcorwin.ru/

FAQ Школы 21 для новичков и не очень https://github.com/daniiomir/faq_for_school_21

amatilda's memory_leaks_manual https://github.com/daniiomir/faq_for_school_21/blob/master/docs/memory_leaks_amatilda.pdf

GNU make https://www.gnu.org/software/make/manual/make.html

42-exam-rank-02 https://github.com/Glagan/42-exam-rank-02

42-exam-rank-03 https://github.com/Glagan/42-exam-rank-03

examrank-02-03-04-05-06 https://github.com/markveligod/examrank-02-03-04-05-06


# Проекты и ресурсы по ним

Лекции без спойлеров: #coding_wiki https://www.notion.so/coding_wiki-1d8b8bc675f5426db90a02dd22324ac8

Чеклисты: school21-checklists https://github.com/secondfry/school21-checklists

## ft_services

Без спойлеров: https://www.notion.so/ft_services-e0700a527d0d45039388f65087c23b21

Что такое Kubernetes https://kubernetes.io/ru/docs/concepts/overview/what-is-kubernetes/

Kubernetes в действии (книга на русском): https://disk.yandex.ru/i/d2oWpYUiDCCi-w

Настройка Minikube HOME folder: https://stackoverflow.com/questions/45947551/minikube-home-folder

Minikube lives here (просто для инфо): https://github.com/kubernetes/minikube

Dockerized nginx is not starting https://stackoverflow.com/questions/24241292/dockerized-nginx-is-not-starting

    Если ошибки с DNS в VirtualBox - использовать alpine:3.12
    
    // move .minikube to /goinfre
    export MINIKUBE_HOME='/goinfre/'$USER
    echo "export MINIKUBE_HOME='/goinfre/'$USER" >> ~/.zshrc
    
    brew install minikube
    minukube version
    
    kubectl version
    kubectl cluster-info
    kubectl get nodes

#mysql

    > SHOW VARIABLES LIKE 'skip_networking';
    should be OFF for network connections


## libasm

    В 64-битных программах первые шесть аргументов передаются через регистры: rdi, rsi, rdx, rcx, r8, r9.
    В 32-битных - через стек.
    
    Возвращаемое значение из функции передаётся через rax и rdx.
    
    Следующие регистры обязательно нужно сохранять (push) и восстановливать их значения (pop)
    перед выходом из функции: rbp, rbx, r12, r13, r14, r15.

Без спойлеров: https://www.notion.so/LibASM-eaf6e4370032461398127c5f41d12279

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
    export PATH="/Users/lelderbe/Library/Python/3.7/bin:$PATH"

Чекер: https://github.com/cacharle/libasm_test (нужен python3: brew install python3)

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

Основы Docker. Большой практический выпуск https://www.youtube.com/watch?v=QF4ZF857m44

Docker самый простой и понятный туториал. Изучаем докер, так, если бы он был игровой приставкой https://badcode.ru/docker-tutorial-dlia-novichkov-rassmatrivaiem-docker-tak-iesli-by-on-byl-ighrovoi-pristavkoi/

Get started with Docker Machine and a local VM https://eternalhost.net/blog/razrabotka/chto-takoe-docker

## ft_printf

Без спойлеров: https://www.notion.so/ft_printf-3e358ed673d14164b88de9eb428f3c6a

https://github.com/gavinfielder/pft

https://github.com/Mazoise/42TESTERS-PRINTF

https://github.com/charMstr/printf_lover_v2

https://github.com/cacharle/ft_printf_test

## get_next_line

Без спойлеров: https://www.notion.so/get_next_line-59fb1381311b4867b4cfaeec5b94c193

https://github.com/Mazoise/42TESTERS-GNL

https://github.com/charMstr/GNL_lover

## libft
