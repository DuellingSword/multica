# Agent recent-work rendering evidence

Synthetic evidence for `perf(agents): virtualize recent work history`, source
commit `d1e72f020a7beb27b49ed9834cabe9d3e3375c97`, compared with upstream
`3c5c8b245359b9b8e913a47f97211f2a3426f149`.

- [Before/after recording](media/recent-work-before-after.mp4): both sides at
  original speed; the shorter side holds its final frame after completion.
- [Before](media/before-wide.png) and [after](media/after-wide.png) screenshots.
- [Compact transcript retained after row recycling](media/after-compact-transcript.png).
- [Measurements (JSON as text)](media/measurements.txt).

Both production Web builds receive 1,000 synthetic terminal runs through
intercepted HTTP and WebSocket boundaries. The existing 200-run API pages and
50 Show more clicks are retained. No real account, API server, database, daemon
or agent execution is used; non-local requests are blocked. Counts concern
mounted rows, not general FPS or backend throughput. Electron main-process
behavior is not exercised.

The code contribution contains no media files; this independent evidence branch
hosts only the synthetic artifacts linked from the pull request.
