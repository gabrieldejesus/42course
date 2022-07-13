# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: gde-jesu <gde-jesu@student.42.rio>         +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/07/04 23:09:00 by gde-jesu          #+#    #+#              #
#    Updated: 2022/07/07 01:25:11 by gde-jesu         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a
SRCS =	ft_printf.c \
			ft_putchar.c \
			ft_strlen.c \
			ft_putstr.c \
			ft_flag_s.c \
			ft_flag_u.c \
			ft_flags_di.c \
			ft_flag_x.c \
			ft_flag_p.c
CC	=	cc
CFLAGS	= -Wall -Wextra -Werror -c
OBJS = $(SRCS:.c=.o)
RM = rm -f
ARC = ar -rcs

$(NAME):
	$(CC) $(CFLAGS) -I. $(SRCS)
	$(ARC) $(NAME) $(OBJS)

all:		$(NAME)

clean:
	$(RM) $(OBJS)

fclean:		clean
	$(RM) $(NAME)

re:			fclean all

.PHONY:		all fclean clean re
