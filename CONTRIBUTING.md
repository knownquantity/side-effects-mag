# Contributing to Side Effects Magazine

Side Effects publishes pieces about the second-order consequences of technology and culture. The editorial process happens in the open, in this repo. Submissions are pull requests. Pitches are issues. Reviews are code reviews. The contributor graph is the masthead.

This page is the working manual. Read it before you pitch.

## The two ways to participate

**Pitch first (recommended for new contributors).** Open an issue using the pitch template. We respond within 7 days. If we're in, you write the piece and open a PR.

**Submit directly (faster, more risk).** Fork the repo, add your finished article, open a PR. We'll read and respond. The risk: we might not be the right home for the piece, and you've already done the work.

We accept both. Pitching first is lower-friction for everyone if you're unsure.

## What we look for

Side Effects is about the *second-order* consequences of technology and culture — the things that follow from the things. Strong pitches share a few traits:

- **A specific, falsifiable claim.** "X is changing" is not enough. "X is changing in this way, and here's what becomes true (or stops being true) as a result" — better.
- **First-hand evidence or original analysis.** Pieces that recombine other people's reporting without adding a new lens are not what we publish. Pieces that connect dots no one's connected yet, do something quantitative no one's done, or report from inside a system most readers don't have access to — that's the bar.
- **Stakes that aren't already obvious.** If the consequences your piece traces are visible from the front page of Hacker News, it's probably been said.
- **A clear time horizon.** When does this happen? Who would notice? What would falsify your read?

## What we don't publish

- Hot takes without analysis. "X is bad" or "X is good" without showing the work.
- Vendor or product PR. If you're writing about your employer or a product you ship, disclose, and assume our bar is higher.
- AI doomerism or AI utopianism without specific, falsifiable claims about what changes when.
- Predictions without a time horizon or a defined failure mode.
- Pieces that are mostly about the writer's reaction to a thing rather than about the thing.

Adjacent or hybrid pieces are fine — a personal essay that makes a sharp structural argument is welcome; a structural argument that's actually just a personal essay is not.

## How to pitch

Open an issue using the pitch template. A good pitch fits in ~200 words and includes:

- **A headline.** Working title. Will probably change.
- **A thesis paragraph.** What's the claim? What's the evidence? What would surprise the reader?
- **Why now.** Is there a specific moment, event, or shift this responds to?
- **What you'd need.** A deadline? Interview access? Research time?
- **A short bio plus one or two writing samples.** Especially helpful if you haven't published with us before.

We respond within 7 days, even if it's a no.

## How to submit a full piece

When a pitch is approved (or you're going direct):

1. **Fork** the repo to your own GitHub account. Your fork is private until you open a PR — drafts live there, not here.
2. **Create your file** at `articles/00X-your-slug.md`. The next available ID is the highest existing one + 1. The slug is kebab-case from the title.
3. **Use this frontmatter format** at the top of the file:

   ```markdown
   **Published:** YYYY-MM-DD
   **Tags:** tag-one, tag-two
   **Read time:** X min

   ---

   # The Title of Your Piece

   First paragraph…
   ```

4. **Write the piece.** Standard markdown — headers, bold, italic, fenced code blocks, lists. Plain markdown only; the CLI's renderer doesn't handle HTML or images.
5. **Don't edit `feed.json` or the README archive table.** Editors handle that on merge — it keeps PRs focused on the prose.
6. **Open a PR** from your fork to `main`. Title it `Issue 00X: <working title>`. Link the originating pitch issue if there is one.

## Format guidelines

- **Length:** typically 500–1500 words. Longer if the argument demands it.
- **Tone:** declarative. Make the claim, then defend it. No throat-clearing.
- **No images.** The CLI renders text only. If a chart is essential, link to a hosted version.
- **No tracking links.** Plain URLs only.
- **Inline code, fenced blocks, and tables are fine.** Anything renderable in vanilla GitHub-flavored markdown.

## Editorial process

What happens after you open a PR:

1. **First read (within 7 days).** A senior contributor (initially: Noah McLaughlin) reads the piece end-to-end and either: (a) requests changes, (b) approves, or (c) declines with a clear reason.
2. **Revision rounds.** Edit suggestions are PR comments. You push commits to your branch; the PR updates automatically. We try to keep rounds to two or fewer.
3. **Approval and merge.** Once approved, an editor merges the PR, updates `feed.json` and the README archive, and queues the email send.
4. **Publish.** The piece goes live on merge — `npx side-effects-mag read 00X` works within seconds via GitHub's raw CDN. The email send to subscribers usually follows within 24 hours.

All review happens in PR comments. The thread is public from the moment you open the PR — including any "this paragraph isn't earning its space"-type notes. If that's not the editorial style you want, this isn't the right home for the piece.

## Compensation

We don't pay writers yet. We credit prominently — author byline on the article, author retained in the contributor graph permanently, full freedom to republish elsewhere.

This will change. When it does, the policy will be stated here and pitches accepted after that date will be paid at the prevailing rate.

## Rights and licensing

Writers retain copyright on their pieces. Each article is published under [Creative Commons Attribution 4.0 (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) — readers can share and adapt with credit.

You're free to republish your piece anywhere else, in any form. We ask only that the version here remain the "of record" version, and that republications credit Side Effects Magazine.

## A note on the public-process trade

Working in the open means your pitch and your in-progress prose are visible to anyone who finds the repo. Some writers find this clarifying; others find it stressful.

If the openness changes your sense of risk, work in your fork until the piece is finished, then open the PR. Drafts in your own fork are not visible from this repo. The public-process commitment applies to the merged PR thread, not to your private writing.

## Questions

Open an issue. Don't email. The point is that this happens in public.
