# Hi, I'm Kate

I automate work people are still doing by hand: intake, documents,
monitoring, integrations, internal tools. Process first, technology second.
If the job can be done in code, I write code. If it needs a model, I use one.

For years I designed interfaces and took processes apart: how people
actually work, where they get stuck, what they quietly give up on. Now I
build the systems myself.

Between February and August 2026 I went from first experiments to services
other people use every month. The dates are in the commits.

## Selected work

**[local-dictation](https://github.com/basova-gonzalez/local-dictation-macos)** — dictation that stays on your
laptop. Hold a hotkey, speak, and the words appear in the field you were
already typing in. A macOS menu-bar app in Swift, transcription by
WhisperKit on-device. No cloud, no account, no telemetry.

It never presses Return and never submits a form. The text lands, you read
it, you send it yourself. The audio file is deleted before transcription
starts: Whisper reads from memory, not from disk. You provision the model
yourself; the app has no downloader. The repository gates reject runtime
networking patterns, external endpoints, and Return-key synthesis in the
release source.

Targets macOS 14+, source-only alpha under MIT, configured and verified for
Russian.

**[sandbox-print-kit](https://github.com/basova-gonzalez/sandbox-print-kit)** — a climbing gym needed a flyer, two posters and a style, so the next poster wouldn't start from scratch. Instead of three files the client got a kit: five layouts in five sizes, from DL to A3, with instructions clear enough for a staff member and an AI assistant to make a new poster without a designer. It shows every layout at once, a person picks by eye, and the kit checks the print mechanics: bleed, crop marks, fonts, QR codes. Demo brand; Node.js and Python, MIT. [Case study](https://kabago.ru/cases/sandbox-print/).

**[orthodox-schedule-generator](https://github.com/basova-gonzalez/orthodox-schedule-generator)** — every month a parish gets its service schedule in a message, and someone spends two hours moving it onto the website by hand. Paste the schedule into any AI chat with the bundled prompt, get a JSON file, run one command, and paste the finished block into Tilda, WordPress or any site builder. Sundays, Pascha and the great feasts are marked by the Julian calendar, computed in code, not guessed. Python, no dependencies, RU/EN, MIT. [Case study](https://kabago.ru/cases/schedule-generator/).

**[patriarchia-calendar-parser](https://pravoslavna.ru)** — the Orthodox
liturgical calendar is published one page per day. To assemble a month, a
priest opened thirty pages one after another, copied each into a document
and formatted it by hand. Every month.

The parser reads the official site and returns a ready-to-print Word file.
Python and FastAPI, no model in it: the task has one right answer, and code
returns it the same way every time. Live at
[pravoslavna.ru](https://pravoslavna.ru).

The rest of my work lives at [kabago.ru](https://kabago.ru), written up as
the problem each one solved: voice intake for a photo studio, a reading
agent that files findings into Telegram and Notion, search across your own
transcripts with timecodes you can open and check, a bilingual schedule that
proofreads its two versions against each other, a dashboard for when you
have more projects than memory.

## How I work

I start by watching how the work is done now. Then a pilot, then the
interface, then I hand it over. The point is that you don't need me a month
later.

The last thing I check is whether the person running it can tell when it's
wrong. Where a model is involved, the answer comes with its source, and
"I don't know" is an allowed reply.

Everything here was built alongside AI agents. The architecture, the product
decisions and the checks are mine; the code was written with them.

## Stack

Swift, Python, FastAPI. OpenAI, Anthropic, Gemini, Kimi, Qwen, LM Studio for
local models, Whisper, LangGraph. Cloudflare, Vercel, Hugging Face, my own
server.

---

Portfolio and work journal: [kabago.ru](https://kabago.ru). This account
starts in May 2026. Before that, from February, I was posting on
[@Fabrichnaya](https://github.com/Fabrichnaya).
