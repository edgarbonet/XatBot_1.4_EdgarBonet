# 🤝 Guia de Contribució i Col·laboració de l'Equip

Aquest document descriu com es organitza l'Edgar, i quines són les regles tècniques per afegir-hi codi nou.

## 👥 Membres de l'Equip
- **[Edgar Bonet Pardo]**

## 🛠️ Flux de treball de l'Equip
1. Tota la feina es guarda al repositori de GitHub.
2. Abans de donar una tasca per acabada, sa de revisar que el codi al Google Colab funcioni correctament.
3. Les imatges i evidències es pugen de forma centralitzada al portafolis d'Edgar Bonet.

---

## ⚠️ Regles d'Or per Modificar el Codi (Important)
Per garantir que l'Assistent de la Talentosa funcioni sense problemes i mantenir la ciberseguretat del projecte, tots els membres han de complir això:

1. **🔒 Seguretat (Cap API Key al codi):** Està totalment prohibit escriure la clau de Gemini directament al codi font (*hardcoding*). Si fas proves, assegura't d'utilitzar sempre els secrets de Colab: `userdata.get("GOOGLE_API_KEY")`.
3. **🤖 Ús de la IA Documentat:** Si utilitzeu Gemini com a copilot per afegir noves funcions al xatbot, deixeu un comentari al codi (`#`) explicant què fa aquella línia. El codi generat per IA sempre ha de ser revisat manualment abans de pujar-lo a GitHub.
4. **📝 Estàndard de Commits:** Quan pugeu canvis a GitHub, utilitzeu missatges descriptius per mantenir la traçabilitat:
   - `feat:` per a noves funcions (ex: `feat: afegit suport per a preguntes de DHCP`)
   - `fix:` per a solucionar errors (ex: `fix: resolt error amb les majúscules`)
   - `docs:` per a documentació (ex: `docs: actualitzat el README`)
