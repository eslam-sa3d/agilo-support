# Agilo privacy policy

Effective 22 November 2026.

Agilo is an extension for Azure DevOps Services and Azure DevOps Server, published by SAFeADO.

## What Agilo collects

Nothing. Agilo has no servers, no database and no analytics of its own. It does not track you, does not use cookies, and does not send data to the publisher or to any third party.

## Where your data stays

- **Work items, teams, sprints and capacity** are read from and written to your own Azure DevOps organization or collection, through the Azure DevOps REST APIs, as the signed-in user.
- **Agilo settings** (field map, Definition of Ready, Planning Poker decks, hierarchy rules and Planning Poker rooms) are stored in Azure DevOps extension data storage, inside your organization or collection.
- **Per-project on/off** is stored as an Azure DevOps feature setting in your organization or collection.

Everything runs in your browser inside Azure DevOps. Nothing leaves your Azure DevOps environment.

## Permissions

Agilo asks Azure DevOps for these permissions and uses them only for the features described:

| Permission | Used for |
| --- | --- |
| Work items (read and write) | Show and update backlog items, risks, objectives and estimates |
| Work items and process (full) | Only when an administrator uses Configuration to create missing work item types and fields |
| Project and team (read) | Read teams, members, sprints and capacity |
| Analytics (read) | Burnup, velocity and cumulative flow charts |
| Identity (read) | Show who changed settings and who is in a Planning Poker room |

## Removing your data

Uninstall Agilo from your organization or collection. Its settings in extension data storage are removed with it. Fields or work item types an administrator created with Configuration stay in your process until you remove them.

## Changes and contact

Changes to this policy are published here with a new effective date. Questions: open an issue at https://github.com/eslam-sa3d/agilo-support/issues.
