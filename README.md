# Attendance.io

A responsive attendance tracker for engineering students. Track attendance by subject, import a timetable, monitor your 75% target, and export reports.

## Run locally

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Deploy to Vercel

1. Import this GitHub repository into Vercel.
2. Framework preset: **Vite**.
3. Build command: `npm run build`; output directory: `dist`.
4. Deploy. No environment variables are required for this local-first version.

## Data and privacy

Attendance records and timetable data are stored in this browser using localStorage. They remain on this device/browser and are not synced across devices. Use **Settings → Export backup** regularly. Authentication and cloud sync are intentionally left for a later phase.

## Timetable import

Use a CSV with columns `day,subject,start,end,room` (header row required). Example:

```csv
day,subject,start,end,room
Monday,Mathematics,09:00,10:00,Room 201
Tuesday,Physics,10:00,11:00,Lab 2
```

You can also add subjects and weekly class slots manually. PDF/image extraction is not included in this first version; manually verify a timetable before relying on attendance forecasts.
