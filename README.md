# 29 Ekim Cumhuriyet Bayramı

An interactive night-scene celebration of the Turkish Republic's founding day
(29 October 1923), built as a single-page WebGL animation.

**Live:** https://cguldogan.github.io/29Ekim/

## What's inside

- **Fireworks** — click anywhere (or press Space/Enter) to launch; bursts also
  fire on their own timer
- **Turkish flag** — drawn to the official construction spec, waving in the
  wind over an animated flagpole
- **Atatürk silhouette** — standing to the right of the flag, backlit with a
  gold rim; cut from a portrait using its alpha mask
- **Easter eggs** — six golden stars are hidden around the scene. Click one to
  reveal a verbatim Atatürk quote (source:
  [ata.msb.gov.tr](https://ata.msb.gov.tr/Sayfa/SayfaGoster/ataturkun-diger-konular-ile-ilgili-vecizeleri)).
  Finding all six triggers a finale. Found eggs are remembered per browser
- **March playlist** — six recordings with prev/next/loop:

  | #   | Piece              | Performance                            |
  | --- | ------------------ | -------------------------------------- |
  | 1   | İzmir Marşı        | TSK Armoni Mızıkası (military band)    |
  | 2   | İzmir Marşı        | CRR Senfoni Orkestrası ve Korosu       |
  | 3   | Onuncu Yıl Marşı   | TSK Armoni Mızıkası                    |
  | 4   | Onuncu Yıl Marşı   | Cumhurbaşkanlığı Senfoni Orkestrası    |
  | 5   | Gençlik Marşı      | TSK Armoni Mızıkası                    |
  | 6   | Biz Atatürk Gençleriyiz | TSK Armoni Mızıkası               |

  All tracks are loudness-normalized to −18 LUFS with fade in/out for
  gapless loop points.

## Running

No build step. Either open `index.html` directly, or serve the folder:

```sh
python3 -m http.server
# then visit http://localhost:8000
```

Deployed automatically by GitHub Pages from `main`.

## Tech

- Three.js r128 (CDN) — flag cloth simulation, particle fireworks, sprites
- Web Audio / HTMLAudio — playlist playback
- Everything else is inline in `index.html`; the only assets are the six
  `.m4a` audio files

## Credits

- Quotes: Atatürk Research Center selections via ata.msb.gov.tr
- Music: performances of İzmir Marşı, Onuncu Yıl Marşı, Gençlik Marşı and
  Biz Atatürk Gençleriyiz by the TSK Armoni Mızıkası, CRR Symphony Orchestra
  and Choir, and the Presidential Symphony Orchestra (personal, non-commercial
  use)
