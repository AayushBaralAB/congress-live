नेपाली कांग्रेस १५औं महाधिवेशन – Live Voting Result Display
====================================================
Source: https://nepalicongress.org/mahadhiveshan/ummedwar/
811 उम्मेदवार • 80 slides (category-wise) • OBS ready

FILES:
- index.html     = Display (OBS Browser Source + projector)
- admin.html     = भोट हाल्ने पेज
- candidates.js  = सबै 811 उम्मेदवार (नाम, फोटो, NCID, पद, सिट)
- votes.json     = भोट database (admin बाट Export गरेर replace गर्ने)

QUICK START:
1. voting-result folder खोल्नुहोस्, admin.html डबल-क्लिक गर्नुहोस्
2. Category छान्नुहोस्, भोट हाल्नुहोस्, Save थिच्नुहोस्
3. index.html खोल्नुहोस् → auto-slide हुन्छ (12 sec मा turn-by-turn)

OBS SETUP:
- OBS → Sources → + → Browser
- URL: file:///D:/Nepali Congress/voting-result/index.html?obs=1&interval=12
  (वा npx serve चलाएर http://localhost:3000/index.html?obs=1)
- Width: 1920, Height: 1080, FPS 30
- ?obs=1 = controls लुकाउने clean output
- ?interval=15 = 15 sec मा slide, ?slide=5 = 6th category बाट सुरु

CONTROLS (display):
- ◀ ▶ = अघिल्लो/अर्को category, Space = pause/play
- Search = उम्मेदवार खोज्ने, Sort = भोट / ब्यालट नं
- Top N (सिट संख्या) = हरियो "Leading" highlight + vote bar

LIVE VOTE UPDATE:
- एउटै Chrome मा admin + display खोल्दा auto-sync (localStorage)
- OBS (अलग browser) को लागि: admin मा Export votes.json → folder मा replace → display 5 sec मा auto-refresh

DEMO:
- admin मा "Demo भोट" थिच्नुहोस् → random votes भर्छ
