# Style Guide

(See also the group document on paper-writing tips to be linked here at a later date.)

## We generally follow the style of:
[ACS Style Guide](https://pubs.acs.org/doi/full/10.1021/acsguide.50101) (which unfortunately lives behind a paywall; at a later date we should port summaries of key insights here), see especially:
- *Effective writing* (Section 5.1) (use direct, declarative sentences, often in active voice!)
- *General style conventions* (Section 5.3) -- Editorial style (hyphenation, capitalization, modifiers, etc.)
- *Grammar, spelling, and punctuation* (Section 5.2)
- [Strunk & White, “Elements of Style”](https://www.amazon.com/Elements-Style-Fourth-William-Strunk/dp/020530902X/ref=sr_1_1?ie=UTF8&qid=1493395544&sr=8-1&keywords=elements+of+style)
- [Plaxco, “The art of writing science”](https://onlinelibrary.wiley.com/doi/full/10.1002/pro.514)
    - Especially note his rule about how the first sentence of every paragraph should tell the reader what you expect them to get out of the paragraph.

But some issues are worth addressing specifically within the group because they come up particularly often in our work.


## Terms and terminology, word choices (alphabetical order):
- “Atom type”, not “atomtype”
- “Dataset”, not “data set”, when used as a description of a particular entity, such as “we collected this dataset to allow validation of…”
- “Force field”, not “forcefield”
- "Parametrize", not "parameterize"
- "Small molecule", not "small-molecule" (in the context of a "small molecule force field")
- “Predicting”, resist the temptation to use when calculating values which you know. Sometimes acceptable to use for values which have already been measured but are blind to you (e.g. in the context of a blind challenge), but best used for values which have not yet been measured. Use “calculating”, “estimating”, or “computing” if comparing to literature values.
- “Side chain” not “side-chain”
- “Underestimate”/”Overestimate”: Only use for quantities where this has a clear and obvious meaning. Don’t use it for binding free energies, where “underestimate” can refer to the magnitude (so “underestimated” means “binds too weakly”) or the value (so “underestimated” means “binds too strongly”). A similar concern applies to Kd values. Just say something direct, like “the computed binding free energy was too favorable”.
- "Van der Waals": Describes the physical interaction/behavior, in contrast to Lennard-Jones, a particular potential function which can be used to describe this interaction.
- "Pose": Usually used to discuss a static placement of a ligand/small molecule in a receptor. Refers primarily to the placement of the small molecule, NOT to the structure of the receptor.
- "Binding mode": Refers to the overall placement/orientation/conformation of a small molecule bound to a receptor, and gives a less static picture than the word "pose". With care, the idea of "binding mode" can be generalized to include the relevant receptor conformation(s), bound waters, etc. It can also include a group of relevant microstates that correspond to a metastable state.
- OpenFF-specific terms:
  - BespokeFit is the name of the package for fitting custom torsions
  - TorsionDrive scans torsions

## General style:
- **Words**:
    - Technical words: Never use a complex, technical word if there is a simple, ordinary word which says the same thing more directly. Technical words are best reserved for use when they differ in meaning or are more precise. We’re not out to demonstrate our vocabulary but to be clear.
    - “Fancy” words when a simpler will do. Example: Normally prefer “use” to “utilize” (unless you need the slightly different nuance of utilize). Or “elucidate” when you mean show/demonstrate.
    - Active voice: See ACS guidance on direct, declarative sentences, often in active voice.
    - Know the rules before you break them, and only break them for good reasons. Example: Don’t use “And” or “But” at the start of a sentence. But do so when you make a deliberate decision to do so for readability.
    - Throwaway words and other words to avoid:
      - Don’t say “Several X exist…” What are we going to do, talk about nonexistent methods? In general avoid the word “exist”
      - “Obviously”. If it were truly obvious it either wouldn’t be necessary to say it or it would risk insulting your readers. Avoid the word, rephrase, or don’t say it.
      - Usually avoid "we want to highlight that", "importantly", "it is important to note that", etc. Just make your point. Use emphasis words sparingly and only if essential.
    - Throwaway words -- general principles: It’s not necessary/helpful to say something is a certain way unless the opposite would also make sense. So usually don’t use:
        - “Data-driven” -- what’s the alternative? Completely made up? Usually writers insert this as a type of buzzword; it sounds good but doesn’t convey information.
    - Avoid contractions because science papers should be modestly more formal than normal writing
    - Tense: For papers, usually past tense for what we did, present tense for results, and past tense for conclusions except when describing implications. Relatedly, things shown in a figure or table can be referred to in present tense, as the data in the figure or table still shows any observed effect.
- **Phrases, complexity and hedging** -- see https://cgi.duke.edu/web/sciwriting/index.php?action=lesson3
    - Avoid meaningless phrases/excessive wordiness
    - Avoid excessive hedging/caveats
    - Ensure your sentences have simple subjects
- **Sentences:**
    - Prefer concise, direct, clear sentences. If you find yourself having lots of clauses, simplify.
    - Opening material gets the most emphasis. So, try to start with the “what”, not the “how”, for example, not “By running MD simulations looking at …., we found…” but rather, “We examined X using MD simulations. We found…”
    - Prefer simple subjects and verbs for easy reading. While a sentence like "The entry of other water molecules into the binding site in EQ runs of a FXa system (PDB: 1EZQ) when the alchemical water was fully decoupled led to sudden changes in work values in transition simulations." might be grammatically correct, it's hard to follow because the subject is too complex.
    - Transitions: Often use transition words to make clear how subsequent sentences follow from prior sentences.
- **Paragraphs**:
    - Length: Journal articles are typically two column, which means you need to err in the direction of short paragraphs (to avoid having paragraphs which fill entire columns and are hard to parse)
    - Opening sentence: See Plaxco rule above
- **Clarity and correctness**:
    - Strive for clarity and correctness
    - Write as simply as you can while still being correct and precise
      - Being overly precise and technical will cost you clarity
      - Writing in an overly simplified way will cost technical precision
    - Simplify to the point of oversimplification then back off slightly to achieve the simplest explanation which is still correct and complete
- **Structure**:
    - **Section/subsection headers**: Apply the “titles should be statements” rule as much as the journal guidelines will allow for section/subsection headers. Don’t make subsection headers just generic headers (like “MD simulation details”) unless journal guidelines REQUIRE it.
    - **Section/subsection divisions and numbering**: Use as many subsections/divisions as you need to break things up for good readability and easy cross-referencing. If you find you have a five page section, for example, it probably needs division into subsections. However, don’t use an additional level of division unless there will be more than one item at that level. For example, if you decide to break Section 5.1 into subsections so that you have Section 5.1.1, you must also have Section 5.1.2. If Section 5.1 doesn’t need multiple subsections, don’t break it up.
- **Lists**: Items in a list must be the same *kind of thing*. Imagine a grocery shopping list reading "Apples, lettuce, crackers, puppies, cheese". One of these would likely be shocking. More typically in academic writing one will be tempted to mix questions with statements, or mix tenses, or other variations. Don't. Ensure items in a list have a consistent kind.
- **Methods**: If describing methods used in a project (such as in a paper) and your work closely follows the methods from a previous study, it's appropriate to cite the prior study and describe your methods more concisely, referring to that study for more details. However:
    - Your study should always at least concisely summarize your methods
    - Your work must make clear how to find full details and reproduce your work
    - Never send your readers on a chase; while you can cite a prior study for details, if THAT study cites a prior study for details you're wasting the reader's time. No "Russian doll" methods sections.
- **References**:
  - Don’t refer to authors by name in the text unless it helps your discussion to do so or is important to your narrative.
  - Ensure your sentences flow naturally and grammatically even without the reference. So DO write "Previous work discussed this extensively [39-47]," but not "For additional discussion, we refer the reader to [37-47]."
- **Acknowledgments**: Be generous. If someone gave you an idea which was helpful, or helped with scripts, code, queuing system, whatever, acknowledge them. It costs you nothing.
- **Authorship**: If someone helped the project significantly, even in terms of providing key ideas, consider asking if they would like to be a co-author (discussing with your PI too). It costs almost nothing.
- **Figure captions**: Try to make them self-contained so they provide a concise summary of the figure, including its main point(s). Figures+captions should be stand-alone enough that someone can understand what it’s showing without reading the text. The main take-away of the figure should be clearly stated in the caption.
- **Figure subtitles**: If journal style allows, the caption should ideally start with a single-phrase header/subtitle in boldface which is not a complete sentence, then the rest of the caption should use complete sentences.
- **Table captions**: Generally the same considerations apply as for figure captions.
- **Other practical tips for clarity and correctness**:
    - Be very careful of the use of "its" in sentences with multiple nouns; [this choice of word often dramatically reduces clarity](https://reason.com/volokh/2022/06/15/its-a-problem/).
    - Exercise considerable care when using negatives. Avoid constructions like "failed to X all the Y" ("failed to sample all of the relevant states" -- did it sample none of the relevant states? Or it sampled some but not all?), or "not X in both of of the Y" ("not sampled in both of the trials" -- was it sampled in one, or neither?)
- **Figure, table and section numbering/naming** (except when journal style dictates otherwise):
  - In text, use "Sec. 1", "Fig. 1", "Table 1" for sections, figures and tables
  - In figures, use lowercase letters for panel numbers, e.g. "(a)" not "(A)"
  - Section titles should use title case, rather than capitalizing only the first letter

## Tips if using LaTeX for writing

We often use LaTeX (e.g. Overleaf) for writing papers. Some LaTeX-specific tips are helpful:
- Figures and floating objects should usually use LaTeX to do the work of placement; don't be overly insistent on where they go, with lots of `[h!]` and `[H]` position instructions in your placements of figures and tables; this can result in odd appearances
- If you are making a final manuscript with LaTeX that needs to be publication quality (e.g. for LiveCoMS) pay careful attention to figure placement in the final version.
- Abbreviate journal titles in bibliographies; if using a citation manager like Zotero, check the "use journal abbreviations" box on export to ensure this happens.

## Graphics and Figures
- Always use clear axis labels, with large enough fonts for the display size
- Consider colorblindness (e.g. see this post for [some considerations](https://www.tableau.com/about/blog/examining-data-viz-rules-dont-use-red-green-together), though Google for many more) and pick colorblind-friendly palettes and ensure that you use more than color to distinguish key aspects of your data

## Writing documentation for software

- **Tone**: Aim for a friendly, conversational, clear tone.
    + Software documentation does not need to be as formal in tone as a paper
        * You can end sentences in prepositions if you want to.
        * It's OK to freely split infinitives.
        * Prefer active voice to passive voice.
    + Avoid slang - documentation should be accessible to as wide a readership as possible
- **Living document**: Unlike a paper, documentation is easy to update if we find readers are commonly making the same misinterpretations. This means we can err on the side of clarity in the clarity/correctness trade-off.
- **Links**: Use hyperlinks liberally.
    + Use links to...
        * Provide detail on technical terms for unfamiliar readers
        * Acknowledge other writing or software projects
        * Connect related parts of documentation that are separated by the flow of prose
    + Make a link out of your natural prose where possible, rather than saying "click here"
    + *Always* link to the API reference of a method or object the first time you introduce it in a page's prose.
- **Check output**: Always do a final proof read on the rendered output, not on the markup. This will let you spot syntax errors and other incorrectly rendered documentation
- **The software does things**: When describing a behavior or principle of the software, write as though the software is an agent that does things rather than a product produced by the developers. Prefer making the software the subject of a sentence rather than the developers
    + "When input is ambiguous, the toolkit should raise an error rather than guess" rather than "When input is ambiguous, we always try to raise an error rather than guess"
        * It's nice/polite to include the reader whenever we use the word "we". If "we" is the dev team, this excludes the reader.
    + "The `rmsd()` function computes the root mean square deviation" rather than "Use the `rmsd()` function to compute the root mean square deviation"
- **Write code examples**: Lots of people find programming easier to learn by example than by theory, and it's convenient to be able to copy-paste the most common usages of a library.
- **Write docstrings**: At minimum, every function or type in a public API should have a docstring.
    + Function docstrings should at minimum describe every argument and what output is produced.
    + Class docstrings should at minimum describe the purpose of the class.
    + Great docstrings include examples of common use; errors, exceptions, and panics that the code can cause; any side effects or argument mutation; background information needed to understand what the code does; and the purpose and intended use of the code.
    + Whenever you change the source of an object, check to make sure that the docstring is still correct and complete.
- **Types**: Code examples and notebooks are much easier to read when the reader knows or can discern the types of each variable
    + When you introduce a function, describe its type signature, especially its return type
    + Talk explicitly in prose about the types of variables - what they're for, what data they hold, and what methods/behaviors they have
    + Link to the API docs for types as you introduce them
- **Code in prose**: Render names taken verbatim from code in `monospaced font` to signal that it is code, but don't overdo it
    + Code used to invoke software often has a similar name to the software itself, but this doesn't mean that they're interchangeable. In prose, call things by their (correctly capitalized) name, not their invoking command.
        * "Python", not "`python`", "`python3`", or "python"
        * "GROMACS", not "`gmx`" or "Gromacs"
        * "Conda", not "`conda`" or "conda".
        * "Amber", not "AMBER"
    + Don't pluralize or otherwise conjugate names from code when they're monospaced. "`ForceField` objects", not "`ForceField`s" or "`ForceFields`". "Run `python`" or "Run Python", not "Run `Python`"
    + Feel free to come up with English names for the objects you're describing. This can make reading easier, as the prose is not constantly changing font, but also makes writing easier
        * "The `np.array()` function returns an array, which stores its contents in contiguous memory. Arrays are instances of the `ndarray` class."


## Git Friendliness

Git's line-based diffing algorithm is great for code, but doesn't play very nicely with prose. There are three strategies for dealing with this:

- **Use hard-wrapping; break at <= 80 characters**: This strategy introduces
    hard line breaks at word boundaries if a word would run over 80
    characters line width. This can be a bit of a pain to write in editors
    that don't automate hard wrapping, but it looks great to read in any
    editor. Paragraph breaks involve a double line break. Diffs usually
    include the remainder of the paragraph after the spot where a change
    occurred, but small changes can be isolated to a single line.
- **Use soft-wrapping and break at paragraph boundaries.**: This strategy uses your text editor's line wrap functionality to wrap text. It's easy to write and doesn't require any post-processing, but can be problematic when viewed without soft-wrapping. With this strategy, git diffs include the entire paragraph surrounding any changes, and multiple changes to a paragraph will be rendered as a single diff.
- **Break at sentence boundaries**: This strategy introduces a line break at the end of every sentence, and a double break at the end of paragraphs.
This establishes an analogy between sentences and lines of code, but usually doesn't look great.
It does, however, produce very clean diffs, as changes to a sentence only include that sentence in the diff, and not the following sentences.

## Other Reminders:
- **Report uncertainties with one significant digit of precision**. Round the associated value to the correct precision based on the uncertainty. For example, “3.247 +/- 0.134” becomes “3.2+/-0.1”, and “0.3247 +/- 0.0134” becomes “0.32+/-0.01”, etc. Deal with the uncertainty first, then round the value accordingly.
- **Render values as number-space-unit** 7.8 mm, not 7.8mm. Prefer SI units over non-SI alternatives. Uncertainties go before units: 31.4±0.9 kJ/mol.
- **Use dashes correctly**
    - hyphen `-` "-": Separates compound words and words broken over a line-break
    - en dash `--` "–": Separates ranges of numbers: 1–5
    - em dash `---` "—": Separates distinct clauses — or parentheticals — within a sentence
- **Use spell check** It makes life easier. All major text editors should either have spell check built in, or have a plugin available for it, so writing in LaTeX or Markdown is not an excuse.
