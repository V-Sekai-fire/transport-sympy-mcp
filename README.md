# transport-sympy-mcp

An MCP server, written in Elixir, that does symbolic mathematics through an embedded SymPy.

## What it is for

It lets an agent solve, simplify, differentiate, integrate, expand, factor and numerically
evaluate symbolic expressions over the Model Context Protocol. The server lists its tools to a
client when asked, so the tool list lives in the code rather than here. `DEVELOPING.md` covers
the tests and the release build.

## Build and run

```sh
mix deps.get
mix mcp.server
```

The build installs the interpreter and SymPy it embeds. The `Dockerfile` builds the same server
as an image.

## Licence

MIT; see `LICENSE.md`.
