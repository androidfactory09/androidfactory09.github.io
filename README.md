# androidfactory09.github.io

Public pages for **Android Factory 09** — the privacy policy and support page for
each published game, and the `app-ads.txt` that AdMob crawls.

## app-ads.txt

`app-ads.txt` must sit at the **root** of this site, because AdMob looks for it
at `<developer website>/app-ads.txt`, using the website URL named on the Google
Play store listing. It is a **per-publisher** file: the single line in it covers
every app on the account, so it does not change when a new game is added.

The Play listing's **Website** field must therefore be the bare root of this
site, not a sub-path. Pointing it at a sub-path makes the file unfindable and
AdMob verification fails with *"your details don't match"*.

## These files are generated — do not edit them by hand

They are built from each app's own privacy policy by a script kept in the
private build repo. That script deliberately **refuses to publish** anything the
source marks as a maintainer note or as a draft section, and it verifies its own
output afterwards rather than trusting that the stripping worked — the first run
removed a drafted section and left two paragraphs still pointing at it.

To update: regenerate in the build repo, copy the output here, commit, push.

## Pages

- `/` — index
- `/app-ads.txt`
- `/sort-safari/privacy/`
- `/sort-safari/support/`

Further games are added on the day each one is published. A privacy page for an
app nobody can install yet is a live promise about software that does not exist.

## The developer name

**Android Factory 09**, matching the Play Console developer name exactly.

It was `AndroidStudi0` until 2026-08-29. That name matched nothing else the
account owns — the package id `com.androidfactory09.sortsafari` is permanent,
this domain is `androidfactory09.github.io`, and the account email is
`androidfactory09@gmail.com` — and it spells "Studio" with a digit zero, a
substitution Play's developer-name policy treats as imitation.

The name lives in one place: `STUDIO` in the site generator. Change it there and
rebuild; do not hand-edit the generated pages.

