# parser
An alternate parser for R (Vaporware for now)

Currently a place for me to collect information / ideas

# Need for an alternate parser

- Current bison/YACC paser is hard (for me) to follow https://github.com/wch/r-source/blob/trunk/src/main/gram.y.
- parsed expressions do not retain detailed per token location information
- comment source locations are not retained.
- `getParseData()`
  - data is limited and somewhat buggy / inconsistant.
  - No great way to map parsed expressions to getParseData output.
- Would prove useful to
  - Existing packages
    - https://github.com/jimhester/lintr
    - https://github.com/jimhester/covr
    - https://github.com/yihui/formatR
  - Future packages similar to
    - https://golang.org/cmd/gofmt/
    - https://babeljs.io/
    - https://github.com/estree/estree
    - https://github.com/marijnh/tern
