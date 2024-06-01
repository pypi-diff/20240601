# Comparing `tmp/aurum_hikari-0.1.5.5.tar.gz` & `tmp/aurum_hikari-0.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.5.5.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.5.6.tar", max compression
```

## Comparing `aurum_hikari-0.1.5.5.tar` & `aurum_hikari-0.1.5.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1080 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/LICENSE
--rw-r--r--   0        0        0     3510 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/README.md
--rw-r--r--   0        0        0      584 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/__init__.py
--rw-r--r--   0        0        0      382 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/__main__.py
--rw-r--r--   0        0        0      563 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/_about.py
--rw-r--r--   0        0        0      183 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/client/__init__.py
--rw-r--r--   0        0        0     9579 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/client/client.py
--rw-r--r--   0        0        0      720 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/client/integration.py
--rw-r--r--   0        0        0      366 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2324 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/message_command.py
--rw-r--r--   0        0        0     5767 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2720 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/__init__.py
--rw-r--r--   0        0        0      312 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     1724 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_integration.py
--rw-r--r--   0        0        0     3462 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     8895 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     5738 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/utils/commands.py
--rw-r--r--   0        0        0      226 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/version.py
--rw-r--r--   0        0        0      360 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/localized.py
--rw-r--r--   0        0        0      479 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/types.py
--rw-r--r--   0        0        0     2360 2024-05-27 16:39:12.007720 aurum_hikari-0.1.5.5/pyproject.toml
--rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/LICENSE
+-rw-r--r--   0        0        0     3038 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/README.md
+-rw-r--r--   0        0        0      643 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/__init__.py
+-rw-r--r--   0        0        0      382 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/__main__.py
+-rw-r--r--   0        0        0      591 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/_about.py
+-rw-r--r--   0        0        0      183 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/client/__init__.py
+-rw-r--r--   0        0        0    10411 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/client/client.py
+-rw-r--r--   0        0        0      720 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/client/integration.py
+-rw-r--r--   0        0        0      366 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2557 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5814 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2720 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2635 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0      180 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/events/__init__.py
+-rw-r--r--   0        0        0      383 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/events/event.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      312 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4866 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     1724 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin_integration.py
+-rw-r--r--   0        0        0     3291 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      220 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     8930 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3020 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     5902 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1912 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0      292 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/includable.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      226 2024-06-01 10:38:22.994762 aurum_hikari-0.1.5.6/aurum/internal/version.py
+-rw-r--r--   0        0        0      360 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0     1185 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      479 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/options/choice.py
+-rw-r--r--   0        0        0     1729 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:38:22.998762 aurum_hikari-0.1.5.6/aurum/py.typed
+-rw-r--r--   0        0        0     2360 2024-06-01 10:38:37.190904 aurum_hikari-0.1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.6/PKG-INFO
```

### Comparing `aurum_hikari-0.1.5.5/LICENSE` & `aurum_hikari-0.1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/__init__.py` & `aurum_hikari-0.1.5.6/aurum/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from __future__ import annotations
 
 __all__: Sequence[str] = (
     "Client",
     "MessageCommand",
     "SlashCommand",
     "UserCommand",
+    "sub_command",
     "InteractionContext",
     "LocalizationProviderInterface",
     "Localized",
     "LocalizedOr",
     "Option",
     "Choice",
 )
 
 import typing
 
 from aurum.client import *
 from aurum.commands import *
+from aurum.commands.decorators import *
 from aurum.interactions import *
 from aurum.l10n import *
 from aurum.options import *
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
```

### Comparing `aurum_hikari-0.1.5.5/aurum/_about.py` & `aurum_hikari-0.1.5.6/aurum/_about.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 import typing
 
 from aurum.internal.version import Version
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
-__version_tuple__: Version = Version(0, 1, 5, 5)
-__version__: str = str(__version_tuple__)
+__version_tuple__: typing.Final[Version] = Version(0, 1, 5, 6)
+__version__: typing.Final[str] = str(__version_tuple__)
```

### Comparing `aurum_hikari-0.1.5.5/aurum/client/client.py` & `aurum_hikari-0.1.5.6/aurum/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import asyncio
 import typing
-from collections.abc import Callable
 from logging import getLogger
 
 from hikari.commands import CommandType, OptionType
+from hikari.errors import HikariError
 from hikari.events import InteractionCreateEvent, StartedEvent, StartingEvent
 from hikari.interactions import CommandInteraction, ComponentInteraction
 
-from aurum.client.integration import IClientIntegration
 from aurum.commands import MessageCommand, SlashCommand, SubCommand, UserCommand
 from aurum.enum.sync_commands import SyncCommandsFlag
 from aurum.interactions import InteractionContext
 from aurum.internal.commands.app_command import AppCommand
 from aurum.internal.commands.command_handler import CommandHandler
 from aurum.internal.exceptions import AurumException, UnknownCommandException
 from aurum.l10n.pass_localization_provider import PassLocalizationProvider
@@ -22,35 +21,36 @@
     from collections.abc import Coroutine, Sequence
     from logging import Logger
 
     from hikari.interactions import (
         CommandInteractionOption,
         PartialInteraction,
     )
+    from hikari.traits import GatewayBotAware
 
+    from aurum.client.integration import IClientIntegration
     from aurum.ext.plugins import PluginManager
-    from aurum.includable import Includable
+    from aurum.internal.includable import Includable
     from aurum.l10n import LocalizationProviderInterface
-    from aurum.types import BotT
 
 
 class Client:
     """A wrapper class for the main bot class, designed to work with the Aurum framework and its features.
 
     Note:
         At the moment, the wrapper only supports gateway connections.
 
     Attributes:
         l10n (LocalizationProviderInterface): The localization provider instance for multi-language support.
             It is recommended to provide a localization provider if multi-language support is required.
-        bot (BotT): The bot instance.
+        bot (GatewayBotAware): The bot instance.
         commands (CommandHandler): The command handler.
 
     Args:
-        bot (BotT): The bot instance that this client will interact with.
+        bot (GatewayBotAware): The bot instance that this client will interact with.
         l10n (LocalizationProviderInterface): Localization provider.
             If a localization provider is not provided, an `EmptyLocalizationProvider`
             will be used, which will pass all functions and return the key.
         integrations: (Sequence[IClientIntegration]): A list of integrations for client.
         sync_commands (SyncCommandFlag): An optional SyncCommandsFlag enum value, indicating how to handle command synchronization.
         ignore_l10n (bool): An optional flag. If `True`, the client will not emit a warning when a localization provider is not provided.
         ignore_unknown_interactions (bool): An optional flag that, if set to `True`, will disable the warning message for unknown interactions.
@@ -65,15 +65,15 @@
         "bot",
         "commands",
         "plugins",
     )
 
     def __init__(
         self,
-        bot: BotT,
+        bot: GatewayBotAware,
         *,
         l10n: LocalizationProviderInterface | None = None,
         integrations: Sequence[IClientIntegration] = (),
         sync_commands: SyncCommandsFlag = SyncCommandsFlag.SYNC,
         ignore_l10n: bool = False,
         ignore_unknown_interactions: bool = False,
     ) -> None:
@@ -88,15 +88,15 @@
                 "a localization provider has not been specified and localization will not be available. "
                 "If you require localization, please use one of the available localization providers "
                 "or create your own implementation based on the LocalizationProviderInterface."
             )
         else:
             self.add_starting_task(self.l10n.start())
 
-        self.bot: BotT = bot
+        self.bot: GatewayBotAware = bot
         self.commands: CommandHandler = CommandHandler(bot, self.l10n)
         self.plugins: PluginManager | None = None
 
         for integration in integrations:
             integration.install(self)
             self.__logger.debug(f"installed integration: {type(integration).__qualname__}")
 
@@ -152,22 +152,26 @@
     async def on_interaction(self, event: InteractionCreateEvent) -> None:
         interaction: PartialInteraction = event.interaction
         if isinstance(interaction, CommandInteraction):
             return await self.proceed_command(interaction)
 
     async def proceed_command(self, interaction: CommandInteraction) -> None:
         context: InteractionContext = self.create_interaction_context(interaction)
-        parent_command: AppCommand | None = self.commands.commands.get(interaction.command_name)
+
+        parent_command: AppCommand | None = self.commands.app_commands.get(interaction.command_id)
         if not parent_command and not self._ignore_unknown_interactions:
             raise UnknownCommandException(interaction.command_name)
-        command: AppCommand | SubCommand | None = parent_command
+
         if interaction.command_type is CommandType.SLASH:
-            assert isinstance(command, SlashCommand)
+            assert isinstance(parent_command, SlashCommand)
+            command: SlashCommand | SubCommand = parent_command
+
             options: Sequence[CommandInteractionOption] | None = interaction.options
             arguments: typing.Dict[str, typing.Any] = {}
+
             if options:
                 option: CommandInteractionOption = options[0]
                 if option.type is OptionType.SUB_COMMAND:
                     command = command.sub_commands.get(option.name)
                     options = option.options
                     if not command and not self._ignore_unknown_interactions:
                         raise UnknownCommandException(option.name, interaction.command_name)
@@ -180,31 +184,46 @@
                         options = options[0].options
                         if not command and not self._ignore_unknown_interactions:
                             raise UnknownCommandException(
                                 option.name, sub_command_group.name, interaction.command_name
                             )
                 for option in options or ():
                     arguments[option.name] = context.resolve_command_argument(option)
-            callback: Callable[..., Coroutine[None, None, typing.Any]] = getattr(
-                command, "callback"
-            )
-            if isinstance(command, SlashCommand):
-                await callback(context, **arguments)
-                return
-            await callback(parent_command, context, **arguments)
+            try:
+                if isinstance(command, SlashCommand):
+                    await command.callback(context, **arguments)
+                    return
+                await command.callback(parent_command, context, **arguments)
+            except Exception as error:
+                self.__logger.exception(
+                    "An unexcepted error occurred in command %s", command.name, exc_info=error
+                )
+                await self.on_command_error(context, error)
             return
         if interaction.command_type is CommandType.MESSAGE:
-            assert isinstance(command, MessageCommand)
+            assert isinstance(parent_command, MessageCommand)
             assert interaction.resolved
-            await command.callback(
+            await parent_command.callback(
                 context,
                 list(interaction.resolved.messages.values())[0],
             )
             return
         if interaction.command_type is CommandType.USER:
-            assert isinstance(command, UserCommand)
+            assert isinstance(parent_command, UserCommand)
             assert interaction.resolved
-            await command.callback(
+            await parent_command.callback(
                 context,
                 list(interaction.resolved.users.values())[0],
             )
             return
+
+    async def on_unexcepted_error(self, context: InteractionContext, error: Exception) -> None:
+        """Response on unexcepted error"""
+        try:
+            await context.create_response("An unexcepted error occurred.", ephemeral=True)
+        except HikariError:
+            await context.edit_response("An unexcepted error occurred.")
+        return
+
+    async def on_command_error(self, context: InteractionContext, error: Exception) -> None:
+        """Handler of commands' errors"""
+        await self.on_unexcepted_error(context, error)
```

### Comparing `aurum_hikari-0.1.5.5/aurum/client/integration.py` & `aurum_hikari-0.1.5.6/aurum/client/integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.5.6/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/commands/message_command.py` & `aurum_hikari-0.1.5.6/aurum/commands/message_command.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from hikari.commands import CommandType
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
 from aurum.internal.commands.context_menu_command import ContextMenuCommand
 
 if typing.TYPE_CHECKING:
+    from collections.abc import Sequence
+
     from hikari.guilds import PartialGuild
     from hikari.messages import Message
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
 
     from aurum.interactions import InteractionContext
 
@@ -34,14 +36,24 @@
                 super().__init__(name="Reverse", is_dm_enabled=True)
 
             async def callback(self, context: InteractionContext, message: Message) -> None:
                 await context.create_response(message.content[::-1])
         ```
     """
 
+    __slots__: Sequence[str] = (
+        "app",
+        "command_type",
+        "name",
+        "guild",
+        "default_member_permissions",
+        "dm_enabled",
+        "is_nsfw",
+    )
+
     def __init__(
         self,
         name: str,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
         is_dm_enabled: bool = False,
```

### Comparing `aurum_hikari-0.1.5.5/aurum/commands/slash_command.py` & `aurum_hikari-0.1.5.6/aurum/commands/slash_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,47 +55,47 @@
         options (Sequence[Option]): Options to the command.
         sub_commands (Dict[str, SubCommand]): Sub-commands of the command.
 
     Example:
         === "With callback"
             ```py
             class HelloCommand(SlashCommand):
-            def __init__(self) -> None:
-                super().__init__(name="hello", description="Say hi to bot")  # (1)
+                def __init__(self) -> None:
+                    super().__init__(name="hello", description="Say hi to bot")  # (1)
 
-            async def callback(self, context: InteractionContext) -> None:
-                await context.create_response(f"Hi, {context.user.mention}!")
+                async def callback(self, context: InteractionContext) -> None:
+                    await context.create_response(f"Hi, {context.user.mention}!")
             ```
 
             1. Base information about your command: name, description, default member permissions and etc.
 
         === "With sub-commands"
             ```py
             class ABCCommand(SlashCommand):  # (1)
-            def __init__(self) -> None:
-                super().__init__(name="a")  # (2)
+                def __init__(self) -> None:
+                    super().__init__(name="a")  # (2)
 
-            @sub_command(name="b")  # (3)
-            async def b_command(self, context: InteractionContext) -> None:
-                ...  # (4)
-
-            @b_command.sub_command(name="c")
-            async def b_c_command(self, context: InteractionContext) -> None:
-                ...
+                @sub_command(name="b")  # (3)
+                async def b_command(self, context: InteractionContext) -> None:
+                    ...  # (4)
+
+                @b_command.sub_command(name="c")
+                async def b_c_command(self, context: InteractionContext) -> None:
+                    ...
             ```
 
             1. When command has a sub-commands, callback will be ignored.
             2. Base information about your command: name, description, default member permissions and etc.
             3. Base information about your sub-command.
                 The same fields with slash-command, but without guild, default member permissions, is nsfw, dm enabled flags.
             4. If sub-command have another sub-command, callback of parent sub-command will be ignored too.
     """
 
     __slots__: Sequence[str] = (
-        "_app",
+        "app",
         "command_type",
         "name",
         "description",
         "guild",
         "default_member_permissions",
         "dm_enabled",
         "is_nsfw",
```

### Comparing `aurum_hikari-0.1.5.5/aurum/commands/sub_command.py` & `aurum_hikari-0.1.5.6/aurum/commands/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/commands/user_command.py` & `aurum_hikari-0.1.5.6/aurum/commands/user_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from hikari.commands import CommandType
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
 from aurum.internal.commands.context_menu_command import ContextMenuCommand
 
 if typing.TYPE_CHECKING:
+    from collections.abc import Sequence
+
     from hikari.guilds import PartialGuild
     from hikari.interactions import InteractionMember
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
     from hikari.users import PartialUser
 
     from aurum.interactions import InteractionContext
@@ -35,14 +37,24 @@
                 super().__init__(name="Hello to")
 
             async def callback(self, context: InteractionContext, target: InteractionMember | User) -> None:
                 await context.create_response(f"Hi, {target.mention}!")
         ```
     """
 
+    __slots__: Sequence[str] = (
+        "app",
+        "command_type",
+        "name",
+        "guild",
+        "default_member_permissions",
+        "dm_enabled",
+        "is_nsfw",
+    )
+
     def __init__(
         self,
         name: str,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
         is_dm_enabled: bool = False,
```

### Comparing `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from __future__ import annotations
 
 import typing
 
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
+from aurum.events import Event
 from aurum.internal.commands.app_command import AppCommand
 from aurum.internal.exceptions.base_exception import AurumException
 
 if typing.TYPE_CHECKING:
-    from collections.abc import Sequence
+    from collections.abc import Callable, Sequence
 
+    from hikari.traits import GatewayBotAware
+    from hikari.api.event_manager import CallbackT
+    from hikari.events.base_events import EventT
     from hikari.guilds import PartialGuild
     from hikari.snowflakes import SnowflakeishOr
     from hikari.undefined import UndefinedType
 
     from aurum.client import Client
-    from aurum.includable import Includable
+    from aurum.internal.includable import Includable
     from aurum.l10n import LocalizedOr
-    from aurum.types import BotT
 
 
 class Plugin:
     """
     Plugins include commands and components and provide bot, client, and etc.
 
     Attributes:
         name (str): The plugin name.
         description (LocalizedOr[str] | None): Optional description of the plugin.
         guild (SnowflakeishOr[PartialGuild] | UndefinedType): Optional guild (server) where the plugin is available.
         default_member_permissions (Permissions): The permissions a user must have to use the plugin by default.
         dm_enabled (bool): Whether the plugin can be used in direct messages.
         is_nsfw (bool): Indicates whether the plugin is age-restricted.
         included (Dict[str, Includable]): Included objects of plugin.
+        events (List[Event]): Events of plugin.
 
     Example:
         ```py
         plugin = Plugin(
             "Admin Plugin",
             default_member_permissions=Permissions.ADMINISTRATOR
         )
@@ -68,61 +72,68 @@
         "name",
         "description",
         "guild",
         "default_member_permissions",
         "is_dm_enabled",
         "is_nsfw",
         "included",
+        "events",
     )
 
     def __init__(
         self,
         name: str,
         description: LocalizedOr[str] | None = None,
         *,
         guild: SnowflakeishOr[PartialGuild] | UndefinedType = UNDEFINED,
         default_member_permissions: Permissions = Permissions.NONE,
         is_dm_enabled: bool = False,
         is_nsfw: bool = False,
     ) -> None:
-        self._bot: BotT | None = None
+        self._bot: GatewayBotAware | None = None
         self._client: Client | None = None
 
         self.name: str = name
         self.description: LocalizedOr[str] | None = description
 
         self.guild: SnowflakeishOr[PartialGuild] | UndefinedType = guild
         self.default_member_permissions: Permissions = default_member_permissions
         self.is_dm_enabled: bool = is_dm_enabled
         self.is_nsfw: bool = is_nsfw
 
         self.included: typing.Dict[str, Includable] = {}
+        self.events: typing.List[Event] = []
+
+    def __call__(self, bot: GatewayBotAware, client: Client) -> Plugin:
+        self._bot = bot
+        self._client = client
+        for event in self.events:
+            bot.event_manager.listen(*event.event_types)(event.callback)
+        return self
 
     @property
-    def bot(self) -> BotT | None:
+    def bot(self) -> GatewayBotAware | None:
         return self._bot
 
-    @bot.setter
-    def bot(self, bot: BotT) -> None:
-        self._bot = bot
-
     @property
     def client(self) -> Client | None:
         return self._client
 
-    @client.setter
-    def client(self, client: Client) -> None:
-        self._client = client
-
     def include(self, includable: typing.Type[Includable]) -> None:
         if issubclass(includable, AppCommand):
             try:
                 instance: AppCommand = (
                     includable()  # type: ignore
                     .set_guild(self.guild)
                     .set_default_member_permissions(self.default_member_permissions)
                     .set_is_dm_enabled(self.is_dm_enabled)
                     .set_is_nsfw(self.is_nsfw)
                 )
             except ValueError:
                 raise AurumException("`__init__` of base includable wasn't overrided")
             self.included[instance.name] = instance
+
+    def listen(self, *event_types: typing.Type[EventT]) -> Callable[[CallbackT[EventT]], None]:
+        def decorator(callback: CallbackT[EventT]) -> None:
+            self.events.append(Event(event_types=event_types, callback=callback))
+
+        return decorator
```

### Comparing `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_integration.py` & `aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin_integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.5.6/aurum/ext/plugins/plugin_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import importlib.util
+import re
 import typing
 from logging import getLogger
 from pathlib import Path
 
 from aurum.ext.plugins.plugin import Plugin
 from aurum.internal.commands.app_command import AppCommand
 from aurum.internal.commands.command_handler import CommandHandler
@@ -12,47 +13,43 @@
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
     from importlib.machinery import ModuleSpec
     from logging import Logger
     from os import PathLike
     from types import ModuleType
 
+    from hikari.traits import GatewayBotAware
+
     from aurum.client import Client
-    from aurum.types import BotT
 
 
 class PluginManager:
     """Plugin manager.
 
     Attributes:
-        bot (BotT): The bot instance.
-        client (Client): The client.
-        commands (CommandHandler): The command handler.
         plugins (Dict[str, Plugin]): A dictionary of loaded plugins, keyed by their names.
     """
 
-    __slots__: Sequence[str] = ("__logger", "bot", "client", "commands", "plugins")
+    __slots__: Sequence[str] = ("__logger", "_bot", "_client", "_commands", "plugins")
 
-    def __init__(self, bot: BotT, client: Client) -> None:
+    def __init__(self, bot: GatewayBotAware, client: Client) -> None:
         self.__logger: Logger = getLogger("aurum.plugins")
 
-        self.bot: BotT = bot
-        self.client: Client = client
-
-        self.commands: CommandHandler = client.commands
+        self._bot: GatewayBotAware = bot
+        self._client: Client = client
+        self._commands: CommandHandler = client.commands
 
         self.plugins: typing.Dict[str, Plugin] = {}
 
     def load_plugin_from_file(self, file: PathLike[str]) -> Plugin | None:
         """Load plugin from file
 
         File must have a `plugin` variable
         """
-        if not isinstance(file, Path):
-            file = Path(file)
+        file = Path(file) if not isinstance(file, Path) else file
         if not file.is_file():
             return None
         module_name: str = file.stem
         spec: ModuleSpec | None = importlib.util.spec_from_file_location(module_name, file)
         if not spec:
             self.__logger.error("count not load module %s from %s.", module_name, file)
             return None
@@ -63,35 +60,33 @@
                     "cannot execute module %s from spec, because spec don't have loader.",
                     module_name,
                 )
                 return None
             spec.loader.exec_module(module)
             plugin: Plugin | None = getattr(module, "plugin", None)
             if isinstance(plugin, Plugin):
-                plugin.bot = self.bot
-                plugin.client = self.client
-                return plugin
+                return plugin(self._bot, self._client)
             self.__logger.error(
-                "variable `plugin` in %s is not an instance of Plugin class or not detected.",
+                "plugin in %s is not not detected.",
                 file,
             )
         except Exception as exception:
             self.__logger.error(
                 "couldn't load module %s due error", module_name, exc_info=exception
             )
             return None
         return None
 
     async def load_folder(self, directory: PathLike[str]) -> None:
         """Load plugins from folder"""
         loaded: typing.List[Plugin] = []
         for file in Path(directory).rglob("*.py"):
+            if re.compile("(^_.*|.*_$)").match(file.name):
+                continue
             plugin: Plugin | None = self.load_plugin_from_file(file)
             if not plugin:
                 return
-            plugin.bot = self.bot
-            plugin.client = self.client
             for includable in plugin.included.values():
                 if isinstance(includable, AppCommand):
-                    self.commands.commands[includable.name] = includable
+                    self._commands.commands[includable.name] = includable
             loaded.append(plugin)
         self.__logger.debug("loaded %s", ", ".join([plugin.name for plugin in loaded]))
```

### Comparing `aurum_hikari-0.1.5.5/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.5.6/aurum/interactions/interaction_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from hikari.messages import MessageFlag
 from hikari.snowflakes import Snowflake
 from hikari.undefined import UNDEFINED
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
+    from hikari.traits import GatewayBotAware
     from hikari.api import ComponentBuilder
     from hikari.channels import PartialChannel
     from hikari.embeds import Embed
     from hikari.files import Resourceish
     from hikari.guilds import GatewayGuild, PartialRole
     from hikari.interactions import (
         CommandInteraction,
@@ -25,31 +26,30 @@
     )
     from hikari.messages import Message
     from hikari.snowflakes import SnowflakeishSequence
     from hikari.undefined import UndefinedOr
     from hikari.users import PartialUser
 
     from aurum.client import Client
-    from aurum.types import BotT
 
 
 @dataclass(slots=True, kw_only=True)
 class InteractionContext:
     """Represents a interaction context.
 
     Attributes:
         interaction (CommandInteraction | ComponentInteraction): The interaction.
-        bot (BotT): The instance of the bot.
+        bot (GatewayBotAware): The instance of the bot.
         client (Client): The client.
         locale (typing.Any): An any locale object for the interaction.
     """
 
     interaction: CommandInteraction | ComponentInteraction
 
-    bot: BotT
+    bot: GatewayBotAware
     client: Client
 
     locale: typing.Any
 
     @property
     def user(self) -> PartialUser | None:
         """User of the interaction"""
```

### Comparing `aurum_hikari-0.1.5.5/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.5.6/aurum/internal/commands/app_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import typing
 
 from hikari.permissions import Permissions
 from hikari.undefined import UNDEFINED
 
-from aurum.includable import Includable
+from aurum.internal.includable import Includable
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
     from hikari.commands import CommandType, PartialCommand
     from hikari.guilds import PartialGuild
     from hikari.snowflakes import SnowflakeishOr
@@ -33,15 +33,14 @@
         dm_enabled (bool): Whether the command can be used in direct messages.
         is_nsfw (bool): Indicates whether the command is age-restricted.
     """
 
     __slots__: Sequence[str] = (
         "app",
         "name",
-        "display_name",
         "guild",
         "default_member_permissions",
         "is_dm_enabled",
         "is_nsfw",
         "description",
         "command_type",
     )
```

### Comparing `aurum_hikari-0.1.5.5/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.5.6/aurum/internal/commands/command_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from __future__ import annotations
 
-import contextlib
 import importlib.util
 import inspect
 import re
 import typing
 from logging import getLogger
 from pathlib import Path
 
-from hikari.undefined import UNDEFINED
-
 from aurum.commands import MessageCommand, SlashCommand, UserCommand
 from aurum.internal.commands.context_menu_command import ContextMenuCommand
 from aurum.internal.exceptions.base_exception import AurumException
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
     from importlib.machinery import ModuleSpec
     from logging import Logger
     from os import PathLike
 
     from hikari.api import CommandBuilder
     from hikari.commands import PartialCommand
     from hikari.guilds import PartialApplication, PartialGuild
-    from hikari.impl import GatewayBot
-    from hikari.snowflakes import SnowflakeishOr
+    from hikari.snowflakes import Snowflake, SnowflakeishOr
+    from hikari.traits import GatewayBotAware
     from hikari.undefined import UndefinedType
 
     from aurum.internal.commands.app_command import AppCommand
     from aurum.l10n import LocalizationProviderInterface
 
 CommandsTypes = MessageCommand, SlashCommand, UserCommand
 
@@ -36,36 +33,40 @@
 class CommandHandler:
     """Handles command building and synchronization for a bot application.
 
     This class is responsible for application commands.
     It registers commands, synchronizes them with the Discord API.
 
     Attributes:
-        commands (typing.Dict[str, AppCommand]): Dictionary that stores the actual AppCommand instances, keyed by their names.
+        commands (typing.Dict[str, AppCommand]): Dictionary that stores the AppCommand instances, keyed by their names.
+        app_commands (typing.Dict[Snowflake, AppCommand]): Dictionary that stores AppCommand instances, keyed by their application ID
     """
 
     __slots__: Sequence[str] = (
         "__logger",
         "_app",
         "_bot",
         "_l10n",
         "_commands_builders",
         "commands",
+        "app_commands",
     )
 
-    def __init__(self, bot: GatewayBot, l10n: LocalizationProviderInterface) -> None:
+    def __init__(self, bot: GatewayBotAware, l10n: LocalizationProviderInterface) -> None:
         self.__logger: Logger = getLogger("aurum.commands")
         self._app: PartialApplication | None = None
-        self._bot: GatewayBot = bot
+        self._bot: GatewayBotAware = bot
         self._l10n: LocalizationProviderInterface = l10n
+
         self._commands_builders: typing.Dict[
             SnowflakeishOr[PartialGuild] | UndefinedType, typing.Dict[str, CommandBuilder]
         ] = {}
 
         self.commands: typing.Dict[str, AppCommand] = {}
+        self.app_commands: typing.Dict[Snowflake, AppCommand] = {}
 
     async def sync(self, debug: bool = False) -> None:
         """Synchronizes the builders of commands with the Discord API for the bot application.
 
         This method will handle both global commands and guild-specific commands,
         ensuring they are up-to-date with the currently stored command builders.
 
@@ -75,44 +76,46 @@
             build: A boolean flag to enable a automatic building of commands.
         """
         if not self._app:
             self._app = await self._bot.rest.fetch_application()
         synchronized: typing.Dict[
             SnowflakeishOr[PartialGuild] | UndefinedType, Sequence[PartialCommand]
         ] = {}
-        for name, command in self.commands.items():
+        for command in self.commands.values():
             self._commands_builders.setdefault(command.guild, {})
-            if isinstance(command, SlashCommand):
-                self._commands_builders[command.guild][name] = command.get_builder(
-                    self._bot.rest.slash_command_builder,
-                    self._l10n,
-                )
-            elif isinstance(command, ContextMenuCommand):
-                self._commands_builders[command.guild][name] = command.get_builder(
-                    self._bot.rest.context_menu_command_builder,
-                    self._l10n,
-                )
-        with contextlib.suppress(KeyError):
-            synchronized[UNDEFINED] = await self._bot.rest.set_application_commands(
-                self._app, list(self._commands_builders.pop(UNDEFINED).values())
-            )
-        for guild, commands_builders in self._commands_builders.items():
+            if builder := self.get_command_builder(command):
+                self._commands_builders[command.guild][command.name] = builder
+        for guild, builders in self._commands_builders.items():
             synchronized[guild] = await self._bot.rest.set_application_commands(
-                self._app, list(commands_builders.values()), guild=guild
+                self._app, list(builders.values()), guild=guild
             )
         for entity, commands in synchronized.items():
             for partial_command in commands:
-                self.commands[command.name].set_app(partial_command)
+                self.commands[partial_command.name].set_app(partial_command)
+                self.app_commands[partial_command.id] = self.commands[partial_command.name]
             if debug:
                 self.__logger.debug(
                     "Set commands for %s: %s",
                     entity,
                     ", ".join(command.name for command in commands),
                 )
 
+    def get_command_builder(self, command: AppCommand) -> CommandBuilder | None:
+        if isinstance(command, SlashCommand):
+            return command.get_builder(
+                self._bot.rest.slash_command_builder,
+                self._l10n,
+            )
+        elif isinstance(command, ContextMenuCommand):
+            return command.get_builder(
+                self._bot.rest.context_menu_command_builder,
+                self._l10n,
+            )
+        return None
+
     def load_commands_from_file(self, file: Path) -> Sequence[AppCommand]:
         commands: typing.List[AppCommand] = []
         spec: ModuleSpec | None = importlib.util.spec_from_file_location(file.name, file)
         if not spec:
             raise
         if not spec.loader:
             raise
```

### Comparing `aurum_hikari-0.1.5.5/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.5.6/aurum/internal/commands/context_menu_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     from hikari.undefined import UndefinedType
 
     from aurum.l10n import LocalizationProviderInterface
 
 
 class ContextMenuCommand(AppCommand):
     __slots__: Sequence[str] = (
-        "_app",
+        "app",
         "command_type",
         "name",
-        "display_name",
         "guild",
         "default_member_permissions",
         "dm_enabled",
         "is_nsfw",
     )
 
     def __init__(
```

### Comparing `aurum_hikari-0.1.5.5/aurum/internal/utils/commands.py` & `aurum_hikari-0.1.5.6/aurum/internal/utils/commands.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.5.6/aurum/l10n/localization_provider_interface.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.5/aurum/options/option.py` & `aurum_hikari-0.1.5.6/aurum/options/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class Option:
     """Represents the command option."""
 
     type: OptionType
     """The option type"""
     name: str  # TODO: make a display_name soon
     """The unique name of the option"""
-    description: LocalizedOr[str]
+    description: LocalizedOr[str] | None = None
     """The description of the option"""
     is_required: bool = True
     """An optional flag is the option is required.
     
     Default: True"""
     choices: Sequence[Choice] = field(default_factory=tuple[Choice])
     """A list of choices to the option"""
```

### Comparing `aurum_hikari-0.1.5.5/pyproject.toml` & `aurum_hikari-0.1.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "v0.1.5.5"
+version = "v0.1.5.6"
 name = "aurum-hikari"
 authors = ["stefanlight8 <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible framework for handling commands and components with integrations."
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `aurum_hikari-0.1.5.5/PKG-INFO` & `aurum_hikari-0.1.5.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6175 7275  : 2.1.Name: auru
 00000020: 6d2d 6869 6b61 7269 0a56 6572 7369 6f6e  m-hikari.Version
-00000030: 3a20 302e 312e 352e 350a 5375 6d6d 6172  : 0.1.5.5.Summar
+00000030: 3a20 302e 312e 352e 360a 5375 6d6d 6172  : 0.1.5.6.Summar
 00000040: 793a 2041 2066 6c65 7869 626c 6520 6672  y: A flexible fr
 00000050: 616d 6577 6f72 6b20 666f 7220 6861 6e64  amework for hand
 00000060: 6c69 6e67 2063 6f6d 6d61 6e64 7320 616e  ling commands an
 00000070: 6420 636f 6d70 6f6e 656e 7473 2077 6974  d components wit
 00000080: 6820 696e 7465 6772 6174 696f 6e73 2e0a  h integrations..
 00000090: 4c69 6365 6e73 653a 204d 4954 0a4b 6579  License: MIT.Key
 000000a0: 776f 7264 733a 2064 6973 636f 7264 2c68  words: discord,h
@@ -239,67 +239,37 @@
 00000ee0: 6f72 2077 696e 646f 7773 0a23 2059 6f75  or windows.# You
 00000ef0: 2063 616e 2075 7365 2074 6865 202d 5520   can use the -U 
 00000f00: 666c 6167 2077 6974 6820 7468 6520 6069  flag with the `i
 00000f10: 6e73 7461 6c6c 6020 636f 6d6d 616e 6420  nstall` command 
 00000f20: 2865 2e67 2e2c 2060 7069 7020 696e 7374  (e.g., `pip inst
 00000f30: 616c 6c20 2d55 202e 2e2e 6029 2074 6f20  all -U ...`) to 
 00000f40: 7570 6461 7465 2061 2070 6163 6b61 6765  update a package
-00000f50: 2e0a 6060 600a 0a23 2055 7361 6765 0a60  ..```..# Usage.`
-00000f60: 6060 7079 0a66 726f 6d20 6869 6b61 7269  ``py.from hikari
-00000f70: 2069 6d70 6f72 7420 4761 7465 7761 7942   import GatewayB
-00000f80: 6f74 0a0a 6672 6f6d 2061 7572 756d 2069  ot..from aurum i
-00000f90: 6d70 6f72 7420 436c 6965 6e74 2c20 536c  mport Client, Sl
-00000fa0: 6173 6843 6f6d 6d61 6e64 2c20 6361 6c6c  ashCommand, call
-00000fb0: 6261 636b 0a0a 626f 7420 3d20 4761 7465  back..bot = Gate
-00000fc0: 7761 7942 6f74 2822 2e2e 2e22 290a 636c  wayBot("...").cl
-00000fd0: 6965 6e74 203d 2043 6c69 656e 7428 626f  ient = Client(bo
-00000fe0: 7429 0a0a 0a40 636c 6965 6e74 2e69 6e63  t)...@client.inc
-00000ff0: 6c75 6465 0a63 6c61 7373 2048 656c 6c6f  lude.class Hello
-00001000: 436f 6d6d 616e 6428 536c 6173 6843 6f6d  Command(SlashCom
-00001010: 6d61 6e64 293a 0a20 2020 2064 6566 205f  mand):.    def _
-00001020: 5f69 6e69 745f 5f28 7365 6c66 2920 2d3e  _init__(self) ->
-00001030: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-00001040: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00001050: 6e61 6d65 3d22 6865 6c6c 6f22 2c20 6465  name="hello", de
-00001060: 7363 7269 7074 696f 6e3d 2253 6179 2068  scription="Say h
-00001070: 6920 746f 2062 6f74 2229 0a0a 2020 2020  i to bot")..    
-00001080: 6173 796e 6320 6465 6620 6361 6c6c 6261  async def callba
-00001090: 636b 2873 656c 662c 2063 6f6e 7465 7874  ck(self, context
-000010a0: 3a20 496e 7465 7261 6374 696f 6e43 6f6e  : InteractionCon
-000010b0: 7465 7874 2920 2d3e 204e 6f6e 653a 0a20  text) -> None:. 
-000010c0: 2020 2020 2020 2061 7761 6974 2063 6f6e         await con
-000010d0: 7465 7874 2e63 7265 6174 655f 7265 7370  text.create_resp
-000010e0: 6f6e 7365 2866 2248 692c 207b 636f 6e74  onse(f"Hi, {cont
-000010f0: 6578 742e 7573 6572 2e6d 656e 7469 6f6e  ext.user.mention
-00001100: 7d21 2229 0a0a 0a69 6620 5f5f 6e61 6d65  }!")...if __name
-00001110: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00001120: 3a0a 2020 2020 636c 6965 6e74 2e72 756e  :.    client.run
-00001130: 2829 0a60 6060 0a4d 6f72 6520 696e 205b  ().```.More in [
-00001140: 6578 616d 706c 6573 2066 6f6c 6465 725d  examples folder]
-00001150: 282e 2f65 7861 6d70 6c65 7329 2e0a 0a23  (./examples)...#
-00001160: 2050 726f 6a65 6374 730a 536f 2066 6172   Projects.So far
-00001170: 2c20 6e6f 206f 6e65 2068 6173 2062 6565  , no one has bee
-00001180: 6e20 7573 696e 6720 6f75 7220 6c69 6272  n using our libr
-00001190: 6172 792e 0a0a 2320 436f 6e74 7269 6275  ary...# Contribu
-000011a0: 7469 6e67 0a4e 6f74 2061 7661 696c 6162  ting.Not availab
-000011b0: 6c65 2079 6574 2e0a 0a23 2049 7373 7565  le yet...# Issue
-000011c0: 7320 616e 6420 6275 6773 0a49 6620 796f  s and bugs.If yo
-000011d0: 7520 6669 6e64 2061 6e79 2065 7272 6f72  u find any error
-000011e0: 7320 696e 2074 6865 206c 6962 7261 7279  s in the library
-000011f0: 2c20 706c 6561 7365 206c 6574 2075 7320  , please let us 
-00001200: 6b6e 6f77 2061 626f 7574 2074 6865 6d20  know about them 
-00001210: 6f6e 2074 6865 205b 6973 7375 6573 2047  on the [issues G
-00001220: 6974 6875 6220 7061 6765 5d28 6874 7470  ithub page](http
-00001230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
-00001240: 6869 6e73 6869 4465 7673 2f61 7572 756d  hinshiDevs/aurum
-00001250: 2d68 696b 6172 692f 6973 7375 6573 292e  -hikari/issues).
-00001260: 2054 6861 6e6b 7321 0a0a 2320 496e 7370   Thanks!..# Insp
-00001270: 6972 6174 696f 6e0a 2d20 5b68 696b 6172  iration.- [hikar
-00001280: 692d 6372 6573 6365 6e74 5d28 6874 7470  i-crescent](http
-00001290: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-000012a0: 696b 6172 692d 6372 6573 6365 6e74 2f68  ikari-crescent/h
-000012b0: 696b 6172 692d 6372 6573 6365 6e74 2920  ikari-crescent) 
-000012c0: 2d20 4120 636f 6d6d 616e 6420 6861 6e64  - A command hand
-000012d0: 6c65 7220 666f 7220 4869 6b61 7269 2074  ler for Hikari t
-000012e0: 6861 7420 6b65 6570 7320 796f 7572 2070  hat keeps your p
-000012f0: 726f 6a65 6374 206e 6561 7420 616e 6420  roject neat and 
-00001300: 7469 6479 2e0a 0a                        tidy...
+00000f50: 2e0a 6060 600a 0a23 2055 7361 6765 0a56  ..```..# Usage.V
+00000f60: 6965 7720 696e 205b 6578 616d 706c 6573  iew in [examples
+00000f70: 2066 6f6c 6465 725d 282e 2f65 7861 6d70   folder](./examp
+00000f80: 6c65 7329 2e0a 0a23 2050 726f 6a65 6374  les)...# Project
+00000f90: 730a 536f 2066 6172 2c20 6e6f 206f 6e65  s.So far, no one
+00000fa0: 2068 6173 2062 6565 6e20 7573 696e 6720   has been using 
+00000fb0: 6f75 7220 6c69 6272 6172 792e 0a0a 2320  our library...# 
+00000fc0: 436f 6e74 7269 6275 7469 6e67 0a4e 6f74  Contributing.Not
+00000fd0: 2061 7661 696c 6162 6c65 2079 6574 2e0a   available yet..
+00000fe0: 0a23 2049 7373 7565 7320 616e 6420 6275  .# Issues and bu
+00000ff0: 6773 0a49 6620 796f 7520 6669 6e64 2061  gs.If you find a
+00001000: 6e79 2065 7272 6f72 7320 696e 2074 6865  ny errors in the
+00001010: 206c 6962 7261 7279 2c20 706c 6561 7365   library, please
+00001020: 206c 6574 2075 7320 6b6e 6f77 2061 626f   let us know abo
+00001030: 7574 2074 6865 6d20 6f6e 2074 6865 205b  ut them on the [
+00001040: 6973 7375 6573 2047 6974 6875 6220 7061  issues Github pa
+00001050: 6765 5d28 6874 7470 733a 2f2f 6769 7468  ge](https://gith
+00001060: 7562 2e63 6f6d 2f53 6869 6e73 6869 4465  ub.com/ShinshiDe
+00001070: 7673 2f61 7572 756d 2d68 696b 6172 692f  vs/aurum-hikari/
+00001080: 6973 7375 6573 292e 2054 6861 6e6b 7321  issues). Thanks!
+00001090: 0a0a 2320 496e 7370 6972 6174 696f 6e0a  ..# Inspiration.
+000010a0: 2d20 5b68 696b 6172 692d 6372 6573 6365  - [hikari-cresce
+000010b0: 6e74 5d28 6874 7470 733a 2f2f 6769 7468  nt](https://gith
+000010c0: 7562 2e63 6f6d 2f68 696b 6172 692d 6372  ub.com/hikari-cr
+000010d0: 6573 6365 6e74 2f68 696b 6172 692d 6372  escent/hikari-cr
+000010e0: 6573 6365 6e74 2920 2d20 4120 636f 6d6d  escent) - A comm
+000010f0: 616e 6420 6861 6e64 6c65 7220 666f 7220  and handler for 
+00001100: 4869 6b61 7269 2074 6861 7420 6b65 6570  Hikari that keep
+00001110: 7320 796f 7572 2070 726f 6a65 6374 206e  s your project n
+00001120: 6561 7420 616e 6420 7469 6479 2e0a 0a    eat and tidy...
```

