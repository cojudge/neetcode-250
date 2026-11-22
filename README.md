# NeetCode 250 — Cojudge plugin

A [Cojudge](https://github.com/cojudge/cojudge) problem pack: the NeetCode 250
list, which is NeetCode 150 plus 100 more problems across the same patterns.

This pack ships the 99 problems that aren't in Blind 75 or NeetCode 150. The
other 151 are core Cojudge problems, and the course references them by slug.

## Install

```bash
cojudge plugin install neetcode-250          # from the catalog
cojudge plugin install cojudge/neetcode-250  # or straight from GitHub
```

Or open the **Plugins** page in the Cojudge web UI. Once installed, the pack
works offline.

## Layout

```
cojudge-plugin.json       plugin manifest
courses/nc250/            course definition
problems/<slug>/          statement.md, metadata.json, official-tests.json, Marker.java, solution.md
```

`"unprefixedIds": true` keeps the bare problem ids these problems had when
they were bundled with Cojudge, so existing progress still matches. 75 of
these problems also ship in the [LeetCode 1000](https://github.com/cojudge/leetcode-1000)
pack, so each pack works on its own. The copies are identical and share ids,
so installing both is fine. See Cojudge's
[`docs/PLUGINS.md`](https://github.com/cojudge/cojudge/blob/main/docs/PLUGINS.md).

## License

MIT
