#Author: mbigras
A command line tool written in Ruby.

Installation

git clone https://github.com/NetMerc/somecli
cd somecli

Usage examples

./somecli
hello world!
"hello world!"
[]
hello world
hello world
ls: idontexist: No such file or directory

./somecli foo bar fail
hello world!
"hello world!"
["foo", "bar", "fail"]
Doing something with foo...
Doing something with bar...
Doing something with fail...
hello world
hello world
ls: idontexist: No such file or directory

./somecli foo bar fail 2>/dev/null
hello world!
"hello world!"
["foo", "bar", "fail"]
Doing something with foo...
Doing something with bar...
hello world
hello world

./somecli foo bar fail 1>/dev/null
Doing something with fail...
ls: idontexist: No such file or directory
