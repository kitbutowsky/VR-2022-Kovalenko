# Виртуальная и дополненная реальность
Отчет по лабораторной работе #4 выполнил:
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
Визуальная доработка проекта из предыдущей лабораторной работы и добавление взаимодействия с объектами.

## Задание 1
### Пошагово выполнить каждый пункт по примеру предоставленных видеоматериалов:
Ход работы:
- Открыть проект из 3 лабораторной работы;
- Зайти в Unity Asset Store, выбрать подходящие ассеты и импортировать их в проект;
- Создать новый материал. Выбрать текстуру будущего пола среди скачанных ассетов. Добавить созданному материалу выбранную текстуру;
- Изменить у материала значения параметров Tiling на подходящие;
- Созданный материал добавить на Plane;
- Выбрать модель стен из префабов среди скачанных ассетов;
- Разместить несколько стен в ряд;
- Скопировать ряд стен и разместить на каждую сторону;
- Разделить большую комнату на две маленькие с помощью скопированных стен;
- Удалить среднюю стену у перегородки;
- Скопировать пол, перевернуть и вставить в качестве потолка;
- Добавить модели факелов на стены;
- Расставить освещение;
- В первую и вторую комнату по центру поставить префаб стола из скачанных ассетов;.
- Создать объект (камень);
- Добавить на него Collider и Rigidbody;
- Добавить на объект GrabInteractible;
- Добавить на контроллеры XR Direct Interactor;
- Добавить Outline;
- Написать скрипт, управляющий включением подсветки;
- Запустить проект и проверить работоспособность;
- Включить физику в Rigidbody на объекте;
- Включить Throw on Detach на GrabInteractible;
- Запустить проект и проверить работоспособность;
- Создать Ray Interactor;
- Настроить внешний вид луча;
- Установить Interaction Layer Mask, чтобы не телепортироваться лучом;
- Продемонстрировать притягивание;
- Написать скрипт для управления появлением/исчезанием луча;
- Запустить проект и проверить работоспособность.
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
### Какой компонент позволяет добавить взаимодействие с объектами в VR? Привести развернутый ответ с примерами



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
### В чём разница между Velocity tracking, Kinematic и Instantaneous Movement Type? Привести развернутый ответ с примерами.



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
