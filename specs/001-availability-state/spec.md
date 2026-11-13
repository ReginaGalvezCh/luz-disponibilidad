# Specification 001: Availability State

**Status:** proposal for validation.

## Purpose

Show others whether it is a good time to interrupt, using a signal that the person using the space can understand and control.

## Candidate sources

Manual control; Google Calendar and Google Meet; Outlook Calendar and Microsoft Teams. This list is provisional and does not imply account access or verified compatibility.

## Expected behavior

1. The light shows at least available, unavailable, and unknown states in distinguishable ways without relying on color alone.
2. Manual control allows the person to set unavailable and return to a normal state.
3. A scheduled meeting may suggest occupancy but does not prove that a call is active.
4. An active call may exist without a calendar event.
5. The precedence rule among sources is decided and documented before automation is enabled.
6. The light receives only a derived state, with no meeting titles, participants, or calendar details.
7. If a source is unavailable or authorization expires, the system avoids a false assertion of availability.

## Pilot acceptance criteria

- Manual control changes the signal and allows it to be reverted.
- Another person can distinguish states at the intended viewing distance without relying only on color.
- Once an integration exists, loss of a connected source is visible in the interface or diagnostics.
- No identifiable meeting data is exposed by the physical signal.

## Out of scope for the first pilot

Account authentication, calendar access, automatic call detection, and a central-display connection. These integrations remain part of the product vision and require validation of capabilities, permissions, and privacy before implementation.

## Open questions

What does “available” mean for the person? From where must the signal be readable? Should a busy calendar event activate the light automatically? Can a real call be detected with the available permissions? Which source takes precedence, and for how long? Who can see the state?
