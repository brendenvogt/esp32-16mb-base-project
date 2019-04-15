# Esp32 Eclipse Template
This is a template project for c/c++ esp32 projects built using makefiles
# Prerequisite
	install esp-idf
	check $PATH
	check $IDF_PATH
   check $ADF_PATH (if applicable)

# Setup
   1. edit include.xml
      change esp32_template to your project name
   2. start eclipse
   3. config make-targets for (if exist copy them from previous project)
      menuconfig
      all (Target "-j8 all")
      clear
      flash (Command gnome-terminal -x make)
      monitor (Command gnome-terminal -x make)
      flash monitor (Command gnome-terminal -x make)
    4. import include.xml 
      Project Explorer -> Properties -> C/C++ General -> Paths and Symbols
		
		Includes -> Import Serttings
		Browse (Open File include.xml) 
      -> Finish
     5. Use Make-Targets menuconfig
     6. Use Make-Targets all, flash and monitor
     7. add preprocessor provider xtensa-esp32-elf-gcc

	




