Malika S D — Portfolio

A single-page portfolio site built from Malika S D's resume, styled around a blueprint/schematic visual theme (fitting for an Electronics & Communication Engineering background) with a hardware-to-software "signal path" as the signature visual.

Files
index.html — the full site. Self-contained: all CSS is inline in a <style> block, and the profile photo is embedded directly as base64, so this one file works standalone with no other assets needed.
How to use it

View it locally Just open index.html in any browser — double-click it, or drag it into a browser window.

Host it for free Any static-hosting service works since it's a plain HTML file:

GitHub Pages — push index.html to a repo, enable Pages in repo settings, done.
Netlify / Vercel — drag-and-drop the file onto their dashboard for an instant live URL.
Structure

The page is organized into sections, each linked from the top nav:

Section	Content
Hero	Name, headline, framed photo, and a diagram linking "Hardware" → "M S D" → "Software"
About	Objective statement + quick stats (CGPA, internships, patent)
Experience	Embedded Systems internship (Emglitz Technologies) and PCB Design internship (Sunshiv Electronics)
Projects	AI-Driven Cyber HoneyPot, Grid-Synchronized Solar Inverter
Patent	Filed patent application on traffic surveillance visibility enhancement
Education	B.E. ECE, Class XII, Class X
Skills	Programming languages, tools, soft skills
Certifications	NPTEL and Infosys courses
Contact	Email, phone, LinkedIn, GitHub
Customizing

Everything lives in one file, so editing is straightforward:

Colors — all colors are CSS variables at the top of the <style> block (--ink, --paper, --copper, etc.). Change these to re-theme the whole site at once.
Photo — replace the base64 string in the <img src="data:image/png;base64,..."> tag, or swap it for a normal file path like src="photo.png" and keep the image alongside index.html.
Text content — all copy is plain HTML inside each <section>; edit directly.
Fonts — loaded from Google Fonts in the <head> (Space Grotesk for headings, Inter for body text, IBM Plex Mono for labels/data).
Notes
Fully responsive down to mobile widths.
Respects prefers-reduced-motion (the hero's animated trace lines are disabled for users who request reduced motion).
Visible keyboard focus states on all links and buttons.
No build step, no dependencies beyond the Google Fonts CDN link — just open and go.
