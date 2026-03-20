Python_Autobot

🚀 Features
Smart Round Detection

> Primary detection via round_start.png image matching (configurable templates and thresholds).

> Fallback row‑movement detection – detects new rounds even if the image trigger fails.

> Automated Betting

> Martingale‑style progression with configurable base bet, max bet, and chip denominations (5,10,20,50).

> Uses the X2 button for efficient bet building.

> Humanized clicking with random delays, offsets, and mouse movement to mimic real‑player behavior.

> Auto‑bet mode can be toggled on/off from the dashboard.

> Real‑Time Dashboard

> Displays current cycle, profit, level, loss streak, and round history percentages.

> Shows runtime and countdown to next controlled restart.

> Buttons to toggle auto‑bet, resume after daily target, and exit gracefully.

> Dashboard auto‑positions on your monitor and is always on top.

> Safety & Limits

> Daily profit target – stops betting when reached (can be overridden).

> Session time limit – stops betting after a set duration.

> Maximum bet limit – resets level and continues monitoring instead of crashing.

> Cycle‑based betting: stops new bets after a configured round (e.g., round 90 of 100).

> Emergency monitor‑only mode when near cycle end with active martingale level.

> Cycle Management

> Tracks 100‑round game cycles, syncing after a full reset.

> Warm‑up period: no betting until the system has enough history (configurable).

> Automatically resets betting after a cycle reset.

> Persistence

> Saves system state (profit, level, bet amount, history, etc.) before restart or exit.

> Loads state on next startup, so you don’t lose progress.

> Configuration saved in spark_settings.ini – edit while the app is closed.

> Calibration Tool

> One‑time setup to click on screen positions for history rows, color references, and bet buttons.

> Saved in spark_calibration.json – reusable across updates.

> Debug Overlay

> Visual feedback on screen for clicks, bet summary, and errors.

> Clusters multiple clicks in the same area to keep the display readable.

> Robust Capture & Stability

> Uses mss (fast screen capture) with periodic restarts to prevent GDI leaks.

> Automatically re‑acquires the Brave window if it’s moved or lost.

> Controlled restart every 40 minutes (configurable) to keep the system fresh.

> Comprehensive Logging

> Logs all actions, errors, and round details to spark_system.log.

> CSV output (spark_results.csv) for round‑by‑round analysis.

> Clean Termination

> Gracefully closes the game window on exit.

> Kills the entire process tree (including the loader) to ensure no leftover background processes.
