# GenomeAI — DNA Intelligence Platform

A responsive, static educational web application for exploring DNA sequence composition and a simple classification example. Built with HTML, CSS and vanilla JavaScript; no build step or API key is required.

## Features

- DNA sequence input with validation (A, T, G, C only)
- Feature extraction: A/T/G/C counts, sequence length and GC content
- Interactive nucleotide composition bar and chart
- Four assignment-provided training samples (S1–S4)
- Educational GC-content decision-rule demonstration for Group A / Group B
- Load sample sequences with one click
- Export the feature table as CSV
- Responsive layout and light/dark appearance toggle

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.

No package installation is needed.

## Deploy to Vercel

### Option 1: Import from GitHub

1. Create a GitHub repository and upload `index.html`, `style.css`, `app.js`, and `README.md`.
2. Sign in to Vercel and choose **Add New → Project**.
3. Import your GitHub repository.
4. Keep the Framework Preset as **Other**.
5. Leave Build Command and Output Directory empty (or use `.` as the output directory if prompted).
6. Click **Deploy**.

### Option 2: Vercel CLI

If you have Node.js and Vercel CLI installed, run `vercel` from this project folder and follow the prompts.

## Important academic note

The assignment asks students to run a Python / Google Colab classifier, report the model output and accuracy, and submit a PDF with screenshots and discussion. This website is an interactive companion/demo, not a replacement for that required Python implementation.

The browser demo uses a transparent one-split rule on GC content (threshold 56.25%) to illustrate classification on the four supplied examples. It is **not** an actual scikit-learn DecisionTreeClassifier, does not perform independent testing, and does not establish reliable predictive performance. With only four samples, training accuracy is not evidence of generalization. The unknown sequence's true group is not supplied, so prediction correctness cannot be confirmed.

This educational tool is not intended for medical, diagnostic, clinical or research use.
