# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jubaldo <jubaldo@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/03/21 22:22:22 by jubaldo           #+#    #+#              #
#    Updated: 2024/03/25 15:33:45 by jubaldo          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME			=			account

SRCS			=			Account.cpp tests.cpp

CC				=			c++

CFLAGS			=			-Wall -Wextra -Werror -std=c++98

RM				=			rm -rf

OBJS			=			$(SRCS:.cpp=.o)

all				:			$(NAME)

$(NAME)			:			$(OBJS)
								$(CC) $(CFLAGS) -o $(NAME) $(OBJS)

%.o				:			%.cpp
								$(CC) $(CFLAGS) -c $< -o $@

clean			:
								$(RM) $(OBJS)

fclean			:			clean
								$(RM) $(NAME)

re				:			fclean all

prog			:			all clean
									clear
											
.PHONY			:			all clean fclean re