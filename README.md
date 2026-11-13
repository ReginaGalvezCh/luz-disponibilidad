# Availability Light

An independent project to make it clear when it is a good time to interrupt someone. The first pilot will use manual control. The product vision includes calendar and active-call signals, subject to permissions and capabilities that still need verification.

## Status

Initial definition. No device or integrations have been implemented. Google Meet, Google Calendar, Microsoft Teams, and Outlook are provisional candidate sources based on the user's stated usage.

## Initial scope

- Show distinguishable available, unavailable, and unknown states.
- Provide manual control and a clear way to override or reset the state.
- Design calendar occupancy and active-call detection as separate signals.
- Define precedence among manual control, calendar, and meeting signals before implementing automation.
- Keep meeting titles, participants, and other details away from the light.

## Documents

- [Pilot specification](specs/001-availability-state/spec.md).
- [Shared method and architecture](docs/method.md).
- [Program coordination in Notion](https://app.notion.com/p/416504754f0881afaaa6e4297e39c813).

## Next decisions

Which personal and work accounts may be connected; available permissions; reliable active-call signals; source precedence; state duration; physical controls; reading distance; and treatment of private data.
