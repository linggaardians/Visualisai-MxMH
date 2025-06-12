# Musik dan Kesehatan Mental
Proyek ini menjelajahi dampak kebiasaan mendengarkan musik pada kesehatan mental menggunakan dataset mxmh_survey_results.csv.

## Visualisasi
- [Scatter Plot](docs/scatter_musik_kecemasan.html)
- [Diagram Batang](docs/bar_kesehatan_mental.html)
- [Diagram Lingkaran](docs/pie_music_effects.html)

## Model AI
- Random Forest: `random_forest_musik_effects.pkl`
- K-Means Clustering: `kmeans_musik_cluster.pkl`
- Cara penggunaan:
  ```python
  import joblib
  model = joblib.load('random_forest_musik_effects.pkl')
  model.predict([[usia, jam_per_hari, genre_encoded, kecemasan, depresi, insomnia, ocd]])