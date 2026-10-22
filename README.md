# CareFlow — Clinic Queue Organizer

CareFlow is a browser-based prototype exploring how a simple digital queue can help organize fictional clinic visits and illustrate how consultation-room capacity affects queue completion time.

**Live demo:** https://samuel-11111.github.io/careflow/

## Project Goals

- Build a simple interface for organizing a demonstration queue.
- Track fictional visits as they move through different statuses.
- Explore queue scenarios using a transparent, simplified simulation.
- Practice web development, usability testing, and responsible handling of sensitive information.

## Features

- **Queue management:** Add and remove fictional visits.
- **Visit status:** Move visits between waiting, in consultation, and completed states.
- **Queue filters:** View visits by status.
- **Summary counts:** Display the number of visits in each status.
- **Browser persistence:** Retain demonstration data using browser local storage.
- **Responsive interface:** Support desktop and narrow-screen layouts.
- **Queue performance simulator:** Compare estimated completion times for one and two consultation rooms.

## How the Simulator Works

The simulator accepts a number of visits and an average service time per visit.

It estimates the time needed to complete the entire batch under two scenarios:

- **One room:** number of visits × service time per visit.
- **Two rooms:** round up the number of visits divided by two, then multiply by service time per visit.

For example, 12 visits at 10 minutes each produce an estimated 120 minutes with one room and 60 minutes with two rooms.

These calculations assume all visits are ready at the start, every visit takes the same amount of time, and consultation rooms operate in parallel.

**Important:** These are hypothetical estimates, not measured patient waiting times or evidence of improved clinic performance.

## Testing

The prototype has been manually tested for core queue interactions, status updates, filters, browser persistence, simulator calculations, invalid-input handling, and responsive layout.

Testing was performed by the developer using fictional demonstration records. This does not constitute clinical validation, formal usability testing, or verification in a real healthcare setting.

## Privacy and Limitations

CareFlow is an independent demonstration project, not a clinical record system.

- Use fictional demonstration records only.
- Do not enter real patient names, diagnoses, phone numbers, or other identifying health information.
- Queue data is stored in the browser's local storage on the device being used.
- The prototype does not provide a shared, synchronized queue across multiple users or devices.
- The simulator does not model triage, interruptions, breaks, unequal consultation durations, or real patient arrivals.
- The project has not been validated for clinical use.

## Technologies

- HTML
- CSS
- JavaScript
- Browser local storage
- GitHub Pages for hosting

## Future Improvements

- Improve accessibility and usability.
- Expand automated and manual testing.
- Explore more realistic queue models and clearly document their assumptions.
- Gather feedback from appropriate mentors or potential users before considering any real-world use.
- Evaluate privacy and security requirements before handling any real patient information.

## Author

Independent software prototype developed as a learning project.
