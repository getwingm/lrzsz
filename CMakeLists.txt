cmake_minimum_required(VERSION 3.12)
project(lrzsz_0_12_20 C)

set(CMAKE_C_STANDARD 11)
ADD_DEFINITIONS(-DNFGVMIN -DLOCALEDIR=\"~\")

include_directories(.)
include_directories(lib)
include_directories(src)

add_executable(lsz
        lib/error.c
        lib/error.h
        lib/getopt.h
        lib/long-options.c
        lib/long-options.h
        lib/xstrtol.c
        lib/xstrtol.h
        lib/xstrtoul.c
        lib/xstrtoul.h
        src/canit.c
        src/crctab.c
        src/lsyslog.c
        src/lsz.c
        src/protname.c
        src/rbsb.c
        src/tcp.c
        src/timing.c
        src/timing.h
        src/zglobal.h
        src/zm.c
        src/zmodem.h
        src/zperr.c
        src/zreadline.c
        config.h)

add_executable(lrz
        lib/error.c
        lib/error.h
        lib/getopt.h
        lib/long-options.c
        lib/long-options.h
        lib/xstrtol.c
        lib/xstrtol.h
        lib/xstrtoul.c
        lib/xstrtoul.h

        src/canit.c
        src/crctab.c
        src/lrz.c
        src/lsyslog.c
        src/protname.c
        src/rbsb.c
        src/tcp.c
        src/timing.c
        src/timing.h
        src/zglobal.h
        src/zm.c
        src/zmodem.h
        src/zperr.c
        src/zreadline.c
        config.h)