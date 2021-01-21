tree-sitter-json
===========================

[![Build Status](https://travis-ci.org/tree-sitter/tree-sitter-json.svg?branch=master)](https://travis-ci.org/tree-sitter/tree-sitter-json)

JSON grammar for [tree-sitter](https://github.com/tree-sitter/tree-sitter)


----

Carlos' test:

- separatedly, cloned (`--dept=1`) https://github.com/tree-sitter/tree-sitter
  and built `libtree-sitter.a` there
- copied the test program from https://tree-sitter.github.io/tree-sitter/using-parsers#an-example-program
- built and ran the test program:

        $ clang                                    \
          -I ~/github/tree-sitter/lib/include      \
          ~/github/tree-sitter/libtree-sitter.a    \
          src/parser.c                             \
          test-json-parser.c                       \
          -o test-json-parser

        $ ./test-json-parser
        Syntax tree: (document (array (number) (null)))

