# Core Context — Android WebView Content Series

Source chat: `https://chatgpt.com/share/698bf088-e430-800f-8067-52678fa98901`

## Objective
Build a high-reach, engineering-grade content series (LinkedIn/Twitter/Medium) focused on Android WebView topics, with high technical credibility and no hype.

## Core Editorial Rules
- No myths, no fabricated claims, no hand-wavy guesses.
- Do not disrespect teams/developers; frame as engineering insights.
- Keep tone professional and practical.
- Avoid binary "good vs bad" framing too early; reveal trade-offs through architecture realities.
- Generate platform-specific variants for each post (LinkedIn, Twitter, Medium).
- Include image generation prompts for each platform when producing posts.

## Topic Inventory
- WebViews
- `shouldInterceptRequest` callback behavior
- Thread behavior (`threadpoolforeg`) in `shouldInterceptRequest`
- JavaBridge handler thread for `@JavascriptInterface`
- Full WebView lifecycle callback order (WebViewClient/WebChromeClient)
- Script injection timing for DOM/page access
- WebAssetLoader usage in `shouldInterceptRequest`
- WebView engine internals
- JS Sandbox on Android (pros/limits)
- `postMessage` vs WebMessageListener deep dive
- JS-thread blocking concerns around postMessage/JavaBridge
- Main-thread WebView init analysis (Perfetto)
- Drawbacks of caching/pooling WebView objects
- WebView vs iOS WebKit
- `prefers-color-scheme` in WebView
- WebView initialization time

## Strategic Structure
Canonical structure is sourced from `LinkedIn_Post_Hierarchy_Conversation.md`
and normalized in `ANDROID_WEBVIEW_SERIES_ARCS.md`:
1. Arc 1: Lifecycle & Session Reality (`Post 1A` to `Post 1D`)
2. Arc 2: Resource Loading & Network Pipeline (`Post 2A` to `Post 2C`)
3. Arc 3: JS Bridge & Execution Model (`Post 3A` to `Post 3C`)
4. Arc 4: Lifecycle & Injection Timing (`Post 4A` to `Post 4C`)
5. Arc 5: Performance & Engine Internals (`Post 5A` to `Post 5C`)
6. Arc 6: Platform Strategy & Architecture (`Post 6A` to `Post 6B`)

Naming convention is canonicalized as `Post 1A/1B/...`, `Post 2A/2B/...`, etc.

## Positioning Decision
WebView should not be framed as a narrow niche. The series should open with broad Android relevance:
- many teams use WebView for full hybrid surfaces,
- dynamic/legal/support/embedded flows,
- and release-velocity use cases.
