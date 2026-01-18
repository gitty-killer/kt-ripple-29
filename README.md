# kt-ripple-29

A small Kotlin tool that computes text statistics for ripple.

## Objective
- Provide quick text metrics for ripple documents.
- Report top word frequencies for fast inspection.

## Use cases
- Validate ripple drafts for repeated terms before review.
- Summarize ripple notes when preparing reports.

## Usage
kotlinc Main.kt -include-runtime -d textstats.jar && java -jar textstats.jar data/sample.txt --top 5

## Output
- lines: total line count
- words: total word count
- chars: total character count
- top words: most frequent tokens (case-insensitive)

## Testing
- run `bash scripts/verify.sh`

## Notes
- Only ASCII letters and digits are treated as word characters.
