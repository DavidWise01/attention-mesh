# THE ATTENTION MESH

Causal attention drawn as its **honest topology** — a complete weighted directed
graph. Not two strands (a double helix has exclusive one-to-one rungs); not a
funnel (a funnel is a pipe). Attention is **one sentence crossed with itself**:
the same tokens on both axes, connected many-to-one with graded weights.

A single offline HTML file, built on ROOT0's foundational instrument scaffold —
zero runtime network fetches, system fonts only, fail-loud, verify-then-build.

## Two channels

- **2D chord diagram** — the attention graph flattened onto a ring, chords bowed
  through the interior. Orange = sink edges (every query reaches token 0),
  green = recency (neighbors attending to neighbors), grey = the rest. Drag the
  slider to isolate one query's edges, or show the full mesh.
- **3D inverse helix** — the helix turned inside-out so the strands run through
  the interior. A **query ring** on top and a **key ring** below (the same
  sentence twice, in its two roles — looker and looked-at); each attention weight
  is a strand bowing through the central axis. Every query's strongest strand
  dives to the same point on the key ring: the **sink**, a convergent many-to-one
  gather made unmistakable. Drag to rotate, wheel to zoom.

## Amber tier — what's real, what isn't

The **topology is exact**: this is genuinely how a causal attention layer connects
— a self-crossed weighted graph, every token able to attend every earlier token,
each edge a continuous weight. The **weights are modeled**, not extracted from a
trained network: a small deterministic model reproduces the documented structure
(attention **sinks** on the first token, **recency** bias, a **heavy tail** to
mid-sequence). So the shape you rotate is honest; the specific numbers are a
faithful stand-in, not a measurement. That is the amber line, stated on the page.

Verify the model yourself: every attention row is a valid causal probability
distribution (sums to 1, no token attends the future), and the sink is dominant
(every query's top-1 is token 0). Open the file — no build step, no network.

## Companion

The topology-companion to [THE ATTENTION HOURGLASS](https://davidwise01.github.io/attention-hourglass/)
— the hourglass shows attention as **flow** (queries and keys pinching to one
prediction); the mesh shows attention as **structure** (the whole weighted graph,
the funnel argued past). See also [TTU1 · Transformer Tech](https://davidwise01.github.io/ttu1/).

---
David Lee Wise / ROOT0 / TriPod LLC · CC-BY-ND-4.0
