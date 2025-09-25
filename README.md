# dual-timer
雙計時器（配方、多輪、長休息、對調播報）使用說明
Dual Timers with Recipes — Guide
這是什麼？

中文：一個單檔 HTML 的雙計時器工具，專為運動類間歇訓練（Tabata、EMOM、HIIT）、拳擊回合訓練、團課節奏，以及需要工位節拍/輪班提示的場景。A/B 兩組交替倒數，接近結束每秒嗶，到點會**「對調播報」（A 結束播 B 的詞；B 結束播 A 的詞），可設定輪數、自動停止**，並支援每 N 輪插入長休息。含配方下拉、儲存/刪除、一鍵啟動與中英雙語 UI。
English: A single-file HTML dual-timer for interval training (Tabata, EMOM, HIIT), boxing rounds, class pacing, and shift/beep cues. Timers A/B alternate; per-second beeps near the end; end-of-round “swapped speech” (A ends → speak B’s word; B ends → speak A’s word). Set rounds, auto stop, and long rest every N rounds. Includes recipe dropdown, save/delete, one-click start, and Chinese/English UI.

核心特色 / Key Features

交替倒數：A → B → A…
Alternate countdown: A → B → A…

臨界嗶聲：可自訂「剩幾秒開始嗶」。
Critical beeps: choose when beeps start (seconds remaining).

對調播報：A 結束播 B 的詞，B 結束播 A 的詞（例如 A→「休息」、B→「開始」）。
Swapped speech: A ends → speak B’s word; B ends → speak A’s word.

配方管理：下拉選既有配方、儲存/覆蓋、刪除、一鍵啟動。
Recipes: select, save/overwrite, delete, one-click start.

輪數與停止：A→B 算 1 輪；可設定目標輪數與自動停止。
Rounds & stop: A→B = 1 round; set target rounds and auto-stop.

長休息：每 N 輪插入 M:SS 長休，結束續跑。
Long rest: add M:SS rest every N rounds, then resume.

震動提示（可選）、高精度計時、暫停/恢復/重設、本機自動保存。
Optional vibration, high-precision timing, pause/resume/reset, local auto-save.

快速開始 / Quick Start

開啟檔案：用瀏覽器打開 dual-timers-recipes.html。
Open the file in any modern browser.

授權聲音：點一次「開始循環」或「一鍵啟動」，瀏覽器才允許音訊/語音。
Enable audio by clicking Start once (mobile policy).

設置 A/B：在「第一組（A）/第二組（B）」輸入 MM:SS，選「嗶聲起點」，挑播報詞（或自訂）。
Set A/B: duration MM:SS, beep threshold, and end word (or custom).

輪數/長休：在「配方管理」下方設定本次輪數、是否自動停止；需要時設定每 N 輪長休 M:SS。
Rounds/Long rest: choose rounds, auto stop, optional long rest every N rounds.

配方：

輸入名稱 → 按「儲存/覆蓋」建立或更新。

下拉選配方 → 「一鍵啟動」。
Recipes: name it → Save/Overwrite; select from dropdown → Start Selected Recipe.

操作區塊說明 / UI Walkthrough

Timer A / 第一組（A）：設定 A 的時間、嗶聲起點、播報詞（但會在 B 結束時被播出）。
Timer A: A’s duration, beep, and word (spoken when B ends).

Timer B / 第二組（B）：設定 B 的時間、嗶聲起點、播報詞（會在 A 結束時被播出）。
Timer B: B’s duration, beep, and word (spoken when A ends).

Controls：

開始循環 / Start：由 A 開始交替。

暫停 / Pause、繼續 / Resume。

重設 / Reset：停止並重置顯示與狀態。

震動 / Vibration：勾選以啟用手機震動提醒（若裝置支援）。

配方管理 / Recipe Manager：
下拉選擇、命名、儲存、刪除、一鍵啟動。
Select, name, save, delete, one-click start.

推薦用法（運動） / Recommended Training Presets

Tabata：A=20 秒高強度、B=10 秒休息、8 輪、自動停止；A 的詞選「開始/運動」，B 的詞選「休息」。
A=20s work, B=10s rest, 8 rounds, auto stop; A word “Start/Workout”, B word “Rest”.

EMOM（每分鐘工作）：A=40 秒訓練、B=20 秒休息、10 輪；必要時每 5 輪長休 60 秒。
A=40s work, B=20s rest, 10 rounds; long rest 60s every 5 rounds.

拳擊/回合制：A=3:00 對打、B=1:00 休息、X 輪；長休息可設 2:00 每 3 輪。
A=3:00 round, B=1:00 rest, X rounds; long rest 2:00 every 3 rounds.

批判提醒 / Critical nudge：
如果你把 A/B 設成太接近（例如 20/20）卻又在「對調播報」放相反語義，腦內節奏會混亂。原則：A 的字眼=「開始/動起來」，B 的字眼=「休息/緩和」。這樣當 A 結束時播「休息」，B 結束時播「開始」，邏輯是線性的。

進階技巧 / Pro Tips

嗶聲起點：建議設 3–10 秒（視運動強度），太長會變噪音。
Set beeps to last 3–10s near the end to avoid alarm fatigue.

長休息策略：力量循環可「每 3–5 輪長休 1–2 分」，心肺循環可「每 4–8 輪長休 1 分」。
Strength vs cardio need different long-rest cadences.

語音詞彙：用動詞（開始、衝刺、恢復、休息）比名詞更有行動性。
Use verbs (“Start”, “Push”, “Recover”, “Rest”) for better cues.

常見問題 / FAQ & Troubleshooting

為何沒聲音？
行動瀏覽器會封鎖自動播放。務必先點一次開始讓音訊解鎖；靜音模式請關閉或接耳機。
Mobile blocks autoplay—click Start once to unlock audio; turn off silent mode.

背景/鎖屏時停滯？
瀏覽器在背景會節流計時。訓練中請保持畫面開啟；若必須鎖屏，請考慮製作 App 或特殊前景策略。
Background throttling is normal; keep screen on for precise timing.

語音語言：預設 zh-TW。如需英文語音，可在程式把 u.lang = 'en-US'。
Default zh-TW. Change to en-US in code if you want English TTS.

數值設為 0 秒會怎樣？
程式已做防呆：直接觸發結束流程並切換，不會卡死。
Zero-second stages immediately trigger end behavior and switch.

安全與責任 / Safety Notes

高強度訓練請量力而為；初學者從較少輪數與更長休息開始。
Scale intensity responsibly; new to HIIT? Fewer rounds, longer rests.

在戶外或交通附近訓練時，不要完全依賴耳機提示，請確保環境安全。
Stay aware of surroundings if training outdoors or near traffic.
