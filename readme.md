# Time Since Tracker

A minimal web app for tracking how long it's been since meaningful moments. No server, no database, no build step — just a single HTML file that stores everything in the URL.

## Features

- Add named events with dates and times
- Live ticking timers showing years, months, days, hours, minutes and seconds
- State persists entirely in the URL — bookmark it or share it
- Confirmation step prevents accidental deletions
- Works offline once loaded
- Mobile friendly

## Usage

Open `index.html` in any modern browser. That's it.

To add an event, enter a name and pick a date and time using your browser's built-in datetime picker, then click Add.

To share your timers or save them for later, click "Copy shareable link" and bookmark the URL or send it to someone.

## How it works

All event data is serialised to JSON, base64 encoded, and stored in the URL's query parameter. When you load the page, it reads from the URL and reconstructs your timers. No data ever leaves your browser.

## Self-hosting

Drop the HTML file on any static hosting service, or just open it directly from your filesystem. There are no dependencies and no build process.
