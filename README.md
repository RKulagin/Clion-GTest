# Как установить CLion и настроить Gtest

Disclaimer: данный туториал написан в для студентов МГТУ им Н. Э. Баумана и в частности для ИУ8 ради облегчения их нелёгкого пути ~~по морям дискретной математики~~ в лабораторных работах по Алгоритмическим языкам

* Подать заявку на предоставление бесплатной лицензии [JetBrains Products for Learning](https://www.jetbrains.com/shop/eform/students)

![Скриншот с сайта подачи заявки](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/studentsLicence.png)

(То, что подчёркнуто красным нужно заполнить)

* Скачать [CLion](https://www.jetbrains.com/clion/)

![Скриншот с сайта загрузки](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/downloadCLion.png)

* Установить CLion. 

Установка стандартная, ничего дополнительно нажимать не требуется(только на своё усмотрение)

* Активировать CLion, используя университетскую почту


**Для Windows или macOS**

* Скачать [Github Desktop](https://desktop.github.com/) для Windows | macOS

* В Github Desktop: `File -> Clone repository` и выбираете нужный Вам репозиторий

![Clone repository](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/cloneRepo.png)

* Изменить ветку на `wp/lab`

![Change branch](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/branch.png)


**Для Linux** (Описано для Debian/Ubuntu и других систем, использующих apt)

```shell script
sudo apt update
sudo apt install git
git clone <ссылка на ваш репозиторий>
```

Где взять ссылку показано на картинке

![Copy link](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/copyLink.png)

```shell script
cd <название репозитория>
git checkout -b wp/lab
git submodule update --init
```

Последняя команда может быть необязательной для выполнения каждый раз, но если что-то не работает, то её нужно выполнить.

**Далее для всех ОС**

* Запускаем CLion

* Выбираем пункт New CMake Project from Sources или `File -> New CMake Project from Sources`

![New Project](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/welcomeToClion.png)

* Выбираем папку с локальным репозиторием (обратите внимание, нужна именно папка, содержащая папку `.git`)

![Choose local repository folder](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/chooseLocalRepo.png)

* Важно! Нажимаем Open Existing Project. Иначе CMakeLists.txt перезапишется

![open existing project](https://github.com/RKulagin/Clion-GTest/blob/inWork/img/openExProject.png)

* Готово. Если делаете всё в первый раз на данной машине, то стоит немного подождать, пока Hunter скачает и установит необходимые зависимости  