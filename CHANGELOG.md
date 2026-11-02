# Changelog

## 0.3.0 — 2026-11-02

Contributed by Jeffrey D Johnson (#1).

- **Native rotation**, optional and off by default: a collection's timed pages
  become apps of their own on the clock, which rotates them itself. Pages can
  be picked with the clock's buttons or the API, a refresh keeps the page on
  show, and lost apps or an interrupted order are put back. Other apps on the
  clock, their order and the disabled ones are left as they are. Needs
  FiestaBoard 10.3.0 or later.
- **Clock transitions**, optional: the clock's own transition effect,
  direction, duration and automatic rotation can be set. Left unset, the
  clock keeps its settings; these apply to every app on the clock.
- **Full-colour 52 x 16 frames** for FiestaBoard's flexible JSON pages, once a
  FiestaBoard release has them (FiestaBoard PR #2395). Older versions are not
  affected.

## 0.2.1 — 2026-11-01

- The display catalog shows only **Ulanzi TC002** under the name, not
  Ulanzi · TC002 · Ulanzi TC002: the manufacturer and model are search
  keywords now.
- The display is called **Ulanzi TC002**: that it runs AWTRIX NG its
  description and the README say already.

## 0.2.0 — 2026-10-26

- Now `fiestaboard-output--ulanzi-tc002`, plugin id `ulanzi_tc002`, named for
  the device; it was `fiestaboard-output--awtrix-ng` with `awtrix_ng`. A board
  added with 0.1.0 belongs to the old id: install this one, add the board
  again, then remove the old board and the old plugin.
- The README says it needs AWTRIX NG: AWTRIX 3 and Ulanzi's own firmware are
  not supported.
- Ready for FiestaBoard's plugin registry: search details for the display
  catalog (LED matrices, Ulanzi TC002, AWTRIX) and a data-only `package.json`
  with the device data, as FiestaBoard's own output plugins have.
- The display is called **Ulanzi TC002 (AWTRIX NG)**: the device first, as
  the device model already was.
- An empty **App name** saves, and means `FiestaBoard`: FiestaBoard's settings
  form does not fill in a setting's default, and the field failed its pattern.
- A page that leaves the third row empty is drawn as two rows in the middle
  of the panel, each with its gap, rather than at the top.
- README: pictures of the clock and of the setup, and how to make pages for
  the clock.

## 0.1.0

- First version: FiestaBoard pages on a Ulanzi TC002 running AWTRIX NG, as a
  pushed app in the clock's rotation, 3 rows × 13 characters in the 3×5 font.
- LED transitions streamed at five frames a second; fade through black or blend.
- Show on change, display time, app name, Basic Auth.
- Find my clock, Test connection, and the page sent again after the clock restarts.
