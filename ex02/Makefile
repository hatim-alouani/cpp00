SRCS = Account.cpp tests.cpp
NAME = Account
CC = c++ -Wall -Wextra -Werror -std=c++98 -g -fsanitize=address

all: $(NAME)

$(NAME): $(SRCS) 
	$(CC) $(SRCS) -o $(NAME)

%.o: %.cpp %.hpp
	$(CC) -c $< -o $@

clean: 
	rm -rf $(NAME)

fclean: clean

re: fclean all
