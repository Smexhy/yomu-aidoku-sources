<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:ff3b69,100:7c5cff&height=180&section=header&text=%E3%82%88%E3%82%80%20Yomu&fontSize=62&fontColor=ffffff&fontAlignY=36&desc=Manga,%20manhwa%20and%20manhua%20for%20Aidoku&descSize=18&descAlignY=58" alt="Yomu: Manga, manhwa and manhua sources for Aidoku" width="100%">

<img alt="Platform: iOS / iPadOS, Aidoku 0.8.3+" src="https://img.shields.io/badge/iOS%20%2F%20iPadOS-Aidoku%200.8.3%2B-ff3b69?style=for-the-badge">
<img alt="Sources: 12" src="https://img.shields.io/badge/sources-12-7c5cff?style=for-the-badge">

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

[Aidoku](https://aidoku.app) is a free, open-source manga reader for iOS and iPadOS. Yomu is my own source list for it: twelve sources I build and maintain for my own reading, kept public so anyone can use them. It is not the official Aidoku community list and is not trying to replace it. I update them when a site changes or something breaks.

## The twelve sources

| Source | Reads | Good for |
|---|---|---|
| <img src="assets/icons/comix.png" width="22" align="top"> **Comix** <sub>[comix.to](https://comix.to)</sub> | English | The biggest library here |
| <img src="assets/icons/kagane.png" width="22" align="top"> **Kagane** <sub>[kagane.moe](https://kagane.moe)</sub> | 60+ languages | Mostly manhwa, with per-upload source badges |
| <img src="assets/icons/mangaball.png" width="22" align="top"> **Mangaball** <sub>[mangaball.com](https://mangaball.com)</sub> | 50+ languages | Wide language coverage and detailed filters |
| <img src="assets/icons/mangadot.png" width="22" align="top"> **MangaDotNet** <sub>[mangadot.net](https://mangadot.net)</sub> | Mostly English | One translation group per series |
| <img src="assets/icons/atsumaru.png" width="22" align="top"> **Atsumaru** <sub>[atsu.moe](https://atsu.moe)</sub> | English | The quickest here to open |
| <img src="assets/icons/onisaga.png" width="22" align="top"> **OniSaga** <sub>[onisaga.com](https://onisaga.com)</sub> | 24 languages | Genre and theme filters, search by author or scanlation group |
| <img src="assets/icons/mangafire.png" width="22" align="top"> **MangaFire** <sub>[mangafire.to](https://mangafire.to)</sub> | 7 languages | One stable entry per chapter, official releases first |
| <img src="assets/icons/baetoon.png" width="22" align="top"> **BaeToon** <sub>[baetoon.com](https://baetoon.com)</sub> | English | Manhwa gathered from many scanlation sites, one entry per chapter |
| <img src="assets/icons/madaradex.png" width="22" align="top"> **MadaraDex** <img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"> <sub>[madaradex.org](https://madaradex.org)</sub> | English | Mostly adult manhwa, some safe for work |
| <img src="assets/icons/mangadistrict.png" width="22" align="top"> **MangaDistrict** <img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"> <sub>[mangadistrict.com](https://mangadistrict.com)</sub> | English | Adult manhwa, uncensored and official releases |
| <img src="assets/icons/manhwah.png" width="22" align="top"> **ManhwaH** <img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"> <sub>[manhwah.com](https://manhwah.com)</sub> | English | Adult manhwa, with optional Korean raws |
| <img src="assets/icons/hiperdex.png" width="22" align="top"> **HiperDex** <img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"> <sub>[hiperdex.com](https://hiperdex.com)</sub> | English, Portuguese | Adult manhwa with a rating on every title |

Multi-language sources default to English; pick yours in each source's settings.

## What they all do

- **Filters that stay current.** Genre and tag lists come from the site itself, so they never go stale between source updates.
- **Hide what you don't want.** Genres, and on most sources tags, types, formats or demographics. Hidden entries vanish from home, listings and search, not just the filter sheet. Adult content is off by default.
- **One upload per chapter.** Where a site carries duplicates, you get one. Read history follows the chapter, not the upload, so nothing re-marks itself unread when a site reshuffles.
- **Covers first.** Requests are batched and cached, and covers load before anything else.
- **Tappable chips.** Genre chips on a series page open matching titles, and on most sources author and tag chips too. Paste a link and the right page opens.

<sub>MangaDistrict is the exception: a single-language adult source with no settings of its own, so there is nothing to hide or deduplicate, and Aidoku rates it adult as a whole. MadaraDex, ManhwaH and HiperDex are adult sources too, so they show adult titles until you narrow that in their settings. MadaraDex, MangaDistrict, BaeToon, ManhwaH and HiperDex have their genre lists built into the source, matched to each site's full list when it was released.</sub>

## Install one at a time

Each source below has an **Add to Aidoku** button that installs only that one and keeps auto-updates. Prefer to import by hand? Every package lives in [`sources/`](https://github.com/Smexhy/yomu-aidoku-sources/tree/main/sources), though a hand import will not auto-update.

<h3><img src="assets/icons/comix.png" width="24" align="top">&nbsp; Comix</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/comix/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://comix.to">comix.to</a> &nbsp;·&nbsp; <strong>needs Aidoku 0.8.4+</strong></sub>

English manga and webtoons. Home has Most Recent Popular, Latest Updates, Most Followed New Comics and Recently Added, plus Trending Webtoon and Trending Manga ranked by views over three months.

- **Filters.** Genres, demographic, format, type, status, content rating, release year, minimum chapters, author, artist and sort. Genres and formats include or exclude, with AND or OR matching.
- **Content rating.** Safe, Suggestive, Erotica and Pornographic, applied across home, listings and search. Defaults to Safe and Suggestive.
- **Content hiding.** Any type, demographic, genre, format or tag, plus Custom Hidden Tags for anything not in the list.
- **Chapter selection.** Official uploads first, then a preferred scanlation group carried across the series, with gaps filled from the next best. Or pick the best upload per chapter instead.
- **Scrambled pages.** Protected pages use Comix's own renderer to undo tile scrambling. Signing and decoding changes are handled where supported.

<details>
<summary><strong>More about Comix</strong></summary>

<p><strong>Title and chapter data.</strong> Chapter lists, descriptions and publication statuses support Comix's updated responses. Older cached title details are refreshed, and responses that remain encrypted trigger decoder recovery instead of being saved as empty metadata. When Comix rotates its signing key during a site update, Yomu fetches the new signing setup again past any caches, remembers the retired key so it is not reused, and briefly waits out a rollout still in progress. Poster links in the newer site-relative format are resolved too. For an unfamiliar authentication error, Yomu checks whether Comix's signing setup changed before attempting the same recovery. Yomu also handles the current move of Comix's signing helpers and common script rearrangements. A different signing protocol can still need a source update.</p>

<p><strong>Automatic connection.</strong> Normal requests are preferred. If Cloudflare blocks the API, Yomu switches only after the web view successfully loads it, and checks the signed API again before returning to normal. Covers choose their connection separately for each host, so a blocked cover cannot switch the whole source. <code>Settings &gt; Connection</code> can pin either mode. If its browser session stops responding, Yomu recreates that session and retries once, keeping cookies and saved chapter progress. A repeated failure stops with an error instead of reusing the same failed session on every refresh.</p>

<p><strong>Fewer requests.</strong> Home cards no longer look up each title's genres and authors by default, which saved about 40 requests per session. Turn it back on under <code>Settings &gt; Content &gt; Home Card Details</code>.</p>

<p><strong>Page loading.</strong> Current full image URLs and older shared-base lists are supported. Healthy ordinary images load directly. If a download fails, Yomu can try up to two fallback locations explicitly supplied by that chapter and return the recovered image automatically. A fallback may use a different node as well as a different domain; a working location is remembered only for that page. Short deadlines, a shared recovery budget and refusal backoff limit waiting and repeated requests. Recovery briefly occupies the source, stops when it cannot finish, and may leave a manual Reload necessary. It cannot repair an unavailable image or guarantee that every CDN will work. An incompatible chapter format reports that a source update may be needed.</p>

<p><strong>Long chapter lists.</strong> Completed histories are cached, and refreshes can reuse the unchanged older portion instead of downloading it all again. Slow or interrupted loads save a checkpoint. A timed pause reports how many uploads were loaded and the reported total; pull down to refresh to continue. A huge first load can still take time or need more than one attempt. Progress cannot replace Aidoku's own loading UI, so Retry can temporarily leave a misleading “No Chapters” label while work continues.</p>

<p><strong>Tidy chapter names.</strong> Upload names that only repeat the chapter number are hidden; real titles stay.</p>

<p><strong>Chapter sources.</strong> Each chapter shows its real source, with a check on licensed platforms like Tappytoon.</p>

<p><strong>Already reading Comix elsewhere?</strong> Yomu uses the same source id, so compatible saved titles continue using it. <strong>Show One Upload Per Chapter</strong> is on by default; a one-time migration carries supported reading history to the deduplicated chapter ids. Turn the setting off to see every upload. If you installed a higher-numbered local test build, Aidoku will not automatically downgrade it to the public package: reinstall the Comix source from Yomu to return to public updates.</p>

</details>

<h3><img src="assets/icons/kagane.png" width="24" align="top">&nbsp; Kagane</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/kagane/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 60+ languages &nbsp;·&nbsp; <a href="https://kagane.moe">kagane.moe</a></sub>

Manhwa, manga and manhua, mostly manhwa. Home has Popular, Recently Added and Recently Updated.

- **Filters.** Genres, tags, demographic, type, status, content rating, original language, source type, release year, author and sort. Genres and tags include or exclude, with AND or OR matching.
- **Content hiding.** Formats, genres, curated tag categories, or any tag by name under Custom Hidden Tags.
- **Upload sources.** Every chapter shows where it came from, like Tapas or Omega Scans, with a check on official ones. Show all uploads, official only, or scanlations only.
- **Spoiler tags.** Genres and tags Kagane marks as spoilers stay hidden unless you ask for them.
- **Over sixty languages.** Korean, Japanese, Chinese, French, German, Spanish and more.
- **Mirror fallback.** Remembers a working address and tries another mirror if it stops responding.

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

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangaball/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 50+ languages &nbsp;·&nbsp; <a href="https://mangaball.com">mangaball.com</a></sub>

Manga, manhwa and manhua. Home has Featured, Latest Updates, Recommended, Most Popular, Recently Added and Top Rated.

- **Filters.** Live genres and tags as separate include or exclude lists with Any or All matching, plus demographic, status, type and author. Sort by update date, added date, title, views or rating.
- **Content hiding.** Hide types, genres or tags across home, listings and search. Adult content is off by default, with an extra check for titles the site flags incorrectly.
- **Over fifty languages.** Spanish, Portuguese, Indonesian, Vietnamese, French and more. Pick any combination and chapter lists follow your choice.
- **Deduplication.** On by default: official first, then most likes, then most views, then newest.
- **Reader layout.** Long Strip titles open in the vertical Webtoon reader automatically.

<details>
<summary><strong>More about Mangaball</strong></summary>

<p><strong>Current API.</strong> Mangaball's rebuilt site now provides a public JSON API, so there is no session or token warmup. Home rows load together, while a title's details and chapters are requested together.</p>

<p><strong>Reliable images.</strong> If an imported cover mirror disappears, Yomu uses the stored copy shown by Mangaball itself. Reader pages use the site's protected image storage directly and allow more time for slow images.</p>

<p><strong>Pages ready before you get there.</strong> Mangaball's image storage is slow for pages nobody has read lately. Yomu asks it to fetch the next ten pages while you read, so they arrive at full speed when you reach them. Very long chapter lists load in parallel pages instead of one huge request.</p>

<p><strong>Quick reopening.</strong> Reopening the most recent series within a minute reuses its chapter list instead of downloading the same list again.</p>

<p><strong>Specific errors.</strong> A real Cloudflare challenge is reported separately from an HTTP failure or an API response the source no longer understands.</p>

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
- **Comics only.** atsu.moe also hosts text novels, which have no pages for Aidoku to show, so they are left out of home, search and author pages.
- **Straight from the site.** Atsumaru's data is public, so Yomu reads straight from the site and page images are direct links. That makes it the quickest here to warm up.

<h3><img src="assets/icons/onisaga.png" width="24" align="top">&nbsp; OniSaga</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/onisaga/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 24 languages &nbsp;·&nbsp; <a href="https://onisaga.com">onisaga.com</a></sub>

Manga, manhwa and manhua. Home opens with the site's Spotlight slider, then Latest Updates, Trending This Week, New on OniSaga, Newly Published, Finished Series and genre shortcuts.

- **Filters.** Genres and themes (include or exclude), type, format, status, demographic, content rating, the language a title is translated into, publication year, and search by author or scanlation group.
- **Content hiding.** Hide genres and themes across home, listings and search. Mature and Explicit titles only appear while Show NSFW Content is on.
- **Twenty-four languages.** Including Simplified and Traditional Chinese, Korean, Japanese, Ukrainian and Persian.
- **Deduplication.** One upload per chapter and language: OniSaga's own pick, the newest, or the one with the most pages.
- **Sized covers.** Covers come at the size the screen needs, so lists load light.

<details>
<summary><strong>More about OniSaga</strong></summary>

<p><strong>Rebuilt for the new site.</strong> OniSaga moved to a new site in November 2026, and Yomu now reads its data straight from the site's own API, with no scraping. The new site has no popularity, rating or likes sorting and no minimum rating or chapter filters, so those are gone; Trending This Week takes the place of Fan Favorites.</p>

<p><strong>Your library carries over.</strong> Some series changed their address on the new site. After this update Aidoku asks to migrate once; Yomu follows the site's own redirects to the new addresses, and reading progress keeps its chapters.</p>

<p><strong>Adult titles and the age check.</strong> The new site only shows Mature and Explicit titles to visitors who confirmed they are 18 or older. With Show NSFW Content on, Yomu confirms that with OniSaga for you, the same way the site's own "I am 18 or older" button does, and turning the setting off withdraws it.</p>

<p><strong>Signed page links.</strong> OniSaga's reader hands out short-lived signed links for each page. A link that has expired by the time you reach its page is renewed through the site's own reader API.</p>

</details>

<h3><img src="assets/icons/mangafire.png" width="24" align="top">&nbsp; MangaFire</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangafire/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; 7 languages &nbsp;·&nbsp; <a href="https://mangafire.to">mangafire.to</a></sub>

Manga, manhwa and manhua. Home opens with a Top Trending slider, then Trending, Latest Updates, Most Viewed This Week, Trending Manga, Trending Webtoons, Recently Added and Most Followed, plus eleven browse listings.

- **One entry per chapter, and it stays put.** MangaFire lists an official release and a fan translation of the same chapter separately, and a re-upload gets a brand new id, so other readers show doubled chapters and old ones turning up unread again. Yomu lists each chapter once per language and keeps your read marks when an upload is replaced. Official release first by default, or fan translation, or newest.
- **Filters.** Genres and themes (include or exclude, all or any), formats, demographic, type, status, content rating, year, minimum chapters, author and artist, with thirteen sorts. The lists come from the site, with a built-in copy if it cannot be reached.
- **Content hiding.** Content ratings, types and genres. MangaFire applies them itself, so hidden titles stay out of home, every listing and search.
- **Seven languages.** English, Spanish, Latin American Spanish, French, Japanese, Portuguese and Brazilian Portuguese.

<details>
<summary><strong>More about MangaFire</strong></summary>

<p><strong>Alongside the community source.</strong> The Aidoku community list also has a MangaFire source. Yomu's uses its own id, so the two never replace each other on update and you can keep both installed. Use Aidoku's Migrate to move a title over.</p>

<p><strong>Quick to open.</strong> A title's details and the first page of its chapter list come back together, and requests that time out are retried once as a group instead of one after another.</p>

<p><strong>When the site changes its request signing.</strong> MangaFire signs every request. Yomu signs them itself, and if the site changes its scheme it falls back to the site's own signer, so a change usually does not need a source update.</p>

</details>

<h3><img src="assets/icons/baetoon.png" width="24" align="top">&nbsp; BaeToon</h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/baetoon/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://baetoon.com">baetoon.com</a></sub>

English manhwa, manga and manhua gathered from many scanlation sites. Home has the site's Spotlight slider, Hot Today, Latest Updates, Recently Added, Top This Week, Top This Month, Top All Time and Popular Genres.

- **One entry per chapter.** BaeToon collects the same chapter from several sites. Yomu lists each chapter once and opens the upload the site itself picks, and every chapter shows the site it came from.
- **Filters.** Sort by most viewed, latest updates, recently added, top rated or A to Z, one genre at a time, and search by author or keyword.
- **Content hiding.** Mature content is off by default (titles tagged Mature, Ecchi or Sexual Violence), and any genre can be hidden across home, listings and search.
- **Pages ready before you get there.** BaeToon's image storage is slow for pages nobody has read lately, so Yomu asks it to fetch the next ten pages while you read.
- **Recovers moved chapters.** If an upload disappears from the site, Yomu finds that chapter's current upload by number.

<h3><img src="assets/icons/madaradex.png" width="24" align="top">&nbsp; MadaraDex &nbsp;<img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/madaradex/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://madaradex.org">madaradex.org</a></sub>

<strong>Mostly adult.</strong> The great majority of madaradex.org is adult manhwa, with a smaller number of safe-for-work series alongside it, so the source is rated adult as a whole. Aidoku filters it with your other content settings, which means it can stay hidden until you allow adult sources.

Home opens with a Popular This Week slider, then Popular Today, Latest Updates, New on MadaraDex, Popular This Month, All-Time Popular and genre shortcuts, plus eight browse listings.

- **Filters.** Eleven sorts (popular today, this week or this month, latest, newest, oldest, rating, views and more), type, status, adult content (exclude, only, or uncensored only), minimum rating, genres to include or exclude with all or any matching, author and artist.
- **Content hiding.** Hide any genre, or turn on Hide Adult Titles to keep only the titles the site marks safe for work. MadaraDex leaves them out itself, so they stay out of home, every listing and search. A genre you pick in a search still shows.
- **Tappable chips.** Genre, author and artist on a series page each open matching titles.
- **The next chapter is already waiting.** While you read, the following chapter loads in the background, so tapping through a series is close to instant.

<details>
<summary><strong>More about MadaraDex</strong></summary>

<p><strong>Pages that load at all.</strong> MadaraDex serves its page images only to a real browser and refuses an app asking for them directly, which is why a straightforward source for it does not work. Yomu passes the site's image check itself, starting as soon as you open a series, then loads the pages normally. From your side it is just a chapter that opens.</p>

<p><strong>Rebuilt for the new site.</strong> MadaraDex moved to its own theme in November 2026, with a new home, a new title index and chapter lists split into pages. Yomu reads all of it, and your saved series keep working.</p>

</details>

<h3><img src="assets/icons/mangadistrict.png" width="24" align="top">&nbsp; MangaDistrict &nbsp;<img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangadistrict/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://mangadistrict.com">mangadistrict.com</a></sub>

<strong>Adult.</strong> mangadistrict.com is an adult manhwa site, so the source is rated adult as a whole and Aidoku filters it with your other content settings.

Home has New Releases, Latest Updates and Today's Trends, plus five browse listings: Latest Updates, Trending, Most Viewed, New Series and Top Rated.

- **Every page loads.** The site loads most pages only as you scroll, and puts a blank stand-in where each page will go. A reader that takes those stand-ins at face value shows black pages or pages that never finish loading. Yomu reads the real image for every page, so a chapter opens complete.
- **No promo banner.** The site puts its own "Where the best stories live" banner at the start of every chapter. Yomu leaves out that one image and nothing else, so credit and "To be continued" pages stay.
- **Real covers.** Adult covers that the site hides behind a placeholder show properly.
- **Filters.** Sort by relevance, latest, A to Z, rating, trending, most views or newest, plus the full genre list with any or all matching, status, adult content, author and artist.
- **Tappable chips.** Genre and author on a series page open matching titles; other tags search by name.
- **Series details.** Genres and tags, status, author, artist and upload dates.

<details>
<summary><strong>More about MangaDistrict</strong></summary>

<p><strong>Alongside the community source.</strong> The Aidoku community list also has a MangaDistrict source. Yomu's uses its own id, so the two never replace each other on update and you can keep both installed. To move a title over, use Aidoku's Migrate; series and chapter links match, so it finds them directly. Older links in the site's previous <code>/title/</code> format still open.</p>

<p><strong>Ready for layout changes.</strong> If the site renames its reader layout, Yomu still finds the chapter's pages from the page itself, and if the chapter list moves off the series page it loads it the way the site's theme does.</p>

</details>

<h3><img src="assets/icons/manhwah.png" width="24" align="top">&nbsp; ManhwaH &nbsp;<img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/manhwah/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English &nbsp;·&nbsp; <a href="https://manhwah.com">manhwah.com</a></sub>

<strong>Adult.</strong> manhwah.com is mostly adult manhwa, so the source is rated adult as a whole and Aidoku filters it with your other content settings.

Home opens with a Trending slider, then Latest Updates, Most Viewed This Week, Recently Added, Top Rated and genre shortcuts, plus nine browse listings.

- **Content rating.** Each title is rated from its genres (Adult, Smut and Hentai count as NSFW; Mature and Ecchi as Suggestive), and you choose which ratings to show. Any genre can be hidden too.
- **Filters.** Sort by most viewed, latest updates, trending, recently added, top rated or A to Z, plus status, genres and author.
- **Korean raws, if you want them.** Show Raw Chapters adds the untranslated Korean chapters the site lists, marked Raw. They often run a few chapters ahead.
- **One entry per chapter.** The site sometimes carries a second upload of a chapter; Yomu lists it once.
- **Pages ready before you get there.** ManhwaH's image storage streams slowly for pages nobody has read lately, so Yomu asks it to fetch the next ten pages while you read. A cold chapter goes from several seconds per page to near instant.

<h3><img src="assets/icons/hiperdex.png" width="24" align="top">&nbsp; HiperDex &nbsp;<img alt="18+" src="https://img.shields.io/badge/18+-ff3b69?style=flat-square" align="top"></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/hiperdex/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; English, Portuguese &nbsp;·&nbsp; <a href="https://hiperdex.com">hiperdex.com</a></sub>

<strong>Adult.</strong> hiperdex.com is mostly adult manhwa, so the source is rated adult as a whole and Aidoku filters it with your other content settings.

Home opens with a Top Trending slider, then Trending This Week, Latest Updates, Most Popular, New Series, Top Rated and Popular Genres, plus eight browse listings including trending today, this week and this month.

- **Content rating.** HiperDex rates every title Safe, Suggestive, Erotica or Pornographic; choose which to show, and hide any genre.
- **Filters.** Seven sorts, type, status, content rating, genres, author and artist.
- **English and Brazilian Portuguese.** Many newer titles are Portuguese only. When a title has no chapters in your chosen languages, Yomu shows the ones it has instead of an empty list.
- **Fast title pages.** A title's details and chapters are requested together, in one round trip.

## If a source gets stuck loading

> 💡 **Keep Aidoku on the latest version.** Almost everything that shows up as a 403, an
> endless spinner or a verification window that never finishes is Cloudflare handling on the
> app side, not the source. Those fixes ship in Aidoku releases, so an update is usually the
> whole answer and by far the quickest one.

Most of these sites sit behind Cloudflare, so the first time you open one in a session its
check can add a few seconds before covers appear. That much is normal.

If a source is still stuck after updating:

1. Open **Browse**, tap the source, then the **three dots → Settings**.
2. Scroll down and tap **Clear Cache**.
3. **Force close Aidoku** (swipe it away) and open it again.

That drops the stale Cloudflare cookie and it loads again.

## Updates

Pull to refresh your source lists in Aidoku to pick up new versions. I update these when a site changes or something breaks, in my free time, so there is no schedule. Everything is built and tested against the current Aidoku app and SDK.

## License and use

These are my own packages, shared so you can read with them in Aidoku. Please do not rehost, repackage or republish the packages or this list as your own. See [LICENSE](LICENSE) for details.

The packages are compiled from Rust and include the open-source Aidoku SDK and other libraries; their notices are in [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

Not affiliated with Aidoku or any of the sites listed here. All names and logos belong to their owners.

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c5cff,100:ff3b69&height=90&section=footer" alt="" width="100%">
</div>
