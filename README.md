# C-_Cross_Platform_GUI_For_Beginners
Getting Started with wxWidgets in Linux

---

##### Install wxWidgets

1. Make sure wxwidgets-gtk3 is installed in your linux distro
2. Download source code from this [link](https://wxwidgets.org/downloads/)
3. Extract the archive
4. Set the extracted directory as an environmental variable
5. Within the extracted directory, create a directory called gtk-build and `cd` into it
6. Run `../configure && make -j2 && sudo make install && sudo ldconfig`
    - replace the 2 in `j2` with the number of cores that your cpu has
7. Then, in another directory like the home directory, run wx-config to ensure status

##### Creating a Hello_World Window

Create a class to represent the window
1. Create the header file and cpp source code from this [link](https://wiki.wxwidgets.org/Hello_World)
2. Run it with `g++ HelloWorldApp.cpp `wx-config --libs` `wx-config --cxxflags` -o HelloWorldApp`
