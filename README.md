# SpendWise - Expense Dashboard

## 1. Layout Techniques Used

### CSS Grid (Main Layout)
Nimetumia Grid kwa layout kuu ya dashboard.
- `.dashboard` -> `display:grid` with `grid-template-columns:250px 1fr` (sidebar 250px, main inachukua iliyobaki)
- `grid-template-rows:70px 1fr` (header 70px)
- `grid-template-areas:"header header" "sidebar main"` - inaweka header juu, sidebar kushoto, main kulia
- `.cards-grid` -> `display:grid` na `grid-template-columns:repeat(3,1fr)` - inaweka cards 3 kwa line moja

### Flexbox (Alignment)
Nimetumia Flexbox kwa alignment ndani ya sections.
- `.header` -> `display:flex; justify-content:space-between; align-items:center` - inaweka logo kushoto na avatar kulia
- `.sidebar` -> `display:flex; flex-direction:column; gap:15px` - inaweka menu items kwa safu wima
- `.card` na `.avatar` -> `display:flex` kwa ku-center content

### Absolute & Relative Positioning
- `.card` -> `position:relative` - parent
- `.badge` -> `position:absolute; top:10px; right:10px` - percentage badge iko juu kulia ya card
- `.avatar` -> `position:relative`
- `.avatar::after` -> `position:absolute; bottom:0; right:0` - green dot ya online status

## 2. CSS Variables
Nimeweka kwenye `:root`:
--p:#6c5ce7 (primary color)
--bg:#f5f6fa (background)
--card:#fff (card background)
--side:#2d3436 (sidebar)
--badge:#dfe6e9
Zinatumika na `var(--p)` - inarahisisha kubadilisha theme.

## 3. Responsive Design
@media(max-width:768px):
- Dashboard inabadilika `grid-template-columns:1fr` na `grid-template-areas:"header" "main" "sidebar"` - sidebar inaenda chini kwa mobile
- Cards zinakuwa `grid-template-columns:1fr` - card moja kwa line

## 4. Animations
- `.card{transition:transform 0.3s}` 
- `.card:hover{transform:translateY(-5px) scale(1.02); box-shadow:0 8px 20px rgba(0,0,0,0.2)}` - inapanda na kuwa kubwa kidogo mtu aki-hover

## 5. Dark Mode
@media(prefers-color-scheme:dark){
:root{--bg:#1e272e;--card:#2f3640;}
}
- Kama user ako na dark mode kwa system, background inakuwa dark.

## Files
- index.html - structure
- style.css - styling yote# SpendWise - Expense Dashboard

## 1. Layout Techniques Used

### CSS Grid (Main Layout)
Nimetumia Grid kwa layout kuu ya dashboard.
- `.dashboard` -> `display:grid` with `grid-template-columns:250px 1fr` (sidebar 250px, main inachukua iliyobaki)
- `grid-template-rows:70px 1fr` (header 70px)
- `grid-template-areas:"header header" "sidebar main"` - inaweka header juu, sidebar kushoto, main kulia
- `.cards-grid` -> `display:grid` na `grid-template-columns:repeat(3,1fr)` - inaweka cards 3 kwa line moja

### Flexbox (Alignment)
Nimetumia Flexbox kwa alignment ndani ya sections.
- `.header` -> `display:flex; justify-content:space-between; align-items:center` - inaweka logo kushoto na avatar kulia
- `.sidebar` -> `display:flex; flex-direction:column; gap:15px` - inaweka menu items kwa safu wima
- `.card` na `.avatar` -> `display:flex` kwa ku-center content

### Absolute & Relative Positioning
- `.card` -> `position:relative` - parent
- `.badge` -> `position:absolute; top:10px; right:10px` - percentage badge iko juu kulia ya card
- `.avatar` -> `position:relative`
- `.avatar::after` -> `position:absolute; bottom:0; right:0` - green dot ya online status

## 2. CSS Variables
Nimeweka kwenye `:root`:
--p:#6c5ce7 (primary color)
--bg:#f5f6fa (background)
--card:#fff (card background)
--side:#2d3436 (sidebar)
--badge:#dfe6e9
Zinatumika na `var(--p)` - inarahisisha kubadilisha theme.

## 3. Responsive Design
@media(max-width:768px):
- Dashboard inabadilika `grid-template-columns:1fr` na `grid-template-areas:"header" "main" "sidebar"` - sidebar inaenda chini kwa mobile
- Cards zinakuwa `grid-template-columns:1fr` - card moja kwa line

## 4. Animations
- `.card{transition:transform 0.3s}` 
- `.card:hover{transform:translateY(-5px) scale(1.02); box-shadow:0 8px 20px rgba(0,0,0,0.2)}` - inapanda na kuwa kubwa kidogo mtu aki-hover

## 5. Dark Mode
@media(prefers-color-scheme:dark){
:root{--bg:#1e272e;--card:#2f3640;}
}
- Kama user ako na dark mode kwa system, background inakuwa dark.

## Files
- index.html - structure
- style.css - styling yote# SpendWise - Expense Dashboard

## 1. Layout Techniques Used

### CSS Grid (Main Layout)
Nimetumia Grid kwa layout kuu ya dashboard.
- `.dashboard` -> `display:grid` with `grid-template-columns:250px 1fr` (sidebar 250px, main inachukua iliyobaki)
- `grid-template-rows:70px 1fr` (header 70px)
- `grid-template-areas:"header header" "sidebar main"` - inaweka header juu, sidebar kushoto, main kulia
- `.cards-grid` -> `display:grid` na `grid-template-columns:repeat(3,1fr)` - inaweka cards 3 kwa line moja

### Flexbox (Alignment)
Nimetumia Flexbox kwa alignment ndani ya sections.
- `.header` -> `display:flex; justify-content:space-between; align-items:center` - inaweka logo kushoto na avatar kulia
- `.sidebar` -> `display:flex; flex-direction:column; gap:15px` - inaweka menu items kwa safu wima
- `.card` na `.avatar` -> `display:flex` kwa ku-center content

### Absolute & Relative Positioning
- `.card` -> `position:relative` - parent
- `.badge` -> `position:absolute; top:10px; right:10px` - percentage badge iko juu kulia ya card
- `.avatar` -> `position:relative`
- `.avatar::after` -> `position:absolute; bottom:0; right:0` - green dot ya online status

## 2. CSS Variables
Nimeweka kwenye `:root`:
--p:#6c5ce7 (primary color)
--bg:#f5f6fa (background)
--card:#fff (card background)
--side:#2d3436 (sidebar)
--badge:#dfe6e9
Zinatumika na `var(--p)` - inarahisisha kubadilisha theme.

## 3. Responsive Design
@media(max-width:768px):
- Dashboard inabadilika `grid-template-columns:1fr` na `grid-template-areas:"header" "main" "sidebar"` - sidebar inaenda chini kwa mobile
- Cards zinakuwa `grid-template-columns:1fr` - card moja kwa line

## 4. Animations
- `.card{transition:transform 0.3s}` 
- `.card:hover{transform:translateY(-5px) scale(1.02); box-shadow:0 8px 20px rgba(0,0,0,0.2)}` - inapanda na kuwa kubwa kidogo mtu aki-hover

## 5. Dark Mode
@media(prefers-color-scheme:dark){
:root{--bg:#1e272e;--card:#2f3640;}
}
- Kama user ako na dark mode kwa system, background inakuwa dark.

## Files
- index.html - structure
- style.css - styling yote# SpendWise - Expense Dashboard

## 1. Layout Techniques Used

### CSS Grid (Main Layout)
Nimetumia Grid kwa layout kuu ya dashboard.
- `.dashboard` -> `display:grid` with `grid-template-columns:250px 1fr` (sidebar 250px, main inachukua iliyobaki)
- `grid-template-rows:70px 1fr` (header 70px)
- `grid-template-areas:"header header" "sidebar main"` - inaweka header juu, sidebar kushoto, main kulia
- `.cards-grid` -> `display:grid` na `grid-template-columns:repeat(3,1fr)` - inaweka cards 3 kwa line moja

### Flexbox (Alignment)
Nimetumia Flexbox kwa alignment ndani ya sections.
- `.header` -> `display:flex; justify-content:space-between; align-items:center` - inaweka logo kushoto na avatar kulia
- `.sidebar` -> `display:flex; flex-direction:column; gap:15px` - inaweka menu items kwa safu wima
- `.card` na `.avatar` -> `display:flex` kwa ku-center content

### Absolute & Relative Positioning
- `.card` -> `position:relative` - parent
- `.badge` -> `position:absolute; top:10px; right:10px` - percentage badge iko juu kulia ya card
- `.avatar` -> `position:relative`
- `.avatar::after` -> `position:absolute; bottom:0; right:0` - green dot ya online status

## 2. CSS Variables
Nimeweka kwenye `:root`:
--p:#6c5ce7 (primary color)
--bg:#f5f6fa (background)
--card:#fff (card background)
--side:#2d3436 (sidebar)
--badge:#dfe6e9
Zinatumika na `var(--p)` - inarahisisha kubadilisha theme.

## 3. Responsive Design
@media(max-width:768px):
- Dashboard inabadilika `grid-template-columns:1fr` na `grid-template-areas:"header" "main" "sidebar"` - sidebar inaenda chini kwa mobile
- Cards zinakuwa `grid-template-columns:1fr` - card moja kwa line

## 4. Animations
- `.card{transition:transform 0.3s}` 
- `.card:hover{transform:translateY(-5px) scale(1.02); box-shadow:0 8px 20px rgba(0,0,0,0.2)}` - inapanda na kuwa kubwa kidogo mtu aki-hover

## 5. Dark Mode
@media(prefers-color-scheme:dark){
:root{--bg:#1e272e;--card:#2f3640;}
}
- Kama user ako na dark mode kwa system, background inakuwa dark.

## Files
- index.html - structure
- style.css - styling yote