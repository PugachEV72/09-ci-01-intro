# Домашнее задание к занятию 7 «Жизненный цикл ПО» - Пугач Евгений.


---

## `Подготовка к выполнению`

1. Получить бесплатную версию Jira.
2. Настроить её для своей команды разработки.
3. Создать доски Kanban и Scrum.


---

## `Основная часть`

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач.


![Скриншот 1](https://github.com/PugachEV72/Images/blob/master/2024-01-08_01-06-13.png)

---

Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.
3. Done reproduce -> On fix.
4. On fix -> On reproduce, Done fix.
5. Done fix -> On test.
6. On test -> On fix, Done.
7. Done -> Closed, Open.


![Скриншот 2](https://github.com/PugachEV72/Images/blob/master/2024-01-08_01-07-12.png)

[Bug workflow](https://github.com/PugachEV72/09-ci-01-intro/blob/main/xml/Bug_workflow.xml)

---

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.
2. On develop -> Open, Done develop.
3. Done develop -> On test.
4. On test -> On develop, Done.
5. Done -> Closed, Open.


![Скриншот 3](https://github.com/PugachEV72/Images/blob/master/2024-01-08_18-52-46.png)

[Any workflow](https://github.com/PugachEV72/09-ci-01-intro/blob/main/xml/Any_workflow.xml)

---
