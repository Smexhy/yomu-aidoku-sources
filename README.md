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

[Aidoku](https://aidoku.app) is a free, open-source manga reader for iOS and iPadOS. Yomu is my own source list for it, six sources I built for my own reading and keep here so anyone else can use them too. It is not the official Aidoku community list and is not trying to replace it. I just maintain my own builds and update them when the sites change or something breaks.

Comix, MangaDot and Atsumaru read in English. Kagane, Mangaball and OniSaga carry several chapter languages, English by default, set in each source's settings.

## What every source shares

Every source here is built on the same foundations, so you get the same experience whichever one you open.

<table>
<tr><td width="200">🧩 <strong>Live filters</strong></td><td>Genres load live from every site, with tags and demographics where the site offers them, so the filter lists stay current on their own without waiting for a source update.</td></tr>
<tr><td>🙈 <strong>Real content hiding</strong></td><td>Hide genres, tags, formats or demographics in settings and they disappear from the home, listings <em>and</em> search, not just the filter sheet. Adult content is off by default.</td></tr>
<tr><td>🎯 <strong>Smart dedupe, no fake updates</strong></td><td>Where a site serves duplicate chapter uploads, the source keeps the best one. Read history is keyed to the chapter, not the upload, so a chapter you read stays read and reordering never fires false "new chapter" notifications.</td></tr>
<tr><td>⚡ <strong>Built to be fast</strong></td><td>Filter data is cached and, on most sources, kept across app launches, network calls are batched into single round trips, and covers start loading before anything else, so browsing stays quick and light.</td></tr>
<tr><td>🛡️ <strong>Cloudflare handled</strong></td><td>The sites behind Cloudflare ride Aidoku's native handling, with a clear message and a quick fix if a check ever gets stuck.</td></tr>
<tr><td>🔗 <strong>Tappable chips and deep links</strong></td><td>Genre and tag chips, and author chips on most sources, jump straight to matching titles, and pasted chapter or series links open the right page.</td></tr>
</table>

## Sources

Want just one instead of the whole list? Each source below has a one-tap **Add to Aidoku** button that installs only that source and keeps auto updates, or a **Download .aix** link to import the package by hand (a hand import does not auto update).

<h3><img src="assets/icons/comix.png" width="24" align="top">&nbsp; Comix &nbsp;<sub><a href="https://comix.to">comix.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/comix/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.comix-v113.aix">Download .aix (v113)</a></sub>

Manga and webtoons from comix.to. Home leads with Most Recent Popular, then Latest Updates, Most Followed New Comics and Recently Added. Filters cover type, demographic, format, status and a long genre list with AND/OR matching. Each chapter is tagged with its real source, and official releases like Tappytoon get a check so licensed uploads stand apart from scanlations.

The clever part is underneath. Comix locks its API behind an obfuscated signing module it rotates often, and serves page images with the tiles scrambled. Yomu pulls the current module, signs every request with it, and lets comix's own renderer work out each page's tile order and puts them back, so chapters just open like normal.

<details>
<summary><strong>Already use Comix from the community list?</strong> (read before adding)</summary>

Mine shares the same source id with a deliberately high version (<strong>100+</strong>), so adding Yomu keeps your existing library and just swaps in my build. You won't lose any saved series or progress. The main difference is chapter handling. Unlike the community build, <strong>Deduplicate Chapters</strong> is on by default here, so Comix keeps one upload per chapter out of the box. Read history is tied to the chapter number, so a chapter you read stays read no matter which upload wins a later dedupe, and the first update runs a one-time migration to carry your existing history across while dedupe is on. On a large library that first open can sit on a plain spinner for a few minutes. That is normal. Prefer the old behavior, with no deduplication? Just use the community Comix instead.

</details>

<h3><img src="assets/icons/kagane.png" width="24" align="top">&nbsp; Kagane &nbsp;<sub><a href="https://kagane.to">kagane.to</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/kagane/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.kagane-v11.aix">Download .aix (v11)</a></sub>

Multi-language manhwa, manga and manhua from kagane.to, mostly manhwa, nine chapter languages with English by default. Each chapter shows its real upload source, like Tapas or Omega Scans, with a check on the official ones, and an optional setting can add that source to the title to tell duplicate titles apart.

Reading a chapter needs a short-lived signed token, so Yomu grabs one and reuses it for about five minutes, and now keeps it across app restarts too, so reopening within that window skips the handshake.

> 💡 **If a chapter goes black or the app closes partway through:** a few Kagane series use very large page images. On those the reader can run out of memory. Turn on **Downsample Images** in Aidoku's reader settings and it shrinks each page to fit your screen as it loads. This is an Aidoku setting, not something a source can do. The images really are that big.

<h3><img src="assets/icons/mangaball.png" width="24" align="top">&nbsp; Mangaball &nbsp;<sub><a href="https://mangaball.net">mangaball.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangaball/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.mangaball-v8.aix">Download .aix (v8)</a></sub>

Multi-language manga, manhwa and manhua from mangaball.net, twelve chapter languages with English by default. Home has Featured, Latest Updates, Recommended and Popular This Season, with tappable tag and author chips and separate genre and tag filters. The site is session-based, so Yomu does a quick handshake first, and if you paste a title with curly quotes it straightens them to the plain ones the site's search expects.

<h3><img src="assets/icons/mangadot.png" width="24" align="top">&nbsp; MangaDot &nbsp;<sub><a href="https://mangadot.net">mangadot.net</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/mangadot/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.mangadot-v11.aix">Download .aix (v11)</a></sub>

Manga, manhwa and manhua from mangadot.net. Home has Most Viewed, Latest Updates, Top Rated and Most Tracked, with title search and tappable genre, author and artist chips. Its nicest trick is the dedupe: it keeps the best upload of each chapter and spots official releases even when the site does not flag them, by recognizing platforms like Tappytoon, Tapas and WEBTOON by name, then marks them with a check.

<h3><img src="assets/icons/atsumaru.png" width="24" align="top">&nbsp; Atsumaru &nbsp;<sub><a href="https://atsu.moe">atsu.moe</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/atsumaru/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/en.atsumaru-v7.aix">Download .aix (v7)</a></sub>

Manga, manhwa and manhua from atsu.moe. Home has Trending, Popular, Top Rated, Recently Updated, Recently Added and Most Bookmarked, with fast search and tappable tag and author chips. Search runs on a Typesense backend, an author tap uses the site's dedicated author endpoint instead of a fuzzy text match, and a title pulls its details and chapter list together so it opens a bit quicker.

<h3><img src="assets/icons/onisaga.png" width="24" align="top">&nbsp; OniSaga &nbsp;<sub><a href="https://onisaga.com">onisaga.com</a></sub></h3>

<sub><a href="https://aidoku.app/add-source-list/?url=https://smexhy.github.io/yomu-aidoku-sources/onisaga/index.min.json"><b>Add to Aidoku</b></a> &nbsp;·&nbsp; <a href="https://smexhy.github.io/yomu-aidoku-sources/sources/multi.onisaga-v6.aix">Download .aix (v6)</a></sub>

Multi-language manga, manhwa and manhua from onisaga.com, eighteen chapter languages with English by default. Home leads with an auto-scrolling Most Popular slider, then Latest Mangas, Top Rated and Fan Favorites, with tappable genre and author chips and a full genre filter you can include or exclude. The site runs on Livewire behind Cloudflare, and a long chapter list, even hundreds across many languages, loads in a single request instead of paging batch by batch, so the biggest series open quickly.

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
