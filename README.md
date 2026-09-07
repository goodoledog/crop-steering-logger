# Crop Steering Logger

Phone-first logger for flower-room crop steering on JR CropTech 1.5 gal coco bags.
Tap zone, bag, checkpoint, type a weight. It prints the P1 shot count or P2 decision
with the rule that made it, and writes the row to the Google Sheet.

| Piece | Where |
|---|---|
| Live app | https://goodoledog.github.io/crop-steering-logger/ |
| How-to (one page) | https://goodoledog.github.io/crop-steering-logger/howto.html |
| GitHub repo | https://github.com/goodoledog/crop-steering-logger (account goodoledog) |
| Backend | Apps Script "Crop Steering Logger API", standalone, in luckydogcannabisco@gmail.com. Web app URL in `apps-script/WEBAPP_URL.txt` |
| Data | Sheet "Crop Steering Master", tabs `CS_Settings`, `CS_Bags`, `CS_Entries`, `CS_Deviations`, `CS_Harvest`. Old tabs untouched. |
| Spec | `SPEC.md` |

## Updating
- Backend: edit `apps-script/Code.gs`, paste into the Apps Script editor (Lucky Dog Cannabis Chrome), Deploy, Manage deployments, New version. Same URL.
- App: edit files in `app/`, upload to the repo (Add file, Upload files). Pages rebuilds in about a minute.
- `setup()` is safe to re-run. `deleteTestRows()` removes rows whose note or reason contains "delete me".

## Before day 1 of a crop
In the app: Me, Room setup. Flip date per zone and the 24 strain names. Saves to CS_Settings and CS_Bags.
Crop of 2026-09: all six zones flipped 2026-09-02 (his word, 2026-09-07).
