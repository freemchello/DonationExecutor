
# DonationExecutor - плагин для Minecraft 1.18+ (ядро "Paper")
[![GitHub license](https://img.shields.io/github/license/link1107/DonationExecutor)](https://github.com/link1107/DonationExecutor)

Плагин, который, получая информацию о новых донатах с Donation Alerts, автоматически генерирует различные события на основании суммы доната.

[Техподдержка в ВК](https://vk.com/donationexecutor) (по вопросам, связанным с установкой или настройкой плагина)

## Видео про этот плагин
[![Watch the video](https://img.youtube.com/vi/48jP4qCb0pM/maxresdefault.jpg)](https://youtu.be/48jP4qCb0pM)

## Установка и использование

#### Как этим пользоваться?

1. Вам понадобится сервер версии 1.18.1 (другие версии не тестировались) на ядре [Paper](https://papermc.io/downloads).
2. [Скачайте](https://github.com/link1107/DonationExecutor/releases) плагин (jar-файл), закиньте его в папку сервера "/plugins".
3. Запустите сервер, подождите полной загрузки, остановите сервер.
4. Откройте появившийся конфигурационный файл DonationExecutor.yml в папке "/plugins/DonationExecutor".
5. Заполните конфигурационный файл в соответствии с инструкциями в нем (особое внимание уделите токенам Donation Alerts, а также никнеймам стримеров). Сохраните изменения, закройте файл.
6. Запустите сервер. В случае корректно заполненного конфиг-файла, все должно работать.
7. Для использования команд плагина либо сделайте себя оператором сервера (пропишите "op <ВАШ_НИКНЕЙМ>" консоль сервера), либо добавьте себе разрешения, используя плагин управления пермишенами (например, LuckPerms) - de.donate, de.reload, de.filter (подробнее - ниже).
8. Составьте список сумм и действий с кратким описанием и разместите его для зрителей в описании к стриму или на странице Donation Alerts.

## FAQ

#### Это плагин или мод?
Это плагин, его необходимо добавить только на сам сервер. Однако, для полной функциональности и работоспособности (например, отображение кастомных скинов на мобах) вам понадобится мод [Optifine](https://optifine.net/downloads) последней версии.

#### Могу ли я вручную сымитировать донат? (например, если донат не сработал автоматически, или я хочу протестировать донат)
Да. Донат можно протестировать командой "/de donate <сумма доната без копеек> <ник донатера (необязательно)>".

#### Какие еще доступны команды?
/de donate <СУММА> <ИМЯ> ## <СООБЩЕНИЕ_необязательно> - сымитировать донат<br>
/de reload - перезагрузить настройки из конфига<br>
/de filter ON|OFF - включить/выключить фильтр никнеймов<br>
/de help - вывести список доступных команд

#### Могу ли я ограничить использование команд?
Да. В плагине имеются пермишены (разрешения) для использование каждой из команд: **_de.donate, de.reload, de.filter<br>_**
Чтобы использовать команды, вам нужно либо добавить разрешения в плагин, управляющий разрешениями (например, luckperms), либо
если вы не используете плагин разрешений, то можете сделать себя оператором сервера, прописав "op <ваш никнейм>" в консоль сервера.
Чтобы разрешить другим игрокам использовать команды, вы можете либо добавить им разрешения в плагине, управляющем разрешениями, 
либо так же сделать их операторами сервера (но учтите, что в этом случае они получат возможность управления сервером).



#### Где я могу увидеть доступные настройки?
После первого запуска сервера с плагином, откройте конфигурационный файл DonationExecutor.yml в папке "/plugins/DonationExecutor".

#### Могу ли я изменить/дополнить этот код и использовать его в коммерческих целях?
Да, данный плагин распространяется по лицензии AGPL 3.0. Если вы являетесь стримером, и хотите, чтобы я специально для вас создал версию плагина с вашими уникальными событиями или фичами, можете связаться со мной по электронной почте - igortokach@gmail.com

#### Планируется ли дальнейшее развитие плагина и добавление новых событий или функций?
Да. Но так как это по большей части мое хобби, я буду обновлять плагин по мере моих возможностей и наличия свободного времени.

#### Почему все комментарии и описание на русском языке?
Плагин в данный отлавливает донаты только с Donation Alerts, которым пользуются в подавляющем большинстве русские стримеры. Также зрители моего видео об этом плагине на YouTube могут не знать английского языка, что сделает процесс ознакомления с кодом для них более сложным.
Я знаю, что на гитхабе и в среде программистов общепринят английский язык, но в данной ситуации я не думаю, что это для кого-то будет критично.

## Автор
- [@link1107](https://www.github.com/link1107)
- [Мой YouTube-канал](https://youtube.com/c/ИгорьЛинк)

