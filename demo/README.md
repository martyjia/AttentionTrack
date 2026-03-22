# ZenScroll Demo (Web Prototype)

## Run
```bash
cd ~/code_projects/zenscroll-hackathon/demo
python3 -m http.server 8080
```
Open: http://localhost:8080

Pages:
- `index.html` → iOS-style polished visual demo
- `mvp.html` → MVP behavior demo (monitor → trigger → intervention → metrics/log/snapshot)

## What MVP demo (`mvp.html`) shows
- App selection + daily threshold
- AI-adjusted threshold stub (`aiThreshold`)
- Background monitoring (silent by default)
- Friction states: none / slowDown / grayscale
- 10-second mandatory breathing gate at threshold
- Metrics: triggered interventions, completion rate, estimated minutes prevented
- Evidence layer: intervention log + snapshot save/restore (localStorage)

## Suggested 90-second MVP script
1. Start monitor with low usage (no interruption).
2. Let usage rise near threshold (slowDown state, still silent).
3. Cross threshold (grayscale + breathing gate appears).
4. Complete gate and show metric/log updates.
5. Save snapshot to show persistent daily evidence.
