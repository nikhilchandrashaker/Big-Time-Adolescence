# Big Time Adolescence: Analytics Project

An analysis of the 2019 Sundance comedy *Big Time Adolescence* (dir. Jason Orley), covering how critics and audiences received it, how its release unfolded, and how four cast members' film output changed afterwards.

## Contents

| File | What it is |
|---|---|
| `big_time_adolescence_report.pdf` | Two-page written report with charts |
| `big_time_adolescence_analysis.ipynb` | Python notebook (already executed) that produces the numbers and charts |
| `big_time_adolescence_dashboard.html` | Interactive dashboard (also published as a hosted artifact) |
| `data_reception.csv` | Metacritic critic and user rating counts and scores |
| `data_timeline.csv` | Sundance, theatrical and Hulu release dates |
| `data_context.csv` | Hulu acquisition price, Rotten Tomatoes scores, box office status |
| `data_cast.csv` | Credited feature-film roles for four cast members, with a source per row |

## Key findings

- Critics and users are equally positive in share (about 71% positive each). Metascore is 64 and user score is 7.1, so users are slightly warmer and more polarized (about 10% negative vs none for critics).
- 410 days passed between the Sundance premiere (Jan 28, 2019) and release. The limited theatrical release (Mar 13, 2020) and Hulu release (Mar 20, 2020) were 7 days apart.
- No domestic box office is listed by The Numbers or Box Office Mojo.
- Rotten Tomatoes currently lists 86% critics and 80% audience (from a cast filmography page, so treat it as a listing).
- Cast film output diverged: Pete Davidson rose from about 0.3 to 2.3 credited feature roles a year (2016 to 2018 vs 2020 to 2025) and Sydney Sweeney from about 0.7 to 2.0, while Griffin Gluck (1.0 to 0.8) and Machine Gun Kelly (1.7 to 1.0) were flat or lower.
- Same-day release *Never Rarely Sometimes Always* sits in a higher acclaim tier (37 of 38 critic reviews positive).

## Run the notebook

```bash
pip install pandas matplotlib jupyter
jupyter notebook big_time_adolescence_analysis.ipynb
```

Keep the `data_*.csv` files in the same folder. Charts are saved to `charts/`.

## Data sources

Metacritic, Rotten Tomatoes, The Numbers, Box Office Mojo, Wikipedia and Alt Press (Hulu deal, reported via Deadline). Every figure in the CSVs comes from these pages and each row names its source.

## Limitations

- Small samples (21 critic reviews, 31 user ratings) from one aggregator, so the comparisons are descriptive, not statistically established.
- The Rotten Tomatoes figures come from a cast filmography page, and the peer film's Metascore (91) is from a snapshot.
- Box office and Hulu viewership are not publicly available.
- Only one peer film is compared.
- Cast counts are lower bounds from web sources and cover scripted feature films only (no TV, music or documentaries). Premiere year is used where sources disagree (Riff Raff, Americana, Eden). They show association, not causation.

## Possible extensions

Attention proxies such as Google Trends or Wikipedia pageviews for March to April 2020, a wider set of peer films, TV credits for the cast, and dialogue analysis if a script or subtitle file is available.
