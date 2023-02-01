# Awesome-CPP
My Awesome C++ List : Quick Notes.

# Blogs & Conferences

## Confs
* CPPCON : The Best conference for C++ : https://github.com/CppCon

## Blogs
* The very pertinent blog of Jonathan Boccara : Fluent CPP : https://www.fluentcpp.com


# Memory Management

## Memory Allocators 
* **Mesh Allocator** by **Emery Berger**, an allocator that avoid memory fragmentation : https://github.com/CppCon/CppCon2019/tree/master/Presentations/mesh_automatically_compacting_your_cpp_applications_memory, presentation : https://www.youtube.com/watch?v=XRAP3lBivYM
* **Hoard** by the same **Emery Berger** (his previous work) a fast memory allocator : http://hoard.org/
* **SnMalloc** and **MiMalloc** are two **Microsoft projects** for Allocators: https://github.com/Microsoft/snmalloc and https://github.com/microsoft/mimalloc. A comprehensive benchmark can be found in Mimalloc page : https://github.com/microsoft/mimalloc#performance where you can retrieve JeMalloc, rpmalloc, jemalloc, Hoard and Mesh allocators.

# Performance 
 
## SIMD
 * **Eve** a simd library by **Joel Falcou** and **Jean-Thierry Lapreste** : https://jfalcou.github.io/eve/index.html
* One of my favourite author when it comes to speak about performance **Agner Fog** and here is a free booklet on simd and the **Vex library** : https://www.agner.org/optimize/vcl_manual.pdf. Be sure to have a look on his website (https://www.agner.org/optimize/) and github (https://github.com/vectorclass)
* **XSIMD** [C++ wrappers for SIMD intrinsics](https://github.com/xtensor-stack/xsimd). Maybe not as complete as EVE but very convenient and easy to use.
* **Highway** [C++ library that provides portable SIMD/vector intrinsics](https://github.com/google/highway) a very complete library (that supports many kind of CPUs) that has been the based framework for Google SIMD based sorting algorithm.
 ## Excellent talks
   * CppCon 2017: [Carl Cook “When a Microsecond Is an Eternity: High Performance Trading Systems in C++”](https://www.youtube.com/watch?v=NH1Tta7purM)
   * Meeting C++ 2018 : [Writing cache friendly C++ - Jonathan Müller]( https://www.youtube.com/watch?v=Nz9SiF0QVKY)
   * CppCon 2019: [Andrei Alexandrescu “Speed Is Found In The Minds of People"](https://www.youtube.com/watch?v=FJJTYQYB1JQ)
   * CppCon 2019 : [Alan Talbot “How to Choose the Right Standard Library Container, and Why You Should Want Some More”] (https://youtu.be/yjPKVOYcw28), because everyone can improve on using the right container.
   * CppCon 2020 : [Emery Berger Plenary: Performance Matters](https://www.youtube.com/watch?v=koTf7u0v41o)
   * CppCon 2022 : [Jan Bielak amazing talk The Most Important Optimizations to Apply in Your C++ programs](https://youtu.be/qCjEN5XRzHc), but don't forget to pick the right algorithms and structure first !!!
 ## Books and papers
 * **Richard Fabian**'s book on Data Oriented Design : https://www.dataorienteddesign.com/dodbook/ ... it's free !
 * **Martin Ankerl** did an excellent benchmark and review on Hash Maps while he created his own implementation : https://martin.ankerl.com/2019/04/01/hashmap-benchmarks-01-overview/
  * **Denis Bakhvalov** Precious performance information scattered on [his "easyperf" site](https://easyperf.net), [YouTube](https://www.youtube.com/channel/UCGmEJdQ993cdCGdnLZDuOOQ/videos) and [GitHub](https://github.com/dendibakh)
  *  **Codee** [knowledge database](https://www.codee.com/knowledge/) a good set of optimization tricks with easy to understand examples
  
# Modern C++
 
* experiments of move constructors and noexept attribute in containers ... quite instructive : http://www.hlsl.co.uk/blog/2017/12/1/c-noexcept-and-move-constructors-effect-on-performance-in-stl-containers
* **Jason Turner** [C++ Weekly on YouTube](https://www.youtube.com/playlist?list=PLs3KjaCtOwSZ2tbuV1hx8Xz-rFZTan2J1) and his [Lefticus GitHub](https://github.com/lefticus) where you can find template to start (or improve) your C++ project https://github.com/cpp-best-practices/cpp_starter_project. Also check his [website](https://articles.emptycrate.com), but a bit outdated IMO...

# Other Awesome lists
* An amazing awesome list;-) (really complete) : https://github.com/fffaraz/awesome-cpp#static-code-analysis
* Another great awesome list (a list of lists) : https://github.com/MattPD/cpplinks
* A list of headers only porject ...wow : https://github.com/p-ranav/awesome-hpp

# Geometry
## Very cool General Mesh and Cloud of Points Libraries
 * **The Polygon Mesh Library**(PMP) : http://www.pmp-library.org  by **Daniel Sieger and Mario Botsch**. A general libraires with a high quality toolbox on Meshes (Remeshing, cleaning, open/write different format) with a viewer.License : MIT
 * **OpenMesh** : http://www.openmesh.org/ or https://www.graphics.rwth-aachen.de/software/openmesh/ from the Aachen University. Founded by some of my most inspiring researchers Pr Leif Kobbelt and Marcel Campen. OpenMesh serves as a foundation to the PMP Library too !. Can be found as a vcpkg packet ! Open Mesh introduced the famous Half-Edge data structure and provide a lot of tools (decimation, read/write STL/OBJ/OFF) and moreover can be easily extended. Have a python binding... what else? License : BSD V3
 * **TriMesh** (from Szymon Rusinkiewicz) : https://gfx.cs.princeton.edu/proj/trimesh2/ adapted by Jeroen Baert : https://github.com/Forceflow/trimesh2 although a bit old in its implementation its simplicity is its asset. Can read and write many differents types (OFF, OBJ, STL ..and older exotic types !) License : GPL
* **LibIGL** : https://libigl.github.io from **Alec Jacobson and Daniele Panozzo and others**. A header only library :-) 

## Dealing with numerical problems
 * A nice demo of floating point computation problems : https://simontoth.substack.com/p/daily-bite-of-c-numbers-are-not-easy
* Boost interval arithmetic can really help to build your predicates canvas https://www.boost.org/doc/libs/1_81_0/libs/numeric/interval/doc/interval.htm
* Within Shewchuck Triangle library you can find a set of robust predicates based on double expansion : http://www.cs.cmu.edu/~quake/triangle.html

## Polygon Triangulation

* The famous "Triangle" Library by **Jonathan Richard Shewchuck** <3 : http://www.cs.cmu.edu/~quake/triangle.html (Constrained Delaunay with robust predicates)
* Extended Ear Clipping methods that can handle holes : https://github.com/mapbox/earcut.hpp (header only, non Delaunay triangulation, non robust...but can be patched to be robust ?)
* **J Ratcliff** "Efficient Polygon Triangulation" on Flipcode (do not handle hole, code is a bit old ...) : https://www.flipcode.com/archives/Efficient_Polygon_Triangulation.shtml
* A review of some polygon implementations available to sue on VTerrain by **Ben Discoe** : http://vterrain.org/Implementation/Libs/triangulate.html
* **Do Anyone tried to implement or know an opensourse implementation of the Bernard Chazelle's "Triangulating a Simple Polygon in Linear Time" algorithm ?** https://www.cs.princeton.edu/~chazelle/pubs/polygon-triang.pdf

## Other Geometry tools
* **PolyLabel** : https://github.com/mapbox/polylabel. A library to find the "polygon pole of inaccessibility, the most distant internal point from the polygon outline (not to be confused with centroid)".

# GUI
 * improve your command line 'Gui' with beautiful progress bars. Don't miss it if you are a true geek :-) https://github.com/p-ranav/indicators
 * Nanogui by **Wenzel Jakob** (it's incredible how many essential good projects this guy have in its github !!) :  https://github.com/wjakob/nanogui
 * Dear ImGui by **Omar 'Ocornut** : https://github.com/ocornut (The documentation and examples are numerous)
 
# CMAKE and Build Tools
As a beginner in CMake i'd need a lot of tutorials to master this powerful tool !!
* Project Option : A lot of resources to have a nice start using Cmake : https://github.com/cpp-best-practices/project_options/
* https://github.com/ttroy50/cmake-examples
* A really simple CMAKE example but usefull for me as a beginner http://techminded.net/blog/modular-c-projects-with-cmake.html
* A starting guide *In french* by **Alexandre Laurent** : https://alexandre-laurent.developpez.com/tutoriels/cmake/
* Understanding Compile Time : http://coding-scars.com/investigating-cpp-compile-times-1/
* Package manager, I use vcpkg https://vcpkg.io/ (simply because I have been able to set it up quicker than Conan ..)
* I try to use GitHub Actions but for now I'm not very successful . Here's some resources I use :
  * A GitHub actions hosted on your computer. https://github.com/nektos/act 5i'm trying to set it up)

## Some Perf tracker 
* Comparing Valgrind, & Sanitizers : https://developers.redhat.com/blog/2021/05/05/memory-error-checking-in-c-and-c-comparing-sanitizers-and-valgrind#performance_benefits_of_sanitizers

