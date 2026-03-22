# ZenScroll Demo (Web Prototype)

## Run
```bash
cd ~/code_projects/zenscroll-hackathon/demo
python3 -m http.server 8080
```
Open: http://localhost:8080

## What this demo shows
- App selection + daily threshold
- AI-adjusted threshold stub (`aiAdjustedThreshold`)
- Friction states: none / slowDown / grayscale
- 10-second mandatory breathing gate
- Simple metrics for hackathon judging

## Suggested 90-second demo script
1. Start at low usage → open app normally.
2. Increase usage to 80% threshold → show slowDown + breathing gate.
3. Increase usage above threshold → grayscale + gate.
4. Show "intercepted opens" and "minutes prevented" metrics.
