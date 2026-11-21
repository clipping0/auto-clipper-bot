# Source archive inventory — clipping_agent.zip

Inspected archive contents (165 entries).

## Relevant code found
- Python agent pipeline: transcription, clip selector, subtitle, metadata, upload, analytics, video, voice and Instagram agents.
- LangGraph orchestration (`orchestrator/workflow.py`).
- FFmpeg tools: cutter, stream downloader, render test edits and `render_pex_edits.py`.
- Dashboard: Flask-style dashboard app and a large HTML template.
- Project/channel management, upload history, campaign rules parsing, scheduler.
- SQLAlchemy database models and DB management.
- Requirements and settings configuration.

## Visual/reference material
- `example reference/pex_reference_presets (1).json` contains **5 COD templates**: `tweet_dark`, `tweet_card_blur`, `tweet_light`, `bold_center_hook`, `square_bar`.
- Six caption style definitions: `neon_glow_word`, `kinetic_glow_type`, `fade_clean_small`, `two_tier_keyword_highlight`, `word_by_word_minimal`, `pink_glow_caps`.
- Quality presets: `reference_match` (720x1280, 30fps, approx 2Mbps), `hd_reels` (1080x1920, 30fps, CRF18, AAC 192k), `smooth_60` (1080x1920, 60fps, CRF19).
- 12 snapshot JPGs under the reference snapshots folder. No separate external reference image or GTA RAR was used.
- Renderer source says COD uses `tweet_dark` and GTA6 uses `tweet_card_blur`; it may need refactoring for user-selectable templates and preview-first.

## Sensitive material caution
Archive contains `.env`, `data/client_secrets.json`, database files, Instagram account data, logs and token-capable integration code. Treat these as sensitive; **do not publish the ZIP or copied secrets**. Rotate any real credentials if this archive has been shared beyond trusted locations.
