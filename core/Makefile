#   Copyright 2014 Check Point Software Technologies LTD
#
#   Licensed under the Apache License, Version 2.0 (the "License");
#	you may not use this file except in compliance with the License.
#   You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
#   Unless required by applicable law or agreed to in writing, software
#   distributed under the License is distributed on an "AS IS" BASIS,
#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#   See the License for the specific language governing permissions and
#   limitations under the License.

# Variable definition

SRCS = core.c 
OBJS = core.o 
HDRS = core.h basic_types.h network_types.h
INC= -I../known

CC = gcc
CFLAGS = -g -Werror -Wall -c -D_FILE_OFFSET_BITS=64 -D__USE_LARGEFILE
RM=rm

# Default Target

$(OBJS):	$(SRCS) $(HDRS) 
	$(CC) $(CFLAGS) $(INC) $(SRCS)
 
clean: 
	@echo "* Cleaning core folder..."
	$(RM) -f *.o
