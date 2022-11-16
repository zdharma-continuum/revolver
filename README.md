# Revolver

A progress spinner for ZSH scripts

[![asciicast](https://asciinema.org/a/ex8z3z6d5m7uv4buww0o2qeq2.png)](https://asciinema.org/a/ex8z3z6d5m7uv4buww0o2qeq2)

## Installation

### [Zinit](https://github.com/zdharma-continuum/revolver)

```sh
zinit for as'command' pick'revolver' @zdharma-continuum/revolver
```

### [Zulu](https://github.com/zulu-zsh/zulu)

```sh
zulu install revolver
```

### zplug

```sh
zplug "zdharma-continuum/revolver", \
  as:command, \
  use:revolver
```

### Manual

```sh
git clone https://github.com/zdharma-continuum/revolver revolver
chmod u+x revolver/revolver
mv revolver/revolver /usr/local/bin
```

## Usage

```sh
revolver start 'Your awesome message'

# Do something here

revolver update 'A different message'

# Do something else here

revolver stop
```

## Hiding cursor

 You can hide the cursor during revolver operation, to do this pass option `-i`
 or `--hide-cursor` for the opening `revolver` invocation:

```sh
revolver -i start "Your awesome message"
```

Or

```sh
revolver --hide-cursor start "Your awesome message"
```

## Styles

Revolver comes with a `revolver demo` command which demonstrates each of the
included spinner styles. Once you've found one you like, select it using the
`--style` option.

```sh
revolver --style 'bouncingBall' start 'The spinner message'
```

## License

Copyright (c) 2016 James Dinsdale <hi@molovo.co> (molovo.co)

Revolver is licensed under The MIT License (MIT)

## Team

* [James Dinsdale](http://molovo.co)
