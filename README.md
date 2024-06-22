# ruIndy-pub

ruIndy project - generate on-line ind files from idx files

project website: [https://latex.js29a.info.pl/](https://latex.js29a.info.pl/)

## Usage

* add `\usepackage{imakeidx}` to document preamble,
* add some `\index{xxx}` into document body,
* add `\printindex` command,
* run LaTeX,
* upload `xxx.idx` file into the page,
* grab `xxx.ind` from this page into your LaTeX - overwrite the file,
* run LaTeX again,

## `\index` syntax

* `\index{keyword}` - the simpliest index entry,
* `\index{keyword!subkeyword}` - nested keyword, max 3 levels,
* `\index{keyword|(} and \index{keyword|)}` - open and close multipage index entry,
* `\index{keyword|minor}` - mark entry as minor - italic page number,
* `\index{keyword|major}` - mark entry as major - underlined page number,
* `\index{keyword|important}` - mark entry as important - bold page number,
* `\index{keyword|see{xxx}}` - emit see,
* `\index{keyword|seealso{xxx}}` - emit see also,
* `\index{keyword|@sort_as}` - change item order - quite useful when you neeed e.g. bold keyword entry like here: `\index{\textbf{keyword}|@keyword}`,

Note: you can mix options.

Note: expect `\indexentry{...}{...}` entries in the `xxx.idx` file.

Examples of supported page ranges in this demo:
* `iv` - roman numbers
* `13` - arabic numbers,
* `B-13` - addendums,

## issues

Please report issues at [https://github.com/js29a/ruIndy-pub/issues](https://github.com/js29a/ruIndy-pub/issues)

## rendered example

![the sample](https://github.com/js29a/ruIndy-pub/assets/78456/c045f97e-6527-4cae-aae3-a750f99b0613)

