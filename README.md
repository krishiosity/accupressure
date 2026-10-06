# Everyday Acupressure

An interactive acupressure guide for everyday issues and common health conditions.

- **Symptoms:** headaches, neck and shoulder tension, low back pain, stress, sleep, eye strain, jaw tension, sinus congestion, nausea and motion sickness, digestion, and low energy.
- **Health conditions:** migraine, knee arthritis, carpal tunnel and RSI, constipation, IBS, high blood pressure, cancer treatment side effects, and hay fever.

Pick what you're feeling and where you are right now, then tap a point on the body chart to zoom in. Each point shows how to find it, how to press it, a guided hold timer, cautions, and the research behind it.

It's a companion to the [Acupressure Guide for Women](../acupressure-guide), which covers periods, PMS, and perimenopause.

## Features

- **Symptom-first flow**
  1. Choose a symptom or a health condition. Each condition shows what the research says and when to see a clinician.
  2. Optionally choose where you are: **at your desk**, **in bed**, or **on the go**. Only places with points you can reach there are shown. "On the go" sticks to hands, wrists, and face, so you can press them discreetly.
  3. Get a short list of points and tap one to open it.
- **Front and back body chart** with 33 points that zoom in when tapped. Dashed measuring guides (for example, "4 fingers") show how to find a point from a landmark.
- **Guided hold timer** with breathing cues and a prompt to switch sides for paired points.
- **Pregnancy safety.** A note at the top of the page, a reminder on every point, and a "Pregnant or could be" switch that marks points traditionally avoided in pregnancy.
- **Evidence labels.** Each point says whether it has been studied directly or comes from traditional practice, with links to the sources.
- **"Get medical help if" list** covering red-flag headaches, chest pain, stroke signs, and serious back pain.
- **Accessible color.** A sage, green, and indigo palette in which all text meets WCAG AA contrast (4.5:1 or higher).

## Run it

It's a single static page with no build step and no dependencies.

- Open `index.html` in a browser, or
- Serve the folder: `python3 -m http.server`, then visit http://localhost:8000

### Publish with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.

The site will be live at `https://<your-username>.github.io/<repo-name>/`.

## Editing

The points, symptoms, places, and references are plain JavaScript arrays near the top of the `<script>` block in `index.html` (`POINTS`, `CONCERNS`, `PHASES`, `REFS`).

- To add a point, add an entry to `POINTS`. Its `concerns` list holds the symptom and condition keys it appears under, and its `where` list (`desk`, `bed`, `go`) decides which "Where are you?" options include it.
- `PHASES` holds the three places. The name is shared with the women's guide, where the same slot holds cycle phases.

## Sources

1. Lee A, et al. *Wrist PC6 acupoint stimulation techniques for preventing postoperative nausea and vomiting.* Cochrane Database of Systematic Reviews, 2025.
2. Waits A, Tang YR, Cheng HM, Tai CJ, Chien LY. *Acupressure effect on sleep quality: a systematic review and meta-analysis.* Sleep Medicine Reviews, 2018.
3. Au DWH, et al. *Effects of acupressure on anxiety: a systematic review and meta-analysis.* Acupuncture in Medicine, 2015.
4. Hsieh LLC, et al. *Treatment of low back pain by acupressure and physical therapy: randomised controlled trial.* BMJ, 2006.
5. Hsieh LL, et al. *Effect of acupressure and trigger points in treating headache: a randomized controlled trial.* American Journal of Chinese Medicine, 2010.
6. Zick SM, et al. *Investigation of 2 types of self-administered acupressure for persistent cancer-related fatigue in breast cancer survivors.* JAMA Oncology, 2016.
7. World Health Organization. *WHO Standard Acupuncture Point Locations in the Western Pacific Region.* 2008.
8. Carr DJ. *The safety of obstetric acupuncture: forbidden points revisited.* Acupuncture in Medicine, 2015.
9. Linde K, et al. *Acupuncture for the prevention of episodic migraine.* Cochrane Database of Systematic Reviews, 2016.
10. Cheung DST, et al. *Self-administered acupressure for knee osteoarthritis in middle-aged and older adults: a pilot randomized controlled trial.* Acupuncture in Medicine, 2019.
11. Abbott R, Ayres I, Hui E, Hui KK. *Effect of perineal self-acupressure on constipation: a randomized controlled trial.* Journal of General Internal Medicine, 2015.
12. Asal MGR, et al. *Self-administered active versus sham acupressure for diarrhea predominant irritable bowel syndrome.* BMC Nursing, 2025.
13. Restawan IG, Sjattar EL, Irwan AM. *Effectiveness of acupressure therapy in lowering blood pressure in patients with hypertension: a systematic review.* Clinical Epidemiology and Global Health, 2023.
14. Ezzo J, et al. *Acupuncture-point stimulation for chemotherapy-induced nausea and vomiting.* Journal of Clinical Oncology, 2005.
15. Liang Y, Lenon GB, Li M, Yang AWH. *Feasibility of self-administered acupressure for allergic rhinitis: a pilot randomized controlled trial.* Acupuncture in Medicine, 2022.
16. Mayo Clinic. *Hypertensive crisis: What are the symptoms?*

Links to each source are in the app.

## Medical disclaimer

This guide is for general information and self-care only. For a health condition, use acupressure alongside your treatment, never instead of it. It is not medical advice and does not replace a diagnosis or treatment from a qualified clinician. If you are pregnant or think you might be, don't use acupressure before consulting your OB-GYN or midwife.

## Feedback

Are you a medical professional with feedback? Email **krishiosity@gmail.com**.
