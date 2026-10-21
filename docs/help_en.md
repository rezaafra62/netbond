# NetBond Help — version 1.4.3

## What is NetBond?
NetBond bonds the internet connections you already own (WiFi + Ethernet +
modem) on the same Windows machine: no server, no VPS, no cloud. The result
is one local "superlink" that your downloads and programs ride.

## Quick start
1. Unpack and run `netbond.exe` (or `netbond run`).
2. Default mode is the local proxy; programs that honour the system proxy
   (browsers, many downloaders) join the bond automatically.
3. For whole-system coverage enable "transparent mode" in Settings so every
   program joins without manual configuration.
4. In IDM: Options → Proxy/Socks → Get System, or point it at 127.0.0.1:8888.

## Links tab: tick, then route
- The "✓" column: tick as many links as you like.
- "Route ticked links to programs…" opens the dropdown sheet opposite the
  table: send the SUM of the ticked links to one or more chosen programs;
  "+" opens the installed-programs picker.
- Clicking the link NAME column opens that single link's sheet (its ticks
  and priorities).
- Last column: steps the link priority up/down.

## Downloads and parallel split
- Big downloads (HTTP and HTTPS) are striped across healthy links in
  parallel, IDM-style but across your own internets.
- If a link dies, the transfer resumes from the same byte via Range
  requests (up to three hops).
- Latency-sensitive live traffic stays on the lowest-RTT link.

## Security and privacy
- Everything stays on your machine; no cloud, no third party in the wire.
- TLS inspection (for seamless HTTPS failover) turns on only with your
  explicit consent; the local CA key is sealed with Windows DPAPI and never
  leaves the box.
- NetBond never cuts your connectivity: if it ever misbehaves, traffic
  flows the normal way (fail-open by design).

## The 48-hour trial edition
- On first run the machine fingerprint is stamped and a countdown appears
  in the title bar; after 48 hours the app refuses to run, ever.
- Rolling the system clock back expires it; copying the stamp to another
  machine helps nothing.

## Quick troubleshooting
- "No links yet": no adapter is up; connect a network card.
- IDM downloads invisible: set IDM's proxy to Get System.
- Two adapters on the same subnet: doctor shows an amber warning; move one
  to another subnet.
- CLI commands: links, probe, run, stats, bench, get, doctor, config,
  win-proxy, win-service, help.

## Help languages
This help ships inside the app in Persian, English, Spanish and Arabic;
switch it from the bar at the top of this window.
