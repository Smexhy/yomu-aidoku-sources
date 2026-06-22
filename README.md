<div align="center">

# 📚 Yomu

### Manga, manhwa, and manhua for the [Aidoku](https://aidoku.app) app

![Platform](https://img.shields.io/badge/iOS%20%2F%20iPadOS-Aidoku%200.8.3%2B-ff3b69?style=for-the-badge)

<br>

<a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/index.min.json">
  <img alt="Add Yomu to Aidoku" src="assets/add-to-aidoku.svg" width="300">
</a>

<br><br>

On iPhone or iPad, tap the button and Aidoku adds the list for you.

To add it by hand, open Aidoku, go to **Settings → Source Lists**, and paste:

`https://smexhy.github.io/yomu-aidoku-sources/index.min.json`

</div>

---

Yomu is my own small source list for Aidoku. I built these sources for my own reading and put them here so other people can use them too if they want. It is not connected to the official Aidoku community list and it is not trying to replace it. I just keep my own versions and update them when I find the time.

Comix, MangaDot and Atsumaru read in English. Kagane, Mangaball and OniSaga carry several chapter languages, English by default, which you pick inside each source's settings.

> [!NOTE]
> Comix is also in the community list, and mine shares the same source id with a deliberately high version number (**100+**). So if you already read Comix from there, adding Yomu keeps your existing library and just swaps in my build, and you won't lose any saved series or progress.

## What's inside

Prefer a single source over the whole list? Each one below has a one-tap **Add to Aidoku** button that installs just that source and keeps auto-updates, or a **Download .aix** link to import the package by hand (importing by hand does not auto-update).

<h3><img src="assets/icons/comix.png" width="24" align="top">&nbsp; Comix &nbsp;<sub><a href="https://comix.to">comix.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/comix/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.comix-v110.aix">Download .aix (v110)</a></sub>

Manga and webtoons from comix.to. The home has a Most Recent Popular row up top, then Latest Updates (Hot), Most Followed New Comics, and Recently Added. Search is keyword based, and the genre and tag chips on a series are tappable, while author and artist are available as filters rather than tappable chips. Filters cover author, artist, type, demographic, status, and a long genre list with AND/OR matching, plus the usual sorts. In settings you can set cover quality, merge duplicate chapters, and hide types, demographics, genres or themes; adult content is off by default. Each chapter is tagged with its source, and official releases like Tappytoon get a check so they stand out from scanlations.

The interesting bit is hidden underneath. Comix locks its API behind an obfuscated signing module that it rotates often, and serves its page images with the tiles scrambled. Yomu pulls the current module, signs every request with it, decodes the responses, and lets comix's own renderer work out how each page's tiles are scrambled, then puts them back in order so chapters just open like normal.

> [!IMPORTANT]
> **Duplicate chapters work differently here, and the first update runs a one time step**
>
> Comix often has the same chapter uploaded more than once: a fan release, then an official one, a more complete version, and so on. The usual Comix build, the one in the community list, ties your read history to whichever single upload it currently treats as the best. The catch is that this pick can change later. When a newer or official upload shows up, a chapter you already read pops back into your updates and shows as unread, as if it were new.
>
> Yomu's Comix ties your read history to the chapter number instead, so a chapter you read stays read no matter which upload wins later. That is the main difference between this build and the community one. If you would rather keep the old behavior, just use the Comix source from the community list instead of this one.
>
> Because the two builds identify chapters in different ways, the first time you update to this version Aidoku runs a one time migration to carry your existing read history across. The migration does its work whenever **Deduplicate Chapters** is on, and this build turns that setting on by default. So on a large library the first update can take a few minutes and may show only a loading spinner with no progress bar, which is normal, so give it time to finish. If you turn the setting off, the update is instant and nothing is fetched. Either way your read progress is kept.

<h3><img src="assets/icons/kagane.png" width="24" align="top">&nbsp; Kagane &nbsp;<sub><a href="https://kagane.to">kagane.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/kagane/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.kagane-v7.aix">Download .aix (v7)</a></sub>

Multi language manhwa, manga and manhua from kagane.to (mostly manhwa), nine chapter languages with English as the default (set in Aidoku's language picker). Popular, latest and newly added on the home, plus listings for popular today through all time. Filters for format, status, content rating and source type, plus a setting for the time window the Popular row uses. In settings you can also hide formats, genres, and certain content tags; adult content is off by default. Each chapter shows its real upload source, like Tapas or Omega Scans, with a check on the official ones so you can tell licensed releases from scanlations at a glance, and an optional setting can add that source to the title too.

Reading a chapter needs a signed token that the site only hands out for a short while, so Yomu grabs one and reuses it for about five minutes. The first chapter of a session does the full handshake and everything after that opens from a single request.

<h3><img src="assets/icons/mangaball.png" width="24" align="top">&nbsp; Mangaball &nbsp;<sub><a href="https://mangaball.net">mangaball.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangaball/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.mangaball-v6.aix">Download .aix (v6)</a></sub>

Multi language manga, manhwa and manhua from mangaball.net, twelve chapter languages with English by default. The home has Featured, Latest, Recommended and Popular This Season, with search, tappable tag and author chips, and filters for original language, demographic, status and tags.

The site is session based, so Yomu does a quick handshake before loading anything. If you paste a title that has curly quotes or an apostrophe, it straightens them to the plain ones the site's search expects, so the search still finds it. It also collapses duplicate chapter uploads down to the best one.

<h3><img src="assets/icons/mangadot.png" width="24" align="top">&nbsp; MangaDot &nbsp;<sub><a href="https://mangadot.net">mangadot.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangadot/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.mangadot-v8.aix">Download .aix (v8)</a></sub>

Manga, manhwa and manhua from mangadot.net. The home has Most Viewed, Latest Updates, Top Rated and Most Tracked, with title search and filters for type, status and genre. The genre, author and artist chips on a series are tappable, so a tap jumps straight to matching titles.

Its nicest trick is the chapter dedupe. It keeps the best upload of each chapter and spots official releases even when the site does not flag them, by recognizing platforms like TappyToon, Tapas and WEBTOON by name. Each chapter is tagged with its source, and the official ones get a check so they stand out from scanlations.

<h3><img src="assets/icons/atsumaru.png" width="24" align="top">&nbsp; Atsumaru &nbsp;<sub><a href="https://atsu.moe">atsu.moe</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/atsumaru/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.atsumaru-v5.aix">Download .aix (v5)</a></sub>

Manga, manhwa and manhua from atsu.moe. The home has Trending, Popular, Top Rated, Recently Updated, Recently Added and Most Bookmarked, with fast search, tappable tag and author chips, and filters for type, status, rating and genre.

Its search runs on a Typesense backend, and an author tap uses the site's dedicated author endpoint instead of a fuzzy text search, so it is more accurate. It also pulls the series details and chapter list together so a title opens a bit quicker.

<h3><img src="assets/icons/onisaga.png" width="24" align="top">&nbsp; OniSaga &nbsp;<sub><a href="https://onisaga.com">onisaga.com</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/onisaga/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.onisaga-v4.aix">Download .aix (v4)</a></sub>

Multi language manga, manhwa and manhua from onisaga.com, eighteen chapter languages with English by default (set in Aidoku's language picker). The home leads with an auto scrolling Most Popular slider, then Latest Mangas, Top Rated and Fan Favorites. Search is title based, the genre and author chips on a series are tappable, and filters cover type, status, minimum rating, sort, and a full genre list you can include or exclude. In settings you can hide genres and merge duplicate chapter uploads; adult content is off by default.

The site runs on Livewire behind Cloudflare, so Yomu talks to it the same way the page does and rides Aidoku's Cloudflare handling. Chapters come either as a single version or as a multi language dropdown and it reads both, pages load one at a time through the site's signed page API, and duplicate uploads of the same chapter collapse down to the best one.

## ⚠️ If a source gets stuck loading

> [!WARNING]
> Most of these sites sit behind Cloudflare. The first time you open one in a session (a cold load), Cloudflare's check can add several seconds before covers and titles appear. That is normal, so give it a moment instead of backing out.
>
> A Cloudflare source can also occasionally get fully **stuck**, hanging on a spinner or showing a **verification window that never finishes**. If that happens, clear that source's cache and restart the app:
>
> 1. Open the **Browse** tab and tap the source.
> 2. Tap the **three dots** at the top right, then **Settings**.
> 3. Scroll to the bottom and tap **Clear Cache**.
> 4. **Force close Aidoku** (swipe it away in the app switcher), then open it again.
>
> That clears the stale Cloudflare cookie and it loads again. It's an Aidoku app quirk with Cloudflare for now, not something the source itself can fix.

## Updates

Pull to refresh your source lists in Aidoku to pick up new versions. I update these when the sites change or something breaks, in my free time, so there is no schedule. Everything here is built and tested against the latest Aidoku app and SDK.

> [!NOTE]
> The latest **MangaDot**, **Mangaball** and **OniSaga** update changes how duplicate chapter uploads are identified, so a chapter you already read no longer reappears as a new unread one when a different upload becomes the top pick. Because of that change, the first time you update those three, your read progress on them may show as unread once. Nothing is deleted, and it stays put afterward.

## Using this list

These are my own packages, shared so you can read with them in Aidoku. Add the list and enjoy it. Please do not rehost, repackage, or republish the packages or this list somewhere else as your own. See [LICENSE](LICENSE) for the details.

The packages are compiled from Rust and include the open source Aidoku SDK and other libraries; their notices are in [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

Not affiliated with Aidoku or any of the sites listed here. All names and logos belong to their owners.
