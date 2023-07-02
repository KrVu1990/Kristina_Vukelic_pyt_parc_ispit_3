# Kristina_Vukelic_pyt_parc_ispit_3

Za pokretanje skripte otići u root projekta i pokrenuti:

venc\scripts\activate -> ako koristimo Command prompt

I onda:

flask run

Stranica je sada dostpna na:

http://127.0.0.1:5000/

Dodavanje cijene u bazu:

from app.models import Prices
app.app_context().push()
p = Prices (article_name='Pletena narukvica', price = '2')
db.session.add(p)
db.session.commit()