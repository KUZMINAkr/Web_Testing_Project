# UI Bugs Report — DemoQA Website

This folder contains screenshots and descriptions of UI bugs discovered during manual testing of several DemoQA components.

Below is a detailed list of defects, including steps to reproduce, expected vs. actual results, and screenshots.

---

## 🐛 Bug 1 — WebTables Page Loads Empty

**Steps to reproduce:**
1. Open https://demoqa.com/webtables  
2. Observe the page content

**Expected result:**
Default table rows should be displayed.

**Actual result:**
The entire table section loads empty, showing no records.

**Screenshot:**  
`webtables.png`

---

## 🐛 Bug 2 — Book Details Page Shows White Screen

**Steps to reproduce:**
1. Open https://demoqa.com/books  
2. Click any book  
3. Observe the page

**Expected result:**
Book details should load.

**Actual result:**
White blank screen appears.

**Screenshot:**  
`books white.png`

---

## 🐛 Bug 3 — "No" Button Is Not Clickable

**Steps to reproduce:**
1. Open https://demoqa.com/radio-button  
2. Try to click “No”

**Expected:**
Radio button should be selectable.

**Actual:**
Click does nothing — button is disabled.

**Screenshot:**  
`button NO.png`

---

## 🐛 Bug 4 — Slider Drags Incorrectly

**Steps:**
1. Open https://demoqa.com/slider  
2. Try dragging the slider circle

**Expected:**
Slider moves smoothly following the cursor.

**Actual:**
- Moves only by **1 step**  
- Shows a “forbidden” cursor icon  
- Feels broken and not interactive

**Screenshot:**  
`Slider.png`

---

## 🐛 Bug 5 — Grid Items Stick to Cursor

**Steps:**
1. Open https://demoqa.com/selectable  
2. Switch to **Grid** tab  
3. Select items quickly

**Expected:**
Selection should toggle cleanly.

**Actual:**
Numbers “stick” to cursor visually.

**Screenshot:**  
`grid.png`

---

## 🐛 Bug 6 — List Items Stick to Cursor

Same as the previous bug but in List mode.

**Screenshot:**  
`list.png`

---

## 🐛 Bug 7 — More Button Inactive

**Steps:**
1. Open https://demoqa.com/menu  
2. Hover or click **More**

**Expected:**
Dropdown submenu should activate.

**Actual:**
“More” is not clickable.

**Screenshot:**  
`More.png`

---

## 🐛 Bug 8 — Resizable Box Behaves Incorrectly

**Steps:**
1. Open https://demoqa.com/resizable  
2. Try resizing the small box

**Expected:**
Should resize smoothly within limits.

**Actual:**
Box jumps, lags, and behaves inconsistently.

**Screenshot:**  
`resizable.png`

---

# ✔ Summary

All bugs were reproducible and visually confirmed.  
This collection demonstrates UI testing, exploratory testing, and bug reporting skills.
