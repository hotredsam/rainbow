# Graph Report - .  (2026-06-07)

## Corpus Check
- Corpus is ~1,849 words - fits in a single context window. You may not need a graph.

## Summary
- 42 nodes · 38 edges · 7 communities (6 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Package Config|Package Config]]
- [[_COMMUNITY_React Dependencies|React Dependencies]]
- [[_COMMUNITY_PWA Manifest|PWA Manifest]]
- [[_COMMUNITY_NPM Scripts|NPM Scripts]]
- [[_COMMUNITY_App Entry Point|App Entry Point]]

## God Nodes (most connected - your core abstractions)
1. `scripts` - 5 edges
2. `browserslist` - 3 edges
3. `eslintConfig` - 2 edges
4. `private` - 1 edges
5. `@testing-library/jest-dom` - 1 edges
6. `@testing-library/react` - 1 edges
7. `@testing-library/user-event` - 1 edges
8. `react` - 1 edges
9. `react-dom` - 1 edges
10. `react-scripts` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (7 total, 1 thin omitted)

### Community 0 - "Package Config"
Cohesion: 0.22
Nodes (8): browserslist, development, production, eslintConfig, extends, name, private, version

### Community 1 - "React Dependencies"
Cohesion: 0.25
Nodes (8): dependencies, react, react-dom, react-scripts, @testing-library/jest-dom, @testing-library/react, @testing-library/user-event, web-vitals

### Community 2 - "PWA Manifest"
Cohesion: 0.25
Nodes (7): background_color, display, icons, name, short_name, start_url, theme_color

### Community 4 - "NPM Scripts"
Cohesion: 0.40
Nodes (5): scripts, build, eject, start, test

## Knowledge Gaps
- **25 isolated node(s):** `name`, `version`, `private`, `@testing-library/jest-dom`, `@testing-library/react` (+20 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `dependencies` connect `React Dependencies` to `Package Config`?**
  _High betweenness centrality (0.145) - this node is a cross-community bridge._
- **Why does `scripts` connect `NPM Scripts` to `Package Config`?**
  _High betweenness centrality (0.090) - this node is a cross-community bridge._
- **What connects `name`, `version`, `private` to the rest of the system?**
  _25 weakly-connected nodes found - possible documentation gaps or missing edges._