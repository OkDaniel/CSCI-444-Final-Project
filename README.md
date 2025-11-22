# CSCI 444 – Final Project (Group 9)
**Topic:** Esports Professionals vs. Software Engineers  

This repository contains the code and data for Group 9’s final project in CSCI 444.  
The project compares career patterns and earnings of **esports professionals** and **software engineers**.

---

## Duy Nguyen – Esports Section

This part of the project focuses on **esports players and games**.

Data sources:

- **Scraped website**  
  - Top 1000 highest-earning players:  
    `https://www.esportsearnings.com/players/highest-earnings`
- **Kaggle datasets**
  - Player / team age and performance:  
    [Esport_dataset – darvinjawton](https://www.kaggle.com/datasets/darvinjawton/esport-dataset)
  - Game-level earnings and prize pools:  
    [Esports Earnings 1998–2023 – rankirsh](https://www.kaggle.com/datasets/rankirsh/esports-earnings/data)

Cleaned data (saved in `data/`):

- `esports_players_top1000_clean.csv`
- `esports_team_performance_clean.csv`
- `general_esport_games_clean.csv`

Main questions in the esports analysis:

1. **Age & experience** – What does the age and experience distribution of esports professionals look like?  
2. **Game age & prize money** – Do older esports titles tend to generate more total prize money?  
3. **Concentration of earnings** – Which games dominate the income of the top 1000 players?

All analysis, visualisations, and narrative for the esports section are in:

- `Duy_Quarto_Esports.qmd`  
  - Renders to **HTML** and **PDF**  
  - Uses `ggplot2`, `plotly`, and `kableExtra` with `code-fold` enabled.

---

## How to Run (Esports Section)

1. Open the project in **RStudio**.  
2. Install required packages (once):

   ```r
   install.packages(c("pacman", "tidyverse", "rvest", "kableExtra", "plotly"))
