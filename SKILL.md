---
name: the-proven-package
description: Use this when a video needs its public face, the titles and thumbnails. The default entry runs BEFORE a word of script exists (the script is written to a locked promise); the second entry, REPACKAGE, takes a published video that flopped and gives the same cut a new face. Run it when the founder says "run the proven package," a winner file is ready, or a published video's numbers came in under the channel's own baseline. It clones the shapes your lane already proved, pairs each title with a proven thumbnail cage, builds the images in layers with your real face, and stops for your review at every decision a human owns. Nothing invented, every number a receipt.
---

# The Proven Package

You are the packaging agent. Views are decided before a second of video plays, by the
title and the thumbnail, so this skill spends real care there and nowhere else. Your
work in one line: **take this week's winner file and the lane's proven shapes, and turn
them into three title-plus-thumbnail pairs the founder locks.** All three pairs SHIP,
and here is the honest mechanism: YouTube's Test & Compare tests up to three
THUMBNAILS, so the three thumbnails fill the test's three slots. The main title goes
on the video; the two sub titles are swap stock for a later CTR swap or a repackage.
Test & Compare needs YouTube Partner Program eligibility: not eligible yet means ship
the main pair, hold the other two, and swap the thumbnail by hand after 7 days,
reading the change against this channel's own trailing median (the REPACKAGE math
below). The build is three pairs either way; only the upload instruction changes.
Packaging comes FIRST: the default entry runs before a word of script exists, and the
script is then written to the locked promise. "Recorded" enters only through
REPACKAGE below.

Everything runs inside THIS founder's own `squad/` workspace. Never borrow another
brand's lane, shapes, or accent color; if this founder's thumb-cages file does not
exist yet, seed it from this skill's shipped copy at `references/thumb-cages.md`.
On that first seed, take the accent color from the roots file when it names one, else
read it off `squad/business.md`'s BRAND line (the Winning Offer writes it there); with
neither, ask the founder for their ONE color and write it back to the roots file.
Either way it goes into their cage copy's law 5: the shipped file's #146ef5 is the
source repo's example, never this founder's default.
And if `squad/lane.md` does not exist, send the founder to run the-winning-scrape
before cloning any shape.

## What you read first (in this order)

Before the list: resolve the workspace from `.claude/squad-roots.md`, created by the
install lesson and filled from the-winning-offer (module 1) onward. Its fields:
founder name · brand words (product word + banned synonyms) · accent color · lane ·
week · episodes · credibility-bank · face · thumb-cages · voice file · wpm (110
default) · data sources · tools (the research mode this repo has). Every `squad/` path
below resolves through it, thumb-cages and the data sources included. A repo carrying
the legacy `.claude/spine-roots.md` keeps working: read it as the fallback when no
squad-roots.md exists. Missing both, the paths below are the defaults. Never
re-interview for a field the roots file already answers, and write back any field
this run learns (the accent color, the episodes root) so next week's run does not
ask again.

1. `squad/week/<latest>-winner.md`, the handoff from the Winning Scrape. **On the
   default entry, no winner file in `squad/week/` = STOP:** send the founder to run
   the-winning-scrape first. REPACKAGE skips this item; its draft is the published
   video's existing packaging.
   A winner file older than 7 days: confirm with the founder before packaging it; the
   hunt is weekly. If the winner is a competitor's video (not this channel's own
   breakout), say so in the package file as an external reference. If its comment
   mining holds fewer than 3 distinct buyer complaints, flag the file as thin before
   wording anything from it. A winner file carrying a re-pull flag
   (transcript-not-comments, description-not-transcript) routes that section back to
   the-winning-scrape's approved pull, done before anything is worded from it.
2. `squad/lane.md`, the standing shapes. A shape is usable only when the file carries
   its full skeleton text AND its proving niche overlaps this founder's audience.
   A multiple with no skeleton is not a shape; ask, never guess one. When an older
   lane file lacks a shape's proving niche, read it off the linked proof video before
   judging overlap.
3. `squad/business.md`, the offer document from the Winning Offer. The document's WHO drives
   the shape-overlap test in item 4, and its SENTENCE and MODEL give the founder's
   real verbs for beat 1's fit gate. Its BRAND line names the founder's accent color,
   the one the cage file's law 5 needs. No document = ask the founder for their audience and
   their real verbs in one question, note the document as absent, and continue.
4. The roots file's thumb-cages path (default `squad/thumb-cages.md`), the thumbnail
   layouts (seeded from this skill's `references/thumb-cages.md` on first run). Cage
   geometry is authoritative; the laws govern whatever a cage does not specify. A
   grown cage file already sitting at that path is read, never re-seeded over.
5. `squad/credibility-bank.md`, the only legal source for any number or claim. Its
   PROOF-ASSET LIST section names the real screenshots a thumbnail may show; LOSSES
   feed hooks and honesty beats, never claims. **Missing bank = STOP:** run the bank
   conversation from the-winning-offer's step 9 (THE BANK) before beat 1; when that
   skill is not installed, run the interview here. The founder's stated receipts,
   interviewed now in their own words, ARE the bank; write the file with the six
   canonical sections (WINS with mechanisms, LOSSES, NEVER-LIST, CLIENT RESULTS,
   PROOF-ASSET LIST, VOICE NOTES), then proceed. A bank that exists but lacks any of
   the six canonical sections triggers the same interview for the absent sections
   only, before beat 1.
6. `squad/face/`, the founder's face refs. The convention is `face-01` to `face-04`
   (jpg or png), but when the folder holds image files under other names, read them
   anyway; off-spec names are not an empty folder. 2 is the floor, 3+ angles is the
   standard. Exactly one file = a degraded warning: proceed on the cheap tier and
   tell the founder to expect a regeneration. **Missing or empty folder:** this run
   owns the setup, because this is where the photos are first used. Create
   `squad/face/` yourself, open it for the founder (macOS `open`, Windows `explorer`,
   Linux `xdg-open`), and ask once ("drop 2-4 face photos in there and say go, or say
   face-free"), then offer to rename whatever lands there to the `face-01` scheme; the
   founder never renames files by hand. Only after that ask does every pair run a
   no-face layout (Cage 3, or a cage's no-face fallback). Never strip a face cage into
   an undocumented layout.
7. The image tool, checked BEFORE any promise about beat 3. The execution path is the
   fal image endpoints: `fal-ai/bytedance/seedream/v4.5/edit` (the default tier) and
   `fal-ai/gemini-3-pro-image-preview/edit` (Nano Banana Pro, the quality tier). The
   credential is `FAL_KEY` in this repo's `.env`, written there by the install. The
   shell does not read `.env` on its own, so every call carrying the key loads it
   first, this check and both beat-3 calls alike:

   ```
   set -a; . ./.env; set +a
   ```

   (or `FAL_KEY=$(grep -m1 '^FAL_KEY=' .env | cut -d= -f2-)` when `.env` holds lines
   the shell cannot source). Then verify before beat 3 with this free auth check
   (nothing is generated, nothing billed):

   ```
   set -a; . ./.env; set +a
   curl -s -o /dev/null -w "%{http_code}" -X POST \
     https://fal.run/fal-ai/bytedance/seedream/v4.5/edit \
     -H "Authorization: Key $FAL_KEY" -H "Content-Type: application/json" -d '{}'
   ```

   Check the variable is non-empty before reading the code, because an empty
   `FAL_KEY` reads as a bad key at the endpoint: empty after the load means the load
   failed or the install never wrote the key, which is the bootstrap ask below, not a
   bad key. With a non-empty key: `422` = the key works (the empty body fails
   validation before anything is queued or billed). `401` = the key itself is bad.
   `404` = the endpoint id has moved; look up the current edit endpoint on
   fal.ai/models, correct it here, and re-check.

   The beat-3 calls are the same shape, with the payload in a FILE. Never inline it:
   a face ref carried as a data URI blows past the shell's argument limit (about 1 MB
   of argv on macOS) and curl dies with "argument list too long". One worked example
   per endpoint:

   ```
   set -a; . ./.env; set +a
   curl -s -X POST https://fal.run/fal-ai/bytedance/seedream/v4.5/edit \
     -H "Authorization: Key $FAL_KEY" -H "Content-Type: application/json" \
     -d @squad/week/thumbs/<date>/payload.json
   ```

   ```
   set -a; . ./.env; set +a
   curl -s -X POST https://fal.run/fal-ai/gemini-3-pro-image-preview/edit \
     -H "Authorization: Key $FAL_KEY" -H "Content-Type: application/json" \
     -d @squad/week/thumbs/<date>/payload.json
   ```

   The payload file, written by a script rather than by hand, holds `{"prompt": "<the
   base prompt>", "image_urls": ["<face ref>", "<cage reference>"], "image_size":
   {"width": 1280, "height": 720}}`. Each `image_urls` entry is a public URL or a
   local file inlined as a data URI (`data:image/jpeg;base64,...`); fal's storage
   upload works too. Downscale each face ref to 1024px on its long edge before
   encoding (`sips -Z 1024 squad/face/face-01.jpg` on macOS, any equivalent
   elsewhere): a phone photo is 2-4 MB and base64 inflates it by another third, and
   nothing above 1024px shows at 1280x720. The response
   JSON's `images[0].url` is the base image; download it into the run's thumbs
   folder. **No key found:** one bootstrap ask before anything degrades: the founder
   creates a free fal.ai account, copies a key from fal.ai/dashboard/keys, and
   pastes it here; save it to `.env` as `FAL_KEY` and continue. Only when that too
   fails, **DEGRADED MODE:** deliver the locked titles plus a complete written
   composite spec per pair (cage, base-image prompt, element sizes in percent of
   frame, exact text layer), each pair marked blocked-on-tooling. Never improvise
   other tooling. Any beat-3 tool failure after two attempts routes into DEGRADED
   MODE the same way.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 1 TITLES | AUTO: three shape clones (1 main + 2 subs, each its own pair) with the five-check sheet, then **STOP · GATE: the voice pass plus the one ask; the founder edits and locks all three** |
| 2 PAIR | AUTO: one cage per locked title, three different cages |
| 3 BASES | AUTO: generate the image bases, no words in any image |
| 4 TYPE | AUTO: composite the mechanical layers in code, then the text layers |
| 5 CHECK | AUTO: the 320px mobile grid + side-by-side against each cage's reference |
| 6 REVIEW | **STOP · GATE: the founder's notes on the pairs; change exactly what the founder names** (repeat 2-6 as routed until they lock) |
| 7 PACKAGE | Write the package file, then **STOP · GATE: final confirm of the three pairs** |

A beat-1 edit that changes a title's CLAIM or mechanism re-runs that pair from beat 2.
A wording-only edit flows into the type layer and touches nothing else.

**The one ask (at the beat-1 gate).** Beats 3-5 spend the founder's money, install
tooling, and reach new hosts, so everything they need is confirmed in the single yes
at the gate that already stops. Say it together with the titles: the expected image
cost, the fal endpoint the auth check verified, the one-time `python3 -m venv .venv &&
.venv/bin/pip install pillow`, and the one-time font fetch. Name the permission kinds
in the same breath (fal.run POSTs, the font fetch from github.com, `i.ytimg.com`
thumbnail downloads, the venv install and the shell commands around it), say allow
each once for the session, and get one yes. With that yes, beats 3-5 run unbroken. A
declined permission is stated plainly as a gap in the run, never worked around. On the
REPACKAGE path, which can skip beat 1, the same ask happens before beat 2.

## The second entry: REPACKAGE (the flops path)

When a published video runs under the channel's own trailing median after 48-72 hours,
the Sunday Score proposes a repackage and this skill executes it. Input: the published
video's URL plus its numbers (views, impressions, CTR, and the channel's trailing
median). The founder reads views, impressions, and CTR from YouTube Studio's Reach
tab and pastes them, plus the view counts of their last 10 long-form uploads from
the Content tab; no Sunday Score card is required. When no card exists, the trailing
median is computed here the way the Winning Scrape computes a channel baseline (its
baseline-exclusion rules included: comparable long-form uploads only, the judged
video excluded, bought-reach spikes excluded) over those last 10 uploads. Under ~10
comparable uploads, say so and use the median of what exists, flagged as the weaker
read; under 4 uploads, decline the repackage, because there is no baseline yet: wait
for impressions rather than re-facing a video on noise. CTR is
judged only past an impressions floor of ~500: under ~500 impressions the CTR is
noise, wait, and say how many more impressions the video needs. No fresh winner
file is needed; the existing packaging is the draft.
The run: show the trigger math first (the video's multiple against the channel's own
median), rerun the five checks on the EXISTING title and thumbnail and name which ones it
fails, then build one new pair on the same cut through beats 2-7. This is also where
SMALL-CHANNEL CTR CALIBRATION runs, as the sixth check: judge the published CTR
against this channel's own baseline, never the absolute CTR of giant channels. The
sub titles from
the original package are the first candidates. When no original title survives the
five checks, run beat 1 once on the current lane shapes (with its gate) before
beats 2-7.

**The repackage writes its own file:** `squad/week/<date>-repackage.md`, one pair,
opening with a header line naming the published video URL it replaces. No `epNN`
folder is created, since the cut already shipped, and beat 7's gate confirms the one
pair rather than three. A repackage file is never the Payoff Script's input: that run
takes the latest `<date>-package.md`.

## Titles (beat 1)

- Every title is a clone of a usable lane shape: the skeleton stays fixed, exactly one
  slot swaps to carry this video's content. Never invent a narrative shape.
- **1 main + 2 subs, defined.** The main is one primary-claim title: the winner file's
  core claim on the strongest usable shape (strongest = the usable shape with the
  highest proving multiple after the fit gate, ties broken by niche overlap). The lane
  file carries each shape's multiple with the baseline it was measured against and the
  date measured; the Winning Scrape measured them at RANK, so rank on what is written
  and never recompute it. Cold-ranking is the fallback for a shape
  written before that field existed: pull the proof video's views and its channel's
  baseline the way the Winning Scrape does (the channel RSS feed for the last ~15
  uploads, the median of the comparable long-form ones, the proof video itself
  excluded), rank on that, say which shapes were ranked cold this way, and write the
  multiple, its baseline, and today's date back into `squad/lane.md` so next week reads
  them instead of measuring again.
  The subs are two alternate-angle titles on two different shapes, not two rewordings of
  the main. All three ship as the platform test's slots.
- **DRESS-branch drafts.** When the winner file carries DRESS title candidates the
  founder already voice-passed at the scrape's gate, they enter beat 1 as the drafts;
  clone from lane shapes only what is missing to reach three. Never silently discard
  a title the founder already approved.
- **Fit gate before cloning.** A shape qualifies only if: its verb matches what the
  founder actually does (build / sell / review / teach / train / coach: the founder's
  real verbs); its structural needs exist (a guest format needs a real guest, a dollar
  skeleton needs a dollar receipt); its point of view survives the swap (a
  third-person shape like "He Makes..." becomes first person for the founder's own
  video, or gets skipped). A shape that fails the gate is skipped and the skip is
  noted. When fewer than three shapes survive the gate, a shape may carry two titles
  with different slot content; the two are still different claims, not rewordings.
- **Slot filling.** A number slot of ANY unit ($, lbs, days, %, count) takes a bank
  receipt whose unit matches the claim: a per-deal number fills a per-deal slot, an
  aggregate fills an aggregate claim, and mixing the two is the cherry-picking the
  audience punishes. Non-dollar slots follow the same receipt-and-unit rule as dollar
  slots. `[Claim]` slots take the receipt's MECHANISM first (the how), the niche
  second, never an invented hook.
- A title with an unresolved number slot is BLOCKED, not shippable: it stops at the
  gate with the ask, and never proceeds to pairing as a placeholder. Its slot
  backfills onto the next usable shape whose slots the bank CAN fill; only when no
  receipt-fillable shape is left does the package ship with fewer than three pairs,
  said plainly in the package file.
- **The five checks.** Every title carries a pass/fail sheet at the gate, and the same
  five pass/fail checks print again on beat 6's review sheet:
  1. TRANSACTION: the back half names the outcome, what someone got or paid, in
     any unit the bank can receipt, never a topic.
  2. JAGGED PAST / ROUND FUTURE: a real past number prints jagged ($77,675), a
     promise prints round.
  3. STEAL: every shape is stolen from a linked proven winner, never invented.
  4. ONE UNIT: one claim, one unit; per-deal never mixes with aggregate.
  5. MOBILE READ: the title's first four words carry the claim, because a phone feed
     truncates the rest; read every title at 320px before passing it. (SMALL-CHANNEL
     CTR CALIBRATION is not on this sheet. A title has no CTR before it publishes, so
     that check runs at REPACKAGE, where a real number exists.)
- **Wording check.** When `squad/offer-research.md` exists, check every title's words
  against its allowed-words section; a word the market never says gets swapped for
  one it does.
- The founder changes any word in a title that does not sound like
  them. The founder's edit wins over the shape when the two fight.

## Thumbnails (beats 2-5)

The laws and cages live in the founder's cage file (item 4's path). The build order:

1. **Pair.** First, the niche precondition: check whether any cage's proving channel
   sits in this founder's niche. The five shipped cages were all proven on builder,
   AI-tool, or business channels, so in a different niche none of them has won in
   front of this buyer. When none does, distill 1-2 cages from the thumbnails the
   Winning Scrape kept in `squad/week/thumbs/<winner-date>/src/` for this lane's
   ranked survivors (the winner file's own date, which is not this run's date whenever
   the package runs a day or more after the hunt; the folder holds the top 8-12, and the
   winner file says how many). Distill under the cage file's grow rule, each new cage
   carrying its proof link, and pair from those first; the shipped five are then the
   fallback, not the default. Folder gone (an older week, a cleaned repo): re-download
   the survivors from the ranked candidate table the Winning Scrape folded into the
   winner file, `i.ytimg.com/vi/<id>/hqdefault.jpg` per row (the id off the row's URL),
   into that same folder.
   Then pick the cage whose mechanism matches each title's claim: a method claim
   takes the annotated chart, a receipt claim takes a proof cage, a blunt one-liner
   takes the quote card. Three different cages is the target, not a gate that can
   block the run: when two claims match the same cage, the second takes that cage's
   nearest neighbour by mechanism and the choice is noted in the build log. When the
   winner file's described thumbnail matches no cage, distill it into a new cage per
   the cage file's grow rule before pairing; never force a claim into a
   mismatched cage. Face rule: the receipt-only claim can honestly go face-free;
   process and authority claims keep
   the founder's face. When the founder's proof cannot be shown verbatim (client
   confidentiality), the proof surface is a redacted REAL UI (blur the names, keep
   the real chrome), never a painted scene. **Consent:** a proof asset showing an
   identifiable person who is not the founder does not enter beat 4 without the
   founder confirming written release for public use. Unconfirmed means the pair is
   blocked-on-assets, the same route as a missing screenshot, never blurred and
   shipped.
2. **Bases.** One image-model call per pair through the endpoint read item 7 verified,
   face refs from `squad/face/` plus the cage's reference thumbnail as the
   layout-and-scale anchor. The reference anchors LAYOUT and SCALE only; the prompt
   names the founder's niche subject for every content element (Cage 2's tool icon
   becomes this niche's tool or prop), so nothing from the reference's niche bleeds
   into the base. Element sizes stated in percent of frame. "No words, no
   letters, no numbers anywhere" in every prompt. The base prompt renders EVERY zone
   beat 4 composites as EMPTY, named off the paired cage's own geometry: the proof
   device, the proof zone, the quote card, badges, pills, list panels, straight
   arrows. Worked example: a Cage 3 or Cage 4 base renders a blank screen and a blank
   receipt zone and the real screenshot lands in beat 4; a Cage 5 base leaves the card
   area as empty ground, never a painted card.
3. **Type.** The mechanical layers first (panels, badges, pills, arrows: built in
   code, crisp, never generated), then the text. The proof surface is one of these
   mechanical layers: a REAL file from the bank's PROOF-ASSET LIST composited in code
   onto the base's empty zone, never generated. **If the thing the claim is about
   appears in the image, it is a real file, composited.** That covers any proof
   surface, not screens alone: a screen, a body, a physical result, a room, a piece of
   equipment. Generating one is fabricated proof and banned. Text is
   never generated. Composite at 2x then downscale. The compositing stack is Python
   Pillow, installed venv-safe (`python3 -m venv .venv && .venv/bin/pip install
   pillow`; a bare `pip install` fails on a managed macOS Python), and every
   compositing script runs with `.venv/bin/python`, never a bare `python3`. No
   `python3` at all on this computer (`python3 --version` fails) marks the pairs
   blocked-on-tooling, the same route as a missing image tool. Fonts: Inter
   Black always, plus whichever fonts the paired cages name (Permanent Marker for
   Cage 4's qualifier, Caveat for Cage 1's handwritten labels), all free from
   Google's own font repo. Fetch them once per repo into `squad/fonts/` and reuse
   them every week after:

   ```
   mkdir -p squad/fonts
   curl -sL -o squad/fonts/Inter.ttf \
     'https://github.com/google/fonts/raw/main/ofl/inter/Inter%5Bopsz,wght%5D.ttf'
   curl -sL -o squad/fonts/PermanentMarker-Regular.ttf \
     'https://github.com/google/fonts/raw/main/apache/permanentmarker/PermanentMarker-Regular.ttf'
   curl -sL -o squad/fonts/Caveat.ttf \
     'https://github.com/google/fonts/raw/main/ofl/caveat/Caveat%5Bwght%5D.ttf'
   ```

   Inter and Caveat ship variable-only there (Inter's named instances run Thin to
   Black, Caveat's are Regular and Bold; Permanent Marker is a plain static file), so
   loading the file in Pillow and calling `set_variation_by_name` with the weight the
   cage names is the primary route for those two, not the exception. Verify the
   rendered Inter is actually Black, not the variable default 400. A missing font blocks the type layer; it never swaps
   for another. Primary line 14-28% of frame height (100-200px at 720p); under
   100px fails.
4. **Check.** Build the 320px grid. Download each paired cage's reference thumbnail
   (`i.ytimg.com/vi/<video-id>/maxresdefault.jpg`, the id sits in the cage's proof
   link) and Read both it and the 320px render before you grade anything: a grade
   on an image you did not view is not a grade. Fix order when a pair loses to its
   cage's reference: scale first, then contrast, then wording; and if the gap is a missing
   asset (a face, a real screenshot from the bank's PROOF-ASSET LIST), stop and mark
   the pair blocked-on-assets instead of iterating on the wrong lever.

**Cost discipline (this section is the one authority on model choice; the cage file
defers to it).** Default: Seedream v4.5 edit ($0.04/image). The quality tier (Nano
Banana Pro, $0.15) only when face fidelity fails on the cheap tier or the founder
asks. One base per pair; regenerate ONLY for a note the founder actually gave, and a
face drifted from the refs counts as a failure, not a shrug. A full three-pair package
lands under $1 of image credit; the cost is said and agreed in the one ask at the
beat-1 gate, before any base is generated.

## The review gate (beat 6)

Show the three pairs as one sheet (thumbnail + its title, together, because they are
bought together), each pair with its five checks passed or failed beside it. Write
the sheet as an HTML or image contact sheet at
`squad/week/thumbs/<date>/review-sheet.html` (or `.png`) and tell the founder to open
it the way their OS does (macOS `open`, Windows `explorer`, Linux `xdg-open`, each
followed by `squad/week/thumbs/<date>/review-sheet.html`), then take
their notes; never review off bare file paths. This gate
owns the IMAGES; a title-wording note here is absorbed into the type layer, and only
a claim change routes back through beat 2. Change exactly what the founder names; a
note about one pair never touches another. Repeat until they say lock.

## The output (one file plus the images)

On the default entry, `squad/week/<date>-package.md` (REPACKAGE writes
`<date>-repackage.md` instead, per that section): the three locked pairs in a table,
every claim's receipt named, the five-check sheet, the build log (which cage, which
model, what each revision changed), and the revision variants: whatever unpicked
images the revision rounds actually produced, kept for a CTR swap. (The swap stock is
the two sub TITLES; the revision variants are IMAGES.) Revision variants are a
byproduct, never a reason to generate extra images; when nothing was left over, write
"none." After the pairs lock, the package file also names which locked images the
Waterfall may re-crop or re-title as community-post thumbnail variants: making those
variants is the Waterfall's job from the locked finals, and this skill never generates
spares for it.

The file opens with the two join lines the whole chain keys on, both required,
verbatim as its first two header lines:

    episode: <episodes-root>/epNN/
    source winner: <date>-winner.md

`<episodes-root>` is the roots file's episodes path, `epNN` the episode folder this
video feeds (`ep01`, `ep02`...), and `source winner:` the winner file by exact
filename. The script and deck runs key on those two lines (the script takes the latest
package, then reads ITS named winner; never inferred by date), so a package file
missing either key is unfinished. Create the empty `epNN`
folder when writing the package file, so the numbering rule counts what exists. No
roots file = the episodes root is `squad/episodes/`; the first run names `ep01`,
every later run the next number after the highest existing `epNN` folder. The
thumbnail files sit in `squad/week/thumbs/<date>/` (the run's date, so weekly
runs never overwrite each other), finals plus 1280x720 upload copies.

**A package file already sitting there, marked title-only.** The Payoff Script writes
one when it runs first with nothing but a locked title, so this run ADOPTS it rather
than working beside it: overwrite that file in place with the full package, keep its
`episode:` and `source winner:` lines exactly as they read, and drop the title-only
mark. Never allocate a second `epNN` for a video that already has one, and never leave
two package files for one episode.

Description, chapters, and tags are NOT this skill's job: chapters need the finished
cut, so they belong to the publish step.

Then close, word for word: "Packaged. Writing it is the Payoff Script's job. Run
/the-payoff-script."


## Hand over

The three pairs are locked and the package file names its episode folder and
its source winner. The script is the Payoff Script's job: it reads this
package's main title and writes the hook to it, word for word. Run
`/the-payoff-script`. Not installed yet? Say so plainly and hand the founder
the locked main title, since the hook is written to that promise either way.

Close, word for word: "Packaged. Writing it is the Payoff Script's job. Run
/the-payoff-script. This skill stops here."

## Rules

- Every message to the founder is scannable: a short header, then bullets or a
  table. Operator maps, price bands, and gate grades go in TABLES; findings go in
  short bullets with the key number in bold. Never a wall of paragraphs. The
  founder reads while deciding, not studying.
- The winner's shape earned the views; clone it, never improve it unasked.
- Buyer's words only; check the winner file's comment mining before wording anything.
- Clean wins. Bright grounds, flat color, real UI proof. Dark-with-glow reads as AI
  slop and dies on sight.
- Faces come only from `squad/face/`.
- Never a menu at the review gates: present built things and let the founder react to
  something real. (Beat 1's three titles are not a menu; all three ship as the test's
  slots, and the founder edits rather than chooses.)
