# YAMY-painter
Object Oriented Paint Program using Java Swing
## Table of Contents
- [Painter](#painter)
  * [Project Description](#project-description)
  * [Project Functionalities](#project-functionalities)
  * [Tools](#tools-libraries--implementations)
  * [Deployment](#deployment)
  * [Design Patterns](#design-patterns)
  * [S.O.L.I.D Principles](#solid-principles)
  * [Documentation](#documentation)
  * [Contributers](#contributers)
  * [Screenshots](#screenshots)
  * [Project Report](#project-report)

## Project Description
Object-oriented paint program which allows the user to unleash their inner Da Vinci!. GUI was designed mainly using javax.swing.  

## Project Functionalities
**This app helps the user unleash their inner Da Vinci! The user can:**
1. Free paint using a brush with variable stroke/thickness ( Antialiasing got you covered ;) )
2. Erase using eraser tool
3. Draw geometric shapes (Line Segment, Circle, Square, Rectangle, Triangle)
4. Change drawing color and stroke
5. Fill shapes with any color
6. Undo and redo any action ***( I actually designed a custom algorithm for that :D )***
7. Move shapes around
8. Resize shapes
9. Copy and paste shapes as many times as you like!
10. Clear the screen
11. Automatic screenshot of your masterpiece with every change! Manual screenshot button is also present.

## Tools, Libraries & Implementations
1. IntelliJ IDEA (IDE)
2. Java 
3. Javax.swing
4. Graphic libraries like java.awt and javax.imageio
5. Creately for UMLs diagrams
6. LaTeX for writing documentation
7. Maintained S.O.L.I.D principles
8. Implemented 6 design patterns

## Deployment
To run the program, you have to run the class named "FinalProjectPaint_V1" as your main class with Java SDK 16

## Design Patterns
**1. Factory Design Pattern**
We have used Factory design pattern to create new objects
without the need of constructors and to avoid coupling and dependency
between classes. So we constructed new instances of classes through
this factory and returned in needed methods or classes.

**2. Prototype Design Pattern**
We have used Prototype design pattern by implementing “Cloneable”
interface and implementing “clone()” method in each and every Shape
class and also Cloning instances of “Point” class. It helped us make
copies of our Objects using values instead of references which helped
in the copy method.

**3. Singleton Design Pattern**
We have used Singleton design pattern to ensure the creation of only
one instance of “ScreenShotter” class whose main aim is to
screenshot the paint board and it is the only instance that is
allowed to do such task.

**4. Façade Design Pattern**
We have used the Façade design pattern as it offers a simple interface to
more complex underlying objects. So we could use draw methods
using objects of “ShapeMakerFacade” class instead of accessing the
shapes classes themselves.

**5. Iterator Design Pattern**
Iterator design Pattern facilitates looping across the array list of
Geometric shapes needed to be drawn by only using 2 basic methods
which are : “hasNext()” and “next()” avoiding looping with varying
conditions which helped enhance the readability of the code.

**6. Observer Design Pattern**
Observer design pattern helped us with automatic
screenshotting(update method) while drawing (auto-documentation) as
it takes screenshot each and every time we release the mouse by only
changing the state in the PaintBoard class.

## S.O.L.I.D Principles
**1. Single-Responsibility Principle**
A class should have one and only one reason to change, meaning that a class should have only one job, that's why we made classes like ShapeCopier, ShapeFiller, ShapeMover and ShapeResizer. Those classes are only responsiple for one job as shown from their names.

**2. Open-Closed Principle**
Objects or entities should be open for extension but closed for modification, so if anyone wants to contribute to project and add another shape, he can do so effortlessly by adding a class and extending it from "GeometricShape" class.

**3. Interface Segregation Principle**
Each method in each class is there for a reason, there is no unused method, so if you are adding extra shape, you probably won't be forced to implement a method you won't use.

## Documentation
[Project Documentation](ProjectDocumentation.pdf)
## Contributers
1. [Adham Mohamed](https://github.com/adhammohamed1)
2. [Yousef Kotp](https://github.com/yousefkotp)
3. [Mohamed Farid](https://github.com/MohamedFarid612)

## Screenshots

***Excuse my evidently limited drawing skills :)***

![hiii](https://user-images.githubusercontent.com/90573502/142770939-02b8e580-01ea-479d-b11c-afb64607a115.jpg)

![Screenshot (121)](https://user-images.githubusercontent.com/90573502/142770988-87fd8657-f500-4a70-bc45-83448c24512d.png)

![Screenshot (122)](https://user-images.githubusercontent.com/90573502/142770986-4977efc4-18af-4c25-a98e-7b26ca6432f6.png)

### The following screenshot was taken using the in-app screenshot feature:

![screenshot](https://user-images.githubusercontent.com/90573502/142770942-5c15741f-fd36-46ff-9873-8c7f9cd71db4.jpg)

![132788122-ab423bb7-a12c-46c9-a90c-c8a78626e492](https://user-images.githubusercontent.com/90573502/142770579-74f99f76-76d9-4325-8ea1-2ad9ee6f3724.png)

![132782674-2f777635-4ae4-45be-b560-2b5a1dc1cde0](https://user-images.githubusercontent.com/90573502/142770582-543deb58-19b0-4e79-bfc4-a3f226010721.png)

![UseCase](https://user-images.githubusercontent.com/90573502/141643003-a023485d-820f-42d5-a8ba-2b8ce612dcb7.jpeg)

![ClassDiagram](https://user-images.githubusercontent.com/90573502/141643009-1faef175-9399-4a91-9bb1-c7501e8cb748.jpeg)

## Project Report
> The following is a report of the whole program : [paint_Final.pdf](https://github.com/adhammohamed1/YAMY-painter/files/7531955/paint_Final.pdf)

