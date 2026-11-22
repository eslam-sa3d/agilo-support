# Agilo release notes

New features, improvements and fixes in every version. The same notes are in Agilo: select **What's new** at the top of any Agilo page.

## 2.0.11: Progress bars, chart tooltips and bug states to ignore

_2026-11-22_

- **Improved:** The backlog shows a progress bar for every item instead of days in state: done story points for epics and features, done tasks for stories.
- **Fixed:** The backlog no longer shows "NaN d" for items without a state change date.
- **New:** Project settings › Agilo › Bug statistics: choose bug states (for example Rejected or Duplicate) to leave out of every bug count and chart.
- **New:** Hover any chart to see its values: burnup, cumulative flow, committed vs completed, velocity and the progress bars.
- **New:** The PI burnup marks where each sprint starts, with the sprint's name.
- **New:** Cumulative flow can switch between epics, features and user stories.

## 2.0.10: White text on blue buttons, compact Poker cards

_2026-11-22_

- **Fixed:** Blue buttons (Reveal, Save Estimate, Save, Create) showed dark text; it is white again.
- **Improved:** Planning Poker cards are smaller, with blue numbers, and fit on one line.

## 2.0.9: Faster, safer, ready for Server 2022.1

_2026-11-22_

- **New:** Planning Poker shows each person's profile picture and name instead of "You".
- **Improved:** Faster on large PIs: squad lookups are cached, the backlog, releases and dependency views no longer slow down with thousands of items, and Traceability is cached until you refresh.
- **Improved:** Fewer calls to Azure DevOps: the work item link check waits for typing to settle, Planning Poker pauses while the browser tab is hidden, and the Analytics check uses a tiny query.
- **Improved:** Azure DevOps Server 2022.1: a call refused at REST 7.0 because of its version is retried at 7.1, and an XML-process collection shows Configuration's explanation instead of an error.
- **Improved:** Fewer permissions: Agilo no longer asks for Graph (read). An administrator approves the change once after updating.
- **Fixed:** Traceability warns when a project has more than 20,000 items of a type, the most one Azure DevOps query returns.
- **Fixed:** Shared settings are checked before use, so a malformed value can't break a query or the project on/off list.

## 2.0.8: Field names everywhere

_2026-11-22_

- **Improved:** Messages and pickers show field names (Target Release, Story Points) instead of codes such as Custom.TargetRelease. Codes still show when you hover a field picker.

## 2.0.7: Cleaner capacity table

_2026-11-22_

- **Improved:** Capacity vs load: cells show the number only; the unit (SP) is in the card's description.

## 2.0.6: Planning Poker fix

_2026-11-22_

- **Fixed:** Planning Poker opened as "saved as the final estimate" with no value before anyone voted.
- **Improved:** Planning Poker no longer repeats its title inside the work item form group.

## 2.0.5: What's new page and per-project on/off fix

_2026-11-22_

- **New:** What's new: every Agilo page links to these release notes.
- **Fixed:** Agilo projects could not save on or off (TF400893). The choice is now kept in Agilo's own storage.
- **Improved:** In a project where Agilo is off, its pages, Planning Poker and the link check say so and do nothing.

## 2.0.4: Planning Poker, animated

_2026-11-22_

- **Improved:** Planning Poker is back to its original design: voting cards, avatars of who voted, comments, revealed votes and a saved state.
- **New:** Cards deal in, lift and pop; votes flip in on reveal; the saved tick draws itself. Motion stays off for people who turn on reduced motion.
- **New:** Shows other items of the same type already estimated at your card's value, as a sizing reference.

## 2.0.3: Configuration fix

_2026-11-22_

- **Fixed:** Configuration failed with "The requested version 7.0 of the resource is under preview".

## 2.0.2: Privacy, license and support

_2026-11-22_

- **New:** Privacy policy, license and a support page, linked from the Marketplace listing.

## 2.0.1: Configuration, sprint dashboard and Agilo projects

_2026-11-22_

- **New:** Configuration (Agilo settings): create missing work item types and fields in an inherited process, one by one or all at once.
- **New:** Sprint dashboard in Agilo Squads and Agilo PI Planning, for all squads or one squad.
- **New:** Agilo projects (Organization settings): choose which projects use Agilo.
- **Improved:** Dependencies card redesigned: full squad names, shading, late badges, and cells that open their items.
- **Improved:** Bug and defect counts open their work items as a query.
- **Improved:** Field pickers show field names instead of reference names.
- **Improved:** Sprints tab: sprints and team subscriptions in two full-width rows.
- **Fixed:** Removed the Σ sign from backlog totals.

## 2.0.0: Every screen on your Azure DevOps data

_2026-11-22_

- **New:** Agilo Program: dashboard, backlog, releases, dependencies, risks, objectives and traceability.
- **New:** Agilo Squads and Agilo PI Planning: squad dashboard, teams and capacity, sprints, dependencies, risks and objectives.
- **New:** Agilo settings and Hierarchy rules in Project settings.
- **New:** Planning Poker on the work item form, and a link check that blocks wrong parent links.

## 1.4.3: Sharper icons

_2026-11-22_

- **Improved:** Sharp menu icon and an icon for each hub.
- **New:** Progress bar showing what is built.

## 1.4.1: Marketplace listing

_2026-11-22_

- **Improved:** Full Marketplace description with screenshots and the Agilo logo.

## 1.4.0: First preview

_2026-11-22_

- **New:** Agilo hubs in Azure DevOps Services and Azure DevOps Server 2022.1.
