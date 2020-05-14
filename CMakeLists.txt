cmake_minimum_required (VERSION 2.6)
project (libfixmath)

add_library(fixmath STATIC libfixmath/fix16.c libfixmath/fix16_exp.c libfixmath/fix16_sqrt.c libfixmath/fix16_trig.c libfixmath/fract32.c libfixmath/uint32.c)
target_include_directories(fixmath PUBLIC libfixmath)
#target_compile_definitions(fixed_point PUBLIC FXP_C99_INLINE)