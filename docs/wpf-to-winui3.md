# Rewriting Bari Plux Tool: WPF to WinUI 3

**By Snow Breaker · Bari Plux**

## Context

BPT began with a narrow purpose: adjusting PUBG Mobile graphics / FPS settings and GameLoop keymapping for an iPad-style view. The PC application officially launched on **16 November 2025**.

As the community grew, requests brought DNS tools, PAK backups, more languages and optimization. By summer 2026, a larger WPF redesign was intended to introduce a new interface, Game Mode, expanded optimization controls and a file manager.

## The problem

On **31 July 2026**, I shared the work with a developer / VIP group. Their feedback was that the interface did not fit the product's identity and could hurt the user experience.

A lot had already changed. Simply reverting the interface would not address everything I wanted to improve in the application underneath it.

## The decision

I chose to set the WPF project aside and rewrite the application with **WinUI 3**. Both implementations used .NET 10; this was a decision about the application and interface, not just a framework version upgrade.

The goals were a more familiar Windows experience, clearer interaction and navigation, and a chance to revisit performance, control and maintainability together.

## What resulted

The rewritten PC application officially launched on **12 October 2026**. The current project uses C#, .NET, WinUI 3 and XAML, with separate views, view models and services.

Its scope includes Game Mode, file management, backups, diagnostics, account and community features, and localization across **27 languages**. Recent additions include an in-game performance overlay and Installed Files for emulators.

The engineering workflow also includes automated checks and a published-build smoke-test script. That distinction matters: a successful build alone does not establish that the installed product works as intended.

The release and change in implementation are concrete outcomes. This case study makes no quantified speed, memory or reliability claims: no comparable before-and-after benchmark is published here.

## What I learned

- Early feedback can challenge a direction before more work is invested in it.
- Interface decisions affect the whole product experience.
- A rewrite needs a clear purpose and verification beyond compilation.
- Community requests are valuable input, while product direction still needs deliberate choices.

## Next

BPT Android is **Coming Soon**. The longer-term goal is to support PC and mobile users with products that work together, while using what I learn here to build beyond BPT.

[Back to the product overview](../README.md)
