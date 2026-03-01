# UniversityLens

UniversityLens helps students check a college degree with practical data, not only rankings.

You can enter university + course and get a simple report with:
- salary range after graduation
- loan/debt pressure
- dropout and placement trend
- visa chance (for international students)
- student pain points like burnout/admin issues

It uses Gemini for analysis and shows output in a clean blue dashboard.

## Main Features

- ROI score
- Academic pressure index
- Social isolation risk
- Career outcome probability
- Role-wise salary insights
- Currency switch (local / USD / other)
- Export report as PNG

## Tech Used

- Python Flask (backend)
- HTML/CSS/JS (frontend)
- Gemini API

## Run Locally

1. Create venv and activate
2. Install requirements
3. Add `.env` with Gemini key
4. Run app

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Open: `http://127.0.0.1:5001`

## .env Example

```env
GEMINI_API_KEY=your_key_here
GEMINI_MODEL=gemini-2.5-flash
GEMINI_FALLBACK_MODELS=gemini-2.0-flash,gemini-1.5-flash
```

## Note

If you see 429 error, it means API free-tier/rate limit issue. Wait a little and retry.
