# Change Log

## [Unreleased]

* Use current [NodeBB Settings Framework](https://nodebb.readthedocs.io/en/latest/plugins/settings.html).

## [1.1.0] \(2017-05-06\)

### Added

* Use category color as embed border color.

### Changed

* Switch to stable discord.js (^11.1.0).

* Switch to a single Webhook URL settings field (a workaround for [#1]).

    Since I could not find an example on how to update plugin configuration in DB, you have to purge old settings manually: `db.objects.remove({_key: "settings:discord-notification"});`


## [1.0.0] \(2017-04-14\)

Requires latest [discord.js](https://github.com/hydrabolt/discord.js/) from GitHub (discord.js v11.0.0, latest in NPM, doesn’t handle webhooks well enough).

[Unreleased]: https://github.com/amargon/city-of-doors/compare/v1.1.0...master
[1.1.0]: https://github.com/amargon/city-of-doors/releases/tag/v1.1.0
[1.0.0]: https://github.com/amargon/city-of-doors/releases/tag/v1.0.0


[#1]: https://github.com/amargon/nodebb-plugin-discord-notification/issues/1