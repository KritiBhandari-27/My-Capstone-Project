HEALTH360 WEBSITE — DEPLOYMENT PACKAGE
Created by Kriti Bhandari

PROJECT STRUCTURE
app.py
requirements.txt
templates/
  base.html
  index.html
  dashboard.html
  story.html
static/
  css/
    style.css

RUN LOCALLY
1. Open this folder in VS Code.
2. In the terminal, run:
   py -m venv venv
   venv\Scripts\activate
   pip install -r requirements.txt
   python app.py
3. Visit http://127.0.0.1:5000/

PUBLISH ONLINE WITH RENDER
1. Create/sign in to GitHub and create a new repository.
2. Upload all files and folders in this package to the repository.
   Keep the folder structure exactly as shown above.
3. Sign in to Render and choose New > Web Service.
4. Connect the GitHub repository.
5. Set:
   Language: Python 3
   Build Command: pip install -r requirements.txt
   Start Command: gunicorn app:app
   Instance Type: Free (if offered)
6. Click Deploy. When the service status becomes Live, copy the
   public https://....onrender.com URL and share that URL with your teacher.

IMPORTANT
- Do not share http://127.0.0.1:5000/; it only works on your computer.
- The Tableau dashboard and story are embedded from Tableau Public.
  Their workbooks/stories must be published with public access.
- A free Render service may sleep after 15 minutes without visitors.
  The first visit after sleeping can take about a minute to load.
