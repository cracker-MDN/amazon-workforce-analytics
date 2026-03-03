# Amazon Fulfillment Center Workforce Analytics

**Analyzing 150% annual turnover through NLP sentiment analysis, workforce segmentation, and intervention design**

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![TextBlob](https://img.shields.io/badge/NLP-TextBlob-green.svg)](https://textblob.readthedocs.io/)
[![NLTK](https://img.shields.io/badge/NLP-NLTK-yellow.svg)](https://www.nltk.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

---

## 📋 Project Overview

Amazon Fulfillment Centers face approximately **150% annual turnover**, creating a vicious cycle of recruiting, retraining, and worker overload. This project applies a 6-phase consulting methodology to identify root causes and design a data-driven intervention.

### The Challenge
> How might we reduce turnover by understanding what's really driving employee dissatisfaction — and design a low-cost, high-impact intervention?

### Key Findings
- **140+ Glassdoor reviews + 7 YouTube transcripts** analyzed using TextBlob (sentiment) and NLTK (keyword extraction)
- **43% negative sentiment** on management theme (highest of all themes)
- **Cross-platform insight:** Glassdoor showed 11% negative sentiment vs YouTube 0% — same tools, different linguistic patterns
- **Full-Time Associates** identified as priority segment (58% of workforce, score: 80)
- **Root cause:** Managers lack communication training — promoted for productivity, not people skills
- **Recommendation:** Weekly 10-minute Team Check-Ins with 4-week pilot

---

## 🔬 Methodology: 6-Phase Consulting Journey

| Phase | Focus | Key Output |
|-------|-------|------------|
| **P1** | Define Problem | Executive Briefing Note |
| **P2** | Collect Data | 140+ reviews + 7 YouTube transcripts |
| **P3** | Analyze Sentiment | TextBlob (sentiment scores) + NLTK (n-grams, keywords) |
| **P4** | Find Root Causes | 5 Whys analysis, Root Cause Tree |
| **P5** | Segment Workforce | 5 segments, priority ranking, friction map |
| **P6** | Recommend Solution | Intervention design + pitch deck |

---

## 📊 Key Results

### Sentiment Analysis
```
Theme                          | Mentions | Negative Sentiment
-------------------------------|----------|-------------------
Physical Labor Intensity       | 12       | 38%
Shift Length & Break Policy    | 11       | 35%
Inconsistent Management        | 7        | 43% ← Highest
```

### Cross-Platform Comparison

| Platform | Positive | Neutral | Negative | Sample Size |
|----------|----------|---------|----------|-------------|
| **Glassdoor** | 46% | 43% | 11% | 140 reviews |
| **YouTube** | 29% | 71% | 0% | 7 transcripts |

**Key Insight:** YouTube videos discussed complaints (quitting, long hours, bathroom breaks) yet scored 0% negative. TextBlob detects emotional *words*, not negative *experiences*. Storytelling tone ≠ sentiment.

### Top YouTube Bigrams (NLTK)
- "bathroom break"
- "conveyor belt"  
- "10hour shift"

*Keywords revealed operational pain points that sentiment scores missed.*

### Workforce Segmentation

| Rank | Segment | Count | Priority Score |
|------|---------|-------|----------------|
| #1 | Full-Time Associates | 73 | **80** |
| #2 | Part-Time Workers | 25 | 24 |
| #3 | Pickers & Stowers | 14 | 12 |
| #4 | Contract Workers | 6 | 10 |
| #5 | Managers & Leadership | 7 | 10 |

*Score = Impact × Severity × Size*

### The Burnout Cycle

```
Physical Labor → Fatigue → Long Shifts → Exhaustion → Poor Management → Low Morale
                                            ↑                                    |
                                            └──────── Higher Turnover ←──────────┘
```

---

## 💡 Recommendation

### Weekly Team Check-Ins

10-minute weekly protocol where managers meet with small groups using a conversation guide.

| Criteria | Status |
|----------|--------|
| ✅ Low-Cost | Existing staff, no new tools |
| ✅ High-Impact | Addresses #1 friction point |
| ✅ Measurable | Results visible in 4 weeks |
| ✅ Team-Led | Floor-level ownership |

**Pilot Design:** 4 weeks, Day Shift Zone A, 15-20 associates + 2-3 managers

---

## 🛠️ Tools & Technologies

- **Python:** Pandas, TextBlob, NLTK
- **NLP:** Sentiment analysis (polarity, subjectivity), n-grams, stopword removal, tokenization
- **Excel:** Pivot tables, cross-tabulation analysis
- **Frameworks:** SCQA, 5 Whys, People-Process-Technology
- **Visualization:** Matplotlib, word clouds, custom flowcharts

---

## 📁 Repository Structure

```
amazon-workforce-analytics/
├── README.md
├── data/
│   ├── glassdoor/
│   │   └── glass_reviews_complete.csv
│   ├── youtube/
│   │   └── youtube_sentiment.csv
│   └── combined/
│       └── combined_with_themes.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_sentiment_analysis.ipynb
│   ├── 03_thematic_coding.ipynb
│   └── 04_segmentation_analysis.ipynb
├── outputs/
│   ├── Externship_Project_Summary.pdf
│   ├── Amazon_FC_Intervention_Pitch_Deck.pptx
│   └── Friction_Flowchart.png
└── visuals/
    └── (sentiment charts, word clouds)
```

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/cracker-MDN/amazon-workforce-analytics.git
cd amazon-workforce-analytics
```

2. Install dependencies
```bash
pip install pandas textblob nltk openpyxl matplotlib wordcloud
```

3. Download NLTK data
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

4. Run notebooks in order (01 → 04)

---

## 📈 Key Learnings

1. **Segmentation reveals what averages hide** — "Employees are unhappy" became "Full-Time Associates face compounding burnout"
2. **The loudest problem isn't the most important** — Physical labor had more mentions, but management had highest negativity
3. **Simple solutions beat complex ones** — 10-minute check-ins > expensive software
4. **Combine methods** — Sentiment + keywords together reveal more than either alone
5. **Understand tool limitations** — TextBlob detects tone, not intent; NLTK keywords caught what sentiment missed

---

## 📄 Deliverables

| Deliverable | Description |
|-------------|-------------|
| [Project Summary (PDF)](outputs/Externship_Project_Summary.pdf) | 1-page overview of entire project |
| [Pitch Deck (PPTX)](outputs/Amazon_FC_Intervention_Pitch_Deck.pptx) | 5-slide executive presentation |
| [Friction Flowchart](outputs/Friction_Flowchart.png) | Visual burnout cycle diagram |

---

## 👤 Author

**MD Noornabi**

- LinkedIn: [Connect with me](https://www.linkedin.com/in/YOUR-LINKEDIN-URL)
- GitHub: [@cracker-MDN](https://github.com/cracker-MDN)

---

## 📝 License

This project is for educational purposes as part of the Extern Workforce Analytics Program (Jan - Mar 2026).

---

*If you found this project interesting, consider giving it a ⭐!*
