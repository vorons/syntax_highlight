Syntax_Highlight
================

Plugin syntax highlighter for Nibbleblog

Plugin for highlights syntax in code examples on blog. Automatically finds blocks of code, detects a language and highlights it.
The plugin knows 54 languages:
Common: 
Bash 
C# 
C++ 
CSS 
Diff 
HTML, XML 
HTTP 
Ini 
JSON 
Java 
JavaScript 
PHP 
Perl 
Python 
Ruby 
SQL
Other: 
1C 
AVR Assembler 
ActionScript 
Apache 
AppleScript 
Axapta 
Brainfuck 
CMake 
Clojure 
CoffeeScript 
D 
DOS .bat 
Delphi 
Django 
Erlang 
Erlang REPL 
GLSL 
Go 
Haskell 
Lisp 
Lua 
MEL 
Markdown 
Matlab 
Nginx 
Objective C 
Parser3 
Python profile 
R 
RenderMan RIB 
RenderMan RSL 
Rust 
Scala 
Smalltalk 
TeX 
VBScript 
VHDL 
Vala
Installing:
Upload plugin and enable it in "Dashboard -> Manage plugins".
Open file "/themes/your_theme/templates/default.bit", find:

<!-- Plugin::Analytics -->
    <?php
        if( isset($plugins_by_name['analytics']) )
        {
            echo $plugins_by_name['analytics']->get_html();
        }
    ?>

and add after:

<!-- Plugin::Highlight -->
    <?php
        if( isset($plugins_by_name['syntax_highlight']) )
        {
            echo $plugins_by_name['syntax_highlight']->get_html();
        }
    ?>

That's it! Enjoy!
