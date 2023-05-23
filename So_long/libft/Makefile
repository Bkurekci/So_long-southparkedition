# ************************************************************************** #
#                                                                            #
#                                                        :::      ::::::::   #
#   Makefile                                           :+:      :+:    :+:   #
#                                                    +:+ +:+         +:+     #
#   By: bukurekc <42istanbul.com.tr>               +#+  +:+       +#+        #
#                                                +#+#+#+#+#+   +#+           #
#   Created: 2022/12/19 17:03:17 by bukurekc          #+#    #+#             #
#   Updated: 2022/12/25 12:23:46 by bukurekc         ###   ########.tr       #
#                                                                            #
# ************************************************************************** #

NAME = libft.a
FLAG = -Wall -Wextra -Werror
SRC = $(shell find . ! -name "ft_lst*.c" -name "ft_*.c")
BONUS = $(shell find . -name "ft_lst*.c")

CC		= gcc

all: $(NAME)

$(NAME):
	@$(CC) $(FLAG) -c $(SRC)
	@echo "\(^-^)/"
	@ar rc $(NAME) *.o
bonus:
	@$(CC) $(FLAG) -c $(BONUS)
	@echo "\(^-^)/"
	@ar rc $(NAME) *.o
clean:
	@/bin/rm -f  *.o *.out
fclean: clean
	@/bin/rm -f $(NAME)
	@echo "🗑️"

re: fclean all

.PHONY: all bonus clean fclean re
