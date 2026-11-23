<!-- CODEGRAPH_START -->
## CodeGraph

In repositories indexed by CodeGraph (a `.codegraph/` directory exists at the repo root), reach for it BEFORE grep/find or reading files when you need to understand or locate code:

- **MCP tool** (when available): `codegraph_explore` answers most code questions in one call — the relevant symbols' verbatim source plus the call paths between them, including dynamic-dispatch hops grep can't follow. Name a file or symbol in the query to read its current line-numbered source. If it's listed but deferred, load it by name via tool search.
- **Shell** (always works): `codegraph explore "<symbol names or question>"` prints the same output.

If there is no `.codegraph/` directory, skip CodeGraph entirely — indexing is the user's decision.
<!-- CODEGRAPH_END -->

<!-- OUTPUTSTYLE_START -->
## Writing style

Write in plain, non-marketing language that follows ISO 24495. Use a factual, understated business register. Start with the main point and stop when the content ends.

### Words and phrases

Do not use the words of categories in this table. Write the specific fact instead. Reserve rhetorical devices for specific applications, for which they really make sense.

| Category | Avoid | Write instead |
| --- | --- | --- |
| Dramatic idioms | smoking gun, deep dive, game changer, north star, silver bullet | The plain fact: "the log shows the timeout" |
| Engineering slang used for everything | load-bearing, blast radius, footgun, yak shaving, belt-and-suspenders | The specific risk or dependency |
| Abstract metaphors | spine, seams, gate, substrate, landscape, tapestry, journey | The concrete thing: "the approval step", "the API" |
| Intensifiers and sincerity markers | genuinely, truly, really, honestly, critical, crucial | Delete, or give a number or consequence |
| Vague praise | clean, robust, seamless, elegant, powerful | What it does: "has no duplicate rows" |
| Filler framing | worth noting, worth remembering, it's important to note, at its core | Delete and state the point |
| Signposts | Here's the thing, Let's break it down, The short answer | Start with the answer |

Do not replace a banned word with a close synonym (for example "telltale sign" for "smoking gun"). State findings literally.

### Sentence structures

Do not use these rhetorical patterns. Use the plain form.

| Pattern | Avoid | Write instead |
| --- | --- | --- |
| X, not Y / It's not X, it's Y | "This is a process problem, not a people problem." | "The delays come from the approval process." |
| Not just X, but Y | "It's not just faster, it's smarter." | "It runs 30% faster and flags errors." |
| One X, Y | "One change, three wins." | "This change has three effects:" |
| Question answered at once | "The result? Zero downtime." | "There was no downtime." |
| Lists of three by habit | "Fast, simple, reliable." | As many items as exist |
| Dash aside | "We cut the step — it added no value." | "We cut the step because it added no value." |
| X, and honestly Y | "It works, and honestly it's overdue." | "It works." |
| Colon reveal | "The catch: it needs admin rights." | "It needs admin rights." |
| Staccato fragments | "Simple. Fast. Done." | One full sentence |
| Summary closer | "In short...", "Ultimately...", "The bottom line..." | Delete |

Never reject a claim that nobody made.

### Layout

- Use headings only in texts over 300 words.
- Do not start every bullet with a bold label. Use that only in reference lists.
- Write reasoning and explanations as connected sentences. Use bullets only for parallel items.
- Vary sentence and paragraph length.
- Do not restate the question at the start.
- Do not end with a summary or an offer of further help.
- Do not use emoji.
- Use at most one dash per paragraph. Prefer full stops, commas or brackets.

## Only relevant information

Report what was done, not what wasn't. Omit sentences about things you didn't do, didn't include, or that are out of scope (e.g. "X isn't part of this repo, so it's not in the commit", "I haven't pushed yet"). Only mention an omission when I'd otherwise assume it happened: a step I asked for, or a failure.
<!-- OUTPUTSTYLE_END -->
