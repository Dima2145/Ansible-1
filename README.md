# Ansible-1
Домашнее задание к занятию «Ansible. Часть 1»
Задание 1
Ответьте на вопрос в свободной форме.

Какие преимущества даёт подход IAC?

Решение 1
Благодаря подходу IAC можно управлять конфигурацией сразу множества серверов без необходимости настраивать каждый вручную, даже неважно кол-во насраиваемых серверов, что 20 что 100 будут настроены достаточно быстро. То же касается и ПО/Сервисов. Также, например, конфигурируя порядка 20 серверов с помощью инструментов IAC мы можем быть уверены, что результат на всех серверах будет одинаковым. Ещё стоит отметить что с помощью инструментов IAC мы можем всегда быстро восстановить нерабочие серверы путем создания новых, что в случае IAC много времени не займет.

Задание 2
Выполните действия и приложите скриншоты действий.

Установите Ansible.
Настройте управляемые виртуальные машины, не меньше двух.
Создайте файл inventory с созданными вами ВМ.
Проверьте доступность хостов с помощью модуля ping.
Решение 2

СКРИНЫ

Задание 3
Ответьте на вопрос в свободной форме.

Какая разница между параметрами forks и serial?

Решение 3
Serial определяет кол-во узлов на которых выполняются задачи за один запуск плейбука/ad-hoc'а. Выполнили задачи на одной части узлов, затем выполняются задачи на другой части узлов и т.д. ...

Forks определяет кол-во узлов на которых единовременно может выполнятся задача плейбука/ad-hoc'а. Выполнили первую задачу на одной части узлов, затем первую задачу на другой части узлов и т.д. ...

Итог: при использовании Serial мы сначала выполняем все указанные задачи на одной части узлов, и только потом переходим и выполняем все задачи на другой части узлов. Forks выполняет задачи на всех узлах, но каждую отдельную задачу выполняет единовременно на определенном кол-ве узлов и выполнив задачу на одной группе переходит к следующей, группы на которых задача выполнена будут ждать пока задача будет выполнена на всех остальных узлах.

Задание 4
В этом задании вы будете работать с Ad-hoc коммандами.

Выполните действия и приложите скриншоты запуска команд.

Установите на управляемых хостах любой пакет, которого нет.
Проверьте статус любого, присутствующего на управляемой машине, сервиса.
Создайте файл с содержимым «I like Linux» по пути /tmp/netology.txt.
Решение 4

СКРИНЫ
