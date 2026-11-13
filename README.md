# Availability Light

An independent project to make it clear when it is a good time to interrupt someone. The first pilot will use manual control. The product vision includes calendar and active-call signals, subject to permissions and capabilities that still need verification.

## Status

Public design and discovery stage. The repository currently contains specifications and a proposed technology map; it does not yet contain firmware, a working device, or account integrations. Google Meet, Google Calendar, Microsoft Teams, and Outlook are provisional candidate sources, not verified integrations.

## Initial scope

- Show distinguishable available, unavailable, and unknown states.
- Provide manual control and a clear way to override or reset the state.
- Design calendar occupancy and active-call detection as separate signals.
- Define precedence among manual control, calendar, and meeting signals before implementing automation.
- Keep meeting titles, participants, and other details away from the light.

## Technology map

| Area | Current direction | Status |
| --- | --- | --- |
| Physical signal | A locally controlled light with available, unavailable, and unknown states readable without color alone. | First-pilot behavior; light and control hardware open. |
| Calendar sources | Google Calendar and Outlook are candidate sources for scheduled busy time. | Product scope; account permissions and integration method unverified. |
| Active-call sources | Google Meet and Microsoft Teams are candidate sources for actual calls. | Product scope; detection capability and permissions unverified. |
| State logic | Keep manual, calendar, and active-call signals separate; define precedence and failure behavior before automation. | Architecture decision pending. |
| Localization | English source copy and Spanish translation. Use Lingui if the control interface is JavaScript/TypeScript. | Language direction agreed; Lingui not installed. |
| Platform and power | Controller, connectivity, power, and enclosure. | Open pending placement and integration tests. |

## Documents

- [Pilot specification](specs/001-availability-state/spec.md).
- [Shared method and architecture](docs/method.md).

## Next decisions

Which personal and work accounts may be connected; available permissions; reliable active-call signals; source precedence; state duration; physical controls; reading distance; and treatment of private data.

## Follow the work

This project is being shared early so its requirements, experiments, and trade-offs can be reviewed as they develop. The pilot specification describes intended behavior, not a validated device. Upcoming measurements and design decisions will be recorded here; GitHub Issues will track bounded next steps. Suggestions and questions are welcome through Issues.

## First development cycle (planned)

The next inspectable artifact is a local, manual-only availability simulator. It can test interaction and localization before a physical device or account integration exists. Work is tracked in small issues:

1. [Validate the viewing scenario and manual states](https://github.com/ReginaGalvezCh/luz-disponibilidad/issues/2).
2. [Define state transitions and the privacy boundary](https://github.com/ReginaGalvezCh/luz-disponibilidad/issues/3).
3. [Build and test an accessible English/Spanish simulator](https://github.com/ReginaGalvezCh/luz-disponibilidad/issues/4).
4. [Exercise external signals with synthetic fixtures](https://github.com/ReginaGalvezCh/luz-disponibilidad/issues/5).
5. [Assess Google and Microsoft integration feasibility](https://github.com/ReginaGalvezCh/luz-disponibilidad/issues/6).

The simulator will not claim that calendar or active-call detection works with real accounts. Hardware, account permissions, and source precedence remain open decisions.

## Safety and privacy

Do not publish OAuth credentials, access tokens, work account information, calendar events, meeting titles, participant names, or schedules. Any future demo should use synthetic data and expose only a derived availability state.

## License

[MIT](LICENSE) covers the current repository content. Hardware design files, if added later, will have their licensing and manufacturing information reviewed before publication.
