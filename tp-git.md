# TP — Git & GitHub : Questions & Réponses

---

## Questions de TP

### Q1. Quelle est la différence entre Git et GitHub ?

- **Git** : logiciel LOCAL qui gère les versions du code sur votre ordinateur. Fonctionne sans internet.
- **GitHub** : plateforme EN LIGNE qui héberge et partage le code. Nécessite internet.

---

### Q2. À quoi sert la commande git init ?

Elle initialise un nouveau dépôt Git dans un dossier.
Elle crée un dossier caché `.git` qui permet à Git de suivre toutes les modifications du projet.

```bash
git init
```

---

### Q3. Quelle commande permet d'envoyer un projet sur GitHub ?

La commande principale est `git push -u origin main`.
Les étapes complètes :

```bash
git add .
git commit -m "mon message"
git remote add origin https://github.com/utilisateur/repo.git
git push -u origin main
```

---

### Q4. Pourquoi utilise-t-on les branches ?

Les branches permettent de travailler sur une nouvelle fonctionnalité
sans toucher au code principal (main).
Chaque développeur travaille sur sa propre branche,
puis fusionne son travail via `git merge` une fois terminé.

---

### Q5. Quelle commande permet de voir l'historique des commits ?

```bash
git log
```

Version plus lisible :

```bash
git log --oneline
```

---

## Exercice Final — Mini Site Web

### index.html

```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mon Projet GitHub</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Mon Premier Projet GitHub</h1>
    <p>Réalisé par Jaafar Gueye</p>
  </header>
  <main>
    <section>
      <h2>À propos</h2>
      <p>Ce site a été créé dans le cadre d'un TP sur Git et GitHub.</p>
    </section>
  </main>
  <footer>
    <p>© 2026 Jaafar Gueye</p>
  </footer>
</body>
</html>
```

---

### style.css

```css
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  font-family: Arial, sans-serif;
  background-color: #f0f4f8;
  color: #333;
}

header {
  background-color: #2E75B6;
  color: white;
  text-align: center;
  padding: 40px;
}

header p { margin-top: 10px; font-size: 18px; }

main {
  max-width: 800px;
  margin: 40px auto;
  padding: 20px;
  background: white;
  border-radius: 8px;
}

h2 { color: #2E75B6; margin-bottom: 10px; }

footer {
  text-align: center;
  padding: 20px;
  color: #888;
  font-size: 14px;
}
```

---

### README.md

```markdown
# Mon Premier Projet GitHub

Mini site web créé dans le cadre d'un TP Git/GitHub.

## Contenu
- `index.html` : page principale
- `style.css` : styles du site

## Auteur
Jaafar Gueye
```

---

## Commandes Git utilisées

```bash
git init
git add .
git commit -m "Premier commit - mini site web"
git remote add origin https://github.com/Amina-codeur/devoirgithub1.git
git branch -M main
git push -u origin main
```

---

## Lien du repository GitHub

https://github.com/Amina-codeur/devoirgithub1
