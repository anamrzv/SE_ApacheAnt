# Методы и средства программной инженерии. 4 семестр. 3 лабораторная
## Темы: утилита Apache Ant, Junit

Написать сценарий для утилиты Apache Ant, реализующий компиляцию, тестирование и упаковку в jar-архив кода проекта из лабораторной работы №3 по дисциплине "Веб-программирование".

Каждый этап должен быть выделен в отдельный блок сценария; все переменные и константы, используемые в сценарии, должны быть вынесены в отдельный файл параметров; MANIFEST.MF должен содержать информацию о версии и о запускаемом классе.

Cценарий должен реализовывать следующие цели (targets):

compile -- компиляция исходных кодов проекта.
build -- компиляция исходных кодов проекта и их упаковка в исполняемый jar-архив. Компиляцию исходных кодов реализовать посредством вызова цели compile.
clean -- удаление скомпилированных классов проекта и всех временных файлов (если они есть).
test -- запуск junit-тестов проекта. Перед запуском тестов необходимо осуществить сборку проекта (цель build).
music - воспроизведение музыки по завершению сборки (цель build).
diff - осуществляет проверку состояния рабочей копии, и, если изменения не касаются классов, указанных в файле параметров выполняет commit в репозиторий git.
