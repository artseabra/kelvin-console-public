# Kelvin Console

Public Kelvin Console surface.

## Live instrument

`index.html` is the standalone Kelvin Console for Simone Conradi's two-parameter
chaotic map:

```text
x[n+1] = sin(x[n]^2 - y[n]^2 + a)
y[n+1] = cos(2*x[n]*y[n] + b)
```

It includes real-time parameter controls, sampled presets, paintbrush particle
seeding, browser-native sonification, PNG export, and a performance guard for
expensive glow rendering.

Production URL:
https://kelvin-console-v18-epistemic-horizo.vercel.app

## Public archive

`archive.html` and `manifest.public.json` are the curated public archive slice.
They intentionally do not include private source manifests or private branch
telemetry.
