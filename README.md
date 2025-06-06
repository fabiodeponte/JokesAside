# Jokes Aside - Measuring the Semantic Distance of Double Meanings

Large language models have significantly enriched the toolkit for computational humor research, particularly in the automated generation of jokes and puns. A key innovation, contextual embedding vectors, offers new opportunities to revisit and refine earlier hypotheses. Notably, Petrovic and Matthews (2013) proposed a joke generation model based on the scheme “I like my X like I like my Y, Z” (e.g. “I like my ice like I like my dreams, crushed”). They suggested that joke hilarity increases with: a) frequent association of Z with X and Y, b) rarity of Z, c) ambiguity of Z, and d) meaning distance between X and Y. Building on this, Winters et al. (2019) proposed a set of metrics, based on Google Ngrams and Word2Vector. In this work, three out of their five metrics are revisited with word embeddings: obviousness, compatibility, and comparison. Another measure, symmetry, defined as closeness of Z to both X and Y, is introduced here for the first time. Two models were used to collect the embedding vectors (OpenAI text-embedding-3-small and MiniLM all-MiniLM-L6-v2) on three datasets: JokeJudger, Expunations, and rJokes. The last two datasets, Expunations, and rJokes, were expanded by adding paired sentences that captured the ambiguous expression at the core of each joke in its two different meanings. Results revealed that models trained on the proposed metrics performed poorly in predicting humor ratings: on JokeJudger, the best model achieved 57.1% accuracy, below the 61.5% baseline, while performance on Expunations and rJokes was even lower. Nevertheless, the symmetry metric seems consistently associated with higher-rated jokes, suggesting it may capture a necessary—though not sufficient—property of humor. Incorporating the two overlooked metrics and employing a broader range of models for both sentence generation and embedding calculations offers further room for investigation.

(Abstract from the paper submitted to the ISHS conference, Kraków, Poland. 7-11 July 2025 - https://ishs2025.pl)

The paper is available here: https://github.com/fabiodeponte/JokesAside/blob/main/fdp%20-%20paper%20-%20Jokes%20Aside.pdf

UPDATE JUNE 6TH 2025: The paper was awarded the GSA AWARD and will be presented during a special plenary session at the ISHS conference.



== NOTE: ==

The largest CSV files were removed from here due to space contraints. The missing datasets can be found on Kaggle, where the entire project was compressed and uploaded:
https://www.kaggle.com/datasets/fabiodeponte/the-complete-humour-project-jokes-aside
