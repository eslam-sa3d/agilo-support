# Agilo release notes

New features, improvements and fixes in every version. The same notes are in Agilo: select **What's new** at the top of any Agilo page.

## 2.2.1: Bug states in a chart of their own

_2026-11-22_

- **New:** Agilo settings › Bug statistics: set each bug state to Count, Show separately or Ignore. States shown separately, for example Deferred, get their own chart on the Program dashboard, by squad and severity with their age, and are left out of every other bug number.
- **Improved:** The squad dashboard's Defects card says how many bugs sit in the separately shown states.

## 2.2.0: A dashboard you can shape: forecast, squad view, sections

_2026-11-22_

- **New:** Forecast: the PI burnup projects the current pace to the PI's end, and a new tile says how much of the scope will be done by then.
- **New:** Story points done is compared with the previous PI at the same point in its time.
- **New:** Pick a squad at the top of the Program dashboard to see every card, the burnup, cumulative flow and PI health for that squad only.
- **New:** Cards are grouped into Progress, Delivery risks and Quality, with links to jump to each and a fold for each section.
- **New:** Customise: choose which cards show and their order. Your layout is saved for you only.
- **New:** Stories done against the stories committed in the PI: a tile with the totals and a chart of committed vs done stories for every sprint.
- **New:** Releases by iteration: when PIs sit under a release iteration (Release > PI > Sprint), the Releases tab shows the release's progress rolled up from all its PIs, PI by PI.
- **Improved:** Capacity vs load works at PI Planning: before a sprint has finished it uses each squad's velocity from the last PI, and every cell shows the squad's capacity hours on hover.
- **Improved:** The confidence vote is anonymous by default: everyone sees the counts, each person sees only their own vote. Project settings › Agilo settings › PI Planning can show names.
- **Improved:** Objectives: planned business value and committed or uncommitted can be set right in the list during PI Planning; uncommitted objectives are shaded.

## 2.1.1: Prioritise and Portfolio hidden for now

_2026-11-22_

- **Improved:** The Prioritise (WSJF) and Portfolio tabs are hidden from Agilo Program while they are refined. WSJF scores already saved stay on the work items.

## 2.1.0: PI Planning, WSJF, flow metrics and a PI health check

_2026-11-22_

- **New:** Program dashboard opens with PI health: On track, At risk or Off track, the reasons behind it, this sprint at a glance, and how the last PI ended.
- **New:** Data quality card: stories without story points, items outside every squad, orphan stories, missing dates and features without a release, each one click from the list.
- **New:** PI review (PDF): a one-page report for business owners with progress, objectives, predictability by squad, releases, risks and data gaps.
- **New:** Prioritise: score features or epics on business value, time criticality, risk reduction and job size; WSJF is computed, ranked and saved on the work item.
- **New:** Portfolio Kanban: epics by state with WSJF, hypothesis and MVP progress from their features; drag an epic to change its state.
- **New:** Flow: SAFe flow distribution, flow time, flow velocity and flow load for the PI.
- **New:** Program board: features by squad and sprint with release milestones and late dependencies; drag a feature to replan it.
- **New:** Confidence vote: everyone votes 1 to 5 for their squad at the end of PI Planning; averages show for squads and the train.
- **New:** Planning Poker sessions: queue the PI's items and estimate them one after another, together, from Agilo Squads.
- **New:** Traceability matrix shows each test case's last result from Test Plans and exports to Excel (CSV).
- **New:** Releases record the RTE's go / no-go decision, and objective scores record who scored them and when.
- **New:** A setup checklist shows what a project still needs, and every page has a Send feedback link.
- **Improved:** Each screen now has one home: Program for the release train, PI Planning for the event, Squads for teams.
- **Fixed:** Dates from Azure DevOps were read wrongly, so days in state, aging, bug age and cycle time showed NaN or 0. They are correct now, and Aging says No data when dates are missing.

## 2.0.12: Traceability matrix

_2026-11-22_

- **New:** Traceability now has a matrix: start from epics, features or user stories and see each item with what it breaks down into, the test cases that cover it and the bugs linked to it.
- **New:** Filter the matrix by PI and squad, show tasks, or show only rows with gaps such as a feature without stories, a story without a test, or a done item with open bugs.

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
