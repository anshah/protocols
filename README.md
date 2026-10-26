# protocols

Interactive pages for learning how distributed-systems protocols work. Each lab is a single self-contained HTML file with an explainer, guided walkthroughs and a playground where you change the parameters yourself.

Live site: https://anshah.github.io/protocols/

## Labs

| Lab | Topic | Source paper |
|---|---|---|
| [Gossip Failure Detector](gossip/gossip-failure-detector.html) | Heartbeat lists, merging, epidemic spread, crash detection, ghost entries, partitions, subnet-aware gossip | [A Gossip-Style Failure Detection Service](http://cs.cornell.edu/home/rvr/papers/GossipFD.pdf) (van Renesse, Minsky, Hayden, 1998) |

## Running locally

No build step and no dependencies. Open `index.html` in a browser, or open a lab directly. An internet connection is only needed for the Google Fonts, and the pages fall back to system fonts without it.

## Layout

```
index.html                         landing page that links to every lab
gossip/gossip-failure-detector.html
```

## Adding a lab

1. Create a folder for the protocol with its HTML file.
2. Add a card for it to the list in `index.html`, using a relative link.
3. Add a row to the table above.

## Publishing

The site is served by GitHub Pages from the `main` branch, root folder. Pushing to `main` redeploys it, and browsers may cache the old version for up to 10 minutes.
