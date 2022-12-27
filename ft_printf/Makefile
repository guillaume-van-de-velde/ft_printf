SRCS = ft_printf.c ft_put_str_char.c ft_address_hex.c ft_nbr.c ft_what.c\
ft_minimum_field_width.c ft_fonctions_bonus.c ft_minus.c ft_check_first_flags.c
HEADER = printf.h
OBJS = ${SRCS:.c=.o}
NAME = libftprintf.a
LIBC = ar rc
LIBR = ranlib
CC 	= gcc
RM 	= rm -f
CFLAGS = -Wall -Wextra -Werror
INCLUDES = -I.

.c.o:
	 ${CC} ${CFLAGS} ${INCLUDES} -c $< -o ${<:.c=.o}

${NAME}: ${OBJS}
	 ${LIBC} ${NAME} ${OBJS}
	 ${LIBR} ${NAME}

all: ${NAME}

bonus: all

clean:
	 ${RM} ${OBJS}

fclean: clean
	 ${RM} ${NAME}

re: fclean all

.PHONY:	all bonus clean fclean re
