# 🦋 Motýlí AI Vyhledávač (obrázek → obrázek)

Projekt pro vyhledávání podobných motýlích obrázků pomocí modelu CLIP a Gradio aplikace.

## 📂 Složky

- `app/` – Gradio aplikace připravená pro nasazení
- `notebooky/` – Jupyter notebooky pro testování a vývoj
- `data/` – CSV a obrázky pro testování
- `docs/` – rozšířená dokumentace

## 🚀 Spuštění

1. Nahraj `clip_image_embeddings.pt` do `app/`
2. Spusť `notebooky/clip_image_to_image_gradio_zip_tempfile.ipynb` v Colabu
3. Nahraj obrázek a stáhni podobné jako ZIP

   ----
 # 🦋 Motýlí AI Vyhledávač (text → obrázek) neboli (Text-to-Image Search)
 
Součástí projektu je také vyhledávání podobných obrázků podle textového dotazu pomocí modelu CLIP.


### ✅ Funkce:
- Uživatel zadá libovolný textový dotaz (např. „modrý motýl se žlutými okraji“)
- CLIP převede dotaz do embeddingu
- Vyhledá se 5 nejpodobnějších obrázků z databáze
- Výsledky se zobrazí jako galerie

### 📓 Notebook:
Najdeš v: notebooky/clip_text_search_interactive.ipynb
Notebook používá uložené embeddingy obrázků, umožňuje zadat dotaz přes interaktivní políčko (text_widget), správně načítá aktuální hodnotu i při stisknutí Enter nebo kliknutí na tlačítko

### 🔍 Ukázka použití:
```python
text_query = "průhledný motýl"
# model.encode_text(...)
# top 5 obrázků podle podobnosti
```
> Tento nástroj je ideální pro hledání vizuálních pojmů, které nelze snadno klasifikovat.
