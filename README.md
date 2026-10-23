# Μονάδα Φροντίδας Ηλικιωμένων «Η Αγία Ταβιθά» — Δήμος Ηλιούπολης

Στατική landing page (HTML/CSS, χωρίς build). Ανοίξτε το `index.html` ή ανεβάστε τον φάκελο σε οποιοδήποτε static hosting (GitHub Pages, Netlify, Vercel).

Μετά από κάθε αλλαγή στο `styles.css`, ενημερώστε το `?v=` στον σύνδεσμο του stylesheet στο `index.html`, ώστε οι browsers να μη φορτώνουν την παλιά έκδοση από την cache:

```sh
sed -i "s|styles.css?v=[0-9a-f]*|styles.css?v=$(sha256sum styles.css | cut -c1-8)|" index.html
```
