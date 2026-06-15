# Maturita z matematiky → Python

Řešení **7 úloh** z didaktického testu CERMAT z matematiky (**MA_2025**, jaro 2025)
pomocí Pythonu — knihovny `sympy`, `numpy`, `matplotlib`.

U každé úlohy je podle zadání uvedena **myšlenka řešení → matematický zápis → Python kód →
výsledek a interpretace**. Hlavním cílem je *porozumět* tomu, co kód počítá.

## Výběr úloh

Z každé kategorie zadání byla vybrána jedna úloha:

| # | Kategorie | Úloha | Co procvičuje |
|---|-----------|-------|---------------|
| 1 | Základní výpočet (povinné) | **1** – nákup borůvek | jednotkové ceny, poměr |
| 2 | Algebra / úpravy | **4** – zjednodušení výrazu | symbolická algebra (`sympy.simplify`) |
| 3 | Rovnice / soustavy | **7** – soustava 3 lin. rovnic | lineární algebra (`numpy.linalg`, `sympy`) |
| 4 | Funkce a graf | **9** – kvadratická a lineární funkce | grafy funkcí (`matplotlib`) |
| 5 | Geometrie | **20** – zvýšení hladiny vody | objem koule a válce |
| 6 | Pravděpodobnost / kombinatorika | **15** – hod dvěma kostkami | klasická pst + simulace (Monte Carlo) |
| 7 | Model / posloupnost / růst | **23** – exponenciální růst bakterií | exponenciální model, logaritmus |

## Výsledky

| Úloha | Výsledek |
|-------|----------|
| 1 — borůvky | **624 Kč** |
| 4 — výraz | **1 − 4a²** |
| 7 — soustava | **x = 18, y = 3, z = −9** |
| 9 — funkce | **g: y = 2x − 2**  (body A[4; 6], B[0; −2]) |
| 20 — hladina | **+1,00 cm** (odpověď D) |
| 15 — kostky | **15.1 A, 15.2 N, 15.3 N** |
| 23 — bakterie | **8 hodin** (odpověď D) |

## Soubory

- `maturita_reseni.ipynb` — hlavní řešení (Jupyter notebook s komentáři, vzorci a grafy)
- `maturita_reseni.py` — totéž jako spustitelný skript (grafy uloží do `img/`)
- `build_notebook.py` — generátor notebooku (reprodukovatelnost)
- `img/` — vygenerované grafy (úlohy 9 a 23)
- `requirements.txt` — seznam knihoven

## Jak spustit

```bash
python3 -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt

# varianta A – notebook
jupyter notebook maturita_reseni.ipynb

# varianta B – skript
python maturita_reseni.py
```

## Poznámka k autorským právům

Zadání úloh pochází z veřejně zveřejněného didaktického testu **Centra pro zjišťování
výsledků vzdělávání (CERMAT)**. Originální testy jsou dostupné na <https://maturita.cermat.cz>.
