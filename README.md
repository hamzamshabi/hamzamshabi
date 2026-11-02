# Hamzah Mashabi

**AI Engineer in Madinah, Saudi Arabia.** I build computer vision for real cameras, and LLM agents with the tests that show they work. BSc in Artificial Intelligence, University of Prince Mugrin (2026).

On four projects, checking the data before trusting the number caught a wrong result before it shipped. That habit runs through everything below.

## Featured projects

<table>
<tr>
<td width="44%" valign="top">
<a href="https://github.com/hamzamshabi/industrial-fire-smoke-detection"><img src="https://raw.githubusercontent.com/hamzamshabi/industrial-fire-smoke-detection/main/docs/header.png" alt="Fire and smoke detection on refinery CCTV"></a>
</td>
<td valign="top">
<h3><a href="https://github.com/hamzamshabi/industrial-fire-smoke-detection">Industrial fire & smoke detection</a></h3>
A YOLO26 detector for plant CCTV, and the alarm layer that decides when a detection is worth waking someone up for. On real refinery footage: smoke alarm <b>2.0 s</b> after the first detection, <b>109</b> weak detections filtered, no alarm lost.<br><br>
Found that a dataset import had silently dropped <b>46%</b> of the images, and that at least <b>51%</b> of the D-Fire benchmark's test images have a near-duplicate in its training split.
</td>
</tr>
<tr>
<td width="44%" valign="top">
<a href="https://github.com/hamzamshabi/mosque-crowd-counting"><img src="https://raw.githubusercontent.com/hamzamshabi/mosque-crowd-counting/main/docs/header.png" alt="Crowd density maps of a mosque courtyard"></a>
</td>
<td valign="top">
<h3><a href="https://github.com/hamzamshabi/mosque-crowd-counting">Mosque crowd counting</a></h3>
CLIP-EBC fine-tuned with LoRA and visual prompts on 10,482 images. <b>−23% MAE</b> and <b>−76% RMSE</b> on all 334 UCF-QNRF test images, training <b>0.43%</b> of the weights. Counts from a density map, not identities.<br><br>
Traced a 2.5× over-count to count bins that saturated on dense crowds, and replaced an evaluation that made a worse model look better.
</td>
</tr>
<tr>
<td width="44%" valign="top">
<a href="https://github.com/hamzamshabi/prayer-area-tracking"><img src="https://raw.githubusercontent.com/hamzamshabi/prayer-area-tracking/main/docs/header.png" alt="Tracking a prayer area at Masjid al-Haram"></a>
</td>
<td valign="top">
<h3><a href="https://github.com/hamzamshabi/prayer-area-tracking">Prayer-area tracking</a></h3>
Prayer areas fill and empty, so a zone drawn once drifts off the crowd. This tracks the area itself, with SAM 2.1 or a homography, and counts only the people inside it. Runs on a 4 GB GPU.<br><br>
When tracking fails, the frame is flagged on screen instead of silently corrupting the count.
</td>
</tr>
</table>

## What I'm working on

- **AI Engineer, General Authority for the Care of the Two Holy Mosques** (voluntary, since June 2026). A five-language assistant (Arabic, English, Urdu, French, Turkish) built as a LangGraph agent: it answers from the official service guide with sources and books services inside the chat. Tested on 200 questions: 98.4% faithfulness, 82/82 requests routed right, 22/22 attacks refused.
- **AI Engineer, MAIA (Madinah AI Alliance)** (voluntary, since September 2026). An agent that grades each team's project PDF: Gemini scores it three times against nine criteria, and plain code does the maths and writes the report. Added to the alliance's website in six pull requests.
- **Technical co-founder, Khutaa** (since August 2026). An Arabic-first Umrah transport platform in NestJS, Next.js and PostgreSQL, hosted in Jeddah so pilgrims' data stays in Saudi Arabia.

<details>
<summary><b>Earlier</b></summary>
<br>

- **QSS AI and Robotics**, computer vision intern (2026). The refinery fire detector above, and a smart-shelf restock alarm: I traced a 0.993 score to the model memorising positions from one fixed camera. Splitting by time and adding 133 edited frames gave a real 0.949 on 79 unseen frames, and it shipped.
- **General Authority for the Care of the Two Holy Mosques**, data scientist, cooperative training (2026). The crowd-counting model above, plus Arabic NLP and forecasting on 19,872 service tickets that sized peak-season staffing at about 545,400 SAR a year.
- **JIF Homes and JIF Studio**, full-stack intern (2026). A bilingual CRM in React and Supabase: 18 of the team's 20 merged pull requests, and five permission bugs fixed, including a financial data leak.
- **Graduation project**, crowd monitoring at Quba Mosque (team of three). CLIP-EBC and PVT-v2 on 573 frames (error 8.63 people, R² 0.97), served across 11 zones with a React and Flask dashboard.

</details>

## Stack

**Computer vision:** PyTorch · YOLO · SAM 2.1 · CLIP-EBC · LoRA · ByteTrack · OpenCV · Hugging Face<br>
**LLMs:** LangGraph · RAG · Qdrant · Gemini API · LLM evaluation · guardrails · Arabic NLP<br>
**Engineering:** Python · SQL · TypeScript · Docker · GitHub Actions · PostgreSQL · React · Next.js · NestJS

## Contact

[LinkedIn](https://linkedin.com/in/hamzah-mashabi) · Arabic (native), English (professional)
