# AGV Water Control

🥇 **1st place, AI for Water Hackathon, Amsterdam, 28 October 2026** (AGV challenge)

**▶ [Open the live demo](https://aiso-water-hackathon.vercel.app)** · [Pitch deck with video](https://finnsim123.github.io/AGV-Water-Control/) · [Pitch deck (PDF)](AGV-Water-Control-pitch-deck.pdf) · [60-second explainer video](video/explainer.mp4)

## The challenge

Water board AGV (Waterschap Amstel, Gooi en Vecht) keeps Amsterdam dry with 43 pumping stations.
Their question: **when do you turn the pumps on, and when do you turn them off?**
With climate change that is getting harder. Sometimes water has to go, fast. And sometimes, in a dry
spell, you want to keep it in.

## What we built

1. **A model.** A gradient-boosting model trained on 26 years of AGV pump data together with the weather.
   Tested on 2022 to 2025, years it had never seen, it predicts what AGV actually pumped with an R² of 0.84.
2. **Rules on top.** They read the 14-day weather forecast. Heavy rain coming? Pump ahead of it.
   A dry spell coming? Keep the water in. Always within safe limits.

Backtested on real history: during heavy rain in 2013, peak pumping would have been 22% lower, and in
the dry spring of 2023 about 1.2 million m³ more water would have stayed in the polders.

## In this repo

| File | What it is |
|---|---|
| [`AGV-Water-Control-pitch-deck.pdf`](AGV-Water-Control-pitch-deck.pdf) | The pitch deck as a PDF |
| [`index.html`](index.html) | The same deck as a web page, with the video playing on slide 2 ([open it](https://finnsim123.github.io/AGV-Water-Control/)) |
| [`video/explainer.mp4`](video/explainer.mp4) | The idea in one minute |

The source code and model stay private. The demo runs at
[aiso-water-hackathon.vercel.app](https://aiso-water-hackathon.vercel.app).

*A hackathon prototype, not an official AGV product.*

Built by Finn Simon and Thijmen Simon.
