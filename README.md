<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ff3b69,100:7c5cff&height=180&section=header&text=%E3%82%88%E3%82%80%20Yomu&fontSize=62&fontColor=ffffff&fontAlignY=36&desc=Manga,%20manhwa%20and%20manhua%20for%20Aidoku&descSize=18&descAlignY=58" alt="Yomu: Manga, manhwa and manhua sources for Aidoku" width="100%">

<img alt="Platform: iOS / iPadOS, Aidoku 0.8.3+" src="https://img.shields.io/badge/iOS%20%2F%20iPadOS-Aidoku%200.8.3%2B-ff3b69?style=for-the-badge">
<img alt="Sources: 6" src="https://img.shields.io/badge/sources-6-7c5cff?style=for-the-badge">

<img src="assets/spacer.png" width="100%" height="28" alt="">

<a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/index.min.json">
  <img alt="Add Yomu to Aidoku" src="https://smexhy.github.io/yomu-aidoku-sources/assets/add-to-aidoku.svg?v=4" width="300">
</a>

<img src="assets/spacer.png" width="100%" height="28" alt="">

On iPhone or iPad, tap the button and Aidoku adds the list for you. To add it by hand, open Aidoku, go to <strong>Settings → Source Lists</strong>, and paste:

<code>https://smexhy.github.io/yomu-aidoku-sources/index.min.json</code>

</div>

---

[Aidoku](https://aidoku.app) is a free, open-source manga reader for iOS and iPadOS. Yomu is my own source list for it: six sources I build and maintain for my own reading, kept here so anyone can use them too. It is not the official Aidoku community list and is not trying to replace it. I update them when the sites change or something breaks.

Comix, MangaDotNet and Atsumaru read in English. Kagane, Mangaball and OniSaga carry several chapter languages, English by default, set in each source's settings.

## What every source shares

These are common to every source here.

- **Dynamic filters.** The genre list in each source's filter sheet, and the tag list where a source has one, come straight from the site, so they stay complete and update on their own as the site changes, without waiting for a source update.
- **Content hiding.** Every source can hide genres in settings, and most can hide tags, types, formats or demographics too. Hidden entries disappear from the home page, listings and search, not only the filter sheet. Adult content is off by default.
- **Chapter deduplication.** Where a site serves duplicate uploads of a chapter, the source keeps one. Read history is tied to the chapter rather than the upload, so a chapter you read stays read and reordering does not trigger false new-chapter notifications.
- **Caching and batching.** Filter data is cached and, on most sources, kept across app launches. The app asks the site for several things at once, and covers load first.
- **Cloudflare handling.** The sites behind Cloudflare go through Aidoku's own Cloudflare check, with a clear message and a fix if a check gets stuck.
- **Chips and deep links.** Tap a genre chip on a series page to see matching titles; on most sources tag and author chips work the same way. Paste a chapter or series link and the right page opens.
- **Search.** The curly quotes iOS inserts are swapped for the plain ones each site's search expects, so a title with an apostrophe is found however you type it.

## Sources

Want just one instead of the whole list? Each source below has a one-tap **Add to Aidoku** button that installs only that source and keeps auto updates, or a **Download .aix** link to import the package by hand (a hand import does not auto update).

<h3><img src="assets/icons/comix.png" width="24" align="top">&nbsp; Comix &nbsp;<sub><a href="https://comix.to">comix.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/comix/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.comix-v119.aix">Download .aix (v119)</a></sub>

English manga and webtoons from comix.to. Home has Most Recent Popular, Latest Updates, Most Followed New Comics and Recently Added. Two more browse listings, Trending Webtoon and Trending Manga, rank titles by views over the last three months.

- **Scrambled pages.** Comix signs its API with an obfuscated module it rotates often, and serves page images with the tiles scrambled. Yomu fetches the current module, signs each request, and uses Comix's own renderer to put the tiles back, so chapters open normally.
- **Bad page images.** When the site's server returns a page with corrupt data that would otherwise show blank, Yomu detects it and refetches a clean copy so the page still loads.
- **Chapter sources.** Each chapter shows its real source, and licensed platforms like Tappytoon are marked with a check.
- **Consistent translation groups.** Unique to this build. Picking each chapter's most liked upload on its own kept switching translation groups mid series, changing character names and phrasing as you read. Deduplication now keeps your whole series with one group: official releases come first (staying with one official source even when a series has several), everything else comes from the group readers like most, and other groups fill only the chapters your group is missing. A series switches groups only when readers clearly prefer another one, and a setting brings back the old per chapter picking. Read history stays tied to the chapter number, so nothing you read is ever lost.
- **Tidy chapter names.** Upload names that only repeat the chapter number are hidden; real chapter titles stay.
- **Content rating.** A four-level setting (Safe, Suggestive, Erotica, Pornographic) decides what shows across home, listings and search. It defaults to Safe and Suggestive.
- **Filters.** Genres, demographic, format, type, status, content rating, release year, minimum chapters, author and artist, plus sort. Genres and formats can be included or excluded, with an AND or OR match.
- **Content hiding.** Hide any type, demographic, genre, format or tag, or type a name under Custom Hidden Tags to hide a tag that is not in the list.

> 💡 **Comix needs Aidoku 0.8.4 or newer.** The descrambler relies on the async page scripting the app added in 0.8.4, so on an older Aidoku the source will not load. Update the app if Comix stays blank. The other five sources run on Aidoku 0.8.3 and up.

<details>
<summary><strong>Already use Comix from the community list?</strong> (read before adding)</summary>

<p>Mine shares the same source id with a deliberately high version (<strong>100+</strong>), so adding Yomu keeps your existing library and just swaps in my build. You won't lose any saved series or progress.</p>

<p>The main difference is chapter handling. Unlike the community build, <strong>Deduplicate Chapters</strong> is on by default here and keeps one consistent translation group across your series. Comix keeps one upload per chapter out of the box, and read history is tied to the chapter number, so a chapter you read stays read no matter which upload wins a later deduplication pass. The first update runs a one-time migration to carry your existing history across while deduplication is on. On a large library that first open can sit on a plain spinner for a few minutes. That is normal.</p>

<p>Prefer the old behavior, with no deduplication? Just use the community Comix instead.</p>

</details>

<h3><img src="assets/icons/kagane.png" width="24" align="top">&nbsp; Kagane &nbsp;<sub><a href="https://kagane.to">kagane.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/kagane/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.kagane-v17.aix">Download .aix (v17)</a></sub>

Manhwa, manga and manhua from kagane.to, mostly manhwa, across more than sixty chapter languages with English by default. Home has Popular, Recently Added and Recently Updated.

- **Chapter sources.** Each chapter shows its real upload source, like Tapas or Omega Scans, with a check on official ones. An optional setting adds the source to the title, which helps tell duplicate titles apart.
- **Upload source setting.** Show all uploads, official only, or scanlations only, across home, listings and search. The per-search Source Type filter can override it.
- **Content rating.** A four-level setting (Safe, Suggestive, Erotica, Pornographic) decides what shows across home, listings and search.
- **Filters.** Genres, tags, demographic, type, status, content rating, original language, source type, release year, author and sort. Genres and tags can be included or excluded, with an AND or OR match.
- **Content hiding.** Hide formats, genres, or curated tag categories, or type a name under Custom Hidden Tags, like Love Triangle or Amnesia, to hide any tag.
- **Spoiler tags.** Genres and tags Kagane marks as spoilers are hidden by default, with a switch to show them.
- **Popular time span.** The Popular list can cover today, this week, this month or all time.
- **Over sixty languages.** Including Korean, Japanese, Chinese, French, German and Spanish. Set the chapter language in settings.
- **Getting into the reader.** Reading a chapter needs a short-lived access token from Kagane. Yomu does that handshake once when you start reading and reuses it for about five minutes, so only the first chapter of a session waits on it; the rest open right away.

> 💡 **If a chapter goes black or the app closes partway through:** a few Kagane series use very large page images, and on those the reader can run out of memory. Turn on **Downsample Images** in Aidoku's reader settings and it shrinks each page to fit your screen as it loads. This is an Aidoku setting, not something a source can do. The images really are that big.

> 💡 **Downloaded chapters now open correctly.** An earlier Aidoku bug silently dropped some of Kagane's downloaded page images, and a downloaded chapter could come up empty or skip pages. It is fixed in **Aidoku 0.8.4**, so update the app if you still see this. Reading online was never affected. ([Aidoku#1008](https://github.com/Aidoku/Aidoku/issues/1008))

<h3><img src="assets/icons/mangaball.png" width="24" align="top">&nbsp; Mangaball &nbsp;<sub><a href="https://mangaball.net">mangaball.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangaball/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.mangaball-v10.aix">Download .aix (v10)</a></sub>

Manga, manhwa and manhua from mangaball.net, across more than fifty chapter languages with English by default. Home has Featured, Latest Updates, Recommended and Most Popular.

- **Chapter deduplication.** On by default. It keeps one upload per chapter (official first, then most likes, then most views, then newest).
- **Filters.** Genres and tags as separate include or exclude lists, with one AND or OR match shared across the genres and tags you include, plus demographic, status, type, author and sort.
- **Content hiding.** Hide types, genres or tags. Adult content is off by default.
- **Over fifty languages.** Including Spanish, Portuguese, Indonesian, Vietnamese and French. Set the chapter language in settings.
- **Session first.** Mangaball only answers inside a live session, so Yomu opens a page to pick up the session and its token before it can search or load, and refreshes them as they expire after a couple of minutes. That handshake is why Mangaball takes a moment longer to warm up than the plain-API sources.

<h3><img src="assets/icons/mangadot.png" width="24" align="top">&nbsp; MangaDotNet &nbsp;<sub><a href="https://mangadot.net">mangadot.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangadot/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.mangadot-v15.aix">Download .aix (v15)</a></sub>

English manga, manhwa and manhua from mangadot.net. Home has Most Viewed, Latest Updates, Top Rated and Most Tracked.

- **Chapter deduplication and official badge.** Keeps one upload per chapter (official first, then English, then a trusted uploader, then the most complete), and recognizes licensed platforms like Tappytoon, Tapas and WEBTOON by name, marking them with a check even when the site does not flag them.
- **Filters.** Genres and tags as tap-to-include, tap-again-to-exclude chips, plus type, status, author, artist and sort.
- **Content hiding.** Hide genres, tags or types, and turn adult content on or off.
- **Straight from the API.** MangaDotNet serves a clean data API. Yomu reads listings, chapters and pages straight from it, with no page scraping and no page-by-page unlocking.

<h3><img src="assets/icons/atsumaru.png" width="24" align="top">&nbsp; Atsumaru &nbsp;<sub><a href="https://atsu.moe">atsu.moe</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/atsumaru/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.atsumaru-v9.aix">Download .aix (v9)</a></sub>

English manga, manhwa and manhua from atsu.moe. Home has Trending, Recently Updated, Popular, Top Rated, Recently Added and Most Bookmarked.

- **Chapter deduplication.** On by default. When duplicate chapters are merged, you choose which to keep, the newest upload or the one with the most pages.
- **Chapter groups.** Each chapter shows the translation group that uploaded it.
- **Filters.** Genres, tags, demographic, type, status, content rating, release year, author and sort, with genres and tags include or exclude and an AND or OR match.
- **Content hiding.** Hide types, genres or tags, and turn adult content on or off. You can still pick an adult rating for a single search when you want it.
- **Open API.** Atsumaru's data is public. Yomu reads it straight from the site, with no tokens or handshakes, and page images are plain direct links.

<h3><img src="assets/icons/onisaga.png" width="24" align="top">&nbsp; OniSaga &nbsp;<sub><a href="https://onisaga.com">onisaga.com</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/onisaga/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.onisaga-v9.aix">Download .aix (v9)</a></sub>

Manga, manhwa and manhua from onisaga.com, across eighteen chapter languages with English by default. Home has an auto-scrolling Most Popular slider, then Latest Mangas and Fan Favorites.

- **Chapter deduplication.** Keeps one upload per language, and you choose the newest or the one with the most pages.
- **Filters.** Genres (include or exclude), type, status, release year, minimum rating, minimum chapters, author, scanlation group and sort.
- **Content hiding.** Hide genres, and turn adult content on or off. A genre you include in a search still shows even if it is on your hidden list.
- **Eighteen languages.** Including Simplified and Traditional Chinese, Korean and Japanese. Set the chapter language in settings.
- **Page-by-page unlocking.** OniSaga doesn't hand out direct image links. Each page is unlocked through the site's own reader with a rolling token, one at a time, so pages load as you reach them, the same way the site does it.

## If a source gets stuck loading

> ⚠️ Most of these sites sit behind Cloudflare. The first time you open one in a session, its check can add a few seconds before covers appear. That is normal, give it a moment.
>
> A Cloudflare source can also occasionally get fully **stuck** on a spinner or a verification window that never finishes. If that happens:
>
> 1. Open **Browse**, tap the source, tap the **three dots → Settings**.
> 2. Scroll down and tap **Clear Cache**.
> 3. **Force close Aidoku** (swipe it away), then open it again.
>
> That drops the stale Cloudflare cookie and it loads again. It is an Aidoku and Cloudflare quirk for now, not something the source can fix on its own.

## Updates

Pull to refresh your source lists in Aidoku to pick up new versions. I update these when the sites change or something breaks, in my free time, so there is no schedule. Everything is built and tested against the latest Aidoku app and SDK.

## License and use

These are my own packages, shared so you can read with them in Aidoku. Please do not rehost, repackage or republish the packages or this list as your own. See [LICENSE](LICENSE) for the details.

The packages are compiled from Rust and include the open-source Aidoku SDK and other libraries; their notices are in [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

Not affiliated with Aidoku or any of the sites listed here. All names and logos belong to their owners.

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c5cff,100:ff3b69&height=90&section=footer" alt="" width="100%">
</div>
