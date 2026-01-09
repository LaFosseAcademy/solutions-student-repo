### Level 1 – Context diagram

- **User** → **Weather‑Watcher API** – “Uses”
- **Weather‑Watcher API** → **External Weather API** – “Pulls current weather”
- **Weather‑Watcher API** → **Push‑Notification Service** – “Pushes alerts”

### Level 2 – Container diagram


| Container                    | Typical technology                    | Responsibility                                                                                 |
|------------------------------|---------------------------------------|------------------------------------------------------------------------------------------------|
| **API Gateway / Web Server** | Node.js / Express, FastAPI, etc.      | Handles `GET /weather` and `POST /alert` from the User                                         |
| **Weather Fetcher**          | Python / Requests, Node / axios, etc. | Scheduled job that calls the External Weather API and caches the latest data                   |
| **Threshold Store**          | Redis, in‑memory map, simple DB       | Persists user‑defined temperature thresholds                                                   |
| **Alert Processor**          | Node.js, Python, etc.                 | Reads cached weather & thresholds; calls Push‑Notification Service when a threshold is crossed |

- User → API Gateway (Uses)
- API Gateway → Weather Fetcher (GET request for current weather)
- API Gateway → Threshold Store (store/retrieve thresholds)
- Weather Fetcher → External Weather API (Pull)
- Alert Processor → Threshold Store (Read thresholds)
- Alert Processor → Push‑Notification Service (Push)
