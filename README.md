# LiteXpansion 工业

LiteXpansion 是一个 Slimefun4 的附属插件，继承了来自 SlimeXpansion 的所有物品与部分功能。开发者正努力让此附属能提供类似工业2(IC2)模组的体验。

## :world_map: 目录

* [下载](#floppy_disk-下载)
* [内容](#内容)
  * [物品](#card_index_dividers-物品)
  * [机器](#electric_plug-机器)
  * [工具](#hammer_and_wrench-工具)
  * [武器](#crossed_swords-武器)
  * [护甲](#shield-护甲)
  * [UU物质](#brain-uu物质)
* [Discord](#computer-discord)

## :floppy_disk: 下载

点击这里下载 LiteXpansion: [下载 LiteXpansion](https://builds.guizhanss.net/ybw0014/LiteXpansion-CN/master)

**重要: 你必须安装 Slimefun 才能使用 LiteXpansion. 如果你还没有安装 Slimefun，请前往这里下载: [Slimefun 汉化版](https://github.com/StarWishsama/Slimefun4/releases)**

<p align="center">
  <a href="https://github.com/ybw0014/LiteXpansion-CN/actions/workflows/maven.yml">
    <img src="https://github.com/ybw0014/LiteXpansion-CN/actions/workflows/maven.yml/badge.svg" alt="Java CI"/>
  </a>

  <a href="https://builds.guizhanss.net/ybw0014/LiteXpansion-CN/master">
    <img src="https://builds.guizhanss.net/f/ybw0014/LiteXpansion-CN/master/badge.svg" alt="Build status"/>
  </a>
</p>

## 内容

### :card_index_dividers: 物品

- 食物合成器 - 用合成的食物填饱你的肚子;
- 镁钍合金 - 坚如磐石的合金;
- 钍 - 一种放射性极强的合金;
- 镁钍合金粉 - ; (制作中，暂无任何用途)
- 钍粉 - ; (制作中，暂无任何用途)
- 废料 - 回收任何物品而来，用于制造UU物质;
- UU物质 - 用于合成任意物品;
- 铱 - 由UU物质合成而来; (制作中，暂无任何用途)
- 铱板 - ; (制作中，暂无任何用途)
- 精炼铁 - 用于制造其他物品/机器;
- 机器方块 - 用于制造机器;

### :electric_plug: 机器
- 回收机 - 回收任何物品来获得废料;
- 物质生成机 - 将废料转换为UU物质, "只需要亿点点电";

### :hammer_and_wrench: 工具
- 扳手 - 可以快速破坏机器; (制作中，暂无任何用途)

### :crossed_swords: 武器
- 纳米剑 - 一把高科技的光剑，可以轻松斩断对手;

### :shield: 护甲
- 电动护甲 - 可以抵消任何对玩家造成的伤害;

### :brain: UU物质

UU物质是一种难以制造的资源，可以在物质生成机中由废料转化而来。你可以使用UU物质制造任何物品，例如草方块、玻璃、铜锭等。

服务器管理员可以修改、添加或删除UU物质的合成配方。

#### :gear: 配置

如需添加、删除或修改配方，你需要修改 `/plugins/LiteXpansion/uumatter.yml` 文件。

在 `recipes` 下，你可以指定输出的物品，这可以是 [原版物品ID](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) 或是 Slimefun 物品ID (支持附属插件)。如果你想让输出的物品数量多于1，你可以在物品ID后面加上一个英文的冒号(`:`)与数量。在接下来的合成表中，`x`代表UU物质，空格为无物品。

以下是一个合成20个煤炭的例子:

```yaml
recipes:
  # 输出的物品, 使用冒号 (:) 来指定数量
  # 可使用原版物品ID (https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Material.html) 或 Slimefun 物品ID
  'COAL:20':
    # 合成表, x = UU物质, 空格 = 无物品
    - '  x'
    - 'x  '
    - '  x'
```

在 `/plugins/LiteXpansion/config.yml` 文件中，可以修改两个配置项：

- `auto-update` - 启用后会开启自动更新 (默认: `true`)
- `nerf-other-addons` - 启用后会削弱充能太阳能板，无尽科技中的所有发电机，战争工艺的元素发电机，以及星际中的聚变反应堆，禁用则会使本附属插件中机器电力消耗翻倍 (默认: `true`)

### :computer: Discord

如果你想找到一个 Slimefun 物品的ID，你可以通过下方的图片链接加入我们的官方 Slimefun Discord 服务器，并在`#bot-spam`频道中发送`!item <name/ID>`即可获取。

你也可以在`#litexpansion`频道中讨论任何有关 LiteXpansion 的内容。

[加入Slimefun 官方Discord服务器](https://discord.gg/slimefun)
