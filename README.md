# graffiti

Fortune-style CLI for [graffiti.moe](https://graffiti.moe) — fetch a random spray, fetch one by id, or spraypaint a new one from your terminal.

## Install

```bash
brew tap ttscoff/thelab
brew install graffiti
```

Or copy `graffiti` onto your `PATH` and `chmod +x` it (requires `curl`).

## Usage

```bash
graffiti                              # random message (color when stdout is a TTY)
graffiti --color=never
graffiti --color=always
graffiti get 42                       # one spray by numeric id
graffiti spraypaint                   # open /add in your default browser
graffiti spraypaint --color cyan --bold 'hello wall'
echo $'ascii\nart' | graffiti spraypaint --color magenta
```

### Environment

| Variable | Meaning |
|----------|---------|
| `GRAFFITI_URL` | API base (default `https://graffiti.moe`) |
| `GRAFFITI_COLOR` | `always`, `never`, or `auto` (default) |
| `NO_COLOR` | Non-empty disables color in `auto` mode |

## License

MIT
