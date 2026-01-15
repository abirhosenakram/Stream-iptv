# Stream‑IPTV

Stream‑IPTV is a lightweight, browser-based IPTV player implemented as a single HTML file (index.html). It provides a simple interface for loading M3U/M3U8 playlists and optional XMLTV EPG data so users can browse and play live channels directly in a browser — no installation required.

## Key features

- Single-file web player (index.html) — easy to host and customize
- M3U / M3U8 playlist parsing
- Optional XMLTV (EPG) support for program guides
- Channel grouping, logos and metadata support via standard M3U tags
- HTML5/HLS playback (client-side HLS via browser or a JS HLS library)
- Minimal, dependency-free base for customization and extension

## Quick start

1. Clone the repository

   git clone https://github.com/abirhosenakram/Stream-iptv.git

2. Serve locally (recommended to avoid CORS issues)

   - Using Python 3:
     python3 -m http.server 8000
     Open: http://localhost:8000/index.html

   - Alternatively, open index.html directly in a browser (some browsers may restrict local file access).

3. Load a playlist

   - Provide an M3U/M3U8 URL or select a local M3U file in the UI (if supported).
   - Optionally provide an XMLTV/EPG URL to enable program guide features.

## Hosting with GitHub Pages

1. Push the repository to your GitHub account.
2. Go to the repository Settings → Pages and set the source to the main branch (root).
3. After a short delay, your app will be available at:
   https://<your-username>.github.io/Stream-iptv

## M3U & EPG notes

- Typical M3U entry:

  #EXTINF:-1 tvg-id="channel.id" tvg-name="Channel Name" tvg-logo="https://example.com/logo.png" group-title="News",Channel Name
  http://stream.example.com/stream/playlist.m3u8

- For best EPG results, ensure the XMLTV channel id (channel/@id) matches the M3U tvg-id values.

## Supported stream types

- HLS (m3u8) — best supported across modern browsers
- Other HTTP(S) progressive streams (MP4, etc.) depending on browser codec support
- Note: DRM‑protected streams and certain codecs may not play in all browsers

## Development

- index.html is the main source file (HTML, CSS, JS combined).
- To extend or modularize:
  - Split scripts/styles into separate files (scripts/, styles/).
  - Integrate hls.js for robust HLS playback on browsers without native HLS support.
  - Add UI improvements, caching, favorites, recording hooks, or server-side playlist aggregation as needed.

## Security & Legal

- This project is a player only. It does not provide or host streams.
- Do not use this project to access or distribute copyrighted streams without proper authorization.
- When loading third‑party streams, ensure you have the right to access and play them.
- Be mindful of CORS policies when using remote playlists or EPG files.

## Troubleshooting

- No playback / black screen: check browser console for CORS, 403/404 errors, or unsupported codec errors.
- Playback stutters: verify network bandwidth and stream bitrate; try a different player or host.
- EPG not matching: confirm tvg-id values in M3U and XMLTV channel ids are consistent.

## Contributing

- Fork the repository, make changes, and open a pull request.
- For issues or feature requests, please open an issue in this repository.

## License

- See the LICENSE file in this repository for license details.

## Author / Contact

- GitHub: https://github.com/abirhosenakram
