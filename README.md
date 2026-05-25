# FRITZ!Box Calllist Card

[![HACS](https://github.com/RF1705/fritzbox-calllist-card/actions/workflows/hacs.yml/badge.svg)](https://github.com/RF1705/fritzbox-calllist-card/actions/workflows/hacs.yml)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-rf1705-ffdd00?logo=buy-me-a-coffee&logoColor=000000)](https://buymeacoffee.com/rf1705)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A Lovelace card for the [FRITZ!Box Calllist](https://github.com/RF1705/fritzbox-calllist) Home Assistant integration.

It shows live calls, call duration and the persistent call history created by the integration.

## Installation

1. Add this repository to HACS as a custom repository:

   ```text
   https://github.com/RF1705/fritzbox-calllist-card
   ```

2. Select the `Lovelace` category.
3. Install `FRITZ!Box Calllist Card`.
4. Reload Home Assistant in your browser.

HACS should add the Lovelace resource automatically. If needed, add it manually:

```text
/hacsfiles/fritzbox-calllist-card/fritzbox-calllist-card.js
```

Resource type: `JavaScript module`.

## Card Configuration

```yaml
type: custom:fritzbox-calllist-card
entity: sensor.fritzbox_calllist
title: Phone
max_items: 4
font_size: 14
language: auto
```

The card includes a visual Lovelace editor for:

- entity
- title
- number of visible entries
- font size
- language (`auto`, `de`, `en`)

## Options

| Option | Type | Default | Description |
| --- | --- | --- | --- |
| `entity` | string | `sensor.fritzbox_calllist` | FRITZ!Box Calllist sensor entity |
| `title` | string | localized | Card title |
| `max_items` | number | `4` | Visible history entries |
| `font_size` | number | `14` | Main text size in pixels |
| `language` | string | `auto` | `auto`, `de` or `en` |

## Support

If you find this card useful, you can support the project here:

[buymeacoffee.com/rf1705](https://buymeacoffee.com/rf1705)

## License

This project is licensed under the MIT License.
