SMART HEALTHCARE PORTFOLIO WEBSITE
Created by Kriti Bhandari
==================================

WHAT IS INCLUDED
- Flask application
- Responsive homepage
- Interactive Tableau Public dashboard page
- Interactive Tableau Public story page
- Shared navigation and styling

PROJECT STRUCTURE
healthcare_portfolio_website/
  app.py
  requirements.txt
  README.txt
  templates/
    base.html
    index.html
    dashboard.html
    story.html
  static/
    css/
      style.css

RUN ON WINDOWS
1. Extract the ZIP file.
2. Open the extracted folder in VS Code.
3. Open Terminal > New Terminal.
4. (Optional but recommended) Create a virtual environment:
      py -m venv venv
      venv\Scripts\activate
5. Install Flask:
      pip install -r requirements.txt
6. Start the website:
      python app.py
7. Open:
      http://127.0.0.1:5000/

TABLEAU
The dashboard and story are embedded from Tableau Public.
They must be published and viewable publicly for visitors to see them.
If you update the Tableau workbook/story URL, edit the iframe src in:
- templates/dashboard.html
- templates/story.html

NOTE
This website embeds your Tableau visualizations; it does not upload or
rebuild the underlying Tableau workbook. The pages need an internet
connection to load Tableau Public.
