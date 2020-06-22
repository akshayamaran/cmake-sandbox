Folder structure :
root-folder
	main.c 
	main.h	
		-dir
			-sub_dir
				file.h
			


sub_dir/file.h is called in main function. To add the above folder structure include path in cmake following steps should be followed.

Step-1:
	create empty CMakeLists.txt file
Step-2:
	Add the below lines in the CMakeLists.txt file

cmake_minimum_required(VERSION 3.17)
project(sample)
include_directories("dir")
add_executable(sample main.c main.h)

To run the file use following command:
cmake .
make
./sample

To remove:
rm -rf CMakeFiles MakeFile cmake_install.cmake 