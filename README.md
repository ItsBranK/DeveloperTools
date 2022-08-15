# ItsBranK's Developer Tools

A collection of features and tools free to use for developers and organizations (BakkesMod Plugin).

All information exported/dumped from this plugin can be found in the `bakkesmod\data\DeveloperTools` directory in either json, csv, or plain text format.

# Settings

### > brank_browsetextures
**Possible Arguments:** 0 or 1, for false or true.

**Description:** This setting is used to control whether you want to display the texture browser feature.

### > brank_thumbnailscale
**Possible Arguments:** -1 to the maximum resolution your screen can display, for example; `256 256` will render thumbnails at 256x256 resolution.

**Description:** The resolution scale to use when drawing product thumbnails, setting to -1 disables scaling.

### > brank_disable_replays
**Possible Arguments:** 0 or 1, for false or true.

**Description:** When set to true, this will disable the advertisements around the stadium when viewing replays; this will only work for replay files and not any other offline or online mode.

# Commands

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
