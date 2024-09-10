java c
SC3060: Computer Graphics and Visualization 
SW Lab or Your Own Computer 
Making Images with Mathematics 
Lab Experiments 1 - 5 
SESSION 2024/2025 
SEMESTER 1 
COMPUTER SCIENCE COURSE 
MAKING IMAGES WITH MATHEMATICS 
1.  OBJECTIVE In this coursework you will learn how to visualize curves, surfaces and solid shapes defined by simple mathematical formulas. Each of 5 experiments takes 2 hours. Upon completion of these experiments you will know:
•   How to define shapes by parametric and implicit functions, and
•   How to transform. and animate shapes.
2.  EQUIPMENT You have to install the latest version of ShapeExplorer from the course site. The software is available for Windows, MacOS and Linux (Ubuntu). You can work on the lab assignments using your either the computers in the lab and your own computers. 
3.  INTRODUCTION In this labs, you will learn how to define geometric shapes by mathematical formulas which are used to compute coordinates of all the points belonging to the shapes. You will be using ShapeExplorer (Fig.  1) which is an interactive software tool designed to display shapes defined by parametric and implicit function scripts and colors defined by explicit functions. It can run on Windows, MacOS and Linux (Ubuntu) computers. Shape  Explorer is just one interactive window where you can type the definitions scripts and other parameters. The definitions can be saved in a proprietary format and loaded later to the software to continue working with them. Shape  Explorer supports only one shape visualization at the time. Its purpose is to work as a quick all-in-one multi-platform. visualization tool.
Figure 1.   ShapeExplorer at a glance. Parametric functions in ShapeExplorer are explicit functions of up to three variables u, v, w (which are called parameters) and time t. They can define Cartesian coordinates x,y, Z  of curves, surfaces and solid objects. To define a curve, only one parameter u, v or w  has to be used, to define a surface–any two parameters u ,v , v, w or u, w are required, for solid objects– all three parameters u, v, w have to be used. When t is added, these objects will become time- dependent. The examples of defining parametrically curves, surfaces and sold objects are given in Figs. 2, 3 and 4.
Figure 2. Displaying a parametric curve.
Figure 3. Displaying a parametric surface.
Figure 4 Displaying a parametric solid.Implicit functions are the functions defined as f(x,y, z, t) =0, where x,y, z  are Cartesian coordinates and tis the time. You will only use them for defining surfaces. The implicit functions are equal to zero for the points located on the surface. By changing this equality into an inequality g = f(x,y, z, t)≥0, known  in computer graphics as FRep, we define not only a surface but the space bounded by this surface, or a half-space. In this case, the function equals to zero for the points located on the surface, positive values of the function indicate points inside the solid object, and negative values are for the points which are outside the object. In the ShapeExplorer script. field, only the left part of the implicit or FRep function has to be written – it is always assumed to be ≥0. The example of defining a surface is given in Fig. 5 and a definition of the solid object using set-theoretic (Boolean) operations is illustrated in Fig. 6.Defining  shapes  and  animations  may  require  multiple  formulas  and  temporary  variables. ShapeExplorer supports a subset of C# language for writing definition scripts. The following mathematical functions are supported:
abs, sqrt, exp, log, sin, cos, tan, acos, asin, atan, ceil, floor, atan2, mod, round, max, min, cosℎ, ssinℎ, tanℎ, log10.There is also if{ } else { } operator. Variables, x,y, z are reserved for Cartesian coordinates, while variables u, v, w are parametric coordinates. Variable t is reserved for defining the time. All other variable can be used without declaration—they will be declared as float. 
Figure 5 Displaying an implicit surface. Both sides of the surface are visible.
Figure 6 Displaying an implicit solid. The inner surface of the object is not visible in solids.
For defining r,g, b diffuse colors, scripts with explicit functions of coordinates x,y, Z have to be used:r|g |b = f(x,y, Z, t); r,g, b ∈ [0,1] . Thus the color is defined for any point of the 3D modelling space and it is then sampled by the geometry (see Fig. 7). Constant colors can also be defined as r|g |b = value ∈ [0,1];
Figure 7 Defining diffuse colors as functions of coordinates.In addition,  in the Visual Appearance fields the Specular Color [0,1], Shininess [0,1] and Transparency [0,1] values can be defined. Specular Color affects overall illumination of the object. It is responsible for displaying reflections or specs on the surface of objects. Parameter Shininess controls the size of such specs. Colors of curves can be only defined if Shininess is set to 1.The remaining Animation fields (Fig. 7) contain TimeSpan and CycleInterval. The TimeSpan contains minimum and maximum values of the time values between which it will be incremented in a cyclic manner. These values can be positive and negative. The TimeSpan interval then is mapped to the real time interval CycleInterval in seconds – this is how the animation will be then displayed.Options fields  (Fig.  7) contain  parameters of the  coordinate axes, an option to toggle to wireframe. visualization mode, and background color. Coordinate axes can be scaled—shorten with the scaling parameters less than 1 or elongated with the scaling parameters greater than 1. Scaling coefficient 0 will toggle off the respective axis.
4.  EXPERIMENTS 
There are 5 lab sessions comprising 5 experiments:
1. Parametric Curves 
12 marks 
代 写SC3060: Computer Graphics and Visualization SESSION 2024/2025 SEMESTER 1SQL
代做程序编程语言2. Parametric Surfaces 
12 marks 
3. Parametric Solids 
12 marks 
4.  Implicit Surfaces and Solids. Colors and 3D Textures 
12 marks 
5.  Animation 
12 marks 
Total: 60 marks 
All the experiments are personalized, i.e. each student will have different data to work with. The personalization is based on using two last digits of your matriculation number:
U1234567G
NM which can be integer numbers from 0 to 9 where 0 will stand for 10. Therefore, the two numbers from 1 to 10 will define your personal variant of the assignments. These numbers will be further referred to as N for penultimate digit and M for the last digit.
This is an individual assignment.In the remaining part of the manual, you will find the assignment instructions. Each of the five lab assignments will be evaluated and awarded up to 12 marks. Partial marks are indicated in the assignment instructions.
After completion of each of five lab assignment, you have to write a report following the template shown in Fig. 8.
WITHIN ONE WEEK (7*24 HOURS) AFTER THE END OF EACH OF FIVE SCHEDULED LAB SESSION you have to do the following:
1.       Create  a  folder  and   name   it exactly as  your   name   is  written  on your matriculation card and add as a suffix the two last matric number NM, e.g., JAMES BOND 67.
2.       Copy to this folder the scan/photo of your matriculation card with clearly readable name, photo, and at least three last characters of the matriculation number. Do not make any additional subfolders
3.       Copy to this folder the PDF fie of the report and all the relevant *.func files.
4.       Zip your assignment folder. The zipped file must have the same name as your folder, e.g., JAMES BOND 67.zip. Please check that your file can be unzipped to the folder with your name.
5.       Submit the zipped file through the respective digital drop box in the lab website (note that website has been created for each lab group).
6.       Check your email  box  regularly. The lab instructors or subject coordinator will email you if something is wrong.
CZ2003: Lab # 1 {, 2, 3, 4 or 5}
Q1a
A screenshot of the shape displayed with coordinate axes (lab 1-4) or 3 screenshots from animation (lab 5)
Name of the file: Q1a.func (for labs 1-3) or Q1.func (for lab 4 and 5)
Q1b 
A screenshot of the shape displayed with coordinate axes (lab 1-4)
Name of the file: Q1b.func (for labs 1-3)
Q1c 
A screenshot of the shape displayed with coordinate axes (lab 1-4)
Name of the file: Q1c.func (for labs 1-3)
Q1c 
A screenshot of the shape displayed with coordinate axes (lab 1-4)
Name of the file: Q1d.func (for labs 1-3)
Q2 
A screenshot of the shape displayed with coordinate axes (lab 1-4) or
3 screenshots from animation (lab 5)
Name of the file: Q2.func
Q3 
A screenshot of the shape displayed with coordinate axes (lab 1-4) or
3 screenshots from animation (lab 5)
Name of the file: Q3.func
Figure 8. Template of the report.
4.1 Experiment 1: Parametric Curves This assignment illustrates Module 3, and it serves a purpose to teach you how to visualize curves defined by parametric functions. To work on this assignment, you have to watch the following TEL lectures:
Module 1:  Lecture 2 (Part 3) - Introduction to Computer Graphics and Foundation Mathematics {Rene Descartes and coordinate systems} 
Module 3:  Lecture 1 (Part 2/3) - Geometric Shapes: 2D Curves {straight-lines} 
Module 3:  Lecture 1 (Part 3/3) - Geometric Shapes: 2D Curves {straight-lines} 
Module 3:  Lecture 2 (Part 1/3) - Geometric Shapes: 2D Curves {circle} 
Module 3:  Lecture 2 (Part 2/3) - Geometric Shapes: 2D Curves {circle and beyond} 
Module 3:  Lecture 2 (Part 3/3) - Geometric Shapes: 2D Curves {ellipse and summary} 
Module 3:  Lecture 3 - Geometric Shapes: 3D Curves 
Assignment instructions: 
Create folder Lab1.  Download  into  it  from the course-site the file ParametricCurve.func (Fig. 9). Use it as a reference for the following exercises with curves. For each of the displayed curves, you have to select a sampling resolution providing for smooth curve visualization. Each of the curves has to be displayed within 1 sec and using red color with black coordinate axes on the white background.
1.       Using  functions  x (u), y(u), u  ∈  [0,1],  define  parametrically  in  4  separate  files  and display:
a.       A straight line segment spanning from the point with coordinates (-N,-M) to the point with coordinates (M,N).
b.       A circular arc with radius N and the polar angle spanning from  to 2π , centered at point with coordinates (N,M).
c.       An  origin-centered  2D  spiral  curve  which  starts  at  the  origin,  makes N+M 
revolutions clockwise (as counted from the positive axis X) and reaches eventually the radius 2*M. 
d.      A 3D cylindrical  helix with radius N which is aligned with axis Z and makes M clockwise revolutions about it (as counted from the positive axis X) while spanning from z1  = −N to z2  = M.    (4 marks)
2.       Based  on  the  explicit  definition  of  the  curve  with  number M (Table  1),  derive  its parametric representation x (u), y(u), u ∈ [0,1], and then modify it to scale and translate the curve so that it will make N full periodic oscillations*  within the given x-domain (Fig. 10). Display the curve.   (4 marks)
3.       A so-called “butterfly curve” is defined in polar coordinates by:
r = esin − 2cos + sin5  T
Derive its parametric representation in Cartesian coordinates as x (u), y(u), u ∈ [0,1] and display the curve with the centre at coordinates (N, M).    (4 marks)
Figure 9.   Displaying the shape defined in ParametricCurve.func. 



         
加QQ：99515681  WX：codinghelp
