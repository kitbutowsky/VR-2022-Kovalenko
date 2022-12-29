# Виртуальная и дополненная реальность
Отчет по лабораторной работе #1 выполнил:
- Коваленко Даниил Антонович 
- РИ-300022
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Ознакомиться с основными функциями Unity и взаимодействием с объектами внутри редактора.

## Задание 1
### Пошагово выполнить каждый пункт по примеру предоставленных видеоматериалов:
Ход работы:
- Создать новый проект из шаблона 3D – Core;

Создаем проект:
![image](https://user-images.githubusercontent.com/91405800/209919544-55677532-794e-4860-94c9-0323a7844203.png)
Открываем проект:
![image](https://user-images.githubusercontent.com/91405800/209919731-f4b503d1-b90a-4882-ad1e-0cb318b637eb.png)

- Проверить, что настроена интеграция редактора Unity и Visual Studio Code (пункты 8-10 введения);

Проверяем:

<img src="https://user-images.githubusercontent.com/91405800/209919862-06b8f933-4d06-4d19-bcab-07c31383036f.png" height="500">           <img src="https://user-images.githubusercontent.com/91405800/209919899-3c698ead-bf00-4e8e-9088-0af6739b3870.png" height="500">

<img src="https://user-images.githubusercontent.com/91405800/209920906-202945c7-0389-4e60-8a27-7b4ed82fb65a.png" height="500">

- Создать объект Plane;

Создаем:

<img src="https://user-images.githubusercontent.com/91405800/209923188-771b606d-c190-4031-b770-38880d8314c0.png" height="350"> <img src="https://user-images.githubusercontent.com/91405800/209923609-bf2b649e-ffe4-431b-9088-3cf87b1b16de.png" height="350">


- Создать объект Cube;

Создаем:

<img src="https://user-images.githubusercontent.com/91405800/209923188-771b606d-c190-4031-b770-38880d8314c0.png" height="350"> <img src="https://user-images.githubusercontent.com/91405800/209923920-3b44bb16-cf79-4e17-994f-5c21256f8d04.png" height="350">

- Создать объект Sphere;

Создаем:

<img src="https://user-images.githubusercontent.com/91405800/209923188-771b606d-c190-4031-b770-38880d8314c0.png" height="350"> <img src="https://user-images.githubusercontent.com/91405800/209924016-c77dab8b-30b7-4deb-a6d6-418dd0a23ac2.png" height="350">

- Установить компонент Sphere Collider для объекта Sphere и настроить Sphere Collider в роли триггера;;

Включаем:

![image](https://user-images.githubusercontent.com/91405800/209924190-5d58d9be-6604-4433-a07b-c636ccbf892b.png)

- Объект куб перекрасить в красный цвет;

Создаем Material в вкладке Assets и меняем его цвет на крассный:

<img src="https://user-images.githubusercontent.com/91405800/209924473-bea85dbb-abe3-4103-b3df-e11c696dec32.png" height="500"> <img src="https://user-images.githubusercontent.com/91405800/209924568-4aa5b306-6ce2-40fc-abfe-a4f6c1bdaf04.png" height="500">

Затем перетаскиваем Material на куб и видим что он перекрасился:

<img src="https://user-images.githubusercontent.com/91405800/209924760-85fa5ff2-48f4-4886-aeff-bf0b22675a79.png" height="500">

- Добавить кубу симуляцию физики, при это куб не должен проваливаться под Plane;

Добавляем кубу компонент Rigidbody и обязательно поднимаем его над Plane:

<img src="https://user-images.githubusercontent.com/91405800/209925098-50d9e949-88e9-4f55-8ef1-26b67c56f64c.png" height="200"> <img src="https://user-images.githubusercontent.com/91405800/209925027-f865470d-fa6a-4bf0-8f07-98b9e6090b86.png" height="400">


- Написать скрипт, который будет выводить в консоль сообщение о том, что объект Sphere столкнулся с объектом Cube;
- При столкновении Cube должен менять свой цвет на зелёный, а при завершении столкновения обратно на красный.
```py

In [ ]:
#Import the required modules, numpy for calculation, and Matplotlib for drawing
import numpy as np
import matplotlib.pyplot as plt
#This code is for jupyter Notebook only
%matplotlib inline

# define data, and change list to array
x = [3,21,22,34,54,34,55,67,89,99]
x = np.array(x)
y = [2,22,24,65,79,82,55,130,150,199]
y = np.array(y)

#Show the effect of a scatter plot
plt.scatter(x,y)

```



## Задание 2
### Продемонстрируйте на сцене в Unity следующее:

- Что произойдёт с координатами объекта, если он перестанет быть дочерним?
- Создайте три различных примера работы компонента RigidBody?

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Задание 3
### Реализуйте на сцене генерацию n кубиков. Число n вводится пользователем после старта сцены.



```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
