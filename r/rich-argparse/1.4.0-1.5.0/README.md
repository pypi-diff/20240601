# Comparing `tmp/rich_argparse-1.4.0.tar.gz` & `tmp/rich_argparse-1.5.0.tar.gz`

## Comparing `rich_argparse-1.4.0.tar` & `rich_argparse-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/__init__.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/__main__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/_common.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/_lazy_rich.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/optparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/rich_argparse/py.typed
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/LICENSE
--rw-r--r--   0        0        0    12877 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/README.md
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 rich_argparse-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    22327 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/__init__.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/__main__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/_common.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/_lazy_rich.py
+-rw-r--r--   0        0        0    13197 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/optparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/rich_argparse/py.typed
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/LICENSE
+-rw-r--r--   0        0        0    13019 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/README.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 rich_argparse-1.5.0/PKG-INFO
```

### Comparing `rich_argparse-1.4.0/rich_argparse/__init__.py` & `rich_argparse-1.5.0/rich_argparse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     usage_markup: ClassVar[bool] = False
     """If True, render the usage string passed to ``ArgumentParser(usage=...)`` as markup.
 
     Defaults to ``False`` meaning the text of the usage will be printed verbatim.
 
     Note that the auto-generated usage string is always colored.
     """
+    help_markup: ClassVar[bool] = True
+    """If True (default), render the help message of arguments as console markup."""
+    text_markup: ClassVar[bool] = True
+    """If True (default), render the descriptions and epilog as console markup."""
 
     _root_section: _Section
     _current_section: _Section
 
     def __init__(
         self,
         prog: str,
@@ -110,15 +114,15 @@
     def console(self, console: r.Console) -> None:
         self._console = console
 
     class _Section(argparse.HelpFormatter._Section):
         def __init__(
             self, formatter: RichHelpFormatter, parent: Self | None, heading: str | None = None
         ) -> None:
-            if heading is not None:
+            if heading is not argparse.SUPPRESS and heading is not None:
                 heading = f"{type(formatter).group_name_formatter(heading)}:"
             super().__init__(formatter, parent, heading)
             self.formatter: RichHelpFormatter
             self.rich_items: list[r.RenderableType] = []
             self.rich_actions: list[tuple[r.Text, r.Text | None]] = []
             if parent is not None:
                 parent.rich_items.append(self)
@@ -161,15 +165,15 @@
                     line.rstrip()
                     yield from console.render(indent + line, options)
             yield ""
 
         def __rich_console__(self, console: r.Console, options: r.ConsoleOptions) -> r.RenderResult:
             if not self.rich_items and not self.rich_actions:
                 return  # empty section
-            if self.heading:
+            if self.heading is not argparse.SUPPRESS and self.heading is not None:
                 yield r.Text(self.heading, style="argparse.groups")
             yield from self._render_items(console, options)
             yield from self._render_actions(console, options)
 
     def __rich_console__(self, console: r.Console, options: r.ConsoleOptions) -> r.RenderResult:
         with console.use_theme(r.Theme(self.styles)):
             root = console.render(self._root_section, options.update_width(self._width))
@@ -268,15 +272,15 @@
             sub = usage[start:end] % params
             prog_start = len(formatted_usage)
             prog_end = prog_start + len(sub)
             formatted_usage += sub
             last = end
             yield r.Span(prog_start, prog_end, "argparse.prog")
 
-    def _rich_usage_spans(  # noqa: C901
+    def _rich_usage_spans(
         self, text: str, start: int, actions: Iterable[Action]
     ) -> Iterator[r.Span]:
         options: list[Action] = []
         positionals: list[Action] = []
         for action in actions:
             if action.help is not argparse.SUPPRESS:
                 options.append(action) if action.option_strings else positionals.append(action)
@@ -372,23 +376,31 @@
             parts.append(help_string[last:start])
             sub = r.escape(help_string[start:end] % params)
             if m.group("mapping") == "default":
                 sub = f"[argparse.default]{sub}[/argparse.default]"
             parts.append(sub)
             last = end
         parts.append(help_string[last:])
-        rich_help = r.Text.from_markup("".join(parts), style="argparse.help")
+        rich_help = (
+            r.Text.from_markup("".join(parts), style="argparse.help")
+            if self.help_markup
+            else r.Text("".join(parts), style="argparse.help")
+        )
         for highlight in self.highlights:
             rich_help.highlight_regex(highlight, style_prefix="argparse.")
         return rich_help
 
     def _rich_format_text(self, text: str) -> r.Text:
         if "%(prog)" in text:
             text = text % {"prog": r.escape(self._prog)}
-        rich_text = r.Text.from_markup(text, style="argparse.text")
+        rich_text = (
+            r.Text.from_markup(text, style="argparse.text")
+            if self.text_markup
+            else r.Text(text, style="argparse.text")
+        )
         for highlight in self.highlights:
             rich_text.highlight_regex(highlight, style_prefix="argparse.")
         text_width = max(self._width - self._current_indent * 2, 11)
         indent = r.Text(" " * self._current_indent)
         return self._rich_fill_text(rich_text, text_width, indent)
 
     def _rich_format_action(self, action: Action) -> Iterator[tuple[r.Text, r.Text | None]]:
```

### Comparing `rich_argparse-1.4.0/rich_argparse/__main__.py` & `rich_argparse-1.5.0/rich_argparse/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,35 @@
 import sys
 
 from rich.terminal_theme import DIMMED_MONOKAI
 
 from rich_argparse import HelpPreviewAction, RichHelpFormatter
 
 if __name__ == "__main__":
-    RichHelpFormatter.highlights.append(r"(?:^|\s)-{1,2}[\w]+[\w-]* (?P<metavar>METAVAR)\b")
     parser = argparse.ArgumentParser(
         prog="python -m rich_argparse",
         formatter_class=RichHelpFormatter,
         description=(
             "This is a [link https://pypi.org/project/rich]rich[/]-based formatter for "
             "[link https://docs.python.org/3/library/argparse.html#formatter-class]"
             "argparse's help output[/].\n\n"
             "It enables you to use the powers of rich like markup and highlights in your CLI help. "
-            "Read below for a glance at available features."
         ),
         epilog=":link: Read more at https://github.com/hamdanal/rich-argparse#usage.",
     )
     parser.add_argument(
         "formatter-class",
         help=(
-            "All you need to make your argparse.ArgumentParser output colorful text like this is to "
-            "pass it `formatter_class=RichHelpFormatter` or any of the available variants."
+            "Simply pass `formatter_class=RichHelpFormatter` to the argument parser to get a "
+            "colorful help like this."
         ),
     )
     parser.add_argument(
         "styles",
-        help=(
-            "All the styles used by this formatter are defined in `RichHelpFormatter.styles`. "
-            "Modify this dictionary with any rich style to change the look of your CLI's help text."
-        ),
+        help="Customize your CLI's help with the `RichHelpFormatter.styles` dictionary.",
     )
     parser.add_argument(
         "--highlights",
         metavar="REGEXES",
         help=(
             "Highlighting the help text is managed by the list of regular expressions "
             "`RichHelpFormatter.highlights`. Set to empty list to turn off highlighting.\n"
@@ -49,24 +44,18 @@
         default=RichHelpFormatter.styles["argparse.syntax"],
         help=(
             "Text inside backticks is highlighted using the `argparse.syntax` style "
             "(default: %(default)r)"
         ),
     )
     parser.add_argument(
-        "-s",
-        "--long-option",
+        "-o",
+        "--option",
         metavar="METAVAR",
-        help=(
-            "Words that look like --command-line-options are highlighted using the `argparse.args` "
-            "style. In addition, this example, adds a highlighter regex for the word 'METAVAR' "
-            "following an option for the sake of demonstrating custom highlights.\n"
-            "Notice also that if an option takes a value and has short and long options, it is "
-            "printed as -s, --long-option METAVAR instead of -s METAVAR, --long-option METAVAR."
-        ),
+        help="Text that looks like an --option is highlighted using the `argparse.args` style.",
     )
     group = parser.add_argument_group(
         "more arguments",
         description=(
             "This is a custom group. Group names are [italic]*Title Cased*[/] by default. Use the "
             "`RichHelpFormatter.group_name_formatter` function to change their format."
         ),
```

### Comparing `rich_argparse-1.4.0/rich_argparse/_common.py` & `rich_argparse-1.5.0/rich_argparse/_common.py`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.4.0/rich_argparse/_lazy_rich.py` & `rich_argparse-1.5.0/rich_argparse/_lazy_rich.py`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.4.0/rich_argparse/optparse.py` & `rich_argparse-1.5.0/rich_argparse/optparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,32 +46,28 @@
     it highlights ``--words-with-dashes`` with the `optparse.args` style and
     ``` `text in backquotes` ``` with the `optparse.syntax` style.
 
     To disable highlighting, clear this list (``RichHelpFormatter.highlights.clear()``).
     """
 
     def __init__(
-        self,
-        indent_increment: int,
-        max_help_position: int,
-        width: int | None,
-        short_first: int,
+        self, indent_increment: int, max_help_position: int, width: int | None, short_first: int
     ) -> None:
         super().__init__(indent_increment, max_help_position, width, short_first)
         self._console: r.Console | None = None
         self.rich_option_strings: dict[optparse.Option, r.Text] = {}
 
     @property
-    def console(self) -> r.Console:  # deprecate?
+    def console(self) -> r.Console:
         if self._console is None:
             self._console = r.Console(theme=r.Theme(self.styles))
         return self._console
 
     @console.setter
-    def console(self, console: r.Console) -> None:  # is this needed?
+    def console(self, console: r.Console) -> None:
         self._console = console
 
     def _stringify(self, text: r.RenderableType) -> str:
         # Render a rich object to a string
         with self.console.capture() as capture:
             self.console.print(text, highlight=False, soft_wrap=True, end="")
         help = capture.get()
@@ -89,38 +85,38 @@
         text_width = max(self.width - 2 * self.current_indent, 11)
         indent = r.Text(" " * self.current_indent)
         rich_text = r.Text.from_markup(text, style="optparse.text")
         for highlight in self.highlights:
             rich_text.highlight_regex(highlight, style_prefix="optparse.")
         return _rich_fill(self.console, rich_text, text_width, indent)
 
-    def rich_format_description(self, description: str) -> r.Text:
+    def rich_format_description(self, description: str | None) -> r.Text:
         if not description:
             return r.Text()
         return self._rich_format_text(description) + r.Text("\n")
 
-    def rich_format_epilog(self, epilog: str) -> r.Text:
+    def rich_format_epilog(self, epilog: str | None) -> r.Text:
         if not epilog:
             return r.Text()
         return r.Text("\n") + self._rich_format_text(epilog) + r.Text("\n")
 
     def format_usage(self, usage: str) -> str:
         if usage is GENERATE_USAGE:
             rich_usage = self._generate_usage()
         else:
             rich_usage = self.rich_format_usage(usage)
         return self._stringify(rich_usage)
 
     def format_heading(self, heading: str) -> str:
         return self._stringify(self.rich_format_heading(heading))
 
-    def format_description(self, description: str) -> str:
+    def format_description(self, description: str | None) -> str:
         return self._stringify(self.rich_format_description(description))
 
-    def format_epilog(self, epilog: str) -> str:
+    def format_epilog(self, epilog: str | None) -> str:
         return self._stringify(self.rich_format_epilog(epilog))
 
     def rich_expand_default(self, option: optparse.Option) -> r.Text:
         assert option.help is not None
         if self.parser is None or not self.default_tag:
             help = option.help
         else:
```

### Comparing `rich_argparse-1.4.0/LICENSE` & `rich_argparse-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_argparse-1.4.0/README.md` & `rich_argparse-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # rich-argparse
 
 ![python -m rich_argparse](
-https://github.com/hamdanal/rich-argparse/assets/93259987/ae4a4968-1008-4fcd-8131-7a90292a7f3f)
+https://github.com/hamdanal/rich-argparse/assets/93259987/8b90e62e-d6e4-4df0-9ced-0d6aac65337e)
 
 [![tests](https://github.com/hamdanal/rich-argparse/actions/workflows/tests.yml/badge.svg)
 ](https://github.com/hamdanal/rich-argparse/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hamdanal/rich-argparse/main.svg)
 ](https://results.pre-commit.ci/latest/github/hamdanal/rich-argparse/main)
 [![Downloads](https://img.shields.io/pypi/dm/rich-argparse)](https://pypistats.org/packages/rich-argparse)
 [![Python Version](https://img.shields.io/pypi/pyversions/rich-argparse)
@@ -22,14 +22,15 @@
 * [Installation](#installation)
 * [Usage](#usage)
 * [Output styles](#output-styles)
   * [Colors](#customize-the-colors)
   * [Group names](#customize-the-group-name-format)
   * [Highlighting patterns](#special-text-highlighting)
   * ["usage"](#colors-in-the-usage)
+  * [Console markup](#disable-console-markup)
   * [--version](#colors-in---version)
   * [Rich renderables](#rich-descriptions-and-epilog)
 * [Subparsers](#working-with-subparsers)
 * [Documenting your CLI](#generate-help-preview)
 * [Third party formatters](#working-with-third-party-formatters) (ft. django)
 * [Optparse](#optparse-support) (experimental)
 * [Legacy Windows](#legacy-windows-support)
@@ -49,15 +50,15 @@
 import argparse
 from rich_argparse import RichHelpFormatter
 
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
 
-*rich-argparse* defines equivalents to argparse's [built-in formatters](
+*rich-argparse* defines equivalents to all argparse's [built-in formatters](
 https://docs.python.org/3/library/argparse.html#formatter-class):
 
 | `rich_argparse` formatter | equivalent in `argparse` |
 |---------------------------|--------------------------|
 | `RichHelpFormatter` | `HelpFormatter` |
 | `RawDescriptionRichHelpFormatter` | `RawDescriptionHelpFormatter` |
 | `RawTextRichHelpFormatter` | `RawTextHelpFormatter` |
@@ -67,16 +68,17 @@
 ## Output styles
 
 The default styles used by *rich-argparse* are carefully chosen to work in different light and dark
 themes.
 
 ### Customize the colors
 
-You can customize the colors in the output by modifying the `styles` dictionary on the formatter
-class. *rich-argparse* defines the following styles:
+You can customize the colors of the output by modifying the `styles` dictionary on the formatter
+class. You can use any rich style as defined [here](https://rich.readthedocs.io/en/latest/style.html).
+*rich-argparse* defines and uses the following styles:
 
 ```python
 {
     'argparse.args': 'cyan',  # for positional-arguments and --options (e.g "--help")
     'argparse.groups': 'dark_orange',  # for group names (e.g. "positional arguments")
     'argparse.help': 'default',  # for argument's help text (e.g. "show this help message and exit")
     'argparse.metavar': 'dark_cyan',  # for metavariables (e.g. "FILE" in "--file FILE")
@@ -124,20 +126,31 @@
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
 
 ### Colors in the `usage`
 
 The usage **generated by the formatter** is colored using the `argparse.args` and `argparse.metavar`
-styles. If you use a custom `usage` message in the parser, it will treated as "plain text" and will
-**not** be colored by default. You can enable colors in user defined usage message through
+styles. If you use a custom `usage` message in the parser, it will be treated as "plain text" and
+will **not** be colored by default. You can enable colors in user defined usage message through
 [console markup](https://rich.readthedocs.io/en/stable/markup.html) by setting
 `RichHelpFormatter.usage_markup = True`. If you enable this option, make sure to [escape](
 https://rich.readthedocs.io/en/stable/markup.html#escaping) any square brackets in the usage text.
 
+### Disable console markup
+
+The text of the descriptions and epilog is interpreted as
+[console markup](https://rich.readthedocs.io/en/stable/markup.html) by default. If this conflicts
+with your usage of square brackets, make sure to [escape](
+https://rich.readthedocs.io/en/stable/markup.html#escaping) the square brackets or to disable
+markup globally with `RichHelpFormatter.text_markup = False`.
+
+Similarly the help text of arguments is interpreted as markup by default. It can be disabled using
+`RichHelpFormatter.help_markup = False`.
+
 ### Colors in `--version`
 
 If you use the `"version"` action from argparse, you can use console markup in the `version` string:
 
 ```python
 parser.add_argument(
     "--version", action="version", version="[argparse.prog]%(prog)s[/] version [i]1.0.0[/]"
@@ -147,15 +160,15 @@
 Note that the `argparse.text` style is applied to the `version` string similar to the description
 and epilog.
 
 ### Rich descriptions and epilog
 
 You can use any rich renderable in the descriptions and epilog. This includes all built-in rich
 renderables like `Table` and `Markdown` and any custom renderables defined using the
-[Console Protcol](https://rich.readthedocs.io/en/stable/protocol.html#console-protocol).
+[Console Protocol](https://rich.readthedocs.io/en/stable/protocol.html#console-protocol).
 
 ```python
 import argparse
 from rich.markdown import Markdown
 from rich_argparse import RichHelpFormatter
 
 description = """
@@ -178,17 +191,14 @@
 ```
 Certain features are **disabled** for arbitrary renderables other than strings, including:
 
 * Syntax highlighting with `RichHelpFormatter.highlights`
 * Styling with the `"argparse.text"` style defined in `RichHelpFormatter.styles`
 * Replacement of `%(prog)s` with the program name
 
-Arbitrary renderables are displayed "as is" except for long runs of empty lines that get truncated
-to two empty lines following the behavior of argparse.
-
 ## Working with subparsers
 
 Subparsers do not inherit the formatter class from the parent parser by default. You have to pass
 the formatter class explicitly:
 
 ```python
 subparsers = parser.add_subparsers(...)
@@ -227,19 +237,18 @@
 python my_cli.py --generate-help-preview my-help.svg  # generates my-help.svg
 # or
 COLUMNS=120 python my_cli.py --generate-help-preview  # force the width of the output to 120 columns
 ```
 
 ## Working with third party formatters
 
-*rich-argparse* can be used with other formatters that **do not rely on the private internals**
-of `argparse.HelpFormatter`. A popular example is [django](https://pypi.org/project/django) that
-defines a custom help formatter that is used with its built in commands as well as with extension
-libraries and user defined commands. To use *rich-argparse* in your django project, change your
-`manage.py` file as follows:
+*rich-argparse* can be used with other custom formatters through multiple inheritance. For example,
+[django](https://pypi.org/project/django) defines a custom help formatter for its built in commands
+as well as extension libraries and user defined commands. To use *rich-argparse* in your django
+project, change your `manage.py` file as follows:
 
 ```diff
 diff --git a/my_project/manage.py b/my_project/manage.py
 index 7fb6855..5e5d48a 100755
 --- a/my_project/manage.py
 +++ b/my_project/manage.py
 @@ -1,22 +1,38 @@
@@ -279,16 +288,15 @@
      execute_from_command_line(sys.argv)
 
 
  if __name__ == '__main__':
      main()
 ```
 
-Now try out some command like `python manage.py runserver --help` and notice how the special
-ordering of the arguments applied by django is respected by the new help formatter.
+Now the output of all `python manage.py <COMMAND> --help` will be colored.
 
 ## Optparse support
 
 *rich-argparse* now ships with experimental support for [optparse](
 https://docs.python.org/3/library/optparse.html).
 
 Import optparse help formatters from `rich_argparse.optparse`:
@@ -297,15 +305,15 @@
 import optparse
 from rich_argparse.optparse import IndentedRichHelpFormatter  # or TitledRichHelpFormatter
 
 parser = optparse.OptionParser(formatter=IndentedRichHelpFormatter())
 ...
 ```
 
-You can also generated a more helpful usage message by passing `usage=GENERATE_USAGE` to the
+You can also generate a more helpful usage message by passing `usage=GENERATE_USAGE` to the
 parser. This is similar to the default behavior of `argparse`.
 
 ```python
 from rich_argparse.optparse import GENERATE_USAGE, IndentedRichHelpFormatter
 
 parser = optparse.OptionParser(usage=GENERATE_USAGE, formatter=IndentedRichHelpFormatter())
 ```
@@ -318,24 +326,21 @@
 RichHelpFormatter.styles["optparse.metavar"] = "bold magenta"
 ```
 
 Syntax highlighting works the same as with `argparse`.
 
 Colors in the `usage` are only supported when using `GENERATE_USAGE`.
 
-Customizing the group name format is not supported. optparse uses Title Case format by default.
-
 ## Legacy Windows support
 
-If your application still runs on legacy Windows versions (older than Windows 10), you'll need to
-enable ANSI escape sequences by calling `colorama.init()` otherwise colors will be disabled:
+When used on legacy Windows versions like *Windows 7*, colors are disabled unless
+[colorama](https://pypi.org/project/colorama/) is used:
 
 ```python
 import argparse
 import colorama
 from rich_argparse import RichHelpFormatter
 
 colorama.init()
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
-This is **not** required on Windows 10 and newer or on other operating systems.
```

### Comparing `rich_argparse-1.4.0/pyproject.toml` & `rich_argparse-1.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rich-argparse"
-version = "1.4.0"
+version = "1.5.0"
 description = "Rich help formatters for argparse and optparse"
 authors = [
   {name="Ali Hamdan", email="ali.hamdan.dev@gmail.com"},
 ]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Topic :: Software Development :: User Interfaces",
 ]
 keywords = ["argparse", "rich", "help-formatter", "optparse"]
 dependencies = [
   "rich >= 11.0.0",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/hamdanal/rich-argparse"
 Documentation = "https://github.com/hamdanal/rich-argparse#rich-argparse"
 Issue-Tracker = "https://github.com/hamdanal/rich-argparse/issues"
 Changelog = "https://github.com/hamdanal/rich-argparse/blob/main/CHANGELOG.md"
 
 [tool.hatch]
 build.packages = ["rich_argparse"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37,py38,py39,py310,py311,py312
+envlist = py{38,39,310,311,312,313}
 skip_missing_interpreters = true
 
 [testenv]
 deps = -rtests/requirements.txt
+set_env =
+  COLUMNS=80
 commands =
   coverage run -m pytest {posargs}
   coverage report
   coverage html
 """
 
-[tool.black]
-line_length = 100
-
 [tool.ruff]
 line-length = 100
-select = ["E", "F", "C", "B", "UP", "RUF100", "TID"]
+
+[tool.ruff.lint]
+extend-select = ["C4", "B", "UP", "RUF100", "TID", "T10"]
+extend-ignore = ["E501"]
 unfixable = ["B"]
-ignore = ["E501"]
 isort.required-imports = ["from __future__ import annotations"]
 isort.extra-standard-library = ["typing_extensions"]
 flake8-tidy-imports.ban-relative-imports = "all"
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 check_untyped_defs = false
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
```

### Comparing `rich_argparse-1.4.0/PKG-INFO` & `rich_argparse-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rich-argparse
-Version: 1.4.0
+Version: 1.5.0
 Summary: Rich help formatters for argparse and optparse
 Project-URL: Homepage, https://github.com/hamdanal/rich-argparse
 Project-URL: Documentation, https://github.com/hamdanal/rich-argparse#rich-argparse
 Project-URL: Issue-Tracker, https://github.com/hamdanal/rich-argparse/issues
 Project-URL: Changelog, https://github.com/hamdanal/rich-argparse/blob/main/CHANGELOG.md
 Author-email: Ali Hamdan <ali.hamdan.dev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: argparse,help-formatter,optparse,rich
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: rich>=11.0.0
 Description-Content-Type: text/markdown
 
 # rich-argparse
 
 ![python -m rich_argparse](
-https://github.com/hamdanal/rich-argparse/assets/93259987/ae4a4968-1008-4fcd-8131-7a90292a7f3f)
+https://github.com/hamdanal/rich-argparse/assets/93259987/8b90e62e-d6e4-4df0-9ced-0d6aac65337e)
 
 [![tests](https://github.com/hamdanal/rich-argparse/actions/workflows/tests.yml/badge.svg)
 ](https://github.com/hamdanal/rich-argparse/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hamdanal/rich-argparse/main.svg)
 ](https://results.pre-commit.ci/latest/github/hamdanal/rich-argparse/main)
 [![Downloads](https://img.shields.io/pypi/dm/rich-argparse)](https://pypistats.org/packages/rich-argparse)
 [![Python Version](https://img.shields.io/pypi/pyversions/rich-argparse)
@@ -50,14 +50,15 @@
 * [Installation](#installation)
 * [Usage](#usage)
 * [Output styles](#output-styles)
   * [Colors](#customize-the-colors)
   * [Group names](#customize-the-group-name-format)
   * [Highlighting patterns](#special-text-highlighting)
   * ["usage"](#colors-in-the-usage)
+  * [Console markup](#disable-console-markup)
   * [--version](#colors-in---version)
   * [Rich renderables](#rich-descriptions-and-epilog)
 * [Subparsers](#working-with-subparsers)
 * [Documenting your CLI](#generate-help-preview)
 * [Third party formatters](#working-with-third-party-formatters) (ft. django)
 * [Optparse](#optparse-support) (experimental)
 * [Legacy Windows](#legacy-windows-support)
@@ -77,15 +78,15 @@
 import argparse
 from rich_argparse import RichHelpFormatter
 
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
 
-*rich-argparse* defines equivalents to argparse's [built-in formatters](
+*rich-argparse* defines equivalents to all argparse's [built-in formatters](
 https://docs.python.org/3/library/argparse.html#formatter-class):
 
 | `rich_argparse` formatter | equivalent in `argparse` |
 |---------------------------|--------------------------|
 | `RichHelpFormatter` | `HelpFormatter` |
 | `RawDescriptionRichHelpFormatter` | `RawDescriptionHelpFormatter` |
 | `RawTextRichHelpFormatter` | `RawTextHelpFormatter` |
@@ -95,16 +96,17 @@
 ## Output styles
 
 The default styles used by *rich-argparse* are carefully chosen to work in different light and dark
 themes.
 
 ### Customize the colors
 
-You can customize the colors in the output by modifying the `styles` dictionary on the formatter
-class. *rich-argparse* defines the following styles:
+You can customize the colors of the output by modifying the `styles` dictionary on the formatter
+class. You can use any rich style as defined [here](https://rich.readthedocs.io/en/latest/style.html).
+*rich-argparse* defines and uses the following styles:
 
 ```python
 {
     'argparse.args': 'cyan',  # for positional-arguments and --options (e.g "--help")
     'argparse.groups': 'dark_orange',  # for group names (e.g. "positional arguments")
     'argparse.help': 'default',  # for argument's help text (e.g. "show this help message and exit")
     'argparse.metavar': 'dark_cyan',  # for metavariables (e.g. "FILE" in "--file FILE")
@@ -152,20 +154,31 @@
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
 
 ### Colors in the `usage`
 
 The usage **generated by the formatter** is colored using the `argparse.args` and `argparse.metavar`
-styles. If you use a custom `usage` message in the parser, it will treated as "plain text" and will
-**not** be colored by default. You can enable colors in user defined usage message through
+styles. If you use a custom `usage` message in the parser, it will be treated as "plain text" and
+will **not** be colored by default. You can enable colors in user defined usage message through
 [console markup](https://rich.readthedocs.io/en/stable/markup.html) by setting
 `RichHelpFormatter.usage_markup = True`. If you enable this option, make sure to [escape](
 https://rich.readthedocs.io/en/stable/markup.html#escaping) any square brackets in the usage text.
 
+### Disable console markup
+
+The text of the descriptions and epilog is interpreted as
+[console markup](https://rich.readthedocs.io/en/stable/markup.html) by default. If this conflicts
+with your usage of square brackets, make sure to [escape](
+https://rich.readthedocs.io/en/stable/markup.html#escaping) the square brackets or to disable
+markup globally with `RichHelpFormatter.text_markup = False`.
+
+Similarly the help text of arguments is interpreted as markup by default. It can be disabled using
+`RichHelpFormatter.help_markup = False`.
+
 ### Colors in `--version`
 
 If you use the `"version"` action from argparse, you can use console markup in the `version` string:
 
 ```python
 parser.add_argument(
     "--version", action="version", version="[argparse.prog]%(prog)s[/] version [i]1.0.0[/]"
@@ -175,15 +188,15 @@
 Note that the `argparse.text` style is applied to the `version` string similar to the description
 and epilog.
 
 ### Rich descriptions and epilog
 
 You can use any rich renderable in the descriptions and epilog. This includes all built-in rich
 renderables like `Table` and `Markdown` and any custom renderables defined using the
-[Console Protcol](https://rich.readthedocs.io/en/stable/protocol.html#console-protocol).
+[Console Protocol](https://rich.readthedocs.io/en/stable/protocol.html#console-protocol).
 
 ```python
 import argparse
 from rich.markdown import Markdown
 from rich_argparse import RichHelpFormatter
 
 description = """
@@ -206,17 +219,14 @@
 ```
 Certain features are **disabled** for arbitrary renderables other than strings, including:
 
 * Syntax highlighting with `RichHelpFormatter.highlights`
 * Styling with the `"argparse.text"` style defined in `RichHelpFormatter.styles`
 * Replacement of `%(prog)s` with the program name
 
-Arbitrary renderables are displayed "as is" except for long runs of empty lines that get truncated
-to two empty lines following the behavior of argparse.
-
 ## Working with subparsers
 
 Subparsers do not inherit the formatter class from the parent parser by default. You have to pass
 the formatter class explicitly:
 
 ```python
 subparsers = parser.add_subparsers(...)
@@ -255,19 +265,18 @@
 python my_cli.py --generate-help-preview my-help.svg  # generates my-help.svg
 # or
 COLUMNS=120 python my_cli.py --generate-help-preview  # force the width of the output to 120 columns
 ```
 
 ## Working with third party formatters
 
-*rich-argparse* can be used with other formatters that **do not rely on the private internals**
-of `argparse.HelpFormatter`. A popular example is [django](https://pypi.org/project/django) that
-defines a custom help formatter that is used with its built in commands as well as with extension
-libraries and user defined commands. To use *rich-argparse* in your django project, change your
-`manage.py` file as follows:
+*rich-argparse* can be used with other custom formatters through multiple inheritance. For example,
+[django](https://pypi.org/project/django) defines a custom help formatter for its built in commands
+as well as extension libraries and user defined commands. To use *rich-argparse* in your django
+project, change your `manage.py` file as follows:
 
 ```diff
 diff --git a/my_project/manage.py b/my_project/manage.py
 index 7fb6855..5e5d48a 100755
 --- a/my_project/manage.py
 +++ b/my_project/manage.py
 @@ -1,22 +1,38 @@
@@ -307,16 +316,15 @@
      execute_from_command_line(sys.argv)
 
 
  if __name__ == '__main__':
      main()
 ```
 
-Now try out some command like `python manage.py runserver --help` and notice how the special
-ordering of the arguments applied by django is respected by the new help formatter.
+Now the output of all `python manage.py <COMMAND> --help` will be colored.
 
 ## Optparse support
 
 *rich-argparse* now ships with experimental support for [optparse](
 https://docs.python.org/3/library/optparse.html).
 
 Import optparse help formatters from `rich_argparse.optparse`:
@@ -325,15 +333,15 @@
 import optparse
 from rich_argparse.optparse import IndentedRichHelpFormatter  # or TitledRichHelpFormatter
 
 parser = optparse.OptionParser(formatter=IndentedRichHelpFormatter())
 ...
 ```
 
-You can also generated a more helpful usage message by passing `usage=GENERATE_USAGE` to the
+You can also generate a more helpful usage message by passing `usage=GENERATE_USAGE` to the
 parser. This is similar to the default behavior of `argparse`.
 
 ```python
 from rich_argparse.optparse import GENERATE_USAGE, IndentedRichHelpFormatter
 
 parser = optparse.OptionParser(usage=GENERATE_USAGE, formatter=IndentedRichHelpFormatter())
 ```
@@ -346,24 +354,21 @@
 RichHelpFormatter.styles["optparse.metavar"] = "bold magenta"
 ```
 
 Syntax highlighting works the same as with `argparse`.
 
 Colors in the `usage` are only supported when using `GENERATE_USAGE`.
 
-Customizing the group name format is not supported. optparse uses Title Case format by default.
-
 ## Legacy Windows support
 
-If your application still runs on legacy Windows versions (older than Windows 10), you'll need to
-enable ANSI escape sequences by calling `colorama.init()` otherwise colors will be disabled:
+When used on legacy Windows versions like *Windows 7*, colors are disabled unless
+[colorama](https://pypi.org/project/colorama/) is used:
 
 ```python
 import argparse
 import colorama
 from rich_argparse import RichHelpFormatter
 
 colorama.init()
 parser = argparse.ArgumentParser(..., formatter_class=RichHelpFormatter)
 ...
 ```
-This is **not** required on Windows 10 and newer or on other operating systems.
```

