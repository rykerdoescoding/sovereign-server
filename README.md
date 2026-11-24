Sovereign dedicated server
========================
Windows 7+: double-click start-server.bat (needs .NET Framework 4.0 or newer, already included in Windows 10/11).
Linux / macOS: install Mono, then run:  mono RoWorldServer.exe

FILES (created next to RoWorldServer.exe on first launch)
  server.properties   settings: name, motd, port, password, limits, defaults, tick rate, logging.
                      Edit it, then restart the server.
  logs/server-YYYY-MM-DD_HH-mm-ss.log
                      one new log file per launch: connections, rooms, game starts/ends,
                      and every chat message ([chat] [room] [alliance] name: text).
                      Set log-chat=false in server.properties to stop logging chat.

Default port is 7777 (TCP). For internet play, forward that TCP port on the router / open it in the VPS firewall.
Players type the server's IP address, port and (if you set one) password in MULTIPLAYER > Connect.
You can override the port: RoWorldServer.exe 8000

The server only relays chat and player commands (the game runs on every client), so it needs very little CPU.
"Host a server on this PC" might not work probably.
