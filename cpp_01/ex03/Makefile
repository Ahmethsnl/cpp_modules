SRCS	= main.cpp HumanA.cpp HumanB.cpp Weapon.cpp

OBJ		= $(SRCS:.cpp=.o)

NAME	= weapon

CPP		= c++

FLAGS	= -Wall -Wextra -Werror -std=c++98

all:	$(NAME)

$(NAME): $(OBJ)
	c++ $(FLAGS) -o $(NAME) $(OBJ)

%.o: %.cpp
	$(CPP) $(FLAGS) -c $< -o $@

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)

re:	fclean all

.PHONY: all clean fclean re