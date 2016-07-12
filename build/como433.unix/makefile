############################################################################
# File:     makefile
#
# Purpose:  Makefile for the shwild project, for the Comeau C/C++ Compiler v4.3.3
#           compiler, on UNIX
#
# Created:  15th February 2005
# Updated:  11th July 2006
#
############################################################################


############################################################################
# symbols

########################################
# project & compiler version

COMP_TAG            =   como433
ARCH_TAG            =   
OS_TAG              =   
PROJ_TAG            =   shwild
PROJ_VER_MAJOR      =   0
PROJ_MOD_TAG        =   core
PROJ_TAG_VER        =   $(PROJ_TAG).$(PROJ_VER_MAJOR).$(PROJ_MOD_TAG)
COMP_ARCH_OS_TAG    =   $(COMP_TAG)$(OS_TAG)$(ARCH_TAG)

########################################
# dependencies

XTESTS_VER_MAJOR    =   0
XTESTS_TAG_VER      =   xtests.$(XTESTS_VER_MAJOR)

UNIXEM_VER_MAJOR    =   1
UNIXEM_TAG_VER      =   unixem.$(UNIXEM_VER_MAJOR)

PROJ_MAKEFILE_NAME  =   makefile

########################################
# testing verbosity

TEST_VERBOSITY      =   2


############################################################################
# directories

########################################
# project directories

PROJ_BASE_DIR           =   ../..
PROJ_BIN_DIR            =   $(PROJ_BASE_DIR)/bin
PROJ_INCLUDE_DIR        =   $(PROJ_BASE_DIR)/include
PROJ_LIB_DIR            =   $(PROJ_BASE_DIR)/lib
PROJ_OBJ_DIR            =   .
PROJ_SRC_DIR            =   $(PROJ_BASE_DIR)/src
PROJ_EXAMPLES_DIR       =   $(PROJ_BASE_DIR)/examples
PROJ_SAMPLES_DIR        =   $(PROJ_BASE_DIR)/samples
PROJ_TEST_ROOT_DIR      =   $(PROJ_BASE_DIR)/test
PROJ_TEST_COMPONENT_DIR =   $(PROJ_TEST_ROOT_DIR)/component
PROJ_TEST_SCRATCH_DIR   =   $(PROJ_TEST_ROOT_DIR)/scratch
PROJ_TEST_UNIT_DIR      =   $(PROJ_TEST_ROOT_DIR)/unit

########################################
# 3rd-party directories

XTESTS_PROJ_INCLUDE		=	
XTESTS_INCLUDE_DIR		=   $(PROJ_BASE_DIR)/include
XTESTS_SRC_DIR			=   $(PROJ_SRC_DIR)/xtests

############################################################################
# tools

CC                      =   como
CPPC                    =   como
AR                      =   ar
LD                      =   como
RM                      =   rm -f
CP                      =   cp
RC                      =   

############################################################
# compiler

########################################
# includes

INCLUDES_LEADER         =   

PROJ_INCLUDE            =   -I$(PROJ_INCLUDE_DIR)

COMMON_INCLUDES         =

STLSOFT_INCLUDES		=\
 -I"$(STLSOFT)/include"\
 \

THIRDPARTY_INCLUDES		=\
 $(XTESTS_PROJ_INCLUDE)\
 \

# CC

CC_INCLUDES_BASE =\
 $(INCLUDES_LEADER)\
 $(PROJ_INCLUDE)\
 $(COMMON_INCLUDES)\
 $(STLSOFT_INCLUDES)\
 $(THIRDPARTY_INCLUDES)\
 \

CC_INCLUDES_ST_D =\
 $(CC_INCLUDES_BASE)\
 \

CC_INCLUDES_ST_R =\
 $(CC_INCLUDES_BASE)\
 \


CC_SHWILD_INCLUDES_BASE =\
 $(CC_INCLUDES_BASE)\
 \

CC_SHWILD_INCLUDES_ST_D =\
 $(CC_SHWILD_INCLUDES_BASE)\
 \

CC_SHWILD_INCLUDES_ST_R =\
 $(CC_SHWILD_INCLUDES_BASE)\
 \


CC_XTESTS_INCLUDES_BASE =\
 $(CC_INCLUDES_BASE)\
 \

CC_XTESTS_INCLUDES_ST_D =\
 $(CC_XTESTS_INCLUDES_BASE)\
 \

CC_XTESTS_INCLUDES_ST_R =\
 $(CC_XTESTS_INCLUDES_BASE)\
 \


CC_INCLUDES_TEST=\
 $(CC_INCLUDES_BASE)\
 -I"$(OPENRJ_ROOT)/include"\
 \

# CPPC

CPPC_INCLUDES_BASE =\
 $(INCLUDES_LEADER)\
 $(PROJ_INCLUDE)\
 $(COMMON_INCLUDES)\
 $(STLSOFT_INCLUDES)\
 $(THIRDPARTY_INCLUDES)\
 \

CPPC_INCLUDES_ST_D =\
 $(CPPC_INCLUDES_BASE)\
 \

CPPC_INCLUDES_ST_R =\
 $(CPPC_INCLUDES_BASE)\
 \


CPPC_SHWILD_INCLUDES_BASE =\
 $(CPPC_INCLUDES_BASE)\
 \

CPPC_SHWILD_INCLUDES_ST_D =\
 $(CPPC_SHWILD_INCLUDES_BASE)\
 \

CPPC_SHWILD_INCLUDES_ST_R =\
 $(CPPC_SHWILD_INCLUDES_BASE)\
 \


CPPC_XTESTS_INCLUDES_BASE =\
 $(CPPC_INCLUDES_BASE)\
 \

CPPC_XTESTS_INCLUDES_ST_D =\
 $(CPPC_XTESTS_INCLUDES_BASE)\
 \

CPPC_XTESTS_INCLUDES_ST_R =\
 $(CPPC_XTESTS_INCLUDES_BASE)\
 \


CPPC_INCLUDES_TEST=\
 $(CPPC_INCLUDES_BASE)\
 -I"$(OPENRJ_ROOT)/include"\
 \

########################################
# defines

CMN_DEF_NO_IMPLICIT_LINK =\
 -DSHWILD_NO_IMPLICIT_LINK\
 \

COMMON_DEFS             =   -Dunix

CUSTOM_DEFS             =

# CC

CC_CUSTOM_DEFS          =   $(CUSTOM_DEFS)

CC_DEFS_BASE =\
 $(CC_CUSTOM_DEFS)\
 $(COMMON_DEFS)\
 \

CC_DEFS_ST_D =\
 $(CC_DEFS_BASE)\
 \

CC_DEFS_ST_R =\
 $(CC_DEFS_BASE)\
 \


# CPPC

CPPC_CUSTOM_DEFS        =   $(CUSTOM_DEFS)

CPPC_DEFS_BASE =\
 $(CPPC_CUSTOM_DEFS)\
 $(COMMON_DEFS)\
 \

CPPC_DEFS_ST_D =\
 $(CPPC_DEFS_BASE)\
 \

CPPC_DEFS_ST_R =\
 $(CPPC_DEFS_BASE)\
 \


########################################
# flags

# CC

CC_F_NOLOGO             =   --no_version
CC_F_COMPILE_ONLY       =   -c
CC_F_FORCE_INCLUDE      =   
CC_F_WARNING_MAX        =   --A --long_long
CC_F_WARNING_ERR        =   
CC_F_MINIMUM_SIZE       =   
CC_F_MAXIMUM_SPEED      =   

CC_TOOL_FLAGS       =   

CC_FLAGS_BASE =\
 $(CC_TOOL_FLAGS)\
 $(CC_F_NOLOGO)\
 $(CC_F_COMPILE_ONLY)\
 $(CC_F_FORCE_INCLUDE)\
 $(CC_F_WARNING_MAX)\
 $(CC_F_WARNING_ERR)\
 \

CC_FLAGS_ST_D =\
 $(CC_FLAGS_BASE)\
 \

CC_FLAGS_ST_R =\
 $(CC_FLAGS_BASE)\
 \


# CPPC

CPPC_F_NOLOGO           =   --no_version
CPPC_F_COMPILE_ONLY     =   -c
CPPC_F_FORCE_INCLUDE    =   
CPPC_F_WARNING_MAX      =   --long_long
CPPC_F_WARNING_ERR      =   
CPPC_F_EXCEPTIONS_ON    =   
CPPC_F_EXCEPTIONS_OFF   =   
CPPC_F_EXCEPTIONS       =   $(CPPC_F_EXCEPTIONS_ON)
CPPC_F_RTTI_ON          =   
CPPC_F_RTTI_OFF         =   
CPPC_F_RTTI             =   $(CPPC_F_RTTI_ON)
CPPC_F_MINIMUM_SIZE     =   
CPPC_F_MAXIMUM_SPEED    =   

CPPC_TOOL_FLAGS     =   

CPPC_FLAGS_BASE =\
 $(CPPC_TOOL_FLAGS)\
 $(CPPC_F_NOLOGO)\
 $(CPPC_F_COMPILE_ONLY)\
 $(CPPC_F_FORCE_INCLUDE)\
 $(CPPC_F_WARNING_MAX)\
 $(CPPC_F_WARNING_ERR)\
 $(CPPC_F_EXCEPTIONS)\
 $(CPPC_F_RTTI)\
 \

CPPC_FLAGS_ST_D =\
 $(CPPC_FLAGS_BASE)\
 \

CPPC_FLAGS_ST_R =\
 $(CPPC_FLAGS_BASE)\
 \


########################################
# arguments

# CC args (= flags + defines + includes)

CC_ARGS_ST_D=\
 $(CC_FLAGS_ST_D)\
 --c -D_DEBUG -UNDEBUG\
 $(CC_DEFS_ST_D)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CC_INCLUDES_ST_D)
CC_ARGS_ST_D_TEST=\
 $(CC_FLAGS_ST_D)\
 --c -D_DEBUG -UNDEBUG\
 $(CC_DEFS_ST_D)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CC_INCLUDES_TEST)
CC_ARGS_ST_R=\
 $(CC_FLAGS_ST_R)\
 --c -U_DEBUG -DNDEBUG $(CC_F_MAXIMUM_SPEED)\
 $(CC_DEFS_ST_R)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CC_INCLUDES_ST_R)
CC_ARGS_ST_R_TEST=\
 $(CC_FLAGS_ST_R)\
 --c -U_DEBUG -DNDEBUG $(CC_F_MAXIMUM_SPEED)\
 $(CC_DEFS_ST_R)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CC_INCLUDES_TEST)

# CPPC args (= flags + defines + includes)

CPPC_ARGS_ST_D=\
 $(CPPC_FLAGS_ST_D)\
 -D_DEBUG -UNDEBUG\
 $(CPPC_DEFS_ST_D)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CPPC_INCLUDES_ST_D)
CPPC_ARGS_ST_D_TEST=\
 $(CPPC_FLAGS_ST_D)\
 -D_DEBUG -UNDEBUG\
 $(CPPC_DEFS_ST_D)\
 $(CPPC_INCLUDES_TEST)
CPPC_ARGS_ST_R=\
 $(CPPC_FLAGS_ST_R)\
 -U_DEBUG -DNDEBUG $(CPPC_F_MAXIMUM_SPEED)\
 $(CPPC_DEFS_ST_R)\
 $(CMN_DEF_NO_IMPLICIT_LINK)\
 $(CPPC_INCLUDES_ST_R)
CPPC_ARGS_ST_R_TEST=\
 $(CPPC_FLAGS_ST_R)\
 -U_DEBUG -DNDEBUG $(CPPC_F_MAXIMUM_SPEED)\
 $(CPPC_DEFS_ST_R)\
 $(CPPC_INCLUDES_TEST)

############################################################
# archiver

AR_F_NOLOGO             =   

AR_ARGS                 =   

############################################################
# linker

########################################
# flags

LD_F_NOLOGO             =   

LD_FLAGS_BASE           =\
 $(LD_F_NOLOGO)\
 \

LD_FLAGS_ST_D =\
 $(LD_FLAGS_BASE)\
 \

LD_FLAGS_ST_R =\
 $(LD_FLAGS_BASE)\
 \


########################################
# paths

LIBPATHS_ENV            =

LIBPATHS_COMMON         =

LIBPATHS_3PTY           =\
 \

LIBPATHS=\
 $(LIBPATHS_COMMON)\
 $(LIBPATHS_3PTY)\
 $(LIBPATHS_ENV)\
 \

LIBPATHS_TEST =\
 $(LIBPATHS)\
 $(OPENRJ_ROOT)/lib\
 \

########################################
# arguments

LD_ARGS_ST_D      =    $(LD_F_NOLOGO) $(LIBPATHS)
LD_ARGS_ST_D_TEST =    $(LD_F_NOLOGO) $(LIBPATHS_TEST)
LD_ARGS_ST_R      =    $(LD_F_NOLOGO) $(LIBPATHS)
LD_ARGS_ST_R_TEST =    $(LD_F_NOLOGO) $(LIBPATHS_TEST)

############################################################################
# names

############################################################
# source

SRCS_HDR_CORE=\
 $(PROJ_INCLUDE_DIR)/shwild/shwild.h\
 $(PROJ_INCLUDE_DIR)/shwild/implicit_link.h\
 \

SRCS_HDR_MAPPING=\
 $(PROJ_INCLUDE_DIR)/shwild/shwild.hpp\
 \

############################################################
# objects / program-databases

########################################
# libraries

# core

OBJ_CORE_matches__ST_D    =   $(PROJ_OBJ_DIR)/core.matches.debug.o
OBJ_CORE_pattern__ST_D    =   $(PROJ_OBJ_DIR)/core.pattern.debug.o
OBJ_CORE_api__ST_D        =   $(PROJ_OBJ_DIR)/core.api.debug.o

OBJS_CORE_ST_D =\
 $(OBJ_CORE_matches__ST_D)\
 $(OBJ_CORE_pattern__ST_D)\
 $(OBJ_CORE_api__ST_D)\
 \

OBJ_CORE_matches__ST_R    =   $(PROJ_OBJ_DIR)/core.matches.o
OBJ_CORE_pattern__ST_R    =   $(PROJ_OBJ_DIR)/core.pattern.o
OBJ_CORE_api__ST_R        =   $(PROJ_OBJ_DIR)/core.api.o

OBJS_CORE_ST_R =\
 $(OBJ_CORE_matches__ST_R)\
 $(OBJ_CORE_pattern__ST_R)\
 $(OBJ_CORE_api__ST_R)\
 \

OBJS_CORE =\
 $(OBJS_CORE_ST_D)\
 $(OBJS_CORE_ST_R)\
 \

# xTests - testing only

OBJ_xt_core_ST_D         =   $(PROJ_OBJ_DIR)/xtests.core.debug.o

OBJS_XTESTS_ST_D=\
 $(OBJ_xt_core_ST_D)\
 \

OBJ_xt_core_ST_R         =   $(PROJ_OBJ_DIR)/xtests.core.o

OBJS_XTESTS_ST_R=\
 $(OBJ_xt_core_ST_R)\
 \


OBJS_XTESTS=\
 $(OBJS_XTESTS_ST_D)\
 $(OBJS_XTESTS_ST_R)\
 \

# *

OBJS_LIBS =\
 $(OBJS_CORE)\
 \

########################################
# examples

OBJ_EXAMPLE_C_1_ST_D = $(PROJ_OBJ_DIR)/example_c_1.debug.o
OBJ_EXAMPLE_C_2_ST_D = $(PROJ_OBJ_DIR)/example_c_2.debug.o
OBJ_EXAMPLE_CPP_1_ST_D = $(PROJ_OBJ_DIR)/example_cpp_1.debug.o
OBJ_EXAMPLE_CPP_2_ST_D = $(PROJ_OBJ_DIR)/example_cpp_2.debug.o
OBJ_EXAMPLE_C_1_ST_R = $(PROJ_OBJ_DIR)/example_c_1.o
OBJ_EXAMPLE_C_2_ST_R = $(PROJ_OBJ_DIR)/example_c_2.o
OBJ_EXAMPLE_CPP_1_ST_R = $(PROJ_OBJ_DIR)/example_cpp_1.o
OBJ_EXAMPLE_CPP_2_ST_R = $(PROJ_OBJ_DIR)/example_cpp_2.o

OBJS_EXAMPLES =\
 $(OBJ_EXAMPLE_C_1_ST_D)\
 $(OBJ_EXAMPLE_C_2_ST_D)\
 $(OBJ_EXAMPLE_C_1_ST_R)\
 $(OBJ_EXAMPLE_C_2_ST_R)\
 $(OBJ_EXAMPLE_CPP_1_ST_D)\
 $(OBJ_EXAMPLE_CPP_2_ST_D)\
 $(OBJ_EXAMPLE_CPP_1_ST_R)\
 $(OBJ_EXAMPLE_CPP_2_ST_R)\
 \

########################################
# samples

OBJ_SAMPLE_C_1_ST_D = $(PROJ_OBJ_DIR)/sample_c_1.debug.o
OBJ_SAMPLE_C_2_ST_D = $(PROJ_OBJ_DIR)/sample_c_2.debug.o
OBJ_SAMPLE_CPP_1_ST_D = $(PROJ_OBJ_DIR)/sample_cpp_1.debug.o
OBJ_SAMPLE_CPP_2_ST_D = $(PROJ_OBJ_DIR)/sample_cpp_2.debug.o
OBJ_SAMPLE_C_1_ST_R = $(PROJ_OBJ_DIR)/sample_c_1.o
OBJ_SAMPLE_C_2_ST_R = $(PROJ_OBJ_DIR)/sample_c_2.o
OBJ_SAMPLE_CPP_1_ST_R = $(PROJ_OBJ_DIR)/sample_cpp_1.o
OBJ_SAMPLE_CPP_2_ST_R = $(PROJ_OBJ_DIR)/sample_cpp_2.o

OBJS_SAMPLES =\
 $(OBJ_SAMPLE_C_1_ST_D)\
 $(OBJ_SAMPLE_C_2_ST_D)\
 $(OBJ_SAMPLE_C_1_ST_R)\
 $(OBJ_SAMPLE_C_2_ST_R)\
 $(OBJ_SAMPLE_CPP_1_ST_D)\
 $(OBJ_SAMPLE_CPP_2_ST_D)\
 $(OBJ_SAMPLE_CPP_1_ST_R)\
 $(OBJ_SAMPLE_CPP_2_ST_R)\
 \

########################################
# tests

OBJ_TEST_C_1_ST_D = $(PROJ_OBJ_DIR)/test_c_1.debug.o
OBJ_TEST_CPP_1_ST_D = $(PROJ_OBJ_DIR)/test_cpp_1.debug.o
OBJ_TEST_CPP_2_ST_D = $(PROJ_OBJ_DIR)/test_cpp_2.debug.o
OBJ_TEST_C_1_ST_R = $(PROJ_OBJ_DIR)/test_c_1.o
OBJ_TEST_CPP_1_ST_R = $(PROJ_OBJ_DIR)/test_cpp_1.o
OBJ_TEST_CPP_2_ST_R = $(PROJ_OBJ_DIR)/test_cpp_2.o

OBJS_TESTS =\
 $(OBJ_TEST_C_1_ST_D)\
 $(OBJ_TEST_C_1_ST_R)\
 $(OBJ_TEST_CPP_1_ST_D)\
 $(OBJ_TEST_CPP_2_ST_D)\
 $(OBJ_TEST_CPP_1_ST_R)\
 $(OBJ_TEST_CPP_2_ST_R)\
 \

########################################
# OBJS

OBJS =\
 $(OBJS_LIBS)\
 \
 $(OBJS_EXAMPLES)\
 $(OBJS_SAMPLES)\
 $(OBJS_TESTS)\
 \

############################################################################
# targets

########################################
# libraries

# core

LIB_CORE_ST_D                 =   $(PROJ_LIB_DIR)/lib$(PROJ_TAG_VER).$(COMP_ARCH_OS_TAG).debug.a
LIB_CORE_UN_ST_D              =   $(PROJ_LIB_DIR)/lib$(PROJ_TAG).$(COMP_ARCH_OS_TAG).debug.a
LIB_CORE_ST_R                 =   $(PROJ_LIB_DIR)/lib$(PROJ_TAG_VER).$(COMP_ARCH_OS_TAG).a
LIB_CORE_UN_ST_R              =   $(PROJ_LIB_DIR)/lib$(PROJ_TAG).$(COMP_ARCH_OS_TAG).a

TARGETS_LIB_CORE=\
 $(LIB_CORE_ST_D)\
 $(LIB_CORE_UN_ST_D)\
 $(LIB_CORE_ST_R)\
 $(LIB_CORE_UN_ST_R)\
 \

# xCover

LIB_XCOVER_ST_D               =
LIB_XCOVER_ST_R               =
TARGETS_LIB_XCOVER                          =
# xTests - testing only

LIB_XTESTS_ST_D               =   $(PROJ_LIB_DIR)/lib$(XTESTS_TAG_VER).shw.$(COMP_ARCH_OS_TAG).debug.a
LIB_XTESTS_ST_R               =   $(PROJ_LIB_DIR)/lib$(XTESTS_TAG_VER).shw.$(COMP_ARCH_OS_TAG).a

TARGETS_LIB_XTESTS=\
 $(LIB_XTESTS_ST_D)\
 $(LIB_XTESTS_ST_R)\
 \

# *

TARGETS_LIB_ALL=\
 $(TARGETS_LIB_CORE)\
 \

TARGETS_LIBS=\
 $(TARGETS_LIB_CORE)\
 $(TARGETS_LIB_XCOVER)\
 $(TARGETS_LIB_XTESTS)\
 \

########################################
# examples

TARGET_EXAMPLE_C_1_ST_D   =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_c_1.$(COMP_ARCH_OS_TAG).debug
TARGET_EXAMPLE_C_2_ST_D   =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_c_2.$(COMP_ARCH_OS_TAG).debug
TARGET_EXAMPLE_CPP_1_ST_D =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_cpp_1.$(COMP_ARCH_OS_TAG).debug
TARGET_EXAMPLE_CPP_2_ST_D =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_cpp_2.$(COMP_ARCH_OS_TAG).debug
TARGET_EXAMPLE_C_1_ST_R   =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_c_1.$(COMP_ARCH_OS_TAG)
TARGET_EXAMPLE_C_2_ST_R   =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_c_2.$(COMP_ARCH_OS_TAG)
TARGET_EXAMPLE_CPP_1_ST_R =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_cpp_1.$(COMP_ARCH_OS_TAG)
TARGET_EXAMPLE_CPP_2_ST_R =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).example_cpp_2.$(COMP_ARCH_OS_TAG)

TARGETS_EXAMPLES =\
 $(TARGET_EXAMPLE_C_1_ST_D)\
 $(TARGET_EXAMPLE_C_2_ST_D)\
 $(TARGET_EXAMPLE_CPP_1_ST_D)\
 $(TARGET_EXAMPLE_CPP_2_ST_D)\
 $(TARGET_EXAMPLE_C_1_ST_R)\
 $(TARGET_EXAMPLE_C_2_ST_R)\
 $(TARGET_EXAMPLE_CPP_1_ST_R)\
 $(TARGET_EXAMPLE_CPP_2_ST_R)\
 \

########################################
# samples

TARGET_SAMPLE_C_1_ST_D    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_c_1.$(COMP_ARCH_OS_TAG).debug
TARGET_SAMPLE_C_2_ST_D    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_c_2.$(COMP_ARCH_OS_TAG).debug
TARGET_SAMPLE_CPP_1_ST_D  =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_cpp_1.$(COMP_ARCH_OS_TAG).debug
TARGET_SAMPLE_CPP_2_ST_D  =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_cpp_2.$(COMP_ARCH_OS_TAG).debug
TARGET_SAMPLE_C_1_ST_R    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_c_1.$(COMP_ARCH_OS_TAG)
TARGET_SAMPLE_C_2_ST_R    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_c_2.$(COMP_ARCH_OS_TAG)
TARGET_SAMPLE_CPP_1_ST_R  =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_cpp_1.$(COMP_ARCH_OS_TAG)
TARGET_SAMPLE_CPP_2_ST_R  =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).sample_cpp_2.$(COMP_ARCH_OS_TAG)

TARGETS_SAMPLES =\
 $(TARGET_SAMPLE_C_1_ST_D)\
 $(TARGET_SAMPLE_C_2_ST_D)\
 $(TARGET_SAMPLE_CPP_1_ST_D)\
 $(TARGET_SAMPLE_CPP_2_ST_D)\
 $(TARGET_SAMPLE_C_1_ST_R)\
 $(TARGET_SAMPLE_C_2_ST_R)\
 $(TARGET_SAMPLE_CPP_1_ST_R)\
 $(TARGET_SAMPLE_CPP_2_ST_R)\
 \

########################################
# tests

TARGET_TEST_C_1_ST_D      =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_c_1.$(COMP_ARCH_OS_TAG).debug
TARGET_TEST_CPP_1_ST_D    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_cpp_1.$(COMP_ARCH_OS_TAG).debug
TARGET_TEST_CPP_2_ST_D    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_cpp_2.$(COMP_ARCH_OS_TAG).debug
TARGET_TEST_C_1_ST_R      =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_c_1.$(COMP_ARCH_OS_TAG)
TARGET_TEST_CPP_1_ST_R    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_cpp_1.$(COMP_ARCH_OS_TAG)
TARGET_TEST_CPP_2_ST_R    =   $(PROJ_BIN_DIR)/$(PROJ_TAG_VER).test_cpp_2.$(COMP_ARCH_OS_TAG)

TARGETS_TESTS =\
 $(TARGET_TEST_C_1_ST_D)\
 $(TARGET_TEST_CPP_1_ST_D)\
 $(TARGET_TEST_CPP_2_ST_D)\
 $(TARGET_TEST_C_1_ST_R)\
 $(TARGET_TEST_CPP_1_ST_R)\
 $(TARGET_TEST_CPP_2_ST_R)\
 \

########################################
# TARGETS

TARGETS =\
 $(TARGETS_LIBS)\
 \
 $(TARGETS_TESTS)\
 $(TARGETS_EXAMPLES)\
 $(TARGETS_SAMPLES)\
 \

############################################################
# libs

LIBS_EXPLICIT_ST_D =\
  \
 \

LIBS_EXPLICIT_ST_R =\
  \
 \


LIBS_3PTY_ST_D =\
 \

LIBS_3PTY_ST_D_TEST =\
 $(LIBS_3PTY_ST_D)\
 -libopenrj.1.$(COMP_ARCH_OS_TAG).debug.a\
 \

LIBS_3PTY_ST_R =\
 \

LIBS_3PTY_ST_R_TEST =\
 $(LIBS_3PTY_ST_R)\
 -libopenrj.1.$(COMP_ARCH_OS_TAG).a\
 \


LIBS_EXAMPLES_ST_D=\
 $(LIB_CORE_ST_D)\
 \


LIBS_EXAMPLES_ST_R=\
 $(LIB_CORE_ST_R)\
 \


LIBS_SAMPLES_ST_D=\
 $(LIB_CORE_ST_D)\
 \


LIBS_SAMPLES_ST_R=\
 $(LIB_CORE_ST_R)\
 \


LIBS_TESTS_ST_D=\
 $(LIB_CORE_ST_D)\
 $(LIB_XTESTS_ST_D)\
 \


LIBS_TESTS_ST_R=\
 $(LIB_CORE_ST_R)\
 $(LIB_XTESTS_ST_R)\
 \



############################################################################
# External Targets (invokable by make)

# primary

_default:					build

usage:
	@echo "make [usage | compile | build | test | clean] - default is 'build'"

# infrastructure

check.lib.dir:				$(PROJ_MAKEFILE_NAME)
	@-mkdir -p $(PROJ_LIB_DIR)

check.bin.dir:				$(PROJ_MAKEFILE_NAME)
	@-mkdir -p $(PROJ_BIN_DIR)


# compile targets

compile.libs.core:			$(PROJ_MAKEFILE_NAME)	$(OBJS_CORE)

compile.libs.shwild:								compile.libs.core

compile.libs:										compile.libs.core

compile.libs.xtests:		$(PROJ_MAKEFILE_NAME)	$(OBJS_XTESTS)

compile.libs.3pty:									compile.libs.xtests

compile.libs.all:                                   compile.libs compile.libs.3pty

compile.examples:			$(PROJ_MAKEFILE_NAME)	$(OBJS_EXAMPLES)

compile.samples:			$(PROJ_MAKEFILE_NAME)	$(OBJS_SAMPLES)

compile.test.component:		$(PROJ_MAKEFILE_NAME)	$(OBJS_TEST_COMPONENT)

compile.test.scratch:		$(PROJ_MAKEFILE_NAME)	$(OBJS_TEST_SCRATCH)

compile.test.unit:			$(PROJ_MAKEFILE_NAME)	$(OBJS_TEST_UNIT)

compile.test:										compile.test.unit compile.test.component compile.test.scratch

compile:											compile.libs compile.libs.3pty compile.test compile.examples compile.samples

compile.all:										compile




# build targets

build.libs.core:			check.lib.dir			$(TARGETS_LIB_CORE)

build.libs.shwild:									build.libs.core

build.libs:											build.libs.core

build.libs.xtests:			check.lib.dir			$(TARGETS_LIB_XTESTS)

build.libs.3pty:									build.libs.xtests

build.libs.all:										build.libs build.libs.3pty

build.examples:				check.bin.dir			$(TARGETS_EXAMPLES)

build.samples:				check.bin.dir			$(TARGETS_SAMPLES)

build.test.component:		check.bin.dir			$(TARGETS_TEST_COMPONENT)

build.test.scratch:			check.bin.dir			$(TARGETS_TEST_SCRATCH)

build.test.unit:			check.bin.dir			$(TARGETS_TEST_UNIT)

build.test:											build.test.unit build.test.component build.test.scratch

build:												build.libs build.test build.examples build.samples

build.all:											build build.libs.all



# test targets

test.component_:
	@echo Running Test:Component programs ...

test.scratch_:
	@echo Running Test:Scratch programs ...

test.unit_:
	@echo Running Test:Unit programs ...

test.component:			$(PROJ_MAKEFILE_NAME)	build.test.component test.component_

test.scratch:			$(PROJ_MAKEFILE_NAME)	build.test.scratch test.scratch_

test.unit:				$(PROJ_MAKEFILE_NAME)	build.test.unit test.unit_

test:											test.unit test.component

test.all:										test test.scratch
test-all:				test.all


# clean targets

clean.libs.core:
	@echo Cleaning Core libraries ...
	@-$(RM) $(LIB_CORE_ST_D)
	@-$(RM) $(LIB_CORE_UN_ST_D)
	@-$(RM) $(LIB_CORE_ST_R)
	@-$(RM) $(LIB_CORE_UN_ST_R)
	@-$(RM) $(OBJS_CORE_ST_D)
	@-$(RM) $(OBJS_CORE_ST_R)

clean.libs.shwild:	clean.libs.core

clean.libs.xtests:
	@echo Cleaning xTests libraries ...
	@-$(RM) $(LIB_XTESTS_ST_D)
	@-$(RM) $(LIB_XTESTS_ST_R)
	@-$(RM) $(OBJS_XTESTS_ST_D)
	@-$(RM) $(OBJS_XTESTS_ST_R)

clean.test.component:
	@echo cleaning Test:Component programs ...

clean.test.scratch:
	@echo cleaning Test:Scratch programs ...

clean.test.unit:
	@echo cleaning Test:Unit programs ...

clean.libs: 									clean.libs.core

clean.libs.3pty:								clean.libs.xtests

clean.libs.all: 								clean.libs clean.libs.3pty

clean.examples:
	@echo cleaning example programs ...
	@-$(RM) $(TARGET_EXAMPLE_C_1_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_C_2_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_CPP_1_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_CPP_2_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_C_1_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_C_2_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_CPP_1_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_CPP_2_ST_R)
	@-$(RM) example_.*.o

clean.samples:
	@echo cleaning sample programs ...
	@-$(RM) $(TARGET_EXAMPLE_C_1_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_C_2_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_CPP_1_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_CPP_2_ST_D)
	@-$(RM) $(TARGET_EXAMPLE_C_1_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_C_2_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_CPP_1_ST_R)
	@-$(RM) $(TARGET_EXAMPLE_CPP_2_ST_R)
	@-$(RM) sample_.*.o

clean.test:										clean.test.component clean.test.scratch clean.test.unit

clean:					$(PROJ_MAKEFILE_NAME)	clean.libs.all clean.test clean.examples clean.samples

clean.all:										clean

############################################################################
# build targets

##################################################
# libraries

########################################
# xTests library - 'xtests.X.core.a'

$(LIB_XTESTS_ST_D): $(OBJS_XTESTS_ST_D) $(PROJ_MAKEFILE_NAME)
	@-mkdir -p $(PROJ_LIB_DIR)
	$(AR) $(AR_ARGS) -o $@ $(OBJS_XTESTS_ST_D)

$(OBJ_xt_core_ST_D): $(XTESTS_SRC_DIR)/xtests.core.cpp $(XTESTS_HEADERS) $(PROJ_MAKEFILE_NAME)
	$(CPPC) $(CPPC_ARGS_ST_D) $(CPPC_XTESTS_INCLUDES_ST_D) -o $@ $(XTESTS_SRC_DIR)/xtests.core.cpp

$(LIB_XTESTS_ST_R): $(OBJS_XTESTS_ST_R) $(PROJ_MAKEFILE_NAME)
	@-mkdir -p $(PROJ_LIB_DIR)
	$(AR) $(AR_ARGS) -o $@ $(OBJS_XTESTS_ST_R)

$(OBJ_xt_core_ST_R): $(XTESTS_SRC_DIR)/xtests.core.cpp $(XTESTS_HEADERS) $(PROJ_MAKEFILE_NAME)
	$(CPPC) $(CPPC_ARGS_ST_R) $(CPPC_XTESTS_INCLUDES_ST_R) -o $@ $(XTESTS_SRC_DIR)/xtests.core.cpp

########################################
# core


$(LIB_CORE_UN_ST_D): $(LIB_CORE_ST_D)
	@$(CP) $(LIB_CORE_ST_D) $@

$(LIB_CORE_ST_D): $(OBJS_CORE_ST_D) makefile
	$(AR) $(AR_ARGS) -o $@ $(OBJS_CORE_ST_D)

$(OBJ_CORE_matches__ST_D): $(PROJ_SRC_DIR)/matches.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_SRC_DIR)/matches.cpp
$(OBJ_CORE_pattern__ST_D): $(PROJ_SRC_DIR)/pattern.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_SRC_DIR)/pattern.cpp
$(OBJ_CORE_api__ST_D): $(PROJ_SRC_DIR)/api.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_SRC_DIR)/api.cpp


$(LIB_CORE_UN_ST_R): $(LIB_CORE_ST_R)
	@$(CP) $(LIB_CORE_ST_R) $@

$(LIB_CORE_ST_R): $(OBJS_CORE_ST_R) makefile
	$(AR) $(AR_ARGS) -o $@ $(OBJS_CORE_ST_R)

$(OBJ_CORE_matches__ST_R): $(PROJ_SRC_DIR)/matches.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_SRC_DIR)/matches.cpp
$(OBJ_CORE_pattern__ST_R): $(PROJ_SRC_DIR)/pattern.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_SRC_DIR)/pattern.cpp
$(OBJ_CORE_api__ST_R): $(PROJ_SRC_DIR)/api.cpp $(SRCS_HDR_CORE) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_SRC_DIR)/api.cpp


########################################
# examples

# C example client

$(TARGET_EXAMPLE_C_1_ST_D):	$(OBJ_EXAMPLE_C_1_ST_D) $(LIBS_EXAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_EXAMPLE_C_1_ST_D) $(LIBS_EXAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_EXAMPLE_C_1_ST_D):	$(PROJ_EXAMPLES_DIR)/c/example_c_1/example_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_D) -o $@ $(PROJ_EXAMPLES_DIR)/c/example_c_1/example_c_1.c

$(TARGET_EXAMPLE_C_2_ST_D):	$(OBJ_EXAMPLE_C_2_ST_D) $(LIBS_EXAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_EXAMPLE_C_2_ST_D) $(LIBS_EXAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_EXAMPLE_C_2_ST_D):	$(PROJ_EXAMPLES_DIR)/c/example_c_2/example_c_2.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_D) -o $@ $(PROJ_EXAMPLES_DIR)/c/example_c_2/example_c_2.c

$(TARGET_EXAMPLE_C_1_ST_R):	$(OBJ_EXAMPLE_C_1_ST_R) $(LIBS_EXAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_EXAMPLE_C_1_ST_R) $(LIBS_EXAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_EXAMPLE_C_1_ST_R):	$(PROJ_EXAMPLES_DIR)/c/example_c_1/example_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_R) -o $@ $(PROJ_EXAMPLES_DIR)/c/example_c_1/example_c_1.c

$(TARGET_EXAMPLE_C_2_ST_R):	$(OBJ_EXAMPLE_C_2_ST_R) $(LIBS_EXAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_EXAMPLE_C_2_ST_R) $(LIBS_EXAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_EXAMPLE_C_2_ST_R):	$(PROJ_EXAMPLES_DIR)/c/example_c_2/example_c_2.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_R) -o $@ $(PROJ_EXAMPLES_DIR)/c/example_c_2/example_c_2.c

# C++ example client

$(TARGET_EXAMPLE_CPP_1_ST_D):	$(OBJ_EXAMPLE_CPP_1_ST_D) $(LIBS_EXAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_EXAMPLE_CPP_1_ST_D) $(LIBS_EXAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_EXAMPLE_CPP_1_ST_D):	$(PROJ_EXAMPLES_DIR)/cpp/example_cpp_1/example_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_EXAMPLES_DIR)/cpp/example_cpp_1/example_cpp_1.cpp

$(TARGET_EXAMPLE_CPP_2_ST_D):	$(OBJ_EXAMPLE_CPP_2_ST_D) $(LIBS_EXAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_EXAMPLE_CPP_2_ST_D) $(LIBS_EXAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_EXAMPLE_CPP_2_ST_D):	$(PROJ_EXAMPLES_DIR)/cpp/example_cpp_2/example_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_EXAMPLES_DIR)/cpp/example_cpp_2/example_cpp_2.cpp

$(TARGET_EXAMPLE_CPP_1_ST_R):	$(OBJ_EXAMPLE_CPP_1_ST_R) $(LIBS_EXAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_EXAMPLE_CPP_1_ST_R) $(LIBS_EXAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_EXAMPLE_CPP_1_ST_R):	$(PROJ_EXAMPLES_DIR)/cpp/example_cpp_1/example_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_EXAMPLES_DIR)/cpp/example_cpp_1/example_cpp_1.cpp

$(TARGET_EXAMPLE_CPP_2_ST_R):	$(OBJ_EXAMPLE_CPP_2_ST_R) $(LIBS_EXAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_EXAMPLE_CPP_2_ST_R) $(LIBS_EXAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_EXAMPLE_CPP_2_ST_R):	$(PROJ_EXAMPLES_DIR)/cpp/example_cpp_2/example_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_EXAMPLES_DIR)/cpp/example_cpp_2/example_cpp_2.cpp

########################################
# samples

# C sample client

$(TARGET_SAMPLE_C_1_ST_D):	$(OBJ_SAMPLE_C_1_ST_D) $(LIBS_SAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_SAMPLE_C_1_ST_D) $(LIBS_SAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_SAMPLE_C_1_ST_D):	$(PROJ_SAMPLES_DIR)/c/sample_c_1/sample_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_D) -o $@ $(PROJ_SAMPLES_DIR)/c/sample_c_1/sample_c_1.c

$(TARGET_SAMPLE_C_2_ST_D):	$(OBJ_SAMPLE_C_2_ST_D) $(LIBS_SAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_SAMPLE_C_2_ST_D) $(LIBS_SAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_SAMPLE_C_2_ST_D):	$(PROJ_SAMPLES_DIR)/c/sample_c_2/sample_c_2.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_D) -o $@ $(PROJ_SAMPLES_DIR)/c/sample_c_2/sample_c_2.c

$(TARGET_SAMPLE_C_1_ST_R):	$(OBJ_SAMPLE_C_1_ST_R) $(LIBS_SAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_SAMPLE_C_1_ST_R) $(LIBS_SAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_SAMPLE_C_1_ST_R):	$(PROJ_SAMPLES_DIR)/c/sample_c_1/sample_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_R) -o $@ $(PROJ_SAMPLES_DIR)/c/sample_c_1/sample_c_1.c

$(TARGET_SAMPLE_C_2_ST_R):	$(OBJ_SAMPLE_C_2_ST_R) $(LIBS_SAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_SAMPLE_C_2_ST_R) $(LIBS_SAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_SAMPLE_C_2_ST_R):	$(PROJ_SAMPLES_DIR)/c/sample_c_2/sample_c_2.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_R) -o $@ $(PROJ_SAMPLES_DIR)/c/sample_c_2/sample_c_2.c

# C++ sample client

$(TARGET_SAMPLE_CPP_1_ST_D):	$(OBJ_SAMPLE_CPP_1_ST_D) $(LIBS_SAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_SAMPLE_CPP_1_ST_D) $(LIBS_SAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_SAMPLE_CPP_1_ST_D):	$(PROJ_SAMPLES_DIR)/cpp/sample_cpp_1/sample_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_SAMPLES_DIR)/cpp/sample_cpp_1/sample_cpp_1.cpp

$(TARGET_SAMPLE_CPP_2_ST_D):	$(OBJ_SAMPLE_CPP_2_ST_D) $(LIBS_SAMPLES_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D) -o $@ $(OBJ_SAMPLE_CPP_2_ST_D) $(LIBS_SAMPLES_ST_D) $(LIBS_3PTY_ST_D) $(LIBS_EXPLICIT_ST_D)

$(OBJ_SAMPLE_CPP_2_ST_D):	$(PROJ_SAMPLES_DIR)/cpp/sample_cpp_2/sample_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D) -o $@ $(PROJ_SAMPLES_DIR)/cpp/sample_cpp_2/sample_cpp_2.cpp

$(TARGET_SAMPLE_CPP_1_ST_R):	$(OBJ_SAMPLE_CPP_1_ST_R) $(LIBS_SAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_SAMPLE_CPP_1_ST_R) $(LIBS_SAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_SAMPLE_CPP_1_ST_R):	$(PROJ_SAMPLES_DIR)/cpp/sample_cpp_1/sample_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_SAMPLES_DIR)/cpp/sample_cpp_1/sample_cpp_1.cpp

$(TARGET_SAMPLE_CPP_2_ST_R):	$(OBJ_SAMPLE_CPP_2_ST_R) $(LIBS_SAMPLES_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R) -o $@ $(OBJ_SAMPLE_CPP_2_ST_R) $(LIBS_SAMPLES_ST_R) $(LIBS_3PTY_ST_R) $(LIBS_EXPLICIT_ST_R)

$(OBJ_SAMPLE_CPP_2_ST_R):	$(PROJ_SAMPLES_DIR)/cpp/sample_cpp_2/sample_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R) -o $@ $(PROJ_SAMPLES_DIR)/cpp/sample_cpp_2/sample_cpp_2.cpp


########################################
# test

# C test client

$(TARGET_TEST_C_1_ST_D):	$(OBJ_TEST_C_1_ST_D) $(LIBS_TEST_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D_TEST) -o $@ $(OBJ_TEST_C_1_ST_D) $(LIBS_TEST_ST_D) $(LIBS_3PTY_ST_D_TEST) $(LIBS_EXPLICIT_ST_D)

$(OBJ_TEST_C_1_ST_D):	$(PROJ_TESTS_DIR)/c/test_c_1/test_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_D_TEST) -o $@ $(PROJ_TESTS_DIR)/c/test_c_1/test_c_1.c

$(TARGET_TEST_C_1_ST_R):	$(OBJ_TEST_C_1_ST_R) $(LIBS_TEST_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R_TEST) -o $@ $(OBJ_TEST_C_1_ST_R) $(LIBS_TEST_ST_R) $(LIBS_3PTY_ST_R_TEST) $(LIBS_EXPLICIT_ST_R)

$(OBJ_TEST_C_1_ST_R):	$(PROJ_TESTS_DIR)/c/test_c_1/test_c_1.c $(SRCS_HDR_CORE) makefile
	$(CC) $(CC_ARGS_ST_R_TEST) -o $@ $(PROJ_TESTS_DIR)/c/test_c_1/test_c_1.c

# C++ test client

$(TARGET_TEST_CPP_1_ST_D):	$(OBJ_TEST_CPP_1_ST_D) $(LIBS_TEST_ST_D) $(LIB_XCOVER_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D_TEST) -o $@ $(OBJ_TEST_CPP_1_ST_D) $(LIBS_TEST_ST_D) $(LIBS_3PTY_ST_D_TEST) $(LIBS_EXPLICIT_ST_D)

$(OBJ_TEST_CPP_1_ST_D):	$(PROJ_TESTS_DIR)/cpp/test_cpp_1/test_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D_TEST) -o $@ $(PROJ_TESTS_DIR)/cpp/test_cpp_1/test_cpp_1.cpp

$(TARGET_TEST_CPP_2_ST_D):	$(OBJ_TEST_CPP_2_ST_D) $(LIBS_TEST_ST_D) $(LIB_XCOVER_ST_D) makefile
	$(LD) $(LD_ARGS_ST_D_TEST) -o $@ $(OBJ_TEST_CPP_2_ST_D) $(LIBS_TEST_ST_D) $(LIBS_3PTY_ST_D_TEST) $(LIBS_EXPLICIT_ST_D)

$(OBJ_TEST_CPP_2_ST_D):	$(PROJ_TESTS_DIR)/cpp/test_cpp_2/test_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_D_TEST) -o $@ $(PROJ_TESTS_DIR)/cpp/test_cpp_2/test_cpp_2.cpp

$(TARGET_TEST_CPP_1_ST_R):	$(OBJ_TEST_CPP_1_ST_R) $(LIBS_TEST_ST_R) $(LIB_XCOVER_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R_TEST) -o $@ $(OBJ_TEST_CPP_1_ST_R) $(LIBS_TEST_ST_R) $(LIBS_3PTY_ST_R_TEST) $(LIBS_EXPLICIT_ST_R)

$(OBJ_TEST_CPP_1_ST_R):	$(PROJ_TESTS_DIR)/cpp/test_cpp_1/test_cpp_1.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R_TEST) -o $@ $(PROJ_TESTS_DIR)/cpp/test_cpp_1/test_cpp_1.cpp

$(TARGET_TEST_CPP_2_ST_R):	$(OBJ_TEST_CPP_2_ST_R) $(LIBS_TEST_ST_R) $(LIB_XCOVER_ST_R) makefile
	$(LD) $(LD_ARGS_ST_R_TEST) -o $@ $(OBJ_TEST_CPP_2_ST_R) $(LIBS_TEST_ST_R) $(LIBS_3PTY_ST_R_TEST) $(LIBS_EXPLICIT_ST_R)

$(OBJ_TEST_CPP_2_ST_R):	$(PROJ_TESTS_DIR)/cpp/test_cpp_2/test_cpp_2.cpp $(SRCS_HDR_CORE) $(SRCS_HDR_MAPPING) makefile
	$(CPPC) $(CPPC_ARGS_ST_R_TEST) -o $@ $(PROJ_TESTS_DIR)/cpp/test_cpp_2/test_cpp_2.cpp

############################### end of file ################################