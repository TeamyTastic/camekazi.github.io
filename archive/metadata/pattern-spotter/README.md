# Pattern Spotter

**Status**: Validated prototype (2026-01-28)
**Live URL**: https://teamytastic.github.io/camekazi.github.io/gist/?cbfb3f3e3fbf11c9cf175799603ad169/pattern-spotter.html
**Gist**: https://gist.github.com/Camekazi/cbfb3f3e3fbf11c9cf175799603ad169

---

## What It Does

Tracks behavioral patterns you notice in real-time. Click cards to increment occurrence count. Celebrates when patterns hit 3+ occurrences (operationalization threshold).

## Why It Worked

- **Immediate feedback**: Every click triggers animation (✓ or 🎯)
- **Clear progression**: Visual journey from 1 → 2 → 3 occurrences
- **Meaningful celebration**: 🎯 emoji + alert at threshold + pulsing badge
- **Stats dashboard**: Creates "game feel" - tracking your own pattern recognition
- **Zero friction**: No login, no setup, just start tracking

## Key Interactions

1. **Form submission** → Creates new pattern card
2. **Click card** → Increments count with ✓ animation
3. **Hit 3 occurrences** → Triggers 🎯 celebration + threshold alert
4. **Pulsing badge** → Visual indicator for patterns ready to operationalize
5. **Stats auto-update** → Live count of total patterns, occurrences, ready-to-operationalize

## Technical Notes

- Single HTML file: 7KB total
- Vanilla JS (no dependencies)
- localStorage with mobile-safe wrapper (iOS Safari file:// protection)
- Gradient aesthetic: Purple (#667eea → #764ba2)
- Touch-friendly: 44px minimum tap targets
- Animations: CSS transitions + scale transforms
- Time formatting: Custom `timeAgo()` function

## What People Noticed

- "The pulsing badge makes me WANT to hit 3"
- Celebration timing feels rewarding (not annoying)
- Stats at top create progress sense
- Example patterns on first load help understanding

## Next Steps

- [ ] Rebuild with `frontend-design` skill (choose: bold maximalist or refined minimal)
- [ ] Add pattern export (download JSON backup)
- [ ] Add pattern relationships (graph view using D3)
- [ ] Add pattern categories/tags
- [ ] Connect to learnings.md (auto-promote at 5+ occurrences)

## Lessons Learned

- **Solution-first works**: Built in 15 minutes, validated in first share
- **Celebration matters**: Small details (🎯 vs ✓) create emotional connection
- **Thresholds create goals**: The "3" target emerged from 5x promotion rule in learnings system
- **Inline everything**: Single file = easy to share, no deployment complexity

---

**Created**: 2026-01-28
**Build time**: ~15 minutes (idea → shareable URL)
**Validation method**: Email share → immediate positive reaction
