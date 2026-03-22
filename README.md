# ZenScroll Hackathon Summary & Ideas

## Hackathon Details
- **Event:** Pioneering Minds AI: Grayscale Hackathon
- **Theme:** The Dual Nature of AI — Dark vs. Light
- **Track:** Attention
- **Tagline:** Mindful by design. Friction on purpose.

## Main Project: ZenScroll
ZenScroll is an OS-level iOS application built on Apple's `FamilyControls` and `DeviceActivity` frameworks.

Core principle: **Don't hard-block. Add calibrated friction to trigger reflection.**

### Core Features
1. **App selection + threshold control** using `FamilyActivityPicker` and `ManagedSettingsStore`.
2. **Friction engine** with 3 intervention states:
   - `<75%`: none
   - `75–99%`: slowDown warning
   - `>=100%`: grayscale mode
3. **10-second breathing gate** before continuing.
4. **Shield extensions** for system-level intervention UX.

### AI Expansion Point
`aiAdjustedThreshold()` in `FrictionEngine.swift` is the intended CoreML integration point for dynamic thresholding.

## Other Brainstormed Ideas
- **RealShield (Truth):** Deepfake anomaly signal during live calls.
- **FairHire (Access):** Bias auditor for job descriptions and screening outputs.

## Build/Test Notes
- `FamilyControls` behavior requires **physical iOS device**.
- Keep App Group ID consistent across all targets.

## Next-Step Product Questions
- What measurable behavior change defines success (screen time drop? fewer compulsive opens?)
- What false-positive rate is acceptable for interventions?
- What intervention level maximizes retention + wellbeing impact?
