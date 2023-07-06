# Comparing `tmp/click_extra-4.4.0.tar.gz` & `tmp/click_extra-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.4.0.tar", max compression
+gzip compressed data, was "click_extra-4.5.0.tar", max compression
```

## Comparing `click_extra-4.4.0.tar` & `click_extra-4.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     5977 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/__init__.py
--rw-r--r--   0        0        0    27916 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/colorize.py
--rw-r--r--   0        0        0    15032 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/commands.py
--rw-r--r--   0        0        0    15847 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/config.py
--rw-r--r--   0        0        0     4014 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6262 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11581 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/logging.py
--rw-r--r--   0        0        0    23480 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/parameters.py
--rw-r--r--   0        0        0    17118 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/py.typed
--rw-r--r--   0        0        0     7685 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5733 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2542 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11217 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    17920 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    12975 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    16381 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7290 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    14348 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10873 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8406 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14343 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     4615 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2398 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/timer.py
--rw-r--r--   0        0        0     7165 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/version.py
--rw-r--r--   0        0        0     7439 2023-06-16 05:42:43.358332 click_extra-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     6631 2023-06-16 05:42:43.358332 click_extra-4.4.0/readme.md
--rw-r--r--   0        0        0     9675 1970-01-01 00:00:00.000000 click_extra-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6017 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    27922 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    15310 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/commands.py
+-rw-r--r--   0        0        0    15776 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/config.py
+-rw-r--r--   0        0        0     4014 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6211 2023-07-06 06:50:43.859600 click_extra-4.5.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11874 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/logging.py
+-rw-r--r--   0        0        0    23477 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7685 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     6038 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11164 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    17922 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    12920 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    16315 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7290 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    14371 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8406 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14478 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     6311 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2613 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/timer.py
+-rw-r--r--   0        0        0    10988 2023-07-06 06:50:43.863600 click_extra-4.5.0/click_extra/version.py
+-rw-r--r--   0        0        0     7490 2023-07-06 06:50:43.871600 click_extra-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-07-06 06:50:43.871600 click_extra-4.5.0/readme.md
+-rw-r--r--   0        0        0     9675 1970-01-01 00:00:00.000000 click_extra-4.5.0/PKG-INFO
```

### Comparing `click_extra-4.4.0/click_extra/__init__.py` & `click_extra-4.5.0/click_extra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.4.0"
+__version__ = "4.5.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -89,14 +89,15 @@
     VerbosityOption,
     extra_basic_config,
 )
 from .parameters import (  # noqa: E402
     ExtraOption,
     ParamStructure,
     ShowParamsOption,
+    search_params,
 )
 from .tabulate import TableFormatOption  # noqa: E402
 from .telemetry import TelemetryOption  # noqa: E402
 from .testing import ExtraCliRunner  # noqa: E402
 from .timer import TimerOption  # noqa: E402
 from .version import VersionOption  # noqa: E402
 
@@ -189,14 +190,15 @@
     "pass_obj",
     "password_option",
     "Path",
     "path",
     "pause",
     "progressbar",
     "prompt",
+    "search_params",
     "secho",
     "Section",
     "SectionMixin",
     "show_params_option",
     "ShowParamsOption",
     "STRING",
     "Style",
```

### Comparing `click_extra-4.4.0/click_extra/colorize.py` & `click_extra-4.5.0/click_extra/colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     """Non-canonical Click Extra properties.
 
     .. note::
         Subheading is used for sub-sections, like `in the help of mail-deduplicate
         <https://github.com/kdeldycke/mail-deduplicate/blob/0764287/mail_deduplicate/deduplicate.py#L445>`_.
 
     .. todo::
-        Maybe this shouln't be in Click Extra because it is a legacy inheritance from
+        Maybe this shouldn't be in Click Extra because it is a legacy inheritance from
         one of my other project.
     """
 
     def with_(
         self,
         ### Cloup properties.
         invoked_command: IStyle | None = None,
@@ -166,15 +166,15 @@
 
 # Populate our global theme with all default styles.
 default_theme = HelpExtraTheme(
     ### Cloup styles.
     invoked_command=Style(fg=Color.bright_white),
     heading=Style(fg=Color.bright_blue, bold=True, underline=True),
     constraint=Style(fg=Color.magenta),
-    # Neutralize Cloup's col1, as it interfers with our finer option styling
+    # Neutralize Cloup's col1, as it interferes with our finer option styling
     # which takes care of separators.
     col1=identity,
     # Style aliases like options and subcommands.
     alias=Style(fg=Color.cyan),
     # Style aliases punctuation like options, but dimmed.
     alias_secondary=Style(fg=Color.cyan, dim=True),
     ### Log styles.
@@ -458,16 +458,16 @@
             formatter.metavars,
             formatter.envvars,
             formatter.defaults,
         ) = self.collect_keywords(ctx)
         return super().format_help(ctx, formatter)
 
 
-def escape_for_help_sceen(text: str) -> str:
-    """Escape a text to be used in a regural expression to match help screen.
+def escape_for_help_screen(text: str) -> str:
+    """Escape a text to be used in a regular expression to match help screen.
 
     Like ``re.escape``, but allows any number of optional blank characters (line
     returns, spaces, tabs) after a dash, to accounts for text wrapping rules and
     columnar layout.
     """
     return re.escape(text).replace("-", "-\\s*")
 
@@ -547,26 +547,26 @@
         return style(str_to_style)
 
     def colorize(self, match: re.Match) -> str:
         """Colorize all groups with IDs in the provided matching result.
 
         All groups without IDs are left as-is.
 
-        All groups are proccessed in the order they appear in the ``match`` object.
+        All groups are processed in the order they appear in the ``match`` object.
         Then all groups are concatenated to form the final string that is returned.
 
         .. caution::
             Implementation is a bit funky here because there is no way to iterate over
             both unnamed and named groups, in the order they appear in the regex, while
             keeping track of the group ID.
 
             So we have to iterate over the list of matching strings and pick up the
             corresponding group ID along the way, from the ``match.groupdict()``
-            dictionnary. This also means we assume that the ``match.groupdict()`` is
-            returning an ordered dictionnary. Which is supposed to be true as of Python
+            dictionary. This also means we assume that the ``match.groupdict()`` is
+            returning an ordered dictionary. Which is supposed to be true as of Python
             3.7.
         """
         # Get a snapshot of all named groups.
         named_matches = list(match.groupdict().items())
 
         txt = ""
         # Iterate over all groups, named or not.
@@ -619,28 +619,28 @@
             (?P<deprecated>{re.escape("(Deprecated)")})  # The flag string.
             """,
             self.colorize,
             help_text,
             flags=re.VERBOSE,
         )
 
-        # Highligh subcommands.
+        # Highlight subcommands.
         for subcommand in self.subcommands:
             help_text = re.sub(
                 rf"""
-                (\ \ )                        # 2 spaces (i.e. section indention).
+                (\ \ )                        # 2 spaces (i.e. section indentation).
                 (?P<subcommand>{re.escape(subcommand)})
                 (\s)                          # Any blank char.
                 """,
                 self.colorize,
                 help_text,
                 flags=re.VERBOSE,
             )
 
-        # Highligh environment variables and defaults in trailing square brackets.
+        # Highlight environment variables and defaults in trailing square brackets.
         help_text = re.sub(
             r"""
             (\ \ )                  # 2 spaces (column spacing or description spacing).
             (?P<bracket_1>\[)                  # Square brackets opening.
 
             (?:                         # Non-capturing group.
                 (?P<envvar_label>
@@ -679,15 +679,15 @@
                 (\s)                                        # Any blank char.
                 """,
                 self.colorize,
                 help_text,
                 flags=re.VERBOSE,
             )
 
-        # Highligh sections.
+        # Highlight sections.
         # XXX Duplicates Cloup's job, with the only subtlety of not highlighting the
         # trailing semicolon.
         #
         # help_text = re.sub(
         #     r"""
         #     ^                       # Beginning of a line preceded by a newline.
         #     (?P<heading>\S[\S+ ]+)  # The section title.
@@ -702,15 +702,15 @@
         for matching_keywords, style_group_id in (
             (sorted(self.long_options, reverse=True), "long_option"),
             (sorted(self.short_options), "short_option"),
             (sorted(self.choices, reverse=True), "choice"),
             (sorted(self.metavars, reverse=True), "metavar"),
         ):
             for keyword in matching_keywords:
-                keyword = escape_for_help_sceen(keyword)
+                keyword = escape_for_help_screen(keyword)
                 help_text = re.sub(
                     rf"""
                     ([               # A keyword is preceded with either:
                         \s           # - a blank char
                         \[           # - an opening square bracket (as in choice string)
                         \|           # - a pipe (again like in choice strings)
                         \(           # - an opening parenthesis
```

### Comparing `click_extra-4.4.0/click_extra/commands.py` & `click_extra-4.5.0/click_extra/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 )
 from .timer import TimerOption
 from .version import VersionOption
 
 
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
-    ``meta`` property at instanciation.
+    ``meta`` property at instantiation.
     """
 
     _extra_meta: dict[str, Any] = {}
 
     def __init__(self, *args, meta: dict[str, Any] = {}, **kwargs) -> None:
         """Like parent's context but with an extra ``meta`` keyword-argument."""
         self._extra_meta = meta
@@ -68,16 +68,16 @@
 
     .. caution::
         The order of options has been carefully crafted to handle subtle edge-cases and
         avoid leaky states in unittests.
 
         You can still override this hard-coded order for easthetic reasons and it
         should be fine. Your end-users are unlikely to be affected by these sneaky
-        bugs, as the CLI context is going to be naturraly resetted after each
-        invokation (which is not the case in unitests).
+        bugs, as the CLI context is going to be naturraly reset after each
+        invocation (which is not the case in unitests).
 
     #. ``--time`` / ``--no-time``
         .. hint::
             ``--time`` is placed at the top so all other options can be timed.
     #. ``-C``, ``--config CONFIG_PATH``
         .. attention::
             ``--config`` is at the top so it can have a direct influence on the default
@@ -102,15 +102,15 @@
     """
     return [
         TimerOption(),
         ColorOption(),
         ConfigOption(),
         ShowParamsOption(),
         VerbosityOption(),
-        VersionOption(print_env_info=True),
+        VersionOption(),
         HelpOption(),
     ]
 
 
 class ExtraCommand(ExtraHelpColorsMixin, Command):
     """Like ``cloup.command``, with sane defaults and extra help screen colorization."""
 
@@ -155,15 +155,15 @@
 
         - ``show_default = True``
 
           `Show all default values
           <https://click.palletsprojects.com/en/8.1.x/api/#click.Context.show_default>`_
           in help screen.
 
-        Additionnaly, these `Cloup context settings
+        Additionally, these `Cloup context settings
         <https://cloup.readthedocs.io/en/stable/pages/formatting.html#formatting-settings>`_
         are set:
 
         - ``align_option_groups = False`` (*Cloup feature*)
 
           `Aligns option groups in help screen
           <https://cloup.readthedocs.io/en/stable/pages/option-groups.html#aligned-vs-non-aligned-groups>`_.
@@ -215,15 +215,18 @@
                     ...
                 }
             )
         """
         super().__init__(*args, **kwargs)
 
         # List of additional global settings for options.
-        extra_option_settings = ["show_choices", "show_envvar"]
+        extra_option_settings = [
+            "show_choices",
+            "show_envvar",
+        ]
 
         default_ctx_settings: dict[str, Any] = {
             # Click settings:
             # "default_map": {"verbosity": "DEBUG"},
             "help_option_names": ("--help", "-h"),
             "show_default": True,
             # Cloup settings:
@@ -269,19 +272,19 @@
 
         # Forces re-identification of grouped and non-grouped options as we re-ordered
         # them above and added our own extra options since initialization.
         _grouped_params = self._group_params(self.params)  # type: ignore[attr-defined]
         self.arguments, self.option_groups, self.ungrouped_options = _grouped_params
 
     def main(self, *args, **kwargs):
-        """Pre-invokation step that is instantiating the context, then call ``invoke()``
+        """Pre-invocation step that is instantiating the context, then call ``invoke()``
         within it.
 
         During context instantiation, each option's callbacks are called. Beware that
-        these might break the execution flow (like ``--version``).
+        these might break the execution flow (like ``--help`` or ``--version``).
         """
         return super().main(*args, **kwargs)
 
     def make_context(
         self,
         info_name: str | None,
         args: list[str],
@@ -297,39 +300,42 @@
         ``ShowParamsOption.print_params()`` to print the table of parameters fed to the
         CLI.
 
         .. seealso::
             This workaround is being discussed upstream in `click#1279
             <https://github.com/pallets/click/issues/1279#issuecomment-1493348208>`_.
         """
-        # ``args`` needs to be copied: its items are consummed by the parsing process.
+        # ``args`` needs to be copied: its items are consumed by the parsing process.
         extra.update({"meta": {"click_extra.raw_args": args.copy()}})
-        ctx = super().make_context(info_name, args, parent, **extra)
-        return ctx
+        return super().make_context(info_name, args, parent, **extra)
 
     def invoke(self, ctx):
         """Main execution of the command, just after the context has been instantiated
         in ``main()``.
 
-        If an instance of ``VersionOption`` has been setup on the command, adds to the
-        normal execution flow the output of ``--version`` in ``DEBUG`` logs. This
-        facilitates troubleshooting of user's issues.
+        If an instance of ``VersionOption`` is found attached to the command, print its
+        output in ``DEBUG`` logs. This facilitates troubleshooting of user's issues.
         """
         logger = logging.getLogger("click_extra")
         if logger.getEffectiveLevel() == logging.DEBUG:
-            # Look for our custom version parameter.
-            version_param = search_params(ctx.command.params, VersionOption)
-            if version_param:
-                version_message = version_param.callback(
-                    ctx,
-                    version_param,
-                    True,
-                    capture_output=True,
-                )
-                for line in version_message.splitlines():
+            # Look for a ``--version`` parameter.
+            version_opt = search_params(ctx.command.params, VersionOption)
+            if version_opt:
+                # Environment info is already present in the version string: use it
+                # as-is.
+                if "%(env_info)s" in version_opt.message:
+                    msg = version_opt.render_message()
+                # Augments the version string with the environment info.
+                else:
+                    msg = version_opt.render_message(
+                        version_opt.colored_template(
+                            version_opt.message + "\n%(env_info)s",
+                        ),
+                    )
+                for line in msg.splitlines():
                     # TODO: pretty print JSON output (easier to read in bug reports)?
                     logger.debug(line)
 
         return super().invoke(ctx)
 
 
 class ExtraGroup(ExtraCommand, Group):
```

### Comparing `click_extra-4.4.0/click_extra/config.py` & `click_extra-4.5.0/click_extra/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,21 +348,19 @@
             if isinstance(v, dict) and isinstance(a.get(k), dict):
                 a[k] = self.recursive_update(a[k], v)
             # Ignore elements unregistered in the template structure.
             elif k in a:
                 a[k] = b[k]
             elif self.strict:
                 msg = f"Parameter {k!r} is not allowed in configuration file."
-                raise ValueError(
-                    msg,
-                )
+                raise ValueError(msg)
         return a
 
     def merge_conf(self, user_conf):
-        """Try-out configuration formats againts file's content and returns a ``dict``.
+        """Try-out configuration formats against file's content and returns a ``dict``.
 
         The returned ``dict`` will only contain options and parameters defined on the
         CLI. All others will be filtered out.
         """
         # Merge configuration file's content into the template structure, but
         # ignore all unrecognized options.
         valid_conf = self.recursive_update(self.params_template, user_conf)
@@ -373,16 +371,15 @@
             """Skip None values and empty dicts."""
             if value is None:
                 return False
             if isinstance(value, dict) and not len(value):
                 return False
             return True
 
-        clean_conf = remap(valid_conf, visit=visit)
-        return clean_conf
+        return remap(valid_conf, visit=visit)
 
     def load_conf(self, ctx, param, path_pattern):
         """Fetch parameters values from configuration file and merge them with the
         defaults.
 
         User configuration is
         `merged to the context default_map as Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
```

### Comparing `click_extra-4.4.0/click_extra/decorators.py` & `click_extra-4.5.0/click_extra/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     Used to create our own collection of decorators for our custom options, based on
     Cloup's.
     """
 
     @allow_missing_parenthesis
     def decorator(*args, **kwargs):
-        """Returns a new decorator instanciated with custom defaults.
+        """Returns a new decorator instantiated with custom defaults.
 
         These defaults values are merged with the user's own arguments.
 
         A special case is made for the ``params`` argument, to allow it to be callable.
         This limits the issue of the mutable options being shared between commands.
 
         This decorator can be used with or without arguments.
```

### Comparing `click_extra-4.4.0/click_extra/docs_update.py` & `click_extra-4.5.0/click_extra/docs_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,36 +64,35 @@
 
 def generate_lexer_table() -> str:
     """Generate a Markdown table mapping original Pygments' lexers to their new ANSI
     variants implemented by Click Extra."""
     table = []
     for orig_lexer, ansi_lexer in sorted(
         lexer_map.items(),
-        key=lambda i: i[0].__qualname__,  # type: ignore[no-any-return]
+        key=lambda i: i[0].__qualname__,
     ):
         table.append(
             [
                 f"[`{orig_lexer.__qualname__}`](https://pygments.org/docs/lexers/#"
                 f"{orig_lexer.__module__}.{orig_lexer.__qualname__})",
                 f"{', '.join(f'`{a}`' for a in sorted(orig_lexer.aliases))}",
                 f"{', '.join(f'`{a}`' for a in sorted(ansi_lexer.aliases))}",
             ],
         )
-    output = tabulate.tabulate(
+    return tabulate.tabulate(
         table,
         headers=[
             "Original Lexer",
             "Original IDs",
             "ANSI variants",
         ],
         tablefmt="github",
         colalign=["left", "left", "left"],
         disable_numparse=True,
     )
-    return output
 
 
 def generate_platforms_graph(
     graph_id: str,
     description: str,
     groups: frozenset[Group],
 ) -> str:
```

### Comparing `click_extra-4.4.0/click_extra/logging.py` & `click_extra-4.5.0/click_extra/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,17 @@
 
 
 class VerbosityOption(ExtraOption):
     """A pre-configured ``--verbosity``/``-v`` option.
 
     Sets the level of the provided logger.
 
+    The selected verbosity level name is made available in the context in
+    ``ctx.meta["click_extra.verbosity"]``.
+
     .. important::
 
         The internal ``click_extra`` logger level will be aligned to the value set via
         this option.
     """
 
     logger_name: str
@@ -247,17 +250,22 @@
                 f"Reset {logger} to {DEFAULT_LEVEL_NAME}.",
             )
             logger.setLevel(DEFAULT_LEVEL)
 
     def set_levels(self, ctx, param, value):
         """Set level of all loggers configured on the option.
 
+        Save the verbosity level name in the context.
+
         Also prints the chosen value as a debug message via the internal
         ``click_extra`` logger.
         """
+        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
+        ctx._meta["click_extra.verbosity"] = value
+
         for logger in self.all_loggers:
             logger.setLevel(LOG_LEVELS[value])
             logging.getLogger("click_extra").debug(f"Set {logger} to {value}.")
 
         ctx.call_on_close(self.reset_loggers)
 
     def __init__(
```

### Comparing `click_extra-4.4.0/click_extra/parameters.py` & `click_extra-4.5.0/click_extra/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,30 +56,30 @@
 
 def auto_envvar(
     param: click.Parameter,
     ctx: click.Context | dict[str, Any],
 ) -> str | None:
     """Compute the auto-generated environment variable of an option or argument.
 
-    Returns the auto envvar as it is exacly computed within Click's internals, i.e.
+    Returns the auto envvar as it is exactly computed within Click's internals, i.e.
     ``click.core.Parameter.resolve_envvar_value()`` and
     ``click.core.Option.resolve_envvar_value()``.
     """
     # Skip parameters that have their auto-envvar explicitly disabled.
     if not getattr(param, "allow_from_autoenv", None):
         return None
 
     if isinstance(ctx, click.Context):
         prefix = ctx.auto_envvar_prefix
     else:
         prefix = ctx.get("auto_envvar_prefix")
     if not prefix or not param.name:
         return None
 
-    # Mimicks Click's internals.
+    # Mimics Click's internals.
     return f"{prefix}_{param.name.upper()}"
 
 
 def extend_envvars(
     envvars_1: str | Sequence[str] | None,
     envvars_2: str | Sequence[str] | None,
 ) -> tuple[str, ...]:
@@ -182,15 +182,15 @@
         .. caution::
             This is a `copy of Click's default value rendering of the default
             <https://github.com/pallets/click/blob/b0538df/src/click/core.py#L2754-L2792>`_
 
             This code **should be keep in sync with Click's implementation**.
 
         .. attention::
-            This doens't work with our own ``--config`` option because we are also
+            This doesn't work with our own ``--config`` option because we are also
             monkey-patching `ConfigOption.get_help_record()
             <https://kdeldycke.github.io/click-extra/config.html#click_extra.config.ConfigOption.get_help_record>`_
             to display the dynamic default value.
 
             So the results of this method call is:
 
                 .. code-block:: text
@@ -467,35 +467,35 @@
 
         self.params_template = template
         self.params_types = types
         self.params_objects = objects
 
     @cached_property
     def params_template(self):
-        """Returns a tree-like dictionnary whose keys shadows the CLI options and
+        """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are ``None``.
 
         Perfect to serve as a template for configuration files.
         """
         self.build_param_trees()
         return self.params_template
 
     @cached_property
     def params_types(self):
-        """Returns a tree-like dictionnary whose keys shadows the CLI options and
+        """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are their expected Python type.
 
         Perfect to parse configuration files and user-provided parameters.
         """
         self.build_param_trees()
         return self.params_types
 
     @cached_property
     def params_objects(self):
-        """Returns a tree-like dictionnary whose keys shadows the CLI options and
+        """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are parameter objects.
 
         Perfect to parse configuration files and user-provided parameters.
         """
         self.build_param_trees()
         return self.params_objects
 
@@ -551,15 +551,15 @@
         )
 
     def print_params(self, ctx, param, value):
         """Introspects current CLI and list its parameters and metadata.
 
         .. important::
             Click doesn't keep a list of all parsed arguments and their origin.
-            So we need to emulate here what's happening during CLI invokation.
+            So we need to emulate here what's happening during CLI invocation.
 
             Unfortunately we cannot even do that because the raw, pre-parsed arguments
             are not available anywhere within Click's internals.
 
             Our workaround consist in leveraging our custom
             ``ExtraCommand``/``ExtraGroup`` classes, in which we are attaching
             a ``click_extra.raw_args`` metadata entry to the context.
```

### Comparing `click_extra-4.4.0/click_extra/platforms.py` & `click_extra-4.5.0/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/pygments.py` & `click_extra-4.5.0/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/sphinx.py` & `click_extra-4.5.0/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tabulate.py` & `click_extra-4.5.0/click_extra/tabulate.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,32 +119,38 @@
     defaults.update(kwargs)
     echo(tabulate.tabulate(tabular_data, headers, **defaults))
 
 
 class TableFormatOption(ExtraOption):
     """A pre-configured option that is adding a ``-t``/``--table-format`` flag to select
     the rendering style of a table.
+
+    The selected table format ID is made available in the context in
+    ``ctx.meta["click_extra.table_format"]``.
     """
 
     def init_formatter(self, ctx, param, value):
-        """Save table format ID in the context, and attach ``print_table()`` method to
-        it.
+        """Save table format ID in the context, and adds ``print_table()`` to it.
 
-        ``print_table(tabular_data, headers)`` is a ready-to-use method that takes a
-        2-dimentional ``tabular_data`` iterable of iterables and a list of headers.
+        The ``print_table(tabular_data, headers)`` method added to the context is a
+        ready-to-use helper that takes for parameters:
+        - ``tabular_data``, a 2-dimensional iterable of iterables for cell values,
+        - ``headers``, a list of string to be used as headers.
         """
-        ctx.table_format = value
+        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
+        ctx._meta["click_extra.table_format"] = value
 
         render_func = None
         if value.startswith("csv"):
             render_func = partial(render_csv, dialect=get_csv_dialect(value))
         elif value == "vertical":
             render_func = render_vertical
         else:
             render_func = partial(render_table, tablefmt=value)
+
         ctx.print_table = render_func
 
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         type=Choice(output_formats, case_sensitive=False),
         default="rounded_outline",
```

### Comparing `click_extra-4.4.0/click_extra/telemetry.py` & `click_extra-4.5.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/testing.py` & `click_extra-4.5.0/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/__init__.py` & `click_extra-4.5.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/conftest.py` & `click_extra-4.5.0/click_extra/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Fixtures, configuration and helpers for tests."""
 
 from __future__ import annotations
 
-from pathlib import Path
-from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import click
 import click.testing
 import cloup
 import pytest
 
 from click_extra.decorators import command, extra_command, extra_group, group
 from click_extra.platforms import is_linux, is_macos, is_windows
 from click_extra.testing import ExtraCliRunner
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 skip_linux = pytest.mark.skipif(is_linux(), reason="Skip Linux")
 """Pytest mark to skip a test if run on a Linux system."""
 
 skip_macos = pytest.mark.skipif(is_macos(), reason="Skip macOS")
 """Pytest mark to skip a test if run on a macOS system."""
 
 skip_windows = pytest.mark.skipif(is_windows(), reason="Skip Windows")
@@ -186,27 +188,24 @@
     return tuple(decorator_params)
 
 
 @pytest.fixture()
 def create_config(tmp_path):
     """A generic fixture to produce a temporary configuration file."""
 
-    def _create_config(filename, content):
+    def _create_config(filename: str | Path, content: str) -> Path:
         """Create a fake configuration file."""
-        assert isinstance(content, str)
-
         if isinstance(filename, str):
             config_path = tmp_path.joinpath(filename)
         else:
-            assert isinstance(filename, Path)
             config_path = filename.resolve()
 
         # Create the missing folder structure, like "mkdir -p" does.
         config_path.parent.mkdir(parents=True, exist_ok=True)
-        config_path.write_text(dedent(content).strip())
+        config_path.write_text(content)
 
         return config_path
 
     return _create_config
 
 
 default_options_uncolored_help = (
@@ -288,15 +287,15 @@
     r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
     r"\x1b\[34mdebug\x1b\[0m: Load configuration"
     r" matching .+\*\.{toml,yaml,yml,json,ini,xml}\n"
     r"\x1b\[34mdebug\x1b\[0m: Pattern is not an URL.\n"
     r"\x1b\[34mdebug\x1b\[0m: Search local file system.\n"
     r"\x1b\[34mdebug\x1b\[0m: No configuration file found.\n"
     r"\x1b\[34mdebug\x1b\[0m: \x1b\[97m\S+\x1b\[0m,"
-    r" version \x1b\[32m\S+\x1b\[0m(\x1b\[90m)?\n"
-    r"\x1b\[34mdebug\x1b\[0m: {.*}\x1b\[0m\n"
+    r" version \x1b\[32m\S+\x1b\[0m\n"
+    r"\x1b\[34mdebug\x1b\[0m: \x1b\[90m{.*}\x1b\[0m\n"
 )
 
 default_debug_colored_log_end = (
     r"\x1b\[34mdebug\x1b\[0m: Reset <RootLogger root \(DEBUG\)> to WARNING.\n"
     r"\x1b\[34mdebug\x1b\[0m: Reset <Logger click_extra \(DEBUG\)> to WARNING.\n"
 )
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_colorize.py` & `click_extra-4.5.0/click_extra/tests/test_colorize.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
         (("hey", "hey"), "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         ({"hey", "hey"}, "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         (
             "heyhey",
             "H\x1b[32mey\x1b[0m-xx-xxx-\x1b[32mhe\x1b[0mY-xXxXxxxxx-\x1b[32mhey\x1b[0m",
             False,
         ),
-        # Case-sensivity and multiple matches.
+        # Case-sensitivity and multiple matches.
         (["hey"], "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         (
             ["Hey"],
             "\x1b[32mHey\x1b[0m-xx-xxx-\x1b[32mheY\x1b[0m-xXxXxxxxx-\x1b[32mhey\x1b[0m",
             True,
         ),
         (
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_commands.py` & `click_extra-4.5.0/click_extra/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,16 @@
     )
     assert not result.stderr
 
 
 def test_integrated_version_value(invoke, all_command_cli):
     result = invoke(all_command_cli, "--version", color=False)
     assert result.exit_code == 0
-
-    regex_stdout = r"command-cli1, version 2021.10.08\n{'.+'}\n"
-    assert re.fullmatch(regex_stdout, result.stdout)
-
     assert not result.stderr
+    assert result.stdout == "command-cli1, version 2021.10.08\n"
 
 
 def test_no_option_leaks_between_subcommands(invoke):
     """As reported in https://github.com/kdeldycke/click-extra/issues/489."""
 
     @click.group
     def cli():
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_config.py` & `click_extra-4.5.0/click_extra/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import re
 from pathlib import Path
+from textwrap import dedent
 
 import click
 import pytest
 from boltons.pathutils import shrinkuser
 from pytest_cases import fixture, parametrize
 
 from click_extra import (
@@ -38,25 +39,26 @@
     IntRange,
     Tuple,
     argument,
     echo,
     get_app_dir,
     option,
 )
-from click_extra.colorize import escape_for_help_sceen
+from click_extra.colorize import escape_for_help_screen
 from click_extra.config import ConfigOption
 from click_extra.decorators import config_option, extra_group
 from click_extra.parameters import search_params
 
 from .conftest import (
     default_debug_uncolored_log_end,
     default_debug_uncolored_log_start,
 )
 
-DUMMY_TOML_FILE = """
+DUMMY_TOML_FILE = dedent(
+    """
     # Comment
 
     top_level_param             = "to_ignore"
 
     [config-cli1]
     verbosity = "DEBUG"
     blahblah = 234
@@ -65,17 +67,19 @@
 
     [garbage]
     # An empty random section that will be skipped
 
     [config-cli1.default-command]
     int_param = 3
     random_stuff = "will be ignored"
-    """
+    """,
+)
 
-DUMMY_YAML_FILE = """
+DUMMY_YAML_FILE = dedent(
+    """
     # Comment
 
     top_level_param: to_ignore
 
     config-cli1:
         verbosity : DEBUG
         blahblah: 234
@@ -87,17 +91,19 @@
         default-command:
             int_param: 3
             random_stuff : will be ignored
 
     garbage:
         # An empty random section that will be skipped
 
-    """
+    """,
+)
 
-DUMMY_JSON_FILE = """
+DUMMY_JSON_FILE = dedent(
+    """
     {
         "top_level_param": "to_ignore",
         "config-cli1": {
             "blahblah": 234,
             "dummy_flag": true,
             "my_list": [
                 "pip",
@@ -112,17 +118,19 @@
                 "random_stuff": "will be ignored"
             }
         },
 
         // Section to ignore
         "garbage": {}
     }
-    """
+    """,
+)
 
-DUMMY_INI_FILE = """
+DUMMY_INI_FILE = dedent(
+    """
     ; Comment
     # Another kind of comment
 
     [to_ignore]
     key=value
     spaces in keys=allowed
     spaces in values=allowed as well
@@ -137,17 +145,19 @@
     # An empty random section that will be skipped
 
     [config-cli1]
     verbosity : DEBUG
     blahblah: 234
     dummy_flag = true
     my_list = ["pip", "npm", "gem"]
-    """
+    """,
+)
 
-DUMMY_XML_FILE = """
+DUMMY_XML_FILE = dedent(
+    """
     <!-- Comment -->
 
     <config-cli1 has="an attribute">
 
         <to_ignore>
             <key>value</key>
             <spaces >    </spaces>
@@ -174,15 +184,16 @@
 
         <default-command>
             <int_param>3</int_param>
             <random_stuff>will be ignored</random_stuff>
         </default-command>
 
     </config-cli1>
-    """
+    """,
+)
 
 
 all_config_formats = pytest.mark.parametrize(
     "conf_name, conf_content",
     (
         pytest.param(f"configuration.{ext}", content, id=ext)
         for ext, content in (
@@ -209,21 +220,14 @@
     @option("--int-param", type=int, default=10)
     def default_command(int_param):
         echo(f"int_parameter = {int_param!r}")
 
     return config_cli1
 
 
-@pytest.mark.xfail(
-    strict=False,
-    reason=(
-        "stderr is not supposed to be filled with debug logs, but it seems there is a "
-        "leak somewhere in our logging system"
-    ),
-)
 def test_unset_conf_no_message(invoke, simple_config_cli):
     result = invoke(simple_config_cli, "default-command")
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
 
 
@@ -251,15 +255,15 @@
     # OS-specific path.
     default_path = shrinkuser(
         Path(get_app_dir("config-cli1")) / "*.{toml,yaml,yml,json,ini,xml}",
     )
 
     # Make path string compatible with regexp.
     assert re.search(
-        rf"\[default:\s+{escape_for_help_sceen(str(default_path))}\]",
+        rf"\[default:\s+{escape_for_help_screen(str(default_path))}\]",
         result.stdout,
     )
 
 
 def test_conf_not_exist(invoke, simple_config_cli):
     conf_path = Path("dummy.toml")
     result = invoke(
@@ -433,25 +437,27 @@
         echo(f"my_list       is {my_list!r}")
 
     @config_cli3.command
     @option("--int-param", type=int, default=10)
     def subcommand(int_param):
         echo(f"int_parameter is {int_param!r}")
 
-    conf_file = """
+    conf_file = dedent(
+        """
         # My default configuration file.
 
         [config-cli3]
         dummy_flag = true   # New boolean default.
         my_list = ["item 1", "item #2", "Very Last Item!"]
 
         [config-cli3.subcommand]
         int_param = 3
         random_stuff = "will be ignored"
-        """
+        """,
+    )
 
     conf_path = create_config("messy.toml", conf_file)
 
     result = invoke(config_cli3, "--config", str(conf_path), "subcommand", color=False)
 
     assert result.exception
     assert type(result.exception) == ValueError
@@ -541,15 +547,15 @@
         assert result.stderr == (
             f"Load configuration matching {conf_path.resolve()}\n"
             "debug: Verbosity set to DEBUG.\n"
         )
 
 
 @all_config_formats
-def test_conf_file_overrided_by_cli_param(
+def test_conf_file_overridden_by_cli_param(
     invoke,
     simple_config_cli,
     create_config,
     httpserver,
     conf_name,
     conf_content,
 ):
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_logging.py` & `click_extra-4.5.0/click_extra/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/test_parameters.py` & `click_extra-4.5.0/click_extra/tests/test_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,19 +306,21 @@
     @extra_command
     @option("--int-param1", type=int, default=10)
     @option("--int-param2", type=int, default=555)
     def show_params_cli(int_param1, int_param2):
         echo(f"int_param1 is {int_param1!r}")
         echo(f"int_param2 is {int_param2!r}")
 
-    conf_file = """
+    conf_file = dedent(
+        """
         [show-params-cli]
         int_param1 = 3
         extra_value = "unallowed"
-        """
+        """,
+    )
     conf_path = create_config("show-params-cli.toml", conf_file)
 
     raw_args = [
         "--verbosity",
         "DeBuG",
         "--config",
         str(conf_path),
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_platforms.py` & `click_extra-4.5.0/click_extra/tests/test_platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,32 +129,32 @@
         assert not is_solaris()
         assert not is_sunos()
         assert not is_wsl1()
         assert not is_wsl2()
 
 
 def test_platform_definitions():
-    for plaform in ALL_PLATFORMS.platforms:
+    for platform in ALL_PLATFORMS.platforms:
         # ID.
-        assert plaform.id
-        assert plaform.id.isascii()
-        assert plaform.id.isalnum()
-        assert plaform.id.islower()
+        assert platform.id
+        assert platform.id.isascii()
+        assert platform.id.isalnum()
+        assert platform.id.islower()
         # Name.
-        assert plaform.name
-        assert plaform.name.isascii()
-        assert plaform.name.isprintable()
-        assert plaform.name in ALL_OS_LABELS
+        assert platform.name
+        assert platform.name.isascii()
+        assert platform.name.isprintable()
+        assert platform.name in ALL_OS_LABELS
         # Identification function.
-        check_func_id = f"is_{plaform.id}"
+        check_func_id = f"is_{platform.id}"
         assert check_func_id in globals()
         check_func = globals()[check_func_id]
         assert isinstance(check_func, functools._lru_cache_wrapper)
         assert isinstance(check_func(), bool)
-        assert check_func() == plaform.current
+        assert check_func() == platform.current
 
 
 def test_unique_ids():
     """Platform and group IDs must be unique."""
     all_platform_ids = [p.id for p in ALL_PLATFORMS]
 
     # Platforms are expected to be sorted by ID.
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_pygments.py` & `click_extra-4.5.0/click_extra/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/test_tabulate.py` & `click_extra-4.5.0/click_extra/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,14 +521,17 @@
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
 @parametrize("option_decorator", (table_format_option, table_format_option()))
 def table_cli(cmd_decorator, option_decorator):
     @cmd_decorator
     @option_decorator
     @pass_context
     def tabulate_cli2(ctx):
+        format_id = ctx.meta["click_extra.table_format"]
+        echo(f"Table format: {format_id}")
+
         data = ((1, 87), (2, 80), (3, 79))
         headers = ("day", "temperature")
         ctx.print_table(data, headers)
 
     return tabulate_cli2
 
 
@@ -537,9 +540,9 @@
     (pytest.param(k, v, id=k) for k, v in expected_renderings.items()),
 )
 def test_all_table_rendering(invoke, table_cli, format_name, expected):
     result = invoke(table_cli, "--table-format", format_name)
     assert result.exit_code == 0
     if not is_windows():
         expected = expected.replace("\r\n", "\n")
-    assert result.stdout == expected
+    assert result.stdout == f"Table format: {format_name}\n{expected}"
     assert not result.stderr
```

### Comparing `click_extra-4.4.0/click_extra/tests/test_telemetry.py` & `click_extra-4.5.0/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/test_testing.py` & `click_extra-4.5.0/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/test_timer.py` & `click_extra-4.5.0/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/click_extra/tests/test_version.py` & `click_extra-4.5.0/click_extra/tests/test_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 from __future__ import annotations
 
 import re
 
 import click
 import pytest
+from boltons.strutils import strip_ansi
 from pytest_cases import parametrize
 
-from click_extra import Style, echo
+from click_extra import Style, __version__, echo, pass_context
 from click_extra.decorators import color_option, extra_group, version_option
 
 from .conftest import command_decorators, skip_windows_colors
 
 
 @skip_windows_colors
 @parametrize("cmd_decorator", command_decorators())
@@ -36,83 +37,138 @@
     @option_decorator
     def standalone_option():
         echo("It works!")
 
     result = invoke(standalone_option, "--version", color=True)
     assert result.exit_code == 0
     assert not result.stderr
-    assert re.fullmatch(
-        r"\x1b\[97mstandalone-option\x1b\[0m, version \x1b\[32m\d+.\d+.\d+\x1b\[0m\n",
-        result.output,
+    assert result.output == (
+        "\x1b[97mstandalone-option\x1b[0m, "
+        f"version \x1b[32m{__version__}"
+        "\x1b[0m\n"
     )
 
 
 @skip_windows_colors
-def test_standalone_version_option_with_env_info(invoke):
+def test_set_version(invoke):
     @click.group
-    @version_option(version="1.2.3.4", print_env_info=True)
+    @version_option(version="1.2.3.4")
     def color_cli2():
         echo("It works!")
 
     # Test default coloring.
     result = invoke(color_cli2, "--version", color=True)
     assert result.exit_code == 0
-
-    regex_stdout = (
-        r"\x1b\[97mcolor-cli2\x1b\[0m, version \x1b\[32m1.2.3.4"
-        r"\x1b\[0m\x1b\[90m\n{'.+'}"
-        r"\x1b\[0m\n"
-    )
-    assert re.fullmatch(regex_stdout, result.stdout)
-
     assert not result.stderr
+    assert result.stdout == (
+        "\x1b[97mcolor-cli2\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
+    )
 
 
-@pytest.mark.xfail(
-    strict=False,
-    reason="version_option always displays click-extra version. See #176.",
-)
 @skip_windows_colors
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
-def test_standalone_version_option_without_env_info(invoke, cmd_decorator):
+@parametrize(
+    "message, regex_stdout",
+    (
+        (
+            "%(prog_name)s, version %(version)s",
+            r"\x1b\[97mcolor-cli3\x1b\[0m, "
+            rf"version \x1b\[32m{re.escape(__version__)}"
+            r"\x1b\[0m\n",
+        ),
+        (
+            "%(prog_name)s, version %(version)s\n%(env_info)s",
+            r"\x1b\[97mcolor-cli3\x1b\[0m, "
+            rf"version \x1b\[32m{re.escape(__version__)}"
+            r"\x1b\[0m\n"
+            r"\x1b\[90m{'.+'}"
+            r"\x1b\[0m\n",
+        ),
+        (
+            "%(prog_name)s v%(version)s - %(package_name)s",
+            r"\x1b\[97mcolor-cli3\x1b\[0m "
+            rf"v\x1b\[32m{re.escape(__version__)}"
+            r"\x1b\[0m - "
+            r"\x1b\[97mclick_extra"
+            r"\x1b\[0m\n",
+        ),
+    ),
+)
+def test_custom_message(invoke, cmd_decorator, message, regex_stdout):
     @cmd_decorator
-    @version_option(version="1.2.3.4", print_env_info=False)
+    @version_option(message=message)
     def color_cli3():
         echo("It works!")
 
-    # Test default coloring.
     result = invoke(color_cli3, "--version", color=True)
     assert result.exit_code == 0
-    assert (
-        result.stdout == "\x1b[97mcolor-cli3\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
+    assert not result.stderr
+    assert re.fullmatch(regex_stdout, result.output)
+
+
+@parametrize("cmd_decorator", command_decorators(no_groups=True))
+def test_style_reset(invoke, cmd_decorator):
+    @cmd_decorator
+    @version_option(
+        version_style=None,
+        package_name_style=None,
+        prog_name_style=None,
+        env_info_style=None,
+        message_style=None,
     )
+    def color_reset():
+        pass
+
+    result = invoke(color_reset, "--version", color=True)
+    assert result.exit_code == 0
     assert not result.stderr
+    assert result.output == strip_ansi(result.output)
+
+
+@parametrize("cmd_decorator", command_decorators(no_groups=True))
+def test_context_meta(invoke, cmd_decorator):
+    @cmd_decorator
+    @version_option
+    @pass_context
+    def version_metadata(ctx):
+        for var in ("version", "package_name", "prog_name", "env_info"):
+            value = ctx.meta[f"click_extra.{var}"]
+            echo(f"{var} = {value}")
+
+    result = invoke(version_metadata, color=True)
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert re.fullmatch(
+        (
+            rf"version = {__version__}\n"
+            r"package_name = click_extra\n"
+            r"prog_name = version-metadata\n"
+            r"env_info = {'.+'}\n"
+        ),
+        result.output,
+    )
+    assert result.output == strip_ansi(result.output)
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
     "params",
     (None, "--help", "blah", ("--config", "random.toml")),
 )
 def test_integrated_version_option_precedence(invoke, params):
     @extra_group(version="1.2.3.4")
     def color_cli4():
         echo("It works!")
 
     result = invoke(color_cli4, "--version", params, color=True)
     assert result.exit_code == 0
-
-    regex_stdout = (
-        r"\x1b\[97mcolor-cli4\x1b\[0m, version \x1b\[32m1.2.3.4"
-        r"\x1b\[0m\x1b\[90m\n{'.+'}"
-        r"\x1b\[0m\n"
-    )
-    assert re.fullmatch(regex_stdout, result.stdout)
-
     assert not result.stderr
+    assert result.stdout == (
+        "\x1b[97mcolor-cli4\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
+    )
 
 
 @skip_windows_colors
 def test_color_option_precedence(invoke):
     """--no-color has an effect on --version, if placed in the right order.
 
     Eager parameters are evaluated in the order as they were provided on the command
@@ -130,14 +186,16 @@
     @color_option
     @version_option(version="2.1.9")
     def color_cli6():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli6, "--no-color", "--version", "command1", color=True)
     assert result.exit_code == 0
-    assert result.stdout == "color-cli6, version 2.1.9\n"
     assert not result.stderr
+    assert result.stdout == "color-cli6, version 2.1.9\n"
 
     result = invoke(color_cli6, "--version", "--no-color", "command1", color=True)
     assert result.exit_code == 0
-    assert result.stdout == "\x1b[97mcolor-cli6\x1b[0m, version \x1b[32m2.1.9\x1b[0m\n"
     assert not result.stderr
+    assert result.stdout == (
+        "\x1b[97mcolor-cli6\x1b[0m, version \x1b[32m2.1.9\x1b[0m\n"
+    )
```

### Comparing `click_extra-4.4.0/click_extra/timer.py` & `click_extra-4.5.0/click_extra/timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,35 +24,39 @@
 from . import echo
 from .parameters import ExtraOption
 
 
 class TimerOption(ExtraOption):
     """A pre-configured option that is adding a ``--time``/``--no-time`` flag to print
     elapsed time at the end of CLI execution.
+
+    The start time is made available in the context in
+    ``ctx.meta["click_extra.start_time"]``.
     """
 
     def print_timer(self):
         """Compute and print elapsed execution time."""
         echo(f"Execution time: {perf_counter() - self.start_time:0.3f} seconds.")
 
     def register_timer_on_close(self, ctx, param, value):
         """Callback setting up all timer's machinery.
 
         Computes and print the execution time at the end of the CLI, if option has been
         activated.
         """
-        # Skip timekeeping if option is not active.
-        if not value:
-            return
-
         # Take timestamp snapshot.
         self.start_time = perf_counter()
 
-        # Register printing at the end of execution.
-        ctx.call_on_close(self.print_timer)
+        # XXX ctx.meta doesn't cut it, we need to target ctx._meta.
+        ctx._meta["click_extra.start_time"] = self.start_time
+
+        # Skip timekeeping if option is not active.
+        if value:
+            # Register printing at the end of execution.
+            ctx.call_on_close(self.print_timer)
 
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         default=False,
         expose_value=False,
         help=_("Measure and print elapsed execution time."),
```

### Comparing `click_extra-4.4.0/pyproject.toml` & `click_extra-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.4.0"
+version = "4.5.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -103,14 +103,15 @@
 furo = "^2023.05.20"
 mypy = "^1.2.0"
 myst-parser = ">=1,<3"
 pytest = "^7.3.1"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cases = "^3.6.14"
 pytest-cov = "^4.0.0"
+pytest-github-actions-annotate-failures = "^0.2.0"
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-copybutton = "^0.5.2"
 sphinx-design = "^0.4.1"
 sphinx-issues = "^3.0.1"
 sphinxext-opengraph = "^0.7.5"
@@ -179,15 +180,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.4.0"
+current_version = "4.5.0"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./click_extra/__init__.py"
 
 [[tool.bumpversion.files]]
 filename = "./pyproject.toml"
```

### Comparing `click_extra-4.4.0/readme.md` & `click_extra-4.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.4.0/PKG-INFO` & `click_extra-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.4.0
+Version: 4.5.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.4.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.5.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
```

