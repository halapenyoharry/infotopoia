# infotopoia

*A spatial information medium.*

---

## What this is

Information has topology. It already exists. It has peaks and valleys, density and sparsity, proximity and distance between ideas. Every platform you've ever used hides this from you. Feeds, timelines, and search results flatten it into a line. infotopoia doesn't create a new structure — it exposes the one that was already there.

This is not a metaphor.

---

## The interface

The graph is not a view of the content. The graph **is** the interface. Reading, writing, exploring, and organizing all happen in the same coordinate space.

When you click a node, the article opens inside it — the node expands in place, automatically resizing to fit the content. The graph doesn't go away. Or you open it in a side panel that slides in alongside the graph, leaving you free to continue scrolling, zooming, and exploring connections while you read. A button enables scroll-in-panel when the content is long. Nothing is obscured. The map and the territory occupy the same screen.

When you write, you write in the graph. The editor opens in the side panel, or inside the node itself. As you write, connections form in real time. You watch the topology shift as you type.

---

## Tags

Tags are not metadata. They are nodes. They are terrain.

Tags are visible, interactive, and first-class citizens of the graph. You can click a tag node and get: related articles, related tags, sorting options, filtering options. You can arrange the view by tag. You can arrange by article. You can arrange by date, by density, by connection count. The organizational structure of the content is as navigable as the content itself.

---

## The topology

The graph has depth. Nodes that are more connected, more referenced, more read — they are higher. Nodes that are less connected recede. The view is like looking down on terrain from above: peaks are prominent and bright, valleys are smaller and dimmer, fading as they recede from the center of attention.

The reader decides what is on the peak. You can reorient the topology around any node — pull it to the top, watch everything else reorganize around it.

---

## 3D mode

You switch into 3D mode the way you switch Google Maps from standard to terrain — a single gesture and the surface lifts. The topology becomes physical. You navigate through it.

In a multi-creator context, each peak might be another content creator. Ripples are activity — new content, comments, connections being made. You see what's moving. You see what's still.

This is the far edge of the vision. The 2D version proves the concept.

---

## Customization

Content creators control their graph. Node arrangement, node size, themes, color. The theme bleeds into the content as it arrives — not a static shell around the article but a living environment the creator has built that the reader enters. No permanent structure is imposed from outside. The shape of a creator's knowledge space is part of their expression.

Readers can also rearrange — sorting, filtering, adjusting their own view of someone else's graph. The creator's arrangement is a starting point, not a cage.

---

## AI

AI is not a chatbot here. It is a set of specific tools, directly invoked, with limited scope.

- Connect: find relationships between two nodes
- Sort: reorder by a criterion
- Refactor: restructure a document
- Tag: suggest connections to existing tags

No conversation. No general-purpose assistant front end. AI assists the organization of information without owning the organizational logic. The human makes the call. AI surfaces the options.

Community contributions — new tags, new connections — are proposed and verified by an AI call before they appear. The AI is a bouncer, not a brain.

---

## Community

The contribution model is tagging and connecting. A reader can propose a tag on a piece of content, or propose a connection between two nodes. The creator (or an AI acting as the creator's proxy) approves or rejects. This is how the topology grows without becoming noise.

Comments as a concept are not yet defined. They may not be needed. The contribution *is* the connection.

---

## Proof of concept

Take any RSS feed — or several large feeds simultaneously. Parse the items. Extract titles, descriptions, tags, dates, images. Map them to the graph. Let the topology emerge from the tag relationships and publication patterns.

The graph handles images. Nodes can carry cover images, displayed as the node background. The visual identity of the content is part of the graph, not stripped out.

This works on a single personal feed. It works on a curated set of feeds from multiple sources. The same interface serves one writer's body of work or an aggregated view of a field.

---

## What this is not

Not a CMS. Not a feed reader. Not Roam or Obsidian bolted onto a website. Not are.na. Not a social network with a graph visualization feature.

The graph is not a feature. It is the medium.

---

## Who this is for

Not a general audience. Specific people with specific frustrations.

**The academic** — has a body of work that connects across years and disciplines. Every platform treats each paper as a separate object. The connections between them are invisible. She needs a space where the topology of her research is the product, not a sidebar feature. Self-hosting matters: institutional work needs to live on institutional infrastructure.

**The artist and therapist** — works in a field where everything connects to everything. His writing doesn't fit categories. A flat blog destroys it. He needs a medium where the relationships between pieces are part of the reading experience, not metadata buried in a tag cloud.

**The Substacker** — has built a real readership but is constrained by Substack's reading UX. Articles scroll off. There's no way to see how the work connects. Readers can't navigate by idea. The platform was designed for consumption, not comprehension.

**The attention economy refugee** — has decided to stop letting the algorithm choose what they read. Wants to curate their own information graph from sources they trust. Needs a tool that maps feeds, shows relationships, and puts them in control of what surfaces. Infotopoia is their replacement for the timeline.

---

## Deployment

Runs in Docker. One command. No DevOps required.

The content creator owns their instance. Articles live in a mounted volume outside the container. Settings live in `settings.json`. The graph is generated at startup and served as a static site.

Phase 1: static only. GitHub Pages or any nginx. Reader mode for visitors. Editor via CLI.

Phase 2: PocketBase added. Editor mode in browser. Reader sessions persisted. Community tagging enabled.

---

## Name

**infotopoia**

Not a typo.

---

*Harold Young — 2026-03-23*
