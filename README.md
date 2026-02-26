# cnr-proto-dashboard

Real-time protobuf event dashboard for ClubWPT Gold poker. React 18 SPA with four tabs:

- **Feed** — Live decoded protobuf events with topic filtering
- **Table** — Visual table layout with seats, cards, pots, and phase
- **Console** — Raw event data inspector
- **Stats** — Session statistics (hands played, events captured, uptime)

## Usage

Served by cnr-ws-server at `http://localhost:13030/proto-dashboard`.

Connects to `ws://localhost:13030/ws` and listens for proto_event, game_status, and card_event broadcasts from the relay server.

## Architecture

Self-contained single HTML file using React 18 UMD + Babel standalone for in-browser JSX transformation. No build step required.
