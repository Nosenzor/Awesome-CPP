# Awesome-CPP
My Awesome C++ List : Quick Notes.

# Blogs & Conferences

## Confs
* CPPCON : The Best conference for C++ : https://github.com/CppCon

## Blogs
* The very pertinent blog of Jonathan Boccara : Fluent CPP : https://www.fluentcpp.com


# Memory Management

## Memory Allocators 
* **Mesh Allocator** by **Emery Berger**, an allocator that avoid memory fragmentation : https://github.com/CppCon/CppCon2019/tree/master/Presentations/mesh_automatically_compacting_your_cpp_applications_memory, presenation : https://www.youtube.com/watch?v=XRAP3lBivYM
* **Hoard** by the same **Emery Berger** (his previous work) a fast memory allocator : http://hoard.org/
* **SnMalloc** and **MiMalloc** are two **Microsoft projects** for Allocators: https://github.com/Microsoft/snmalloc and https://github.com/microsoft/mimalloc. A comprehensive benchmark can be found in Mimalloc page : https://github.com/microsoft/mimalloc#performance where you can retrieve JeMalloc, rpmalloc, jemalloc, Hoard and Mesh allocators.

# Performance 
 * **Richard Fabian**'s book on Data Oriented Design : https://www.dataorienteddesign.com/dodbook/ ... it's free !
 * **Eve** a simd library by **Joel Falcou** and **Jean-Thierry Lapreste** : https://jfalcou.github.io/eve/index.html
* One of my favourite author when it comes to speak about performance **Agner Fog** and here is a free booklet on simd and the Vex library : https://www.agner.org/optimize/vcl_manual.pdf. Be sure to have a look on his website (https://www.agner.org/optimize/) and github (https://github.com/vectorclass)
 * Excellent talks
   * CppCon 2017: [Carl Cook “When a Microsecond Is an Eternity: High Performance Trading Systems in C++”](https://www.youtube.com/watch?v=NH1Tta7purM)  
   * Meeting C++ 2018 : [Writing cache friendly C++ - Jonathan Müller]( https://www.youtube.com/watch?v=Nz9SiF0QVKY)
   * CppCon 2019: [Andrei Alexandrescu “Speed Is Found In The Minds of People"](https://www.youtube.com/watch?v=FJJTYQYB1JQ)
   * CppCon 2020 : [Emery Berger Plenary: Performance Matters](https://www.youtube.com/watch?v=koTf7u0v41o)
  
  
# Modern C++
 
* experiments of move constructors and noexept attribute in containers ... quite instructive : http://www.hlsl.co.uk/blog/2017/12/1/c-noexcept-and-move-constructors-effect-on-performance-in-stl-containers

# Other Awesome lists
* An amazing awesome list;-) (really complete) : https://github.com/fffaraz/awesome-cpp#static-code-analysis
* Another great awesome list (a list of lists) : https://github.com/MattPD/cpplinks
* A list of headers only porject ...wow : https://github.com/p-ranav/awesome-hpp

# Geometry

## Polygon Triangulation

* The famous "Triangle" Library by **Jonathan Richard Shewchuck** <3 : http://www.cs.cmu.edu/~quake/triangle.html (Constrained Delaunay with robust predicates)
* Extended Ear Clipping methods that can handle holes : https://github.com/mapbox/earcut.hpp (header only, non Delaunay triangulation, non robust...but can be patched to be robust ?)
* **J Ratcliff** "Efficient Polygon Triangulation" on Flipcode (do not handle hole, code is a bit old ...) : https://www.flipcode.com/archives/Efficient_Polygon_Triangulation.shtml
* A review of some polygon implementations available to sue on VTerrain by **Ben Discoe** : http://vterrain.org/Implementation/Libs/triangulate.html
* **Do Anyone tried to implement or know an opensourse implementation of the Bernard Chazelle's "Triangulating a Simple Polygon in Linear Time" algorithm ?** https://www.cs.princeton.edu/~chazelle/pubs/polygon-triang.pdf

# GUI
 * improve your command line 'Gui' with beautiful progress bars. Don't miss it if you are a true geek :-) https://github.com/p-ranav/indicators
 * Nanogui by **Wenzel Jakob** (it's incredible how many essential good projects this guy have in its github !!) :  https://github.com/wjakob/nanogui
 * Dear ImGui by **Omar 'Ocornut** : https://github.com/ocornut (The documentation and examples are numerous)
 
# CMAKE and Build Tools
As a beginner in CMake i'd need a lot of tutorials to master this powerful tool !!
* https://github.com/ttroy50/cmake-examples
* A really simple CMAKE example but usefull for me as a beginner http://techminded.net/blog/modular-c-projects-with-cmake.html
* A starting guide *In french* by **Alexandre Laurent** : https://alexandre-laurent.developpez.com/tutoriels/cmake/
## Some Perf tracker 
* Comparing Valgrind, & Sanitizers : https://developers.redhat.com/blog/2021/05/05/memory-error-checking-in-c-and-c-comparing-sanitizers-and-valgrind#performance_benefits_of_sanitizers
