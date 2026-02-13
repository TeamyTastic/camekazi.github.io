# Triple Learning Loops

**Status**: Validated prototype (2026-01-28)
**Live URL**: https://teamytastic.github.io/camekazi.github.io/gist/?f7f942b7ba61e9767b297406329d9ab3/triple-learning-loops.html
**Gist**: https://gist.github.com/Camekazi/f7f942b7ba61e9767b297406329d9ab3

---

## What It Does

Analyzes conversation transcripts to identify learning moments at three levels:
- **Loop 1 (Single)**: Fixing problems, tactical improvements ("let's optimize this")
- **Loop 2 (Double)**: Questioning goals, rethinking strategy ("are we solving the right problem?")
- **Loop 3 (Triple)**: Transforming systems, learning how to learn ("our whole process is broken")

## Why It Worked

- **Visual hierarchy**: Concentric circles instantly show which loop dominates
- **Pattern matching feels smart**: Regex scoring assigns sentences to loops automatically
- **Dark theme stands out**: Cyan/magenta/orange on dark = anti-generic-AI aesthetic
- **Slide-in animations**: Each detected moment feels discovered, not just listed
- **Clear definitions**: Loop descriptions help users understand the framework

## Key Interactions

1. **Paste transcript** → Textarea with helpful placeholder examples
2. **Click "Analyze"** → Split sentences, score against patterns, categorize
3. **View stats** → Big numbers show distribution across loops
4. **Concentric viz** → SVG circles with hover effects (opacity + stroke-width changes)
5. **Read moments** → Cards with colored borders, slide-in animations
6. **Reset button** → Return to input, analyze another transcript

## Technical Notes

- Single HTML file: 13KB
- Vanilla JS (no dependencies)
- Pattern matching: Regex arrays for each loop level
- Scoring logic: Higher loop wins (triple > double > single)
- SVG for concentric circles
- Dark theme: `#1a1a2e` → `#16213e` gradient background
- Color system: Cyan (#00d4ff), Magenta (#ff00ff), Orange (#ffaa00)
- Mobile-safe localStorage wrapper (iOS Safari protection)

## Pattern Detection

**Loop 1 patterns**: fix, debug, optimize, bug, error, better, faster
**Loop 2 patterns**: why, should we, rethink, goal, alternative, what if we
**Loop 3 patterns**: process broken, how we learn, meta, paradigm, culture

Priority: If sentence matches multiple loops, assign to highest (3 > 2 > 1).

## What People Would Notice

- Dark theme feels serious/professional (not toy prototype)
- Concentric circles metaphor matches "nested loops" concept
- Pattern matching catches surprisingly nuanced language
- Stats at top create immediate sense of balance/imbalance
- Animation timing feels responsive (0.4s slide-in)

## Next Steps

- [ ] Rebuild with `frontend-design` skill (options: cyberpunk maximalism OR zen minimalism)
- [ ] Add export (download categorized moments as JSON/MD)
- [ ] Add pattern customization (user-defined regex for each loop)
- [ ] Add timeline view (show progression through transcript)
- [ ] Connect to learnings system (promote triple-loop moments to learnings.md)
- [ ] Add comparison mode (analyze multiple transcripts side-by-side)

## Lessons Learned

- **Dark themes work**: Not every prototype needs white background
- **SVG concentric circles**: Simple, semantic, scalable
- **Pattern matching is enough**: Don't need LLM for useful categorization
- **Stats + viz = clarity**: Numbers show what, viz shows why
- **Framework definitions matter**: Clear explanations help users map their own content

## Build Context

**Inspired by**: Chris Argyris's learning loops theory
**Built with**: html-prototyping skill (solution-first, skip process)
**Build time**: ~25 minutes (idea → shareable URL → archived)
**Validation method**: Email share → test with real transcripts

---

**Created**: 2026-01-28
**File size**: 13KB (single HTML file)
**Aesthetic**: Dark cyberpunk (cyan/magenta/orange gradients)
