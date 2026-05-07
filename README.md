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

## 🚀 Projets en vitrine — outils opérationnels

> Aide à la décision pour praticiens. Tous **pédagogiques, non certifiés**.

<table>
<tr>
<td width="50%" valign="top">

### 🚒 [FireOps](https://github.com/wilf974/FireOps)

**Aide à la décision sapeurs-pompiers**

Calculs hydrauliques (débit, lances, pression pompe), autonomie ARI, périmètre NRBC, tri multi-victimes (NOVI).

- 💧 Hydraulique · ☣️ NRBC · 🚑 NOVI
- ~130 exemples / 21 invariants

[![Live demo](https://img.shields.io/badge/Live_demo-online-b91c1c?logo=githubpages)](https://wilf974.github.io/FireOps/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/FireOps)

> ⚠️ Pédagogique — non certifié.

</td>
<td width="50%" valign="top">

### 🏥 [MedTriage](https://github.com/wilf974/MedTriage)

**Scoring clinique d'urgence**

Scores NEWS2, qSOFA, HEART avec fusion conservatrice pour un triage global CRITIQUE / URGENT / SEMI-URGENT / STABLE.

- 📊 NEWS2 · 🦠 qSOFA · ❤️‍🔥 HEART
- 14/14 invariants vérifiés

[![Live demo](https://img.shields.io/badge/Live_demo-online-1a7a4a?logo=githubpages)](https://wilf974.github.io/MedTriage/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/MedTriage)

> ⚠️ Démonstration — pas certifié.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🌡️ [HeatGuard](https://github.com/wilf974/HeatGuard)

**Prévention coup de chaleur**

Heat Index + WBGT + plan NIOSH (travail/repos, hydratation). Géolocalisation + Open-Meteo gratuit. 5 niveaux ajustés selon vulnérabilité.

- 🌞 Heat Index · WBGT · NIOSH
- 95 exemples / 18 invariants

[![Live demo](https://img.shields.io/badge/Live_demo-online-c2410c?logo=githubpages)](https://wilf974.github.io/HeatGuard/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/HeatGuard)

> ⚠️ Pédagogique — non médical.

</td>
<td width="50%" valign="top">

### 🪞 [MindMirror](https://github.com/wilf974/MindMirror)

**Sors de ta bulle algorithmique**

Audit URL + test 12 biais cognitifs + onglet Formation (8 biais, 6 manipulations). 100 % local, 100 % privé, aucune donnée envoyée.

- 🔗 Audit · 🧠 Test biais · 📚 Formation
- 71 exemples / 16 invariants

[![Live demo](https://img.shields.io/badge/Live_demo-online-7c3aed?logo=githubpages)](https://wilf974.github.io/MindMirror/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/MindMirror)

> ⚠️ Auto-évaluation — pas clinique.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧾 [PaieAudit](https://github.com/wilf974/PaieAudit)

**Audit de ta fiche de paie française**

Upload PDF (parsé localement via pdf.js) → extraction des 3 nets (imposable/social/à payer), heures sup, primes, retenues. **6 vérifications de cohérence math** : brut = base + hsup + primes, net social = brut − cotisations, taux cotisations ∈ fourchette, etc.

- 📄 Import PDF · 📊 Cohérence math · ⚖️ Indemnités
- 111 exemples / 32 invariants

[![Live demo](https://img.shields.io/badge/Live_demo-online-1d4ed8?logo=githubpages)](https://wilf974.github.io/PaieAudit/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/PaieAudit)

> ⚠️ Audit indicatif — pas un avis juridique.

</td>
<td width="50%" valign="top">

<!-- emplacement libre pour le prochain outil opérationnel -->

</td>
</tr>
</table>

---

## 🔬 Research prototypes

> Travaux de recherche exploratoires sur l'attestation et la défendabilité de claims numériques. **Pas des outils métier — des terrains d'expérience.**

### ⚖️ [VERITAS Stack](https://github.com/wilf974/Veritas)

**Linter symbolique pour claims numériques scientifiques.**

Pipeline en 6 algorithmes Aether qui génèrent, attestent et critiquent des claims numériques :

| Couche | Question posée |
|---|---|
| **Joseph** | Génération d'une claim auto-attestée |
| **Mané Thékel Pharès** | Attestation arithmétique (le calcul se prouve lui-même) |
| **Sept Sceaux** | Structure du raisonnement en 7 dimensions |
| **VERITAS** | Cross-link formule ↔ raisonnement |
| **Pentecôte** | Consensus 12 témoins indépendants |
| **Tribunal** | Réfutation par 7 objections systématiques |

**Objectif** : aider à détecter les incohérences de calcul, les conclusions trop fortes, et les claims insuffisamment défendables — *avant* la peer review humaine, pas à sa place.

**What it is** : a symbolic linter for numerical claims.
**What it is not** : a truth machine, a medical device, or an automated peer reviewer.

| Métrique | Valeur |
|---|---|
| Lignes Aether (stack complet) | ~1 600 · ~140 fonctions |
| Stack complet | 300+ `@example` · 80+ `@invariant` |
| Tribunal seul | 80+ `@example` · 16 `@invariant` · 0 violation |
| Adversarial / benchmark | 400+ probes · 170 tests · case study 10 claims |

[![📖 Lire le cas d'étude (5 min)](https://img.shields.io/badge/📖_Lire_le_cas_d'étude-5_min-b8860b?style=for-the-badge)](https://github.com/wilf974/Veritas/blob/main/examples/case_study.md)
[![Live demo](https://img.shields.io/badge/Live_demo-online-b8860b?logo=githubpages)](https://wilf974.github.io/Veritas/)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?logo=github)](https://github.com/wilf974/Veritas)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/wilf974/Veritas/blob/main/LICENSE)

> ⚠️ **Prototype de recherche** — ne remplace pas la peer review humaine ni l'expertise scientifique. Ne lit pas les papiers tout seul : un humain encode les métadonnées, le stack applique une grille de décision stable.

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
