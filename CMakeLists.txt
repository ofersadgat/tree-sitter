cmake_minimum_required(VERSION 3.10)
project(tree_sitter C)

set(CMAKE_C_STANDARD 11)

include_directories(lib/include)
include_directories(lib/src)

add_library(tree_sitter
        lib/include/tree_sitter/api.h
        lib/include/tree_sitter/parser.h
        lib/src/unicode/ptypes.h
        lib/src/unicode/umachine.h
        lib/src/unicode/urename.h
        lib/src/unicode/utf.h
        lib/src/unicode/utf16.h
        lib/src/unicode/utf8.h
        lib/src/alloc.h
        lib/src/array.h
        lib/src/atomic.h
        lib/src/bits.h
        lib/src/clock.h
        lib/src/error_costs.h
        lib/src/get_changed_ranges.c
        lib/src/get_changed_ranges.h
        lib/src/language.c
        lib/src/language.h
        lib/src/length.h
        lib/src/lexer.c
        lib/src/lexer.h
        lib/src/node.c
        lib/src/parser.c
        lib/src/point.h
        lib/src/query.c
        lib/src/reduce_action.h
        lib/src/reusable_node.h
        lib/src/stack.c
        lib/src/stack.h
        lib/src/subtree.c
        lib/src/subtree.h
        lib/src/tree.c
        lib/src/tree.h
        lib/src/tree_cursor.c
        lib/src/tree_cursor.h
        lib/src/unicode.h)
