<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ff3b69,100:7c5cff&height=180&section=header&text=%E3%82%88%E3%82%80%20Yomu&fontSize=62&fontColor=ffffff&fontAlignY=36&desc=Manga,%20manhwa%20and%20manhua%20for%20Aidoku&descSize=18&descAlignY=58" alt="Yomu: Manga, manhwa and manhua sources for Aidoku" width="100%">

<img alt="Platform: iOS / iPadOS, Aidoku 0.8.3+" src="https://img.shields.io/badge/iOS%20%2F%20iPadOS-Aidoku%200.8.3%2B-ff3b69?style=for-the-badge">
<img alt="Sources: 7" src="https://img.shields.io/badge/sources-7-7c5cff?style=for-the-badge">

<img src="assets/spacer.png" width="100%" height="28" alt="">

<a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/index.min.json">
  <img alt="Add Yomu to Aidoku" src="https://smexhy.github.io/yomu-aidoku-sources/assets/add-to-aidoku.svg?v=4" width="300">
</a>

<img src="assets/spacer.png" width="100%" height="28" alt="">

Tap the button on iPhone or iPad and Aidoku adds the list. To add it by hand, open <strong>Settings → Source Lists</strong> and paste:

<code>https://smexhy.github.io/yomu-aidoku-sources/index.min.json</code>

</div>

---

## What this is

[Aidoku](https://aidoku.app) is a free, open-source manga reader for iOS and iPadOS. Yomu is my own source list for it: seven sources I build and maintain for my own reading, kept public so anyone can use them. It is not the official Aidoku community list and is not trying to replace it. I update them when a site changes or something breaks.

## The seven sources

| | Source | Reads | Good for |
|---|---|---|---|
| <img src="assets/icons/comix.png" width="20"> | **Comix** <sub>[comix.to](https://comix.to)</sub> | English | Ten filter fields and a four-level content rating |
| <img src="assets/icons/kagane.png" width="20"> | **Kagane** <sub>[kagane.to](https://kagane.to)</sub> | 60+ languages | Mostly manhwa, with per-upload source badges |
| <img src="assets/icons/mangaball.png" width="20"> | **Mangaball** <sub>[mangaball.net](https://mangaball.net)</sub> | 50+ languages | Wide language coverage |
| <img src="assets/icons/mangadot.png" width="20"> | **MangaDotNet** <sub>[mangadot.net](https://mangadot.net)</sub> | English + others | One translation group per series, start to finish |
| <img src="assets/icons/atsumaru.png" width="20"> | **Atsumaru** <sub>[atsu.moe](https://atsu.moe)</sub> | English | The quickest to load, with public data and direct images |
| <img src="assets/icons/onisaga.png" width="20"> | **OniSaga** <sub>[onisaga.com](https://onisaga.com)</sub> | 18 languages | Chinese, Korean and Japanese chapters |
| <img src="assets/icons/madaradex.png" width="20"> | **MadaraDex** <sub>[madaradex.org](https://madaradex.org)</sub> | English | Adult manhwa &nbsp;<strong>18+</strong> |

Multi-language sources default to English; pick yours in each source's settings.

> ⚠️ **MadaraDex is an adult source.** Every title on it is 18+. It is marked as adult in the list, so Aidoku filters it with your other content settings and it may stay hidden until you allow adult sources.

## What they all do

- **Filters that stay current.** Genre and tag lists come from the site itself, so they never go stale between source updates.
- **Hide what you don't want.** Genres, and on most sources tags, types, formats or demographics. Hidden entries vanish from home, listings and search, not just the filter sheet. Adult content is off by default.
- **One upload per chapter.** Where a site carries duplicates, you get one. Read history follows the chapter, not the upload, so nothing re-marks itself unread when a site reshuffles.
- **Covers first.** Requests are batched and cached, and covers load before anything else.
- **Tappable chips.** Genre chips on a series page open matching titles, and on most sources author and tag chips too. Paste a link and the right page opens.

<sub>MadaraDex is the exception on hiding: it is a single-language adult source with no settings of its own, so there is no mixed content to filter.</sub>

## Install one at a time

Each source below has an **Add to Aidoku** button that installs only that one and keeps auto-updates. Prefer to import by hand? Every package lives in [`sources/`](https://github.com/Smexhy/yomu-aidoku-sources/tree/main/sources), though a hand import will not auto-update.

<h3><img src="assets/icons/comix.png" width="24" align="top">&nbsp; Comix</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/comix/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://comix.to">comix.to</a> &nbsp;·&nbsp; <strong>needs Aidoku 0.8.4+</strong></sub>

English manga and webtoons. Home has Most Recent Popular, Latest Updates, Most Followed New Comics and Recently Added, plus Trending Webtoon and Trending Manga ranked by views over three months.

- **Filters.** Genres, demographic, format, type, status, content rating, release year, minimum chapters, author, artist and sort. Genres and formats include or exclude, with AND or OR matching.
- **Content rating.** Safe, Suggestive, Erotica and Pornographic, applied across home, listings and search. Defaults to Safe and Suggestive.
- **Content hiding.** Any type, demographic, genre, format or tag, plus Custom Hidden Tags for anything not in the list.
- **Chapter selection.** Official uploads first, then a preferred scanlation group carried across the series, with gaps filled from the next best. Or pick the best upload per chapter instead.
- **Scrambled pages, handled.** Comix signs its API with a module it rotates often and ships page images with the tiles shuffled. Yomu keeps up and chapters open normally.

<details>
<summary><strong>More about Comix</strong></summary>

<p><strong>Blocked requests.</strong> On some devices Cloudflare refuses Aidoku's normal requests even after you pass its check, leaving the source unable to load. Yomu notices, routes through a web view instead, and returns to normal once the block lifts. <code>Settings &gt; Connection</code> can pin either mode.</p>

<p><strong>Comix's own captcha.</strong> Comix sometimes gates the whole site, including the data Yomu reads. Aidoku cannot show that check by itself, so <code>Settings &gt; Access &gt; Verify Captcha</code> opens it. A solve lasts about half an hour and the button re-arms when it runs out. If that friction is too much, the other sources are unaffected.</p>

<p><strong>Bad page images.</strong> When the server returns corrupt data that would show blank, Yomu refetches a clean copy.</p>

<p><strong>Tidy chapter names.</strong> Upload names that only repeat the chapter number are hidden; real titles stay.</p>

<p><strong>Chapter sources.</strong> Each chapter shows its real source, with a check on licensed platforms like Tappytoon.</p>

<p><strong>Already reading Comix elsewhere?</strong> This build shares the same source id with a high version number, so adding Yomu keeps your library and swaps the build in. Nothing saved is lost. <strong>Show One Upload Per Chapter</strong> is on by default, and the first update runs a one-time migration to carry your history across; on a large library that first open can sit on a spinner for a few minutes, which is normal. Turn the setting off to see every upload.</p>

</details>

<h3><img src="assets/icons/kagane.png" width="24" align="top">&nbsp; Kagane</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/kagane/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 60+ languages &nbsp;·&nbsp; <a href="https://kagane.to">kagane.to</a></sub>

Manhwa, manga and manhua, mostly manhwa. Home has Popular, Recently Added and Recently Updated.

- **Filters.** Genres, tags, demographic, type, status, content rating, original language, source type, release year, author and sort. Genres and tags include or exclude, with AND or OR matching.
- **Content hiding.** Formats, genres, curated tag categories, or any tag by name under Custom Hidden Tags.
- **Upload sources.** Every chapter shows where it came from, like Tapas or Omega Scans, with a check on official ones. Show all uploads, official only, or scanlations only.
- **Spoiler tags.** Genres and tags Kagane marks as spoilers stay hidden unless you ask for them.
- **Over sixty languages.** Korean, Japanese, Chinese, French, German, Spanish and more.

<details>
<summary><strong>More about Kagane</strong></summary>

<p><strong>Content rating.</strong> Safe, Suggestive, Erotica and Pornographic, applied across home, listings and search.</p>

<p><strong>Popular time span.</strong> Today, this week, this month or all time.</p>

<p><strong>Blocked requests.</strong> As with Comix, if Cloudflare refuses Aidoku's normal requests, Yomu routes through a web view and switches back on its own. <code>Settings &gt; Connection</code> can pin either mode.</p>

<p><strong>Getting into the reader.</strong> Kagane needs a short-lived token before it serves chapters. Yomu does that once and reuses it for about five minutes, so only the first chapter of a session waits.</p>

<p><strong>If a chapter goes black or the app closes partway through:</strong> a few series use very large page images and the reader can run out of memory. Turn on <strong>Downsample Images</strong> in Aidoku's reader settings. That is an Aidoku setting, not something a source controls.</p>

<p><strong>Downloaded chapters.</strong> An older Aidoku bug dropped some downloaded pages, fixed in <strong>0.8.4</strong>. Reading online was never affected. (<a href="https://github.com/Aidoku/Aidoku/issues/1008">Aidoku#1008</a>)</p>

</details>

<h3><img src="assets/icons/mangaball.png" width="24" align="top">&nbsp; Mangaball</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangaball/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 50+ languages &nbsp;·&nbsp; <a href="https://mangaball.net">mangaball.net</a></sub>

Manga, manhwa and manhua. Home has Featured, Latest Updates, Recommended and Most Popular.

- **Filters.** Genres and tags as separate include or exclude lists sharing one AND or OR match, plus demographic, status, type, author and sort.
- **Content hiding.** Types, genres or tags. Adult content is off by default.
- **Over fifty languages.** Spanish, Portuguese, Indonesian, Vietnamese, French and more.
- **Deduplication.** On by default: official first, then most likes, then most views, then newest.

<details>
<summary><strong>More about Mangaball</strong></summary>

<p><strong>Session first.</strong> Mangaball only answers inside a live session, so Yomu picks up a session and token before it can search or load, refreshing them as they expire every couple of minutes. That handshake is why it warms up a moment slower than the plain-API sources.</p>

</details>

<h3><img src="assets/icons/mangadot.png" width="24" align="top">&nbsp; MangaDotNet</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangadot/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English + others &nbsp;·&nbsp; <a href="https://mangadot.net">mangadot.net</a></sub>

Manga, manhwa and manhua, mostly English. Home has Most Viewed, Latest Updates, Top Rated and Most Tracked.

- **One group, start to finish.** Deduplication keeps a whole series with a single translation group, so names and phrasing stay consistent as you read. Official releases come first. Among fan groups it picks whichever covers the most of the series and fills gaps from the next best, in stretches rather than single-chapter jumps.
- **Official badge.** MangaDotNet has no official marker of its own, so Yomu honors its Official group label and also recognizes licensed platforms and publishers by name, from WEBTOON and Tapas to Viz, Kodansha and DLsite.
- **Filters.** Genres and tags as tap-to-include, tap-again-to-exclude chips, plus type, status, author, artist and sort.
- **Content hiding.** Genres, tags or types, and adult content on or off.
- **Your languages.** The same chapter can exist in several; pick yours and each keeps its own consistent group.

<details>
<summary><strong>More about MangaDotNet</strong></summary>

<p><strong>Tidy chapter names.</strong> Upload names that only repeat the chapter number are hidden, so a chapter reads as a clean number instead of doubling up. Real titles are kept.</p>

<p><strong>Straight from the API.</strong> MangaDotNet serves clean data, so listings, chapters and pages are read directly, with no scraping and no page-by-page unlocking.</p>

<p><strong>A setting brings back per-chapter picking</strong> if you prefer the older behaviour. Read history stays tied to the chapter either way.</p>

</details>

<h3><img src="assets/icons/atsumaru.png" width="24" align="top">&nbsp; Atsumaru</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/atsumaru/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://atsu.moe">atsu.moe</a></sub>

English manga, manhwa and manhua. Home has Trending, Recently Updated, Popular, Top Rated, Recently Added and Most Bookmarked.

- **Filters.** Genres, tags, demographic, type, status, content rating, release year, author and sort, with include or exclude and AND or OR matching.
- **Content hiding.** Types, genres or tags, and adult content on or off. You can still pick an adult rating for a single search.
- **Deduplication.** On by default. You choose whether merged chapters keep the newest upload or the one with the most pages.
- **Chapter groups.** Each chapter shows the group that uploaded it.
- **Nothing to wait for.** Atsumaru's data is public, so Yomu reads straight from the site and page images are direct links. That makes it the quickest here to warm up.

<h3><img src="assets/icons/onisaga.png" width="24" align="top">&nbsp; OniSaga</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/onisaga/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 18 languages &nbsp;·&nbsp; <a href="https://onisaga.com">onisaga.com</a></sub>

Manga, manhwa and manhua. Home opens with an auto-scrolling Most Popular slider, then Latest Mangas and Fan Favorites.

- **Filters.** Genres (include or exclude), type, status, release year, minimum rating, minimum chapters, author, scanlation group and sort.
- **Content hiding.** Genres, and adult content on or off. A genre you include in a search still shows even when it is on your hidden list.
- **Eighteen languages.** Including Simplified and Traditional Chinese, Korean and Japanese.
- **Deduplication.** One upload per language, newest or most pages, your choice.

<details>
<summary><strong>More about OniSaga</strong></summary>

<p><strong>Page-by-page unlocking.</strong> OniSaga hands out no direct image links. Each page is unlocked through the site's own reader with a rolling token, one at a time, the same way the site does it, so pages arrive as you reach them.</p>

</details>

<h3><img src="assets/icons/madaradex.png" width="24" align="top">&nbsp; MadaraDex &nbsp;<sub><strong>18+</strong></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/madaradex/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://madaradex.org">madaradex.org</a></sub>

<strong>Adults only.</strong> Every title here is adult manhwa, so unlike the rest of this list there is no safe-for-work side to it.

Home has New Manga and Latest Updates, plus five browse listings: Most Popular, Latest Updates, Trending, New Series and Top Rated.

- **Filters.** Sort by relevance, latest, A-Z, rating, trending, most views or newest, plus the site's full genre list and search by author or artist.
- **Tappable chips.** Genre, author and artist on a series page each open matching titles.
- **The next chapter is already waiting.** While you read, the following chapter loads in the background, so tapping through a series is close to instant.

<details>
<summary><strong>More about MadaraDex</strong></summary>

<p><strong>Pages that load at all.</strong> MadaraDex serves its page images only to a real browser and refuses an app asking for them directly, which is why a straightforward source for it does not work. Yomu opens each chapter through the site's own reader first so the images become available, then loads them normally. From your side it is just a chapter that opens.</p>

<p><strong>No settings of its own.</strong> It is single-language and entirely adult, so there is no mixed content to filter and nothing to configure.</p>

</details>

## If a source gets stuck loading

> ⚠️ Most of these sites sit behind Cloudflare. The first time you open one in a session, its check can add a few seconds before covers appear. That is normal.
>
> A Cloudflare source can also get fully **stuck** on a spinner or a verification window that never finishes. If that happens:
>
> 1. Open **Browse**, tap the source, then the **three dots → Settings**.
> 2. Scroll down and tap **Clear Cache**.
> 3. **Force close Aidoku** (swipe it away) and open it again.
>
> That drops the stale Cloudflare cookie and it loads again. It is an Aidoku and Cloudflare quirk, not something a source can fix on its own.

## Updates

Pull to refresh your source lists in Aidoku to pick up new versions. I update these when a site changes or something breaks, in my free time, so there is no schedule. Everything is built and tested against the current Aidoku app and SDK.

## License and use

These are my own packages, shared so you can read with them in Aidoku. Please do not rehost, repackage or republish the packages or this list as your own. See [LICENSE](LICENSE) for details.

The packages are compiled from Rust and include the open-source Aidoku SDK and other libraries; their notices are in [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

Not affiliated with Aidoku or any of the sites listed here. All names and logos belong to their owners.

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c5cff,100:ff3b69&height=90&section=footer" alt="" width="100%">
</div>
