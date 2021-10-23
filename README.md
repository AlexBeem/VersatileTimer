# VersatileTimer

THE SOFTWARE IS PROVIDED "AS IS," WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGE, USE OR OTHER LIABILITY WHETHER IN CONTRACT, TORT OR OTHERWISE, ARISING OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER CONCESSIONS OF THE SOFTWARE.

                                                     (Описание на русском языке - ниже)

Sorry for google-translate...

**Universal multichannel weekly and / or daily programmable timer.**

Tested on ESP8266 in version ESP-01 and NodeMCU.

All management is via the web interface.

The exact time receives from the Internet (NTP), after the first synchronization, the temporary loss of WiFi / Internet does not affect the work.

**Device capabilities:**

Arbitrary (1-15) number of control channels (on / off), configured in the web interface. For each channel, configurable on / off, GPIO, direct / inverse control.

An arbitrary (1-100) number of tasks (timers), configured in the web interface. For each task, a channel, an action (on / off / task disabled), a condition by time of day and day, or a group of days of the week are configured. The accuracy of setting the condition in time is a second.

Channel management is possible by tasks, manually until the next task, only manually;
  - manually until the next task and only manually - after a power failure, the last channel state is restored;
  - by tasks - after a power failure, the state is set in which the channel should be in accordance with the task settings for the current day of the week and time of day;

Channel state changes log.

Ability to save / restore all settings to files on the ESP8266, upload / download files via the web interface.

Language selection (English / Russian) in the web interface.

The login and password for authorization (admin and admin by default) are configured in the web interface (I refused https due to the slow rendering of the web interface and the lack of a special need).

Indication of the number of tasks for the channel.

Shows the current active and next tasks for the channel.

Indication of duplicate and conflicting tasks.

Indication of duplicate channels.

The time zone is configured in the web interface.

Downloading firmware via web interface.

Rebooting via the web interface.

With Multicast DNS (mDNS) available as host vt.local.

# VersatileTimer

**Универсальный многоканальный недельный и/или суточный программируемый таймер.** 

Протестирован на ESP8266 в исполнении ESP-01 и NodeMCU.

Всё управление - через веб-интерфейс.

Точное время получает из Интернета (NTP), после первой синхронизации временное пропадание WiFi/Internet на работу не влияет.

**Возможности устройства:**

Произвольное (1-15) количество каналов управления (вкл/выкл), настраивается в веб-интерфейсе.
Для каждого канала настраивается "включен/отключен", GPIO, прямое/инвертированное управление.

Произвольное (1-100) количество заданий(таймеров), настраивается в веб-интерфейсе.
Для каждого задания настраивается канал, действие (вкл/выкл/задание отключено), условие по времени суток и дню, или группе дней недели.
Точность установки условия по времени - секунда.

Управление каналами возможно по заданиям, вручную до следующего задания, только вручную;
  - вручную до следующего задания и только вручную - после пропадания питания восстанавливается последнее состояние канала;
  - по заданиям - после пропадания питания устанавливается состояние, в котором канал должен находиться согласно настройкам заданий для текущего дня недели и времени суток;

Журнал изменений состояния каналов. 

Возможность сохранения / восстановления всех настроек в файлы на ESP8266, загрузка / выгрузка файлов через веб-интерфейс.

Выбор языка (английский / русский) в веб-интерфейсе.

Логин и пароль авторизации (admin и admin по умолчанию) настраиваются в веб-интерфейсе (от https я отказался по причине медленной отрисовки веб-интерфейса и отсутствия особой необходимости).

Индикация количества заданий для канала.

Индикация текущего активного и следующего заданий для канала.

Индикация дублирующих и конфликтующих заданий.

Индикация дублирующих каналов.

Часовой пояс настраивается в веб-интерфейсе.

Загрузка прошивки через веб-интерфейс.

Перезагрузка через веб-интерфейс.

При наличии Multicast DNS (mDNS) доступен как хост vt.local.
