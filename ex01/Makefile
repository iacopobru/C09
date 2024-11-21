COMPILER = cc
CFLAGS = -Wall -Wextra -Werror
INCLUDES = includes
SRC_DIR = scrs

SRCS = $(SRC_DIR)/ft_putchar.c $(SRC_DIR)/ft_putstr.c $(SRC_DIR)/ft_strcmp.c $(SRC_DIR)/ft_strlen.c $(SRC_DIR)/ft_swap.c
OBJS = $(SRCS:.c=.o)

all: libft.a

libft.a: $(OBJS)
	ar -rc $@ $(OBJS)

$(SRC_DIR)/%.o: $(SRC_DIR)/%.c
	$(COMPILER) -c $< -o $@ -I$(INCLUDES)

clean:
	rm -f $(OBJS)

fclean: clean
	rm -f libft.a

re: fclean all
