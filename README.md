# Edge-Centric ML Framework for Energy-Aware Industrial Control

Quickstart (local):
1. python -m venv .venv && source .venv/bin/activate
2. pip install -r requirements.txt
3. python data/generator.py --profile office --days 7 --out data/samples/office_sample.csv
4. python simulator/env.py  # run minimal sim loop
5. docker build -t edge-emulator ./edge && docker run -p 8000:8000 edge-emulator
6. streamlit run dashboard/app.py

