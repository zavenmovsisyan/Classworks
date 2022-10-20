T=make_res
cc=g++
PATH_SRC=./src/
PATH_OBJ=./obj/

$(info $("I am here"))
SRC=$(wildcard $(PATH_SRC)*.cpp)
OBJ=$(patsubst $(PATH_SRC)%.cpp, $(PATH_OBJ)%.o, $(SRC))

$(PATH_OBJ)%.o : $(PATH_SRC)%.cpp
	$(cc) -c $< -o $@ 
all: $T

$T: $(OBJ)
	$(cc) $(OBJ) -o $T

install:
	sudo install ./$T /usr/local/bin

uninstall:
	sudo rm  /usr/local/bin/$T

clear:
	rm -f $(PATH_OBJ)*.o $T
