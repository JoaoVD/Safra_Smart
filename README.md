# SafraSmart

### Connecting agricultural producers and buyers.

SafraSmart is an agricultural marketplace project designed around two ways to trade: **direct sales** and **auctions**. It explores how a mobile interface, timely bid notifications and agricultural market information can make commercial opportunities easier to discover.

**Status:** in development. This public repository currently contains project documentation; application source code, a runnable release and screenshots have not been uploaded here. The sections below describe the project's scope and intended technical architecture, rather than a verified build in this repository.

## The problem

Producers and buyers need a clear way to discover products, distinguish fixed-price offers from auctions and follow changes to bids. SafraSmart brings these workflows into a single mobile product concept.

## Product scope

| Area | Project scope |
| --- | --- |
| Marketplace | Product registration, product search and direct-sale / auction filters |
| Auctions | Bid notifications for the seller and the previous leading bidder |
| Accounts | Producer and buyer accounts backed by Firebase Authentication |
| Market information | Agricultural quotations, including soybeans, corn, coffee, cattle and the US dollar |
| Shipping | Shipping calculations through a Melhor Envio sandbox integration |
| Background updates | Scheduled quotation and freight-table update workflows |

These capabilities belong to the development scope. They cannot yet be tested or audited from this documentation-only repository.

## Technical direction

| Layer | Technology |
| --- | --- |
| Mobile application | Flutter / Dart |
| Authentication | Firebase Authentication |
| Application data | Cloud Firestore |
| Product media | Firebase Storage |
| Push notifications | Firebase Cloud Messaging |
| Backend workflows | Cloud Functions for Firebase, second generation |

Android is the initial target. iOS support is planned and is not represented as a published release.

### Main data domains

- Products and sale types.
- Users and account information.
- Market quotations.
- Application configuration.

### Backend workflow responsibilities

The project includes work on bid notifications, scheduled and manually triggered quotation updates, shipping calculations and freight-table updates. Shipping integration is intended for sandbox testing at this stage.

## Engineering focus

- Keep direct-sale and auction journeys easy to distinguish.
- Move notification and scheduled-update responsibilities into backend workflows.
- Use an explicit sandbox boundary for shipping integration.
- Make product discovery and the daily mobile experience straightforward.
- Document configuration and integration requirements alongside the application source when it is published.

## Running locally

Local setup instructions are pending the source-code upload. This repository does not currently contain a Flutter manifest, Firebase project configuration, backend dependency manifest or executable application.

Once source is available, this section should document:

1. The required Flutter, Dart and Node.js versions.
2. Firebase project setup and local configuration.
3. Backend and sandbox integration configuration.
4. Commands for installing dependencies, running the app and executing checks.
5. Any test accounts or emulator workflow needed for a reproducible demonstration.

No installation or test commands are provided until they can be checked against the actual project.

## Next documentation milestones

- [ ] Publish the reviewed application source.
- [ ] Add screenshots and a short walkthrough captured from the app.
- [ ] Document the source layout and configuration.
- [ ] Verify and publish local run instructions.
- [ ] Document automated checks and known limitations.
- [ ] Add a license before offering reuse rights.

## Author

**João Vitor Dalseno**  
Software Engineering student · Brazil

[GitHub](https://github.com/JoaoVD) · [Contact](mailto:joaovitordalseno@gmail.com)

---

This repository is a work in progress. No production availability, commercial traction or measured outcomes are claimed.
