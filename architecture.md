# Technical Design / Architecture

## Implemented demonstration flow

```text
Optional image upload (preview only)
             |
             v
Manual selection of demo outcome
             |
             v
Manually entered sample latitude / longitude
             |
             v
Browser-side JavaScript validates coordinate range
             |
             v
Simulated alert record created in page memory
             |
             v
Dashboard table + OpenStreetMap link + CSV export
```

## Components
- **User interface:** HTML and CSS in `index.html`.
- **Demo logic:** JavaScript in `index.html`.
- **Location:** manually entered/sample coordinates, not live GPS.
- **Alert log:** held in browser memory while the page is open; no server/database.
- **Map link:** opens OpenStreetMap at the provided coordinates; requires an internet connection.

## Proposed future architecture
Road camera/video -> validated accident-detection model -> human verification -> GPS/location source -> secure backend/database -> monitoring dashboard -> authorised emergency-service workflow.

## Limitations and safety
No AI inference, live GPS, real dispatch, hospital connection, or permanent database is implemented. Human verification and formal emergency-service integration would be necessary before any real-world deployment.
