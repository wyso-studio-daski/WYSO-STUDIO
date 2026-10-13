# WYSO Studio — file del sito

Stile, script, immagini e video del sito **wyso.it** (Webflow).
Sono serviti dal CDN jsDelivr con l'indirizzo
`https://cdn.jsdelivr.net/gh/wyso-studio-daski/WYSO-STUDIO@<commit>/...`

- `css/`, `js/` — stile e script di ogni pagina (il nome contiene un'impronta: ogni modifica crea un file nuovo)
- `assets/` — immagini e video
- `embed/` — l'HTML di ogni pagina, così com'è nei blocchi di codice di Webflow (`_shared/` = header e footer comuni)
- `webflow/` — per ogni pagina: indirizzo, attributi del contenitore, codice di testa e di chiusura
- `pages/` — ogni pagina completa in un solo file, come copia di riferimento

Non rinominare né spostare i file: il sito li richiama per nome.
Il sito richiama ogni file fissato al commit in cui è stato pubblicato: le versioni precedenti restano disponibili anche dopo gli aggiornamenti.
