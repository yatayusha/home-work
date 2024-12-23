# Лабораторная работа (задание)
# "Шифрование файлов и каталогов"

В данной лабораторной мы научимся работать с утилитой GPG и рассмотрим различные способы шифрования файлов.
Если вы используете macOS, то вам нужно установить GPG-Suite, или воспользоваться командой `brew install gnupg2`. Если вы используете Windows, то рекомендуется установить GPG4Win.

# Разминка
(её не нужно включать в отчёт, но стоит выполнить в качестве ознакомления с первым типом шифрования)
Шифрование с помощью пароля - это метод шифрования, при котором для шифрования и дешифрования применяется один и тот криптографический ключ.

1. Создаём пустой файл с названием,например, shifr с помощью команды `touch shifr.txt`
2. Записываем что-нибудь в этот файл (стихотворение, цитату или просто набор слов)
3. Вводим команду `gpg -c shifr.txt`
4. Далее нужно будет ввести фразу-пароль, которая станет ключом, например нашим ключом будет слово: `ITMOFamily`
5. В директории с исходным файлом появится файл с расширением `gpg`. Это и есть наш зашифрованный файл.
6. Для расшифровки этого файла следует ввести в терминале команду `gpg --decrypt shifr.txt.gpg`. Утилита запросит пароль. Если был введён верный пароль, то на экране отобразится исходный текст

# Задание 1
Зашифруйте текстовый файл с помощью ключей: создайте файл по образцу из разминки, но только теперь задача несколько усложняется, Вам нужно самостоятельно изучить метод шифрования с помощью ключей. После того, как файл будет зашифрован, нужно выполнить его дешифрование.
В качестве результата выполнения данного задания прикрепите скриншот зашифрованного файла при его открытии, и результат дешифрования.

# Задание 2
И наконец попробуем зашифровать текстовый файл с помощью цифровой подписи.
Аналогичным образом создаём текстовый файл и изучаем метод шифрования с помощью цифровой подписи. После того, как файл будет зашифрован, нужно выполнить его дешифрование.
В качестве результата выполнения данного задания прикрепите скриншот зашифрованного файла при его открытии, и результат дешифрования.

Для записи дешифрованной информации в отдельный файл добавьте опцию `--output` и после укажите название файла.

А также: к каждому заданию нужно прикрепить скриншоты с проверкой на подлинность файлов.

# Источники, где можно найти информацию для выполнения работы:
[Шифрование и утилита GPG](https://habr.com/ru/articles/659755/)

[Источник, где можно найти ВСЁ](https://www.google.ru/?hl=ru)
