# Kodi медиацентр на основе Orange Pi 4

# **ПРЕДИСЛОВИЕ**

**Данный репозиторий разделён на 3 ветки в целях экономии свободного места и трафика при клонировании основного репозитория. Образы и изображения находятся в отдельных ветках, поэтому вы их не найдёте в ветке master.**

Данное руководство содержит готовый образ медиацентра для Orange Pi 4 (на Orange Pi 4b не тестировал, но единственное отличие между ними - дополнительный ИИ модуль, так что всё должно работать, кроме него).

Если вы хотите просто быстро установить прошивку для вашей Orange Pi 4 (4b), не разбираясь в деталях,
[**тут вы найдёте простые инструкции**](#1-быстрая-установка-прошивки)

Если же вы используете любую другую плату Raspberry Pi, Orange Pi, Banana Pi, Asus Tinker Board или нечто ещё, тогда вы можете скачать нужную версию прошивки (желательно ubuntu или ubuntu based os) с оффициального сайта производителя платы, произвести настройку видеодрайверов OpenGL (ES) по необходимости и самостоятельно установить все пакеты, [**следуя всем инструкциям этго и последующих разделов**](#2-установка-официальной-прошивки)

Также вы можете расширять набор пакетов, которые вы устанавливаете, на ваше усмотрение. Если вы создадите свой образ или найдёте другой набор пакетов для Kodi, убедительная просьба добавить информацию в обсуждение к этому репозиторию. Главное требование, чтобы вашим решением можно было воспользоваться свободно и бесплатно, как завещал Ричард Столлман.

# **ОГЛАВЛЕНИЕ**

[**1 Быстрая установка прошивки для тех, кто хочет "ctrl+c ctrl+v"**](#1-быстрая-установка-прошивки)

[**2 Установка и настройка официальной прошивки**](#2-установка-и-настройка-официальной-прошивки)

[**3 Настройка дров для gpu Mali-T860 MP4 в образе Orange Pi 4**](#3-настройка-дров-для-gpu-Mali-T860-mp4-в-образе-orange-pi-4)

[**4 Установка и настройка Kodi**](#4-установка-и-настройка-kodi)







# 1 Быстрая установка прошивки

Для начала вам потребуется, неожиданно, Micro SD карта. Скорость class 10 не просто так рекомендуется даже для обычных дистрибутивов, ведь с sd карты происходит загрузка систмы. В случае с использованием Kodi фильмы будут временно чуть ли не полностью загружаться на эту sd карту для просмотра, поэтому хорошая надёжная sd-карта обязательна для комфортного просмотра видео без тормозов. Рекомендую брать Kingston или Samsung, проживут на порядок дольше, чем карты других компаний, а также проверены временем. 

Далее карту необходимо форматировать. Если вы знаете хотя бы 2 таблицы разделов (GPT и MBR), то рекомендую MBR - дефолт для винды. Что же касается файловой системы - в сети рекомендуют fat32. 

Форматирование и подготовку SD карты рекомендую проводить в программе: [SDCardFormatterv5_WinEN.zip](https://github.com/ITMO-lab/Orange-Pi-4-Kodi/raw/firmware/tools/SDCardFormatterv5_WinEN.zip)

После чего можно залить готовый образ: [ubuntu_18.04_kodi_orange_pi_4_full.zip](https://github.com/ITMO-lab/Orange-Pi-4-Kodi/tree/firmware/images/ubuntu_18.04_kodi_orange_pi_4_full) 

Сначала нужно распаковать [name].img, например, через WinRAR или 7zip. Пытался хранить целый в git lfs, но загрузить файл не получалось из-за бессмысленных ограничений гита, поэтому качать архив придётся по частям либо сразу клонировать/качать всю ветку firmware.

Заливать образ на sd карту можно с помощью программы: [win32diskimager-1.0.0-install.exe](https://github.com/ITMO-lab/Orange-Pi-4-Kodi/raw/firmware/tools/win32diskimager-1.0.0-install.exe) 

После заливки образа загружаемся с него, для этого просто вставляем в слот для sd карты на Orange Pi, подключаем монитор и подаём питание. Если получаем зелёный экран или артефакты - выключаем питание и включаем снова, такое иногда случается при первом запуске.

По умолчанию существует учётная запись orangepi с паролем orangepi.

После успешной загрузки (пароль у вас не потребуют) требуется первым делом расширить системный раздел. Для этого запускаем gparted и делаем resize системного раздела так, чтобы он занимал всё оставшееся место на sd карте. 



# 2 Установка и настройка официальной прошивки













# 3 Настройка дров для gpu Mali-T860 MP4 в образе Orange Pi 4







# 4 Установка и настройка Kodi







