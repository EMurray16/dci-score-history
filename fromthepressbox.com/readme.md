# fromthepressbox.com

This folder contains historical data from fromthepressbox.com. 

## File Formats

### allScores.csv

This is the main score file, *with minimal QA checks*. There is no penalty information. Empty cells note missing data, which is normally because a subcaption was not scored in that particular show.

| Column                             | Interpretation                                                                                                                                                                                                                                     |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| showID                             | Each show has a unique ID, which starts at 101. Each month has its own set of 100 IDs (so the first month starts at 100, second at 200, etc) and each show is indexed from there. It is not safe to assume that the showID is in order temporally. |
| date                               | The date of the show, in `MM/DD/YYYY` format, with leading 0s removed.                                                                                                                                                                             |
| corps                              | The name of the corps. Corps names may vary in time, and it is up to the user to be able to match these changes in their own analysis.                                                                                                             |
| GEMusic1, GEMusic2                 | The Music portion of GE, per judge where applicable, typically out of 20.                                                                                                                                                                          |
| GEVisual1, GEVisual2               | The Visual protion of GE, per judge where applicable, typically out of 20.                                                                                                                                                                         |
| GETotal                            | Total GE score, typically out of 40.                                                                                                                                                                                                               |
| VisualEnsemble                     | Score for the Visual Ensemble caption, typically out of 20.                                                                                                                                                                                        |
| VisualColorGuard                   | Score for the Visual Color Guard caption, typically out of 20.                                                                                                                                                                                     |
| VisualPerformance                  | Score for the Visual Performance caption, typically out of 20.                                                                                                                                                                                     |
| VisualProficiency                  | Score for the Visual Proficiency caption, typically out of 20.                                                                                                                                                                                     |
| VisualAnalysis                     | Score for the Visual Analysis caption, typically out of 20.                                                                                                                                                                                        |
| VisualTotal                        | Combined total Visual score, typically out of 30. Note that it may be out of 40 if the music panel is incomplete.                                                                                                                                  |
| MusicEnsemble                      | Score for the Music Ensemble caption, typically out of 20.                                                                                                                                                                                         |
| MusicBrass                         | Score for the Music Brass caption, typically out of 20.                                                                                                                                                                                            |
| MusicPercussion1, MusicPercussion2 | Scores for the Music Percussion caption, per judge where applicable. This score it typically out of 20.                                                                                                                                            |
| MusicAnalysis                      | Score for the Music Analysis caption, typically out of 20.                                                                                                                                                                                         |
| MusicTotal                         | Combined total Music score, typically out of 30. Note that it may be out of 40 if the visual panel is incomplete.                                                                                                                                  |
| Subtotal                           | Overall score, before penalties or other reductions. It would be a good idea to verify this total against the caption totals, and use the caption totals where they disagree.                                                                      |

### metadata.csv

This file contains the information on the last time the fromthepressbox data was scraped and parsed.

| Column       | Interpretation                                                          |
|--------------|-------------------------------------------------------------------------|
| filename     | The filename of the recap that was parsed.                              |
| lastModified | The last time the scores were modified, according to the file metadata. |
| status       | HTTP status code when the recap file was downloaded.                    |
| url          | The URL at which the recap file can be found.                           |
