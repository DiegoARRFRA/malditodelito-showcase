<p align="center">
  <img src="assets/cover.svg" alt="MalditoDelito — Case, document and calendar management" width="100%">
</p>

# MalditoDelito

**Keep the context of each case in one place.**

A Windows desktop application being developed for small legal practices, with an expanding property community management module. Built with Flutter, Dart and Supabase.

[Español](README.md) · [Gallery](docs/GALERIA.md) · [Architecture](docs/ARQUITECTURA.md) · [Roadmap](docs/ROADMAP.md)

## The problem

Case information often lives across contact lists, folders, documents and calendars. MalditoDelito brings people, case activity, document versions and scheduled work into a connected desktop workflow.

The project starts from practical organisational needs in a small practice. Development and validation currently use fictional data.

## Current capabilities

| Area | Scope | Status as of 29 October 2026 |
| --- | --- | --- |
| Contacts | Searchable directory, groups, profiles and reversible retirement with historical relationships preserved. | Integrated |
| Cases | Related people, notes, activity records and annual numbering per workspace. | Integrated |
| Documents | Private storage, version history, out-of-court/court categorisation and selected downloads. | Integrated |
| Calendar | Month/week/day/agenda views, recurring events, exceptions and personal review status. Reminders while the app is open. | Integrated |
| Shared workspace | Authentication, server-side access controls, Realtime updates and conflict-aware writes. | Integrated |
| Export | A complete case ZIP with documents, versions, a manifest and readable HTML. | Integrated |
| Backups | Manual snapshots, local read-only browsing, comparison and version extraction. | Partial; full recovery remains pending |
| Property communities | Properties, owners/occupants, history, meetings and versioned minutes. | Implemented on a review branch; not yet integrated |
| Financial and operational modules | Financial tracking, suppliers, contracts, renewals and maintenance incidents. | Planned |
| AI assistance | Potential support for retrieval, summaries and drafts with human review. | Future direction; not implemented |

“Integrated” describes the main development branch. It does not mean production readiness or completion of a user pilot.

## Interface preview

![MalditoDelito calendar and personal review panel using fictional demonstration data](assets/screenshots/agenda.jpg)

*Development widget render from 28 October 2026, captured for this showcase. It is a demonstration of the interface, not a production deployment or a manual acceptance test. See the [gallery notes](docs/GALERIA.md).*

| Contacts | Cases |
| --- | --- |
| ![Contact directory with fictional examples](assets/screenshots/contactos.jpg) | ![Case details with fictional participants](assets/screenshots/expediente.jpg) |

*Development iterations from 25 and 26 October 2026, respectively.*

## Engineering approach

- Flutter/Dart desktop interface, currently focused on Windows.
- Supabase Auth, PostgreSQL and row-level security for shared workspaces.
- Private document storage with immutable versions and integrity checks.
- Realtime notifications followed by authorised reads; explicit conflict handling and idempotent retries.
- A separate individual mode using SQLite and local documents.
- Python tooling for backups and local historical consultation.

The individual and shared stores are independent. This is not an offline write-sync system, and shared writes require connectivity. No macOS, Android or iOS release is announced here.

## Development stage

**Early development.** Full recovery, protection review, installer and multi-machine pilot work remain on the roadmap. Existing automated checks and Windows validation do not replace human acceptance, a full pilot or compliance assessment.

Future AI assistance is exploratory. Scope, provider integration, data permissions and operating costs remain to be defined; no AI connection is currently active in the application.

## About this repository

This is a public product showcase. It contains selected documentation and demonstration imagery. Application source code, credentials, deployment configuration, client records, databases and operational backups are not distributed here. There is no public installer in this repository.

Created and directed by **[Diego de Arriba](https://github.com/DiegoARRFRA)**. Product and presentation feedback is welcome through [public issues](https://github.com/DiegoARRFRA/malditodelito-showcase/issues); do not include private records or credentials.

The product is not released as open source. See [NOTICE.md](NOTICE.md).

*Last reviewed: 29 October 2026.*
