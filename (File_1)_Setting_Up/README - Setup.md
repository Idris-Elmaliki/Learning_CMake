How to Begin Setting up with CMake (The Basics)

===

When using CMake, there are multiple ways that you can build your CMake system:

1. *Using the GUI/Command Line*

   * When using the GUI or Command Line, it is very easy and while they differ in steps. What they produce is the same!
   * **GUI:**

     * For the GUI you simply just use the GUI and tell CMake what project you want to build for and what denpedcies you want to get linked
   * **CLI**:

     * For the CLI, it is more involved but is much easier than the GUI
     * In the project directory, run the following commands:

       * mkdir build -> cd build -> cmake ..
   * Both will create the build folder and the CMake files for the specific solution, and it will create seperate solutions for each project listed in the CMakeList.txt
   * The Problem with this apporach is that you have to keep on rebuilding your CMake files whenever you update your linked files
   * Luckily there's another way

2. *Letting Visual Studio do the Work*

   * Instead of creating the build folder ourselves (through the gui or cmd), we can just get Visual Studio to make it for us.
   * How can we do this? We just simply open the project with visual studio in the project folder itself.
   * This allows us to use CMake without worrying about manually reupdating CMake and having multiple solution configs!
* Note: If you have any issues, either update the *Cmakelist.txt* file with the cmd **ctrl + s**, else delete the **/out** folder and reload the Cmake file with **ctrl + s**.


That is how you get CMake running on a basic application!

