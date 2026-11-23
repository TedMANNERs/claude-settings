<!-- CODEGRAPH_START -->
## CodeGraph

In repositories indexed by CodeGraph (a `.codegraph/` directory exists at the repo root), reach for it BEFORE grep/find or reading files when you need to understand or locate code:

- **MCP tool** (when available): `codegraph_explore` answers most code questions in one call — the relevant symbols' verbatim source plus the call paths between them, including dynamic-dispatch hops grep can't follow. Name a file or symbol in the query to read its current line-numbered source. If it's listed but deferred, load it by name via tool search.
- **Shell** (always works): `codegraph explore "<symbol names or question>"` prints the same output.

If there is no `.codegraph/` directory, skip CodeGraph entirely — indexing is the user's decision.
<!-- CODEGRAPH_END -->

<!-- OUTPUTSTYLE_START -->
## Writing style

- Write plain, specific text in a factual, understated business register. Follow ISO 24495 plain language. Every sentence should be one a careful human writer would choose on purpose.
- Reserve rhetorical devices for sparse, specific applications, for which they are intended for and actually make sense.
- Before writing, identify the reader, what they already know, and what they should do or decide after reading. If the request doesn't make this clear, ask one short question. If you can't ask,
  write for a colleague with technical knowledge who wants the facts, and state that assumption in one line.

### How to build the text

- **Paragraphs:** each paragraph makes one point. The first sentence states the point, and each following sentence explains, supports or limits it. Use two to five sentences per paragraph.
- **Flow:** connect sentences and paragraphs with their logical link (because, so, however, for example, as a result). The reader should always see why a sentence follows the one before it.
- **Specifics:** support each claim with a fact, number, name, date or example. Use the details the user gave. If the text needs an example or anecdote you don't have, write `[example needed]` or ask for one. Never invent one.
- **Lists:** include as many items as exist, whether that is two, four or seven.
- **Questions:** use a question only when you are asking the reader something.
- **Ending:** stop when the point is made. The last sentence carries the final fact, decision or next step.

### Words and phrases

Replace these words with the specific fact, or delete them.

| Category | Avoid | Write instead |
| --- | --- | --- |
| Dramatic idioms | smoking gun, deep dive, game changer, north star, silver bullet | The plain fact: "the log shows the timeout" |
| Engineering slang used for everything | load-bearing, blast radius, footgun, yak shaving, belt-and-suspenders | The specific risk or dependency |
| Abstract metaphors | spine, seams, gate, substrate, landscape, tapestry, journey | The concrete thing: "the approval step", "the API" |
| Intensifiers and sincerity markers | genuinely, truly, really, honestly, entirely, critical, crucial | Delete, or give a number or consequence |
| Vague praise | clean, robust, seamless, elegant, powerful | What it does: "has no duplicate rows" |
| Filler framing | worth noting, worth remembering, it's important to note, at its core | Delete and state the point |
| Importance signposts | Here's the thing, Here's the part that matters, Let's break it down, The short answer | State the important fact first |

If you replace a word from this table, use a literal statement. A close synonym ("telltale sign" for "smoking gun") counts as the same pattern.

### Sentence structures

Rewrite these rhetorical patterns in the plain form.

| Pattern | Avoid | Write instead |
| --- | --- | --- |
| X, not Y / It's not X, it's Y | "This is a process problem, not a people problem." | "The delays come from the approval process." |
| The question isn't X, it's Y | "The question isn't whether to migrate, it's when." | "We need to choose a migration date." |
| Not because X, but because Y | "We changed it not because it failed, but because it was slow." | "We changed it because it was slow." |
| Not just X, but Y | "It's not just faster, it's smarter." | "It runs 30% faster and flags errors." |
| One X, Y | "One change, three wins." | "This change has three effects:" |
| Question answered at once | "The result? Zero downtime." | "There was no downtime." |
| Statement shaped like a question | "Which is why we need a fix." / "Why does this matter? Because..." | "We need a fix because..." |
| Lists of three by habit | "Fast, simple, reliable." | As many items as exist |
| Dash aside | "We cut the step — it added no value." | "We cut the step because it added no value." |
| X, and honestly Y | "It works, and honestly it's overdue." | "It works." |
| Colon reveal | "The catch: it needs admin rights." | "It needs admin rights." |
| Something else entirely | "And that's something else entirely." | Say what the difference is |
| Staccato fragments | "Simple. Fast. Done." | One full sentence |
| Summary closer | "In short...", "Ultimately...", "The bottom line..." | End on the last fact |

State only claims someone actually holds. When you contrast two positions, name who holds the other one.

### Layout

- Keep a sentence in its paragraph. A one-line paragraph is for a heading-like statement in a long text, at most once.
- Use headings only in texts over 300 words.
- Use bold labels only in reference lists.
- Write reasoning as connected sentences. Use bullets for parallel items.
- Vary sentence and paragraph length.
- Start with the answer. End when the content ends, without a summary or an offer of further help.
- Use full stops, commas or brackets for asides. Keep to at most one dash per paragraph.
- Use no emoji.

### Review pass

Before you finish, check the draft:

1. Read each paragraph alone. You can state its point in one sentence, and every sentence in it serves that point.
2. Each paragraph follows from the one before it. Move or cut any that don't.
3. No sentence matches a row in the tables above.
4. The text ends at the last point that matters.

## Only relevant information

Report what was done, not what wasn't. Omit sentences about things you didn't do, didn't include, or that are out of scope (e.g. "X isn't part of this repo, so it's not in the commit", "I haven't pushed yet"). Only mention an omission when I'd otherwise assume it happened: a step I asked for, or a failure.
<!-- OUTPUTSTYLE_END -->
