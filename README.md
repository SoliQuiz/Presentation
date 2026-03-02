---
marp: true
theme: default
_class: lead
_paginate: false
paginate: true
backgroundColor: #ffffff
style: |
  section {
    font-size: 22px;
    color: #333;
    line-height: 1.6;
    padding: 60px 80px;
  }
  footer { width: 100%; text-align: right; font-size: 14px; color: #888; }
  .logo-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: absolute;
    top: 40px;   
    left: 60px;
    right: 60px;
  }
  .logo-header img { height: 140px; margin: 0; margin-left:10px; margin-right:10px }
  h1 { color: #088dc7; font-size: 2.8em; margin-top: 100px; text-align: left; }
  h2 { color: #088dc7; font-size: 2em; border-bottom: 2px solid #088dc7; margin-bottom: 40px;}
  h3 { text-align: left; color: #444; margin-top: 0; }

  .sommaire-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 20px;
  }
  .sommaire-item {
    display: flex;
    align-items: center;
    background: #f4faff;
    border-radius: 12px;
    padding: 15px 20px;
    border-left: 5px solid #088dc7;
  }
  .sommaire-num {
    background: #088dc7; color: white; width: 35px; height: 35px;
    display: flex; justify-content: center; align-items: center;
    border-radius: 50%; font-weight: bold; margin-right: 15px; flex-shrink: 0;
  }
  
  .img-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
  }
  .img-methodo {
    width: 85%;
    height: auto;
    max-height: 450px;
    object-fit: contain;
    border-radius: 10px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }

  .dt-card {
    background: #f0f7fa;
    padding: 30px;
    border-radius: 10px;
    border-top: 6px solid #088dc7;
    text-align: left;
    margin-top: 20px;
    width: 100%;
  }

  /* --- FIX COULEURS TECH STACK --- */
  .tech-container {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 20px;
  }
  .badge-simple {
    padding: 8px 18px;
    border-radius: 6px;
    font-weight: 600;
    background-color: #545353ff; /* Gris foncé unique */
    color: #ffffff !important;
    font-size: 0.85em;
    border: 1px solid #222;
  }
  .maquette-grid {
    display: flex;
    gap: 15px;
    justify-content: center;
    align-items: flex-start;
    height: 350px;
  }

  .context-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 10px;
  }
  .context-card {
    background: #f4faff;
    border-radius: 10px;
    padding: 20px 25px;
    border-left: 5px solid #088dc7;
  }
  .context-card h4 { color: #088dc7; margin: 0 0 10px 0; }
  .problem-card {
    background: #fff5f5;
    border-left-color: #e74c3c;
  }
  .problem-card h4 { color: #e74c3c; }

  /* New Premium Cards for Empathie/Ideation */
  .persona-card {
    background: #ffffff;
    padding: 18px;
    border-radius: 14px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.05);
    border-top: 5px solid #088dc7;
    transition: transform 0.3s ease;
  }
  .persona-card strong { font-size: 1.1em; display: block; margin-bottom: 8px; }
  .persona-card p { font-size: 0.85em; margin: 0; color: #555; line-height: 1.4; }

  .ideation-badge {
    display: inline-block;
    padding: 4px 10px;
    border-radius: 20px;
    font-size: 0.75em;
    font-weight: bold;
    margin-right: 5px;
    margin-bottom: 5px;
  }

---


<div class="logo-header">
  <img src="images/ofppt-logo.png" alt="Logo Left">
  <img src="images/solicode_logo.png" alt="Logo Right">
</div>

# **Projet de Fin de Formation**
### Système de QCM Interactif — **SoliQuiz**

**Réalisé par :** <span class="highlight">BENYEKHLEF Anouar</span>  
**Encadré par :** <span class="highlight">M. ESSARRAJ Fouad</span>  
**Filière :** Développement Mobile et Web

---

## Sommaire

<div class="sommaire-grid">
  <div class="sommaire-item"><div class="sommaire-num">1</div><div class="sommaire-text">Contexte du projet</div></div>
  <div class="sommaire-item"><div class="sommaire-num">2</div><div class="sommaire-text">Méthodologie de travail</div></div>
  <div class="sommaire-item"><div class="sommaire-num">3</div><div class="sommaire-text">Branche Fonctionnelle</div></div>
  <div class="sommaire-item"><div class="sommaire-num">4</div><div class="sommaire-text">Branche Technique</div></div>
  <div class="sommaire-item"><div class="sommaire-num">5</div><div class="sommaire-text">Conception</div></div>
  <div class="sommaire-item"><div class="sommaire-num">6</div><div class="sommaire-text">Démonstration</div></div>
  <div class="sommaire-item"><div class="sommaire-num">7</div><div class="sommaire-text">Conclusion</div></div>
</div>

---

## 1. Contexte du projet

<div class="context-grid">
  <div class="context-card">
    <h4>🎯 Présentation</h4>
    <p><strong>SoliQuiz</strong> est un projet de fin de formation, conçu pour répondre aux besoins concrets du centre digital <strong>Solicode</strong>.</p>
    <p>Il s'agit d'une plateforme centralisée pour la <strong>création, le passage et l'analyse de QCM</strong>.</p>
  </div>

  ---
  <div class="context-card problem-card">
    <h4>⚠️ Problématique</h4>
    <ul>
      <li>**Aveuglement pédagogique** : Manque de visibilité en temps réel sur l'acquisition des compétences (scores déconnectés des objectifs).</li>
      <li>**Invisibilité des lacunes** : Incapacité technique d'associer les questions aux micro-objectifs pédagogiques.</li>
      <li>**Stagnation de l'apprentissage** : Feedback "sec" sans explications, limitant les axes d'amélioration.</li>
      <li>**Rupture administrative** : Report manuel chronophage vers SoliLMS et fragmentation de l'expérience (pas de mobile).</li>
    </ul>
  </div>

  ----
  
  <div class="context-card">
    <h4>👥 Acteurs</h4>
    <ul>
      <li><strong>Étudiant :</strong> Passer les QCM & suivre sa progression</li>
      <li><strong>Formateur :</strong> Créer les QCM & consulter les résultats</li>
      <li><strong>Administrateur :</strong> Superviser & piloter la plateforme</li>
    </ul>
  </div>
  
  <div class="context-card">
    <h4>✅ Objectifs</h4>
    <ul>
      <li>Remplacer Google Forms par un outil interne</li>
      <li>Automatiser le flux d'évaluation</li>
      <li>Lier chaque QCM à un objectif précis</li>
      <li>Synchroniser les notes avec SoliLMS via API</li>
    </ul>
  </div>
</div>

---

## 2. Méthodologie : Design Thinking



<div class="img-container">
  <img src="images/design-thinking.png" class="img-methodo" alt="Design Thinking">
</div>

---

## Méthodologie : Scrum (Agile)

<div class="img-container">
  <img src="images/scrum-process.jpg" class="img-methodo" alt="Scrum">
</div>

---

## Méthodologie : Processus 2TUP

<div class="img-container">
  <img src="images/2tup.png" class="img-methodo" alt="2TUP">
</div>

---

## 3. Branche Fonctionnelle : Design Thinking
### 1. EMPATHIE

<div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; margin-top: 10px;">
  <div class="persona-card" style="border-top-color: #f39c12; background: linear-gradient(180deg, #fff9f0 0%, #ffffff 100%);">
    <strong style="color: #f39c12;">👩‍🏫 Fatine (Formatrice)</strong>
    <p>Besoin de QCM simples avec correction automatique et calcul instantané du score pour gagner du temps.</p>
  </div>
  <div class="persona-card" style="border-top-color: #088dc7; background: linear-gradient(180deg, #f0f7ff 0%, #ffffff 100%);">
    <strong style="color: #088dc7;">👨‍🏫 Youssef (Formateur)</strong>
    <p>Exige une structuration fine par session et une liaison directe avec les objectifs pédagogiques suivis.</p>
  </div>
  <div class="persona-card" style="border-top-color: #27ae60; background: linear-gradient(180deg, #f0fff4 0%, #ffffff 100%);">
    <strong style="color: #27ae60;">👤 Fouad (Admin)</strong>
    <p>Priorise la gestion sécurisée des accès, des rôles et le pilotage global des performances du centre.</p>
  </div>
</div>

<div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 20px; margin-top: 20px; width: 80%; margin-left: auto; margin-right: auto;">

---

  <div class="persona-card" style="border-top-color: #9b59b6; background: linear-gradient(180deg, #fdf2ff 0%, #ffffff 100%);">
    <strong style="color: #9b59b6;">🎓 Mehdi (Étudiant)</strong>
    <p>Réclame une expérience Mobile-first, avec auto-sauvegarde et timer pour réduire l'anxiété pendant les tests.</p>
  </div>
  <div class="persona-card" style="border-top-color: #e74c3c; background: linear-gradient(180deg, #fff5f5 0%, #ffffff 100%);">
    <strong style="color: #e74c3c;">🎓 Soufiane (Étudiant)</strong>
    <p>Attend un feedback pédagogique détaillé et un suivi visuel clair de sa progression par compétence.</p>
  </div>
</div>

---

## Branche Fonctionnelle : Design Thinking
### 2. DÉFINITION

<div class="dt-card" style="border-top-color: #e74c3c; margin-top: 10px;">
  <h4 style="color: #e74c3c;">Le Problème Central : L'aveuglement pédagogique</h4>
  <p style="font-size: 0.95em; line-height: 1.4;">
    Provoqué par l'utilisation d'outils génériques et non intégrés. Les formateurs et apprenants manquent de <strong>visibilité en temps réel</strong> sur l'acquisition des compétences car les scores sont déconnectés des objectifs précis.
  </p>

  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px; margin-top: 15px;">
    <div style="background: white; padding: 10px; border-radius: 8px; border-left: 4px solid #e74c3c; font-size: 0.8em;">
      <strong>🔍 Invisibilité des lacunes</strong><br>Incapacité d'associer les questions aux micro-objectifs.
    </div>
    <div style="background: white; padding: 10px; border-radius: 8px; border-left: 4px solid #e74c3c; font-size: 0.8em;">
      <strong>📉 Stagnation (Feedback)</strong><br>Notes "sèches" sans explications ni analyse d'erreurs.
    </div>
    <div style="background: white; padding: 10px; border-radius: 8px; border-left: 4px solid #e74c3c; font-size: 0.8em;">
      <strong>🔄 Rupture Administrative</strong><br>Report manuel vers SoliLMS, chronophage et risqué.
    </div>
    <div style="background: white; padding: 10px; border-radius: 8px; border-left: 4px solid #e74c3c; font-size: 0.8em;">
      <strong>📱 Fragmentation UX</strong><br>Multiplication d'outils et interface mobile inadaptée.
    </div>
  </div>
</div>

---

## Branche Fonctionnelle : Design Thinking
### 3. IDÉATION

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 10px;">
  <div class="persona-card" style="border-top-color: #088dc7; background: linear-gradient(135deg, #f0faff 0%, #ffffff 100%);">
    <strong>🔄 SoliLMS Sync Engine</strong>
    <p>Automatisation totale : synchronisation en temps réel des scores et des micro-objectifs vers le profil apprenant SoliLMS.</p>
  </div>
  <div class="persona-card" style="border-top-color: #27ae60; background: linear-gradient(135deg, #f0fff4 0%, #ffffff 100%);">
    <strong>📅 Daily Streak System</strong>
    <p>Engagement quotidien : questionnaires courts ("Daily Quiz") pour valider les acquis chaque matin et booster la rétention.</p>
  </div>
  <div class="persona-card" style="border-top-color: #f39c12; background: linear-gradient(135deg, #fff9f0 0%, #ffffff 100%);">
    <strong>📡 Résilience Offline-First</strong>
    <p>Auto-sauvegarde locale systématique : aucune donnée n'est perdue en cas de coupure réseau pendant un QCM.</p>
  </div>
  <div class="persona-card" style="border-top-color: #9b59b6; background: linear-gradient(135deg, #fdf2ff 0%, #ffffff 100%);">
    <strong>🧠 Adaptive Feedback</strong>
    <p>Correction pédagogique augmentée : explications contextuelles ciblées sur l'erreur pour transformer l'échec en apprentissage.</p>
  </div>
</div>

---

## Branche Fonctionnelle : Cas d'utilisation

<div class="img-container">
  <h3>Interaction Utilisateur — Vue globale (UML)</h3>
  <img src="images/cas-utilisation-global.png" class="img-methodo" alt="Use Case Global">
</div>

---

## Branche Fonctionnelle : Cas d'utilisation — Sprint 1 MVP

<div class="img-container">
  <img src="images/cas-utilisation-sprint-1-mvp.png" class="img-methodo" alt="Use Case Sprint 1">
</div>

---

## Branche Fonctionnelle : Cas d'utilisation — Sprint 2 Avancé

<div class="img-container">
  <img src="images/cas-utilisation-sprint-2-avance.png" class="img-methodo" alt="Use Case Sprint 2">
</div>

---

## Branche Fonctionnelle : Maquettes (UI/UX)

<div class="maquette-grid">
  <div style="text-align: center;">
    <img src="images/maquette.png" class="img-methodo" style="height: 360px; width: auto;" alt="Maquette Desktop">
    <p style="font-size: 0.3rem; color: #666;">Interface Administration</p>
  </div>
</div>

---

## 4. Branche Technique : Tech Stack
<div class="sommaire-grid">
  <div class="dt-card" style="margin-top:0;">
    <h4>Back-end & Architecture</h4>
    <ul>
      <li><strong>Base de données:</strong> MySQL</li>
      <li><strong>Framework:</strong> Laravel 12</li>
      <li><strong>Architecture:</strong> N-Tiers / MVC</li>
      <li><strong>Controller:</strong> Requêtes HTTP</li>
      <li><strong>Service:</strong> Logique métier</li>
      <li><strong>Model:</strong> Base de données</li>
      <li><strong>Blade :</strong> Templates réutilisables (components, layouts).</li>
    </ul>
  </div>
  <div class="dt-card" style="margin-top:0; border-top-color: #27ae60;">
    <h4>Front-end & Outils</h4>
    <ul>
      <li><strong>AJAX :</strong> Interactions dynamiques sans rechargement de page.</li>
      <li><strong>Alpine.js :</strong> Librairie JavaScript pour les interactions dynamiques.</li>
      <li><strong>Spatie :</strong> Gestion des permissions et rôles.</li>
      <li><strong>Vite :</strong> Outil de build rapide.</li>
      <li><strong>Lucide :</strong> Librairie d'icônes.</li>
      <li><strong>Tailwind CSS :</strong> Développement rapide, responsive.</li>
    </ul>
  </div>
</div>

---


## 5. Conception : Diagramme de classe

 <h3>Modélisation des données (MLD)</h3>
<div class="img-container">
 
  <img src="images/diagramme-class.png" style="width: 100%;" alt="Diagramme de classe">
</div>

---

## 6. Démonstration : Environnement & Outils

<div class="sommaire-grid">
  <div class="dt-card" style="margin-top:0;">
    <h4>Environnement de Développement</h4>
    <ul>
      <li><strong>IDE :</strong> VS Code & Antigravity</li>
      <li><strong>Monitoring DB :</strong> MySQL Workbench</li>
      <li><strong>Navigateur :</strong> Chrome DevTools</li>
    </ul>
  </div>
  <div class="dt-card" style="margin-top:0; border-top-color: #27ae60;">
    <h4>Gestion & Déploiement</h4>
    <ul>
      <li><strong>Modélisation UML :</strong> Mermaid / PlantUML</li>
      <li><strong>Gestion de version :</strong> Git (GitHub)</li>
    </ul>
  </div>
</div>

<br>

---

## 7. Conclusion

- **Objectifs atteints** : Application QCM fonctionnelle, responsive et intégrée à SoliLMS.
- **Compétences** : Maîtrise du cycle Agile (Scrum), de la méthodologie 2TUP, Design Thinking et de la stack Full-stack Laravel.
- **Apport pédagogique** : Remplacement complet de Google Forms par un outil interne centré sur les besoins des formateurs et étudiants.
- **Perspectives** : Intégration d'un module d'IA pour l'analyse prédictive des performances et la génération automatique de QCM.

<br>

### Merci pour votre attention ! 🎓