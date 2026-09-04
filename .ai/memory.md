# memory.md · [AppName]

## [PROJECT]
Name    : game_anak_edukasi
Stack   : HTML5 + CSS3 + Vanilla JavaScript (Single-file)
Root    : C:/Users/Administrator/Documents/project/game_anak_edukasi
Created : 2026-09-03

## [KNOWN LIMITS] ← source: Gemini API dashboard, Free tier, project "aku1", 28-day peak
```
MODEL                                    RPM     TPM      RPD    TIER (per RATE LIMIT PROTOCOL)
────────────────────────────────────────────────────────────────────────────────────────────────
Antigravity (Agents)                      60    100K       100    Tier 1+3
Gemini 2.5 Flash                           5    250K        20    Tier 1+3+4 (RPD<50 → mandatory)
Gemini 2.5 Flash Lite                     10    250K        20    Tier 1+3+4
Gemini 2.5 Flash TTS                       3     10K        10    Tier 1+3+4
Gemini 3 Flash                             5    250K        20    Tier 1+3+4
Gemini 3.1 Flash Lite                     15    250K       500    Tier 1+3
Gemini 3.1 Flash TTS                       3     10K        10    Tier 1+3+4
Gemini 3.5 Flash                           5    250K        20    Tier 1+3+4
Gemini 3.5 Flash Lite                     15    250K       500    Tier 1+3
Gemini 3.5 Transcribe (Live API)           3     10K        25    Tier 1+3+4
Gemini 3.6 Flash                           5    250K        20    Tier 1+3+4
Gemini 3.7 Flash                           5    250K        20    Tier 1+3+4
Gemini 3.8 Flash                           5    250K        20    Tier 1+3+4
Gemini Embedding 1                       100     30K       1K     Tier 1+3
Gemini Embedding 2                       100     30K       1K     Tier 1+3
Gemini Robotics ER 2 Preview                5    250K        20    Tier 1+3+4
Gemma 4 26B                                30     16K     14.4K    Tier 1+3
Gemma 4 31B                                30     16K     14.4K    Tier 1+3

Live API (no RPM/RPD cap, TPM only):
Gemini 2.5 Flash Native Audio Dialog    Unlimited    1M    Unlimited    Tier 3 only (watch TPM)
Gemini 3 Flash Live                     Unlimited    65K   Unlimited    Tier 3 only
Gemini 3.5 Live Translate               Unlimited    20K   Unlimited    Tier 3 only
Gemini 3.5 Transcribe Live              Unlimited    20K   Unlimited    Tier 3 only

Zero-quota (not usable on Free tier — do not call, will always 429):
Deep Research Pro Preview, Gemini 2 Flash, Gemini 2 Flash Lite, Computer Use Preview,
Nano Banana (all variants), Gemini 2.5 Pro, Gemini 2.5 Pro TTS, Gemini 3.1 Pro,
Gemini Omni (1.1 Flash / Flash), Lyria 3 (Clip/Pro), Veo 3 (Fast/Generate/Lite)

Tools (RPD only):
Search grounding (Gemini 2 / 2.5)     1.5K/day
Search grounding (Gemini 3+)          0/day — unusable on Free tier
Map grounding (most models)           500/day
Map grounding (Gemini 3 / 3.5 / 3.6 / 3.7 / 3.8 Flash, 3.1 Pro, 2.5 Pro)   0/day — unusable
```

## [ENV & PORTS]
```
(fill as discovered — ports, DB paths, API key locations, service URLs)
```

## [OPEN ISSUES] ← AI reads this before starting any work
```
STATUS      PRI   DESCRIPTION
──────────────────────────────────────────────────────────
(none)
```
Add:     `UNRESOLVED  HIGH/MED/LOW  [desc] | Suspect:[x] | File:[x] | Next:[x]`
Resolve: move to [LOG] with RESOLVED tag

## [LOG] ← paste MEMORY UPDATE blocks here, newest on top
```
[2026-09-03 11:00]  FILE_EDIT — Renamed game_kata_hewan_v2.html to index.html
        Purpose: Enable automatic deployment for GitHub/Cloudflare Pages.
        Updated README.md and FILE INDEX.
[2026-09-03 10:00]  EXEC_OK — Initialize project under TSA-X v6.3 contract
        Stack identified: HTML5/JS (game_kata_hewan_v2.html)
        Memory file configured for game_anak_edukasi.

[2026-09-03 00:00]  INIT — KNOWN LIMITS loaded from Gemini API dashboard (free tier, project aku1)
```

## [FILE INDEX]
```
FILE                         LAST TOUCHED
─────────────────────────────────────────
README.md                    2026-09-03
TSA-X.md                     2026-09-03
.ai/memory.md                2026-09-03
index.html                   2026-09-03
```

## [NOTES]
```
Any model NOT listed in [KNOWN LIMITS] or with 0/0 across RPM/TPM/RPD = unusable on
current tier. AI must check this table first before writing any Gemini API call —
never assume, never re-ask, this table is ground truth per RATE_LIMIT_FROM_SOURCE.
```
