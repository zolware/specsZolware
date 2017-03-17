============
Architecture
============

|

.. comments

:Author(s):
   Francois Roy

:Date Created: 03-12-2017

:Language: None

:Status: :red:`Draft`

-----------


Description
-----------

The data service is a web application that allows the user to get real data and/or generate simulated signals in real time.


Architecture
------------

A guide for understanding what things evolved from as a project ages and grow in scope.

.. graphviz::

   digraph Flatland {
   
      a -> b -> c -> g; 
      a  [shape=polygon,sides=4,label="Signal Emulator"]
      b  [shape=polygon,sides=5,label="Model DB (postgresql)"]
      c  [shape=polygon,sides=6,label="Data DB (MongoDB)"]
   
      g [peripheries=3,color=yellow,label="Static files server"];
      s [shape=invtriangle,peripheries=1,color=red,style=filled];
      w  [shape=triangle,peripheries=1,color=blue,style=filled];
      
      }

