SRCS	=	main.cpp PhoneBook.cpp Contact.cpp Utils.cpp UtilsTwo.cpp
OBJS	=	$(SRCS:.cpp=.o)
CC		=	c++
CFLAGS	=	-Wall -Wextra -Werror -std=c++98 #-fsanitize=address
NAME	=	replace

all: $(NAME)

$(NAME): $(OBJS)
	$(CC) $(CFLAGS) -o $(NAME) $(OBJS)

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re