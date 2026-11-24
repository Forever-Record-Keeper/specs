# Glossary

The project uses 1 word for each concept.
This glossary lists the words, what they mean, and the words not to use for the same concept.
Add a new term here before you use it in a spec, in code or in the docs.

The release of the FRK Vale package turns the terms into a vocabulary (decision 0021).

<!-- Until the release of the Vale package reads this file, the new terms fail the spelling check. -->
<!-- vale FRK.Spelling = NO -->

## System names

In a requirement, the system is always 1 of these terms.

| Term | Meaning | Don't use |
| --- | --- | --- |
| addon | The add-on for the game client. It turns on logging, offers keybinds and the dungeon reminder, and sends screenshot signals. | `add-on`, `plugin`, `mod` |
| app | The desktop app of Forever Record Keeper, with a tray icon. It controls OBS, reads the logs, manages storage and runs the library. | `agent`, `tool`, `application`, `client` |
| library | The part of the app that shows sessions in a browser, on this PC or on the local network. | `web library`, `web UI`, `server` |
| website | The project website. | `homepage`, `site` |

## Game and services

| Term | Meaning | Don't use |
| --- | --- | --- |
| Archon App | The official uploader of Warcraft Logs. It uploads the combat logs. | `uploader`, `WCL uploader` |
| character | A character of the player in the game. The app detects it per segment. | `toon`, `alt` |
| chat log | The file `WoWChatLog.txt` that the game writes, with loot, quests, resets and chat. | |
| combat log | A file `WoWCombatLog-*.txt` that the game writes during play, with each combat event. | `log file` |
| dungeon | An instance for a small group. | |
| encounter | A boss fight. The combat log marks its start and end. | `boss fight` |
| flavor | An installed edition of the game, such as Forever, Classic or Retail. Each flavor has its own folder. | `version`, `edition` |
| game | World of Warcraft Forever, the game that the app records. | `WoW` in requirements |
| guild member | Another player in the same guild. | `guildmate` |
| hotkey | A global keyboard shortcut of the app. It works while the game has focus. | `shortcut` |
| instance | A dungeon or a raid. Each group gets its own copy of it. | |
| keybind | A key binding inside the game, set in the key bindings menu of the game. | `binding`, `hotkey` |
| OBS | OBS Studio, the recording program that the app controls over its WebSocket. | |
| player | The person who plays the game and uses the app. | `user`, `gamer` |
| raid | An instance for a large group. | |
| report | A report on Warcraft Logs, with the fights of a span of play. | `log` |
| Warcraft Logs | The website that analyzes combat logs. Short form: WCL. | |
| zone | An area of the game world. The combat log marks each zone change. | `map` |

## Recording

| Term | Meaning | Don't use |
| --- | --- | --- |
| clip | A short video from the replay buffer, saved with a hotkey. | `highlight` |
| grace period | The time after the game exits before the app stops the recording. Default: 2 min. | `timeout` |
| health check | The check of a test recording or the first session: tracks, chapters, dropped frames and bitrate. | |
| lead-in | The part of the replay buffer that the app saves in front of a recording that starts late. | `pre-roll` |
| preflight check | The check before each recording start: format, track layout and free disk space. | |
| recording | 1 video file that OBS writes during a session. | `video`, `capture` |
| replay buffer | The memory buffer of OBS that keeps the last minutes of video. | |
| screenshot signal | A screenshot in a special format. The addon creates it, and the app reads it as a command. | |
| session | A span of play from the game start to the game exit, plus the grace period. It holds recordings, logs and clips. | `play session`, `stream` |
| start mode | The choice between an automatic start with the game and a manual start from the addon. | `recording mode` |
| track | 1 audio track in a recording: Mix, Game, Mic or Discord. | `channel` |

## Tagging

| Term | Meaning | Don't use |
| --- | --- | --- |
| chapter | A named point in a recording, for a pull, a zone change or a marker. | `bookmark` |
| event | A moment that the app finds in the logs, such as a pull, a death or a loot. | |
| kill | A pull that ends with the death of the boss. | |
| marker | A moment that the player marks with a hotkey or a screenshot. | `bookmark`, `flag` |
| pre-roll | The time that a chapter or a jump starts before its event. Default: 5 s. | `offset`, `lead-in` |
| pull | 1 attempt at an encounter, from its start to its end. It ends in a kill or a wipe. | `attempt`, `try` |
| run | 1 pass through an instance, from the entry or a reset to the exit. | |
| segment | A stay in a zone or a run within a session, with its character. | `section` |
| sidecar file | The JSON file next to a recording, with its events and chapters. | |
| tagging | The work of the app that finds events in the logs and writes chapters. | `labeling` |
| trash wipe | 3 or more group deaths within 60 s while no encounter is active. | |
| wipe | A pull that ends with the death of the group. | |

## Storage

| Term | Meaning | Don't use |
| --- | --- | --- |
| budget | The disk space that recordings may use in total. | `quota`, `cap` |
| excerpt | A part of a recording that the player exports. | `cut`, `snippet` |
| keep flag | A mark on a session, run or pull. The app never deletes what it marks. | `pin`, `favorite` |
| tier | The storage state of a recording: tier 1 as recorded, tier 2 compressed. | `level` |

## Library

| Term | Meaning | Don't use |
| --- | --- | --- |
| log pane | The part of the library that shows the combat log lines next to the video. | `log view` |
| share link | A link with a random token. It opens the library on another device on the local network. | `invite`, `login` |
| timeline lane | A row under the video that shows 1 kind of event, such as pulls or deaths. | `track` |

## Process

| Term | Meaning | Don't use |
| --- | --- | --- |
| agent | An AI coding agent that works on the project. | |
| capability | A part of the product behavior with its own spec, such as recording or storage. | `feature`, `module` |
| change | A planned change to behavior, as an OpenSpec change in the `specs` repo. It can touch several repos. | `feature request`, `epic` |
| check | An automated test of code or text that must pass, such as a lint or the coverage limit. | `gate` |
| decision record | A short file in `decisions/` that records 1 decision and its reason. | `ADR` |
| fix | A small change in 1 repo, through an issue and a PR. | `hotfix`, `patch` |
| maintainer | The person who reviews and merges every PR. | `owner`, `admin` |
| requirement | 1 sentence in an EARS pattern with SHALL. | `user story` |
| scenario | An example of a requirement with GIVEN, WHEN and THEN, named with its scenario ID. | `test case` |
| scenario ID | The ID of a scenario, such as `REC-01`. The Gherkin scenario has it as a tag. | |
| store | The OpenSpec store `forever-record-keeper`, which is the `specs` repo. | |

<!-- vale FRK.Spelling = YES -->
