# dci.org

This folder contains scores from dci.org. 

## File Formats

In this data, a value of -1 indicates missing data, which normally occurs when a particular subcaption was not judged for a particular show.

### eventual_filename.csv

In these files, a value of -1 indicates empty/missing data, which is most commonly due to a subcaption not being scored a particular show.

### eventual_filename.csv

| Column | Interpretation |
| ---- | ---- |
| showID | Each show is assinged a unique ID at random during compilation, starting at 10000 to avoid conflicting with the fromthepressbox data. It is not safe to assume the IDs are in chronological order, nor is it safe to assume they are the same through time. |
| date | The date of the performance, in `YYYYMMDD` format. |
| corps | The name of the corps as it appeared in the recap. Corps names may vary in time, and it is up to the user to be able to match these changes in their own analysis. |
| GETotal | Total GE score, typically out of 40. |
| MusicTotal | Combined total Music score, typically out of 30. Note that it may be out of 40 if the visual panel is incomplete, or out of 20 if the music panel is incomplete. |
| VisualTotal | Combined total Visual score, typically out of 30. Note that it may be out of 40 if the music panel is incomplete, or out of 20 if the visual panel is incomplete. |
| Subtotal | Overall score, before penalties or other reductions. It would be a good idea to verify this total against the caption totals, and use the caption totals where they disagree. |
| Penalty | Penalty that should be subtracted from the Subtotal to calculate the final score, if applicable. |
| Total | Final, overall score. |
| ColorGuard1, ColorGuard2 | Score for the Visual Color Guard caption, typically out of 20. In practice, there's only ever been 1 color guard judge. |
| VisualAnalysis1, VisualAnalysis2 | Score for the Visual Analysis caption, typically out of 20. In practice, there has only ever been 1 VA judge. |
| VisualProficiency1, VisualProficiency2 | Score for the Visual Proficiency caption, typically out of 20. In practice, there has only ever been 1 VP judge. |
| MusicAnalysis1, MusicAnalysis2 | Score for the Music Analysis caption, typically out of 20, by judge where applicable. |
| MusicBrass1 | Score for the Music Brass caption, typically out of 20. |
| MusicPercussion1, MusicPercussion2 | Scores for the Music Percussion caption, per judge where applicable. This score it typically out of 20. |
| GE1A, GE1B, GE2A, GE2B | Scores by individual GE judge, where applicable. Typically each one judges out of 20, but not always. |


