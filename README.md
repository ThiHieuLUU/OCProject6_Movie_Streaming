#1. Launch the part of API
```bash
sudo apt install -y python3-venv
mkdir OCProject6
cd OCProject6
git clone https://github.com/ThiHieuLUU/OCProject6.git
cd OCMovies-API-EN-FR
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
python manage.py create_db
python manage.py runserver
```

#2. Launch the part of website
Open the file "index.html" in the "OCMovies-FrontEnd" directory.
```bash
cd OCMovies-FrontEnd
firefox index.html &
```
Click on the page, the page will load image films
#3. Discussion
Why the website works with "onclick" but not with "onload"? (see index.html: body onclick="showImages())