# Mongo guardian 🛡️

- 💾 Creates a mongo dump periodically.
- 👴 Deletes N oldest dumps.
- 📦 Can be limited by size


# API

```js

require("mongoguardian")({
	cron: "0 3 * * *", // every night at 3 am
	folder: "./mongodumps",
	maxFolderSizeMb: 1024 * 2, // 2 Gb
	maxDumps: 10,
});

```