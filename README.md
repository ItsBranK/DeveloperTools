# ItsBranK's Developer Tools

A collection of features and tools free to use for developers and organizations (BakkesMod Plugin).

All information exported/dumped from this plugin can be found in the `bakkesmod\data\DeveloperTools` directory in either json, csv, or plain text format.

# Table of Contents

<!-- TOC -->

- [Settings](#settings)
    - [brank_browsetextures](https://github.com/ItsBranK/DeveloperTools#-brank_browsetexturest)
    - [brank_thumbnailscale](https://github.com/ItsBranK/DeveloperTools#-brank_thumbnailscale)
    - [brank_disable_replays](https://github.com/ItsBranK/DeveloperTools#-brank_disable_replays)
- [Texture Commands](https://github.com/ItsBranK/DeveloperTools#texture-commands)
    - [brank_drawtexture](https://github.com/ItsBranK/DeveloperTools#-brank_drawtexture)
    - [brank_drawthumbnail](https://github.com/ItsBranK/DeveloperTools#-brank_drawthumbnail)
    - [brank_erasetexture](https://github.com/ItsBranK/DeveloperTools#-brank_erasetexture)
    - [brank_browsetextures](https://github.com/ItsBranK/DeveloperTools#-brank_browsetextures-1)
    - [brank_exportthumbnail](https://github.com/ItsBranK/DeveloperTools#-brank_exportthumbnail)
    - [brank_exporttexture](https://github.com/ItsBranK/DeveloperTools#-brank_exporttexture)
- [Dump/ExportCommands](https://github.com/ItsBranK/DeveloperTools#dumpexport-commands)
    - [brank_dump_functions](https://github.com/ItsBranK/DeveloperTools#-brank_dump_functions)
    - [brank_dump_textures](https://github.com/ItsBranK/DeveloperTools#-brank_dump_textures)
    - [brank_dump_errors](https://github.com/ItsBranK/DeveloperTools#-brank_dump_errors)
    - [brank_dump_slots](https://github.com/ItsBranK/DeveloperTools#-brank_dump_slots)
    - [brank_dump_products](https://github.com/ItsBranK/DeveloperTools#-brank_dump_products)
    - [brank_dump_inventory](https://github.com/ItsBranK/DeveloperTools#-brank_dump_inventory)
    - [brank_dump_paints](https://github.com/ItsBranK/DeveloperTools#-brank_dump_paints)
    - [brank_dump_certifications](https://github.com/ItsBranK/DeveloperTools#-brank_dump_certifications)
    - [brank_dump_specialeditions](https://github.com/ItsBranK/DeveloperTools#-brank_dump_specialeditions)
    - [brank_dump_titles](https://github.com/ItsBranK/DeveloperTools#-brank_dump_titles)
    - [brank_dump_teameditions](https://github.com/ItsBranK/DeveloperTools#-brank_dump_teameditions)
    - [brank_dump_playlists](https://github.com/ItsBranK/DeveloperTools#-brank_dump_playlists)
    - [brank_dump_maps](https://github.com/ItsBranK/DeveloperTools#-brank_dump_maps)
    - [brank_dump_esports](https://github.com/ItsBranK/DeveloperTools#-brank_dump_esports)
    - [brank_dump_population](https://github.com/ItsBranK/DeveloperTools#-brank_dump_population)
    - [brank_dump_tournaments](https://github.com/ItsBranK/DeveloperTools#-brank_dump_tournaments)
<!-- /TOC -->

# Settings

### > brank_browsetextures
**Possible Arguments:** 0 or 1, for false or true.

**Description:** This setting is used to control whether you want to display the texture browser feature. Please see [here](https://github.com/ItsBranK/DeveloperTools#-brank_browsetextures-1) on how to use the texture browser.

### > brank_thumbnailscale
**Possible Arguments:** -1 to the maximum resolution your screen can display, for example; `256 256` will render thumbnails at 256x256 resolution.

**Description:** The resolution scale to use when drawing product thumbnails, setting to -1 disables scaling.

### > brank_disable_replays
**Possible Arguments:** 0 or 1, for false or true.

**Description:** When set to true, this will disable the advertisements around the stadium when viewing replays; this will only work for replay files and not any other offline or online mode.

# Texture Commands

### > brank_drawtexture

This command draws a texture to the screen based on its name.

**Example Usage:**

`brank_drawtexture Noise_Fire`

**Example Output:**

![](https://i.imgur.com/f0FZKSW.png/)

### > brank_drawthumbnail

This command draws a product thumbnail to the screen based on its product id.

**Example Usage:**

`brank_drawthumbnail 32`

**Example Output:**

![](https://i.imgur.com/y2i4r7k.png/)

### > brank_erasetexture

This command stops/erases any texture on the screen that is currently being drawn by the commands [brank_drawtexture](https://github.com/ItsBranK/DeveloperTools/blob/main/README.md#-brank_drawtexture) and [brank_drawthumbnail.](https://github.com/ItsBranK/DeveloperTools#-brank_drawthumbnail)

**Example Usage:**

`brank_erasetexture`

### > brank_browsetextures

This command allows you to browse all textures currently loaded in the scene, you can use either the scroll wheel or the arrow keys to browse through them all.

**Example Usage:**

`brank_browsetextures 1`

**Example Output:**

![](https://i.imgur.com/bLl7vxp.png)

### > brank_exportthumbnail

This is an experimental command and may not work as intended!

This command attempts to export a products thumbnail texture to a dds file.

**Example Usage:**

`brank_exportthumbnail 32`

### > brank_exporttexture

This is an experimental command and may not work as intended!

This command attempts to export a texture to a dds file by its name, it takes the same arguments as the [brank_drawtexture](https://github.com/ItsBranK/DeveloperTools/blob/main/README.md#-brank_drawtexture) command.

**Example Usage:**

`brank_exporttexture Engine`

# Dump/Export Commands

### > brank_dump_functions

This command does not take any arguments.

**Example Usage:**

`brank_dump_functions`

**Example Output:**

```
Function Core.Object.RSmoothInterpTo
Function Core.Object.VSmoothInterpTo
Function Core.Object.GetSmoothInterpLerpValue
Function Core.Object.FSmoothInterpTo
Function Core.Object.VLerp
...continued
```

### > brank_dump_textures

This command does not take any arguments.

**Example Usage:**

`brank_dump_textures`

**Example Output:**

```
Texture2D EngineResources.WhiteSquareTexture
Texture2D EngineResources.DefaultTexture
TextureCube EngineResources.DefaultTextureCube
Texture2D EngineMaterials.DefaultNormal
Texture2D EngineMaterials.DefaultDiffuse
...continued
```

### > brank_dump_errors

This command does not take any arguments.

**Example Usage:**

`brank_dump_errors`

**Example Output:**

```
AccountNotFound
ServerNotFound
ExpiredDsConnectToken
MatchmakingNoInternet
PartyRankDisparity
...continued
```

### > brank_dump_slots

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#product-slots)

**Example Usage:**

`brank_dump_slots slot_online_label slot_description slot_index [JSON]`

**Example Output:**

```json
{
	"Slot Online Label": "Body",
	"Slot Description": "Completely change your vehicle's style with a new body!",
	"Slot Index": 0
}
```

### > brank_dump_products

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#offline-products)

**Example Usage:**

`brank_dump_products product_id product_long_label product_quality_label product_bool_paintable product_trade_restrictions [JSON]`

**Example Output:**

```json
{
	"Product Id": 1300,
	"Product Long Label": "Octane: RLCS",
	"Product Quality Label": "Limited",
	"Product Paintable": false,
	"Product Trade Restrictions": [ "TradeIn" ]
}
```

### > brank_dump_inventory

A full list of arguments for this command can be found [here](brank_dump_inventory), this command also accepts the same arguments as the [brank_dump_products ](https://github.com/ItsBranK/DeveloperTools/blob/main/README.md#-brank_dump_products) command.

**Example Usage:**

`brank_dump_inventory product_id product_long_label online_instance_id online_added_timestamp online_trade_hold [JSON]`

**Example Output:**

```json
{
	"Product Id": 1300,
	"Product Long Label": "Octane: RLCS",
	"Online Instance Id": "2033203160",
	"Online Added Timestamp": "1509241699",
	"Online Trade Hold": "P2P"
}
```

### > brank_dump_paints

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_paints database_paint_id database_paint_label database_paint_name database_paint_colors [JSON]`

**Example Output:**

```json
{
	"Paint Database Id": 1,
	"Paint Database Label": "Crimson",
	"Paint Database Name": "Red_00",
	"Paint Database Colors": [ "#990000", "#FF0B0B", "#720000", "#FF0000" ]
}
```

### > brank_dump_certifications

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_certifications database_certified_id database_certified_label database_certified_description [JSON]`

**Example Output:**

```json
{
	"Certified Database Id": 1,
	"Certified Database Label": "Aviator",
	"Certified Database Description": "When equipped in an online match, this item keeps track of how many aerial goals you score."
}
```

### > brank_dump_specialeditions

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_specialeditions database_special_id database_special_label database_special_name [JSON]`

**Example Output:**

```json
{
	"Special Database Id": 1,
	"Special Database Label": "Holographic",
	"Special Database Name": "Edition_Holographic"
}
```

### > brank_dump_titles

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_titles database_title_id database_title_text database_title_color database_title_glowcolor [JSON]`

**Example Output:**

```json
{
	"Title Database Id": "S15_SuperSonic_Legend",
	"Title Database Text": "S1 Supersonic Legend",
	"Title Database Color": "#E8E8E8",
	"Title Database Glow": "#E8E8E8"
}
```

### > brank_dump_teameditions

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_teameditions database_team_id database_team_label database_team_name [JSON]`

**Example Output:**

```json
{
	"Team Database Id": 26,
	"Team Database Label": "NRG Esports",
	"Team Database Name": "NRG_Season8"
}
```

### > brank_dump_series

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#internal-database)

**Example Usage:**

`brank_dump_series database_series_id database_series_label [JSON]`

**Example Output:**

```json
{
	"Database Series Id": 8,
	"Database Series Label": "Player's Choice"
}
```

### > brank_dump_playlists

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#matchmaking-playlists)

**Example Usage:**

`brank_dump_playlists playlist_id playlist_title playlist_description playlist_player_count [JSON]`

**Example Output:**

```json
{
	"Playlist Id": 3,
	"Playlist Title": "Standard",
	"Playlist Description": "Ranked play with a team",
	"Playlist Player Count": 6
}
```

### > brank_dump_maps

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#stadium-maps)

**Example Usage:**

`brank_dump_maps map_base_name map_file_name map_variant_name map_random_weight [JSON]`

**Example Output:**

```json
{
	"Map Base Name": "DFH Stadium",
	"Map File Name": "stadium_day_p",
	"Map Variant Name": "Day",
	"Map Random Weight": 1.300000
}
```

### > brank_dump_esports

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#esports-events)

**Example Usage:**

`brank_dump_esports esports_title esports_description esports_epoch_start_time esports_epoch_end_time esports_url [JSON]`

**Example Output:**

```json
{
	"Esports Title": "FT",
	"Esports Description": "FT Show",
	"Esports Epoch Start Time": "1634064600",
	"Esports Epoch End Time": "1634070600",
	"Esports Url": "https://www.twitch.tv/rocketleague"
}
```

### > brank_dump_population

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#player-populations)

**Example Usage:**

`brank_dump_population [JSON]`

**Example Output:**

```json
{
	"Population Total Players": 309815,
	"Population Playlist Id": 1,
	"Population Playlist Players": 4702
}
```

### > brank_dump_tournaments

A full list of arguments for this command can be found [here.](https://github.com/ItsBranK/DeveloperTools/blob/main/ARGUMENTS.md#auto-tournaments)

**Example Usage:**

`brank_dump_tournaments tournament_id tournament_title tournament_epoch_start_time tournament_region_label [JSON]`

**Example Output:**

```json
{
	"Tournament Id": "24610827",
	"Tournament Title": "2v2 Hoops",
	"Tournament Epoch Start Time": "1660248000",
	"Tournament Region Label": "USE"
}
```
