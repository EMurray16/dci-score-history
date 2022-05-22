# combined

This folder contains the full DCI score history that exists in this repository, in a single csv file. It also contains the code used to merge the data sources together.

## File Format

In this file, empty cells note missing data, which is normally because a subcaption was not scored in that particular show.

### allScores_2000to2019.csv

This is the only file in this folder. It has had *minimal QA*, which means there are likely some inaccuracies. Users should therefore do thier own QA before using this file.

| Column | Interpretation | Max Score |
| ---- | ---- | ---- |
| date | The date of the performance, in `YYYYMMDD` format. |
| showID | Each show is assinged a unique ID, set differently depending on the data source. It is not safe to assume the IDs are in chronological order, nor is it safe to assume they are the same through time. |
| corps | The name of the corps. Corps names may vary in time, and it is up to the user to be able to match these changes in their own analysis. |
| Subtotal | Score before adjustments, like penalties, are applied. It should be the sum of each of the 3 caption scores, but this may not always be the case. If they disagree, the sum should be used. | 100 |
| GETotal | Total GE score. | Typically 40 |
| MusicTotal | Combined total Music score. | Typically 30, but may be 40 if the visual panel is incomplete or 20 if the music panel is incomplete. |
| VisualTotal | Combined total Visual score | Typically 30, but may be 40 if the music panel is incomplete or 20 if the visual panel is incomplete. |
| GE1A, GE1B, GE2A, GE2B | GE scores of individual judges where applicable. This is used after GE scores were split by Music and Visual. | 20 |
| GEMusic1, GEMusic2 | Music portion of GE score, by individual judge where applicable. | 20 |
| GEVisual1, GEVisual2 | Visual portion of GE score, by individual judge where applicable. | 20 |
| MusicAnalysis1, MusicAnalysis2 | Score for the Music Analysis caption, by individual judge where applicable. | 20 |
| MusicBrass1 | Score for the Music Brass caption. | 20 |
| MusicEnsemble | Score for the Music Ensemble caption. | 20 |
| MusicPercussion1, MusicPercussion2 | Score for the Music Percussion caption, by judge where applicable. | 20 |
| ColarGuard1 | Score for the Visual Color Guard caption. | 20 |
| VisualAnalysis1 | Score for the Visual Analysis caption. | 20 |
| VisualEnsemble | Score for the Visual Ensemble caption. | 20 |
| VisualPerformance | Score for the Visual Performance caption. | 20 |
| VisualProficiency1 |Score for the Visual Proficiency caption. | 20 |
