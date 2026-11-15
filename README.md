# LISTEN (hosted app)

Streamlit app for LISTEN (Legal Issue Spotting in Textual Everyday Narratives), a COSC 72 project by Garret Duo, Lyndon Huang and Sohum Sarwate. It suggests which of 20 LIST legal categories a story may involve. It is not legal advice.

This repo only holds what the hosted app needs. The full project, training code and results are in https://github.com/garretduo/LISTEN.

Run locally: `pip install -r requirements.txt`, then `streamlit run app/streamlit_app.py`.

## License and attribution

- Code: MIT (`LICENSE`).
- Model files in `artifacts/app/` are trained on the Learned Hands dataset, which is CC BY-NC-SA 4.0 from the Suffolk LIT Lab and the Stanford Legal Design Lab (https://learnedhands.law.stanford.edu/). The model files carry the same license: give credit, non-commercial use only, share alike.
- `artifacts/story_view/` holds the cleaned Learned Hands stories, labels and splits shown on the data page, under the same CC BY-NC-SA 4.0 license. Links and usernames were removed and whitespace was normalised, so the text differs from the original.
- `emb_mlp.joblib` contains the GloVe 6B 50d word vectors (Pennington, Socher and Manning, 2014; Public Domain Dedication and License v1.0, https://nlp.stanford.edu/projects/glove/).
