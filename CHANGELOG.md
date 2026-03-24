# Nova Funcionalitat: Crawler Web Dinàmic [1.2.0] - 2026-03-24

1. **Integració de BeautifulSoup4 i Requests:** S'ha implementat un sistema de web scraping que recorre automàticament el domini ebonet.inscastellbisbal.net.

2. **Automatització del Context:** El bot ja no depèn de dades escrites a mà; ara llegeix fins a 99 subpàgines per extreure contingut actualitzat del portafolis digital de l'Edgar Bonet.

3. **Gestió d'Enllaços Interns:** Lògica de navegació per evitar duplicats (neteja d'àncores #) i exclusió de fitxers no textuals (.pdf, .jpg, .zip).

## 🌐 Infraestructura i Connectivitat [1.2.0] - 2026-03-24

1. **Servidor Flask amb CORS:** Creació d'una API interna per permetre que el xatbot rebi consultes des d'entorns externs (com un lloc web de WordPress).

2. **Túnel amb Pyngrok:** Implementació de ngrok per exposar el servidor local de Colab a una URL pública segura, permetent la interacció en temps real fora de Google Colab.

3. **Integració amb Frontend:** Configuració de la ruta /chat (mètode POST) per processar missatges JSON i retornar respostes de la IA.

## 🛠️ Millores Tècniques

1. **Neteja de dades:** El crawler s'ha optimitzat per eliminar elements irrellevants de la web (scripts, styles, nav, footer) i centrar-se només en el contingut textual útil.

2. **Actualització del Model:** Migració a la versió gemini-2.5-flash per a respostes més ràpides i eficients.

3. **Optimització del Prompt de Sistema:** Injecció dinàmica de les dades obtingudes del crawler directament a les "System Instructions".

## 🛡️ Seguretat

**Token d'Autenticació:** Ús de userdata.get("NGROK_TOKEN") per gestionar la connexió del túnel de forma segura sense exposar credencials al codi fon
