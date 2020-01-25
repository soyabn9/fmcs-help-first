# Bedrock FAQ

## Can I create a bedrock server?

Yes, but the official bedrock server is not available on the server due to it being a exe and not a jar file. The only alternative to the bedrock is a nukkit server, as that is the only bedrock server that is supported by FMCS. The only downside is that, many of the latest bedrock things are not supported by nukkit.

## I'm having the server outdated error or the client outdated error?

If you are getting the server outdated error when joining a server, it means that the server is using a previous version and not supported by the latest client version.

If you are getting the client outdated error when joining a server, it means that the app is not updated to the current server version.

## What is the latest Nukkit Version that relates to the latest MCBE version?

Latest Nukkit version (588) which is MCBE version (1.14) is available on [freemcserver.net](https://freemcserver.net/).

## My nukkit server does not start?

If you are having troubles trying to start your nukkit server and it is your first time starting one, then there is a a choice of languages to choose from, before the server can start.

```text
2019-06-28 17:55:04.511 [main] INFO  - §aWelcome! Please choose a language first!
2019-06-28 17:55:04.516 [main] INFO  - eng => English
2019-06-28 17:55:04.516 [main] INFO  - chs => 中文（简体）
2019-06-28 17:55:04.516 [main] INFO  - cht => 中文（繁體）
2019-06-28 17:55:04.517 [main] INFO  - jpn => 日本語
2019-06-28 17:55:04.517 [main] INFO  - rus => Pyccĸий
2019-06-28 17:55:04.517 [main] INFO  - spa => Español
2019-06-28 17:55:04.517 [main] INFO  - pol => Polish
2019-06-28 17:55:04.517 [main] INFO  - bra => Português-Brasil
2019-06-28 17:55:04.517 [main] INFO  - kor => 한국어
2019-06-28 17:55:04.518 [main] INFO  - ukr => Українська
2019-06-28 17:55:04.518 [main] INFO  - deu => Deutsch
2019-06-28 17:55:04.518 [main] INFO  - ltu => Lietuviškai
2019-06-28 17:55:04.518 [main] INFO  - idn => Indonesia
2019-06-28 17:55:04.518 [main] INFO  - cze => Czech
2019-06-28 17:55:04.518 [main] INFO  - tur => Turkish
2019-06-28 17:55:04.519 [main] INFO  - fin => Suomi
```

Choose a language from above and type it in the console. Do **NOT** type English for English. To select the language type out the three letter character that represents the language so, for example, `eng` for English, `deu` for Deutsch or `spa` for Español.

Once the language has been typed and entered in to the console, the following lines will appear with a line at the end saying `Done (12.725s)! For help, type "help" or "?"`.

```text
2019-06-28 17:55:11.740 [main] INFO  - Loading §anukkit.yml§f ...
2019-06-28 17:55:11.857 [main] INFO  - Loading §aserver properties§f ...
2019-06-28 17:55:11.868 [main] INFO  - Selected English (eng) as the base language
2019-06-28 17:55:11.869 [main] INFO  - Starting Minecraft: BE server version §bv1.11.0§f
2019-06-28 17:55:11.877 [main] INFO  - Selected Zlib Provider: 2 (cn.nukkit.utils.ZlibThreadLocal)
2019-06-28 17:55:11.921 [main] INFO  - Opening server on 136.243.71.281:26865
2019-06-28 17:55:11.942 [main] INFO  - This server is running Nukkit version §egit-259923d§f "§b§f" (API 1.0.8)
2019-06-28 17:55:11.942 [main] INFO  - Nukkit is distributed under the LGPL License
2019-06-28 17:55:15.658 [main] INFO  - Loading recipes...
2019-06-28 17:55:16.474 [main] INFO  - Loaded 1393 recipes.
2019-06-28 17:55:16.476 [main] INFO  - Successfully loaded 0 resource packs
2019-06-28 17:55:16.671 [main] WARN  - Level "world" not found
2019-06-28 17:55:16.850 [main] INFO  - Preparing level "§aworld§f"
2019-06-28 17:55:17.091 [main] WARN  - Level "nether" not found
2019-06-28 17:55:17.091 [main] INFO  - No level called "nether" found, creating default nether level.
2019-06-28 17:55:17.104 [main] INFO  - Preparing level "§anether§f"
2019-06-28 17:55:17.105 [RakNet Thread #15] INFO  - Epoll is available. EpollEventLoop will be used.
2019-06-28 17:55:17.192 [main] INFO  - Starting GS4 status listener
2019-06-28 17:55:17.192 [main] INFO  - Setting query port to 26865
2019-06-28 17:55:17.193 [main] INFO  - Query is running on 136.243.71.281:26865
2019-06-28 17:55:17.193 [main] INFO  - Default game type: Survival Mode
2019-06-28 17:55:17.193 [main] INFO  - Done (12.725s)! For help, type "help" or "?"
```

> [!WARNING]
> **The IP and PORT in the log above is made up and might not exist!**
