
## Note:

Due to a change in the API of asciinema, this tool no longer works correctly.

See also: https://asciinema.org/docs/embedding

## asciinema2gif

Generate animated GIFs from [asciinema terminal recordings].

![Demo](http://tav.espians.com/asciinema/demo.gif)

### Motivation

The [`asciinema`] tool is a wonderful way to record and share terminal sessions.  
Unfortunately, it's not [currently possible] to embed the output in places like  
README files on GitHub repos. This tool provides a solution for that.

### Usage

Simply pass in the corresponding API url for the recording, e.g.

```bash
$ ./asciinema2gif https://asciinema.org/api/asciicasts/8332
```

An `asciicast.gif` file will then be generated for you to embed and share.

The API url supports a few customisable parameters you might want to use:

* `?size=`: `small`, `medium`, `big`
* `?theme=`: `tango`, `solarized-dark`, `solarized-light`

### Requirements

#### OS X

```bash
brew install imagemagick gifsicle npm
npm install phantomjs2
```

#### Ubuntu

```bash
apt-get install imagemagick gifsicle npm
npm install phantomjs2
```

### License

Public domain.

—  
Enjoy, tav <<tav@espians.com>>


[`asciinema`]: https://asciinema.org/
[asciinema terminal recordings]: https://asciinema.org/
[currently possible]: https://github.com/asciinema/asciinema.org/issues/152
