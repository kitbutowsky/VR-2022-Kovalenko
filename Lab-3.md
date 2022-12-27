# Виртуальная и дополненная реальность
Отчет по лабораторной работе #3 выполнил:
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
Изучить принципы создания и настройки передвижения пользователя в VR с помощью стиков на контроллерах и с помощью телепортации.

## Задание 1
### Пошагово выполнить каждый пункт по примеру предоставленных видеоматериалов:
Ход работы:
- Откройте проект, созданный в предыдущей лабораторной работе;
- Создайте у XR Rig дочерний объект Locomotion System;
- Добавьте Объект XR Rig в Locomotion System;
- Удалите из Locomotion System все компоненты, кроме Locomotion System;
- Добавьте в Locomotion System компоненты плавного передвижения и поворота;
- Настройте добавленные компоненты для левого контроллера;
- Добавьте и настройте компонент Character Controller для XR Rig;
- Скопировать из скрипта CharacterControllerDriver.cs процедуру, связанную с обновление Character Controller;
- Создать на объекте XR Rig новый компонент скрипта;
- Прописать вызов добавленной процедуры каждый кадр проекта;  
- Запустите проект и проверьте, что передвижение работает;
- Удалите из Locomotion System все компоненты, кроме Locomotion System;
- Добавить на Plane, компонент пространства для телепортации.
- На объекте, отвечающем за правый контроллер убрать все объекты кроме Transform и XR Controller;
- На объекте левого контроллера изменить толщину линии луча на 0.01;
- Изменить тип линии на Projectile Curve;
- Изменить в Input System Teleport Mode Active Direction на Everything
- Добавить на Locomotion System новый скрипт;
- Настроить в скрипте отображение луча, только при активации кнопки телепорта.
- Запустить проект и проверить его работу.
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
### В чём разница между Continuous Turn Provider и Snap Turn Provider? Привести развернутый ответ с примерами.



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
### Продемонстрируйте, для чего используется Character Controller?



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
