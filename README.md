# CPSPA Connect

A responsive, frontend-only appointment and faculty messaging prototype for the College of Political Science and Public Administration at PUP. The prototype uses in-memory mock data; actions update the interface for the current session.

## Run locally

```sh
npm install
npm run dev
```

Create a production build with `npm run build`.

## Prototype areas

- Student overview, upcoming appointments, calendar, faculty directory, and appointment request form.
- Faculty messages with a local demo reply. To connect a Socket.IO server, set `VITE_SOCKET_URL` and provide a session token in `sessionStorage` under `cpspa-session-token`. The socket uses the Pigsy `send_message` acknowledgement and `new_message` event pattern.
- Monday through Saturday office hours, initially 7:00 AM to 5:00 PM, editable in the Office hours view.
- Super-admin professor invitation form and mock faculty access list.

No backend or registration flow is required for the demo.
