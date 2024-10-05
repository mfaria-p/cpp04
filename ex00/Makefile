SRCS =	main.cpp \
		Animal.cpp \
		Cat.cpp \
        Dog.cpp

OBJS = $(SRCS:.cpp=.o)

NAME = scavtrap
CC = c++
CPPFLAGS = -std=c++98 -Wall -Wextra -Werror

all: $(NAME)

$(NAME): $(OBJS)
	$(CC) $(CPPFLAGS) $(OBJS) -o $(NAME)

%.o: %.cpp
	$(CC) $(CPPFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS)

fclean: clean
	$(RM) $(NAME)

re: fclean all