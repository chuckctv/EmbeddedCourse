#******************************************************************************
# Copyright (C) 2017 by Alex Fosdick - University of Colorado
#
# Redistribution, modification or use of this software in source or binary
# forms is permitted as long as the files maintain this copyright. Users are 
# permitted to modify this and use it to learn about the field of embedded
# software. Alex Fosdick and the University of Colorado are not liable for any
# misuse of this material. 
#
#*****************************************************************************

#------------------------------------------------------------------------------
# MAKEFILE : Week-2 Assignment Project
#
# Use: make [TARGET] [PLATFORM-OVERRIDES]
#
# Build Targets:
#      MSP432: msp432p401r.lds / Host: DMSP432
#
# Platform Overrides
#      
#
#------------------------------------------------------------------------------
include sources.mk

# Platform Overrides
PLATFORM = MSP432

	ifeq ($(PLATFORM),MSP432)
		CC = arm-none-eabi-gcc
		# etc
	else
		CC = gcc
		# etc
	endif

# Architectures Specific Flags
LINKER_FILE = -T msp432p401r.lds
CPU = -mcpu=cortex-m4
ARCH = -mthumb
SPECS = --specs=nosys.specs

# Compiler Flags and Defines
CC = arm-none-eabi-gcc
LD = 
LDFLAGS = -Wl
CFLAGS = -Wall -g -mthumb
CPPFLAGs = 

