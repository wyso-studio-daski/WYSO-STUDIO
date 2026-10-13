# Messa online del nuovo sito WYSO

Copia di staging: "Copy of WYSO WEBSITE" (6ace6d468d0eb3900f33a04f)
https://wyso-studio-site-6294e71603a82cf9923015.webflow.io

## 301 redirect (Site settings > Publishing > 301 redirects)

Aggiungerli a mano con "Add redirect", in quest'ordine (prima i specifici, poi i jolly).
Non usare "Import": un import CSV sostituisce tutti i redirect esistenti.

| Vecchio percorso | Nuovo percorso |
|---|---|
| /-agenzia-marketing-bergamo-studio | /agenzia-marketing-bergamo-studio |
| /agenzia-comunicazione-marketing-bergamo | /agenzia-marketing-bergamo-studio |
| /progetti-cms/(.*) | /progetti/%1 |
| /servizi-digitali-agenzia-comunicazione-bergamo/(.*) | /servizi |

Note
- I 12 progetti del vecchio CMS hanno lo stesso slug delle nuove pagine /progetti/<slug>,
  quindi basta una regola sola. Le 4 pagine nuove (Ciglia, Medcom, Quise, Wesionary) non avevano un URL prima.
- Articoli del Magazine: stesso percorso di prima (/novita-marketing-aggiornamenti-agenzia-web/<slug>), nessun redirect.
- Già fatto sulla copia: voci CMS Progetti e Categorie non pubblicate, pagina
  "wyso studio bergamo" in bozza, vecchia About in bozza (/about-vecchio).
  Webflow applica un redirect solo se al vecchio percorso non c'è più una pagina.

## Sequenza
1. Cartella Pagine "Progetti" (slug progetti) + 16 pagine case study.
2. Test modulo Contatti e newsletter (Forms + notifiche email).
3. Redirect qui sopra.
4. Piano di hosting e dominio wyso.it spostati sulla copia.
5. Pubblicazione su wyso.it e www.wyso.it; controllo dei vecchi URL.
