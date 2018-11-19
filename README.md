# wow_hong_golang

这是一个为魔兽世界玩家制作的游戏工具，该工具提供给玩家一个分享游戏中宏命令的平台，也同时提供给玩家以搜索功能。
This is a game tool for World of Warcraft players that provides players with a platform to share macro commands in the game, as well as a search function.

# 功能
- 快速创建（fast create）

  - 提供给对游戏中宏命令感兴趣，却不懂的玩家，融合搜索和自动生成的功能，返回给玩家一个命令列表以供选择。
  - Players who are interested in the macro commands in the game but do not understand, combine the search and auto-generated functions, and return a list of commands to the player for selection.

- 手动组合（create by hand）

  - 提供给熟悉游戏的玩家，通过工具，手动组合出自己所需的命令。
  - Provided to players who are familiar with the game, through the tools, manually combine the commands they need.

- 分享及搜索（share and search）

  - 提供给玩家一个分享自己收集的宏命令的功能，同时也可以搜索其他玩家分享的宏命令。
  -Provides the player with the ability to share the macro commands they have collected, as well as the macro commands shared by other players.

# 优化
  由于服务器能力的问题，为了优化访问，所做的更改
1. 把部分数据写死在html中，以减少客户端访问次数，提高服务器处理能力。
2. bootstrap/vue.js/axios.min.js 等，采用官网cdn，加速访问速度。
3. 使用supervisor监控服务进程，自动管理，防止程序退出，无法访问。
