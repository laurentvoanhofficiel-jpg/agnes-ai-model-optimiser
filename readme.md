# AGNES·Anvil

> **La forge des capacités manquantes.**
>
> **Détection d’angles morts. Tests adversariaux. Patchs de prompt validés par falsification.**
>
> **Le modèle n’est pas le produit. La capacité à révéler ses faiblesses, à les mesurer et à les corriger est le produit.**

---

## 🎯 La thèse que tout PDG d’IA doit lire avant son prochain board

Pendant deux ans, le marché a confondu **puissance** et **stratégie**.

On a branché les modèles les plus gros. On a empilé les appels API. On a applaudi la consommation de tokens comme d’autres applaudissaient la croissance à tout prix. Puis les factures sont arrivées. Puis les DAF ont posé une question simple :

> **« Combien coûte une décision IA, et pourquoi ce modèle-là ? »**

La plupart des entreprises n’ont pas eu de réponse.

**AGNES·Anvil** existe pour donner une autre réponse — plus profonde, plus opérationnelle, plus stratégique :

> **Un modèle que vous ne savez pas sonder est un modèle que vous ne savez pas gouverner.**
>
> **Un prompt que vous ne savez pas falsifier est un prompt que vous ne savez pas améliorer.**
>
> **Une capacité que vous ne savez pas mesurer est une capacité que vous ne savez pas vendre.**

AGNES·Anvil n’est pas un wrapper d’API. Ce n’est pas un benchmark de plus. Ce n’est pas un dashboard vanity.

C’est un **laboratoire de forge de capacités** : un système qui sonde un modèle cible, détecte ses angles morts, génère des tests adversariaux, arbitre chaque réponse avec un agent critique et un ancrage externe, propose des patchs de prompt, les A/B teste, et ne promeut que ceux qui passent **toutes** les épreuves.

> **Vos applications appellent un modèle. AGNES·Anvil apprend où il casse.**
>
> **Vos équipes écrivent des prompts. AGNES·Anvil prouve lesquels tiennent.**
>
> **Votre board demande des preuves. AGNES·Anvil fournit des traces.**

---

## 📉 Le problème que les grands groupes voient déjà

Les entreprises ne souffrent pas d’un manque de modèles.

Elles souffrent d’un **manque de gouvernance des capacités**.

- Un modèle frontier est appelé pour des tâches triviales.
- Un modèle léger est sous-utilisé sur des tâches où il suffirait.
- Le fine-tuning est lancé sans seuil économique.
- Le RAG, le prompt engineering, le LoRA et la distillation sont arbitrés au feeling.
- La dépendance à un fournisseur devient un risque stratégique.
- Le coût par équipe, par produit, par agent, par décision devient invisible.
- Les faiblesses réelles du modèle — factualité, logique, causalité, calibration, éthique — ne sont ni mesurées ni suivies.
- Les prompts sont modifiés sans A/B test, sans falsification, sans circuit breaker.

Le résultat est toujours le même :

> **Trop de tokens. Trop de fournisseurs. Trop de coûts cachés. Trop peu d’optionalité.**
>
> **Trop de prompts non testés. Trop de faiblesses non mesurées. Trop de décisions non prouvées.**

Le marché a un nom pour la sortie de cette trajectoire : **model maxing**.

Pas le modèle le plus gros partout. Le **bon modèle au bon endroit**, avec le **bon prompt**, sur la **bonne capacité**, au **bon coût**. Les modèles frontier réservés aux raisonnements complexes. Les modèles spécialisés, open-weight ou distillés pour le volume. Une couche d’orchestration qui décide, mesure, arbitre et rend des comptes.

Brian Armstrong l’a formulé comme une prédiction. Satya Nadella l’a formulé comme un avertissement. Les PDG les plus lucides le formulent déjà comme un **impératif de marge**.

AGNES·Anvil ajoute la couche qui manquait :

> **La capacité à sonder, falsifier et patcher les modèles avant qu’ils ne cassent en production.**

---

## ⚡ La réponse AGNES·Anvil

AGNES·Anvil est un **framework de sondage adversarial et d’auto-amélioration** conçu pour les entreprises qui ont dépassé le POC et qui veulent industrialiser l’IA sans sacrifier la marge ni la qualité.

Il s’insère dans votre démarche d’évaluation et d’optimisation. Il classe la tâche. Il génère une sonde. Il teste le modèle. Il évalue la réponse. Il critique la sonde. Il ancre la réponse dans des sources externes. Il détecte les angles morts. Il propose des patchs de prompt. Il les A/B teste. Il les promeut ou les rollbacke.

> **AGNES·Anvil ne remplace pas les grands modèles.**
>
> **AGNES·Anvil les met sous tension.**
>
> **AGNES·Anvil rend les grandes entreprises libres de choisir, de mesurer et de corriger leurs modèles.**

---

## 🏗️ Architecture en un coup d’œil

```text
Application / Agent / Produit / Copilote
        │
        ▼
┌──────────────────────────────────────────────┐
│              AGNES·ANVIL                     │
│        Forge des capacités manquantes        │
│                                              │
│  ┌────────────────────────────────────────┐  │
│  │  Bootstrap méthodologique              │  │
│  │  Axes • Règles • Direction             │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Générateur de sondes adversariales    │  │
│  │  Question • Attendu • Fragilité        │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Test sur le modèle cible              │  │
│  │  Réponse • Latence • Coût              │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Évaluateur impartial                  │  │
│  │  Correct • Partiel • Type d’erreur     │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Agent critique adversarial            │  │
│  │  Non-ambiguïté • Falsifiabilité        │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Ancrage externe                       │  │
│  │  Wikipedia • arXiv • Cache • TTL       │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Détection d’angles morts              │  │
│  │  Sévérité • Reproductibilité • Score   │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Patchs de prompt                      │  │
│  │  Proposition • A/B • Tri-score         │  │
│  └────────────────────────────────────────┘  │
│  ┌────────────────────────────────────────┐  │
│  │  Circuit breaker                       │  │
│  │  Erreurs JSON • Rollback • Trace       │  │
│  └────────────────────────────────────────┘  │
└──────────────────────────────────────────────┘
        │
        ├── Modèle cible : Agnes, ChatGPT / OpenAI, DeepSeek, Mistral, Claude, Gemini, Llama, modèles open-weight
        ├── Sources externes : Wikipedia, arXiv
        └── Stockage local : IndexedDB, localStorage, export JSON
