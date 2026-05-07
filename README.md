<div align="center">

# 🛠️ wilf974 / Open Source

**Auditable, deterministic, browser-only decision-support tools.**

*Petits outils open source — déterministes, auditables, sans backend.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with: Vanilla JS](https://img.shields.io/badge/Made_with-Vanilla_JS-f7df1e?logo=javascript&logoColor=black)](#)
[![No tracking](https://img.shields.io/badge/Tracking-None-success)](#)

</div>

---

## 📖 Philosophie

Tous les projets de cette page partagent **la même approche** :

- 🧮 **Calculs déterministes** — chaque résultat est traçable, reproductible, auditable
- 🔒 **Invariants formels** — les règles métier sont explicites et testées (bornes, monotonicité, idempotence)
- 🌐 **100 % navigateur** — un fichier HTML, pas de backend, pas de bundler, pas de framework
- 📱 **Mobile-first** — utilisable sur smartphone en intervention / au lit du patient
- 🚫 **Zéro tracking, zéro pub, zéro dépendance runtime** — code lisible et inspectable
- 📖 **Transparence totale** — toutes les hypothèses et formules sont affichées dans l'app

---

## 🚀 Projets en vitrine

<table>
<tr>
<td width="50%" valign="top">

### 🚒 [FireOps](https://github.com/wilf974/FireOps)

**Aide à la décision sapeurs-pompiers**

Outil pédagogique pour interventions : calculs hydrauliques (débit, lances, pression pompe), autonomie ARI, périmètre NRBC, tri multi-victimes (NOVI). Synthèse worst-case avec action prioritaire toujours visible. Export bilan radio + main courante.

- 💧 Hydraulique · ☣️ NRBC · 🚑 NOVI · 📋 Synthèse
- PWA installable · 100 % offline
- ~130 exemples / 21 invariants formels validés

[![Live demo](https://img.shields.io/badge/Live_demo-wilf974.github.io%2FFireOps-b91c1c?logo=githubpages)](https://wilf974.github.io/FireOps/)
[![Code](https://img.shields.io/badge/Code-FireOps-181717?logo=github)](https://github.com/wilf974/FireOps)

> ⚠️ Outil pédagogique — non certifié opérationnel.

</td>
<td width="50%" valign="top">

### 🏥 [MedTriage](https://github.com/wilf974/MedTriage)

**Scoring clinique d'urgence**

Calcul des scores cliniques NEWS2, qSOFA, HEART avec fusion conservatrice (worst-case) pour un triage global CRITIQUE / URGENT / SEMI-URGENT / STABLE. Audit log complet pour chaque calcul.

- 📊 NEWS2 · 🦠 qSOFA · ❤️‍🔥 HEART
- 14/14 invariants formels vérifiés
- Single HTML — 100 % offline

[![Live demo](https://img.shields.io/badge/Live_demo-wilf974.github.io%2FMedTriage-1a7a4a?logo=githubpages)](https://wilf974.github.io/MedTriage/)
[![Code](https://img.shields.io/badge/Code-MedTriage-181717?logo=github)](https://github.com/wilf974/MedTriage)

> ⚠️ Démonstration technique — pas un dispositif médical certifié.

</td>
</tr>
</table>

---

## 🧰 Stack commun

| Couche | Choix |
|---|---|
| **Front** | HTML5 + CSS3 + Vanilla JavaScript (ES2020+) |
| **Polices** | DM Sans + JetBrains Mono (Google Fonts) |
| **PWA** | Service Worker cache-first + manifest |
| **Hébergement** | GitHub Pages (statique, gratuit) |
| **Build** | Aucun. `python -m http.server` suffit. |
| **Dépendances runtime** | **Zéro**. |

> Le code est volontairement contenu dans un seul fichier `index.html` — un audit de sécurité ou de cohérence métier se fait en 30 minutes.

---

## 🔬 Approche : invariants & auditabilité

Chaque calcul critique est encadré par des **invariants formels** vérifiés à l'exécution :

```js
// Exemple FireOps : pression à la pompe
pression_pompe(p_lance, perte, denivele) {
  // ...calcul...
  this._check(result >= 0 && result <= 16, 'pression_pompe hors bornes');
  return result;
}
```

```js
// Exemple MedTriage : invariant de triage
triage(n2, qs, ht) {
  // @invariant qSOFA ≥ 2 → triage = CRITICAL
  Engine._assert(criticalRequired === isCritical, 'Triage CRITICAL invariant mismatch');
  // ...
}
```

Si un invariant est violé, l'app **affiche un toast d'erreur visible** au lieu de produire un résultat silencieusement faux.

---

## 🗺️ Roadmap commune

- [ ] Validation métier avec des praticiens (pompier formateur, médecin urgentiste)
- [ ] Export PDF des bilans / mains courantes
- [ ] Internationalisation (anglais, espagnol)
- [ ] Versions desktop natives (Tauri ou Electron léger)
- [ ] Bibliothèque partagée d'engine pur (`@wilf974/decision-engine`)

---

## 🤝 Contribuer

Les retours métier sont **précieux**. Si vous êtes pompier, médecin, formateur, infirmier, ou tout autre praticien :

- 📝 [Issues FireOps](https://github.com/wilf974/FireOps/issues)
- 📝 [Issues MedTriage](https://github.com/wilf974/MedTriage/issues)
- 💬 Pull requests bienvenues — surtout les corrections doctrinales

---

## 📜 Licence

Tous les projets sont sous [MIT License](LICENSE) — © 2026 wilf974.

Vous pouvez les utiliser, les modifier et les redistribuer librement, y compris à des fins commerciales, à condition de conserver la mention de copyright et la note de licence.

---

<div align="center">

*Conçu avec rigueur — sans tracking, sans pub, sans backend.*

</div>
