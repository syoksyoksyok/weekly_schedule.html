# Weekly Life Rhythm Scheduler

生活リズムを整えることを目的とし、気軽に編集できるシンプルな週間スケジューラーを HTML 単体で作りました。

「高機能タスク管理」ではなく、

- なんとなく生活を整えたい
- 起床・就寝を可視化したい
- スマホで気軽に編集したい
- ざっくり1週間を眺めたい

という用途向けです。

---

## Features

- Single HTML file
- No server required
- Mobile-first layout
- Monday–Sunday tab switching
- Calm greige color palette
- Add / delete rows with one tap
- Row height changes according to duration
- AM / PM / EVENING section dividers
- Undo / Redo
- Copy & paste entire weekday schedules
- Automatic sleep duration calculation
- Local auto-save using localStorage
- Desktop HTML export with embedded schedule data
- GitHub Pages compatible

---

## Designed For

This scheduler is intentionally simple.

It does NOT include:

- notifications
- reminders
- cloud sync
- account systems
- heavy task management features

The goal is to make schedule editing feel lightweight and low-pressure.

---

## Sleep Tracking

When selecting `就寝` from the time menu:

- the row becomes a sleep row
- the next day’s first schedule is automatically detected
- estimated sleep duration is calculated automatically

Example:

23:30 → sleep  
06:30 → wake up

↓

就寝（睡眠時間：7時間）

---

## Mobile Usage

Recommended workflow:

1. Edit on PC
2. Export HTML using 💾
3. Place exported HTML into Dropbox
4. Open/edit from smartphone browser

Smartphone browsers can edit schedules normally.

However, HTML export is intentionally disabled on mobile devices because download behavior is unstable on some mobile browsers and in-app browsers.

---

## Controls

### Header buttons

| Button | Action |
|---|---|
| ⟲ | Undo |
| ⟳ | Redo |
| ⧉ | Copy current weekday |
| ⤓ | Paste copied weekday |
| 💾 | Export current state as HTML (desktop only) |

### Row buttons

| Button | Action |
|---|---|
| ↑ | Add row above |
| ↓ | Add row below |
| × | Delete row |

---

## Persistence

Schedule data is automatically saved to browser localStorage.

Exported HTML files also contain embedded schedule data, allowing schedules to be transferred between devices simply by sharing the HTML file itself.

---

## Notes

- Mobile HTML export is disabled intentionally
- localStorage may be cleared by browser cleanup
- Only lightly tested on iPhone and Android devices
- Intended as a lightweight personal rhythm tool

---

## GitHub Pages

This project works well with GitHub Pages.

Example:

https://yourname.github.io/weekly-scheduler/

---

## License

MIT
