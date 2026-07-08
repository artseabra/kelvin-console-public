# Kelvin Console

Reviewed: 2026-07-08
Status: public instrument and curated archive slice
Production: [kelvin-console-v18-epistemic-horizo.vercel.app](https://kelvin-console-v18-epistemic-horizo.vercel.app)

Kelvin Console is a browser-native chaotic-map instrument from Art Seabra / Ifthis Studio.

This public repository contains the inspectable surface: the live standalone instrument, the curated public archive slice, and the manifest that defines what is intentionally exposed.

## Live Instrument

`index.html` is the standalone Kelvin Console for Simone Conradi's two-parameter
chaotic map:

```text
x[n+1] = sin(x[n]^2 - y[n]^2 + a)
y[n+1] = cos(2*x[n]*y[n] + b)
```

It includes real-time parameter controls, sampled presets, paintbrush particle
seeding, browser-native sonification, PNG export, and a performance guard for
expensive glow rendering.

Open the production instrument here:

https://kelvin-console-v18-epistemic-horizo.vercel.app

## Public Archive

`archive.html` and `manifest.public.json` are the curated public archive slice.
They intentionally do not include private source manifests or private branch
telemetry.

## Local Use

No build step is required for the static public surface.

```bash
open index.html
open archive.html
```

## Public Boundary

This repo is not the full private Kelvin lineage archive. It exposes the public instrument and the curated public manifest only. Private manifests, unreleased experiments, branch telemetry, and source-control provenance stay outside this public surface unless they are intentionally promoted.

Art Seabra · Ifthis Studio
