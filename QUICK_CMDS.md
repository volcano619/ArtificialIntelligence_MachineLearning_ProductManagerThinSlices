# Quick Commands
python eval/build_eval_set.py --n_phone 12 --n_eyes 12 --n_safe 8
python scripts/generate_mock_predictions.py --labels eval/labels.csv --out eval/inference_logs.csv --hit_rate 0.92
python eval/score_eval_plus.py
streamlit run app/streamlit_app.py --server.port 8502 -- --mock true
