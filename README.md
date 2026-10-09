# cratedig
a better discogs front end

A fast, phone-friendly way to browse your own Discogs collection: a cover wall or list view, search, filters for genre, style, format and decade, and a quick way to check whether you already own a record while you're out digging.

It's a single static `index.html` with no build step and no server. Open the hosted page, enter your Discogs username and (optionally) a personal access token, and the app loads your collection straight from the Discogs API.

## Your token stays with you

This repo contains no credentials. Your username and token are saved only in the browser where you enter them and are sent only to `api.discogs.com` over HTTPS. Use **Sign out** in the app to remove them from a device. If you think a token has leaked, generate a new one under Settings › Developers on Discogs, which invalidates the old one.

A token is only needed if your collection is private, though it also raises the API rate limit.

## Freshness

To stay within the Discogs API Terms of Use, the app re-syncs automatically when its copy of your collection is more than six hours old. If you're offline, it shows your last saved copy with a notice until you're back online.

## Discogs

This app is an independent project built on the Discogs API. It is not affiliated with, sponsored by or endorsed by Discogs. Discogs is a trademark of Zink Media, LLC.

All release and collection data shown in the app is provided by [Discogs](https://www.discogs.com) and is subject to the [Discogs API Terms of Use](https://support.discogs.com/hc/en-us/articles/360009334593-API-Terms-of-Use). Nothing in this repository grants any rights to Discogs data.
