# Audit `index.html` (grille impeccable `audit`/`critique`, règles emil-design-eng / mobile-native / apple-design, craft-floor)

## Avant : 9/20 (Poor)
| Dimension | Note | Constat |
|---|---|---|
| Accessibilité | 2 | textes 10–11 px, gris #8a948b (contraste < 4,5), cases 25 px, dots 20 px, `confirm()` natif |
| Performance | 3 | léger, mais `transition` sur propriétés larges, innerHTML partout |
| Thèmes | 1 | couleurs en dur, aucun mode sombre |
| Responsive / touch | 2 | `100vh`, pas de `touch-action`, pas de swipe, pas d'icône écran d'accueil |
| Intégrité | 1 | emoji/glyphes en guise d'icônes (☀ ☾ ✳ ✨), eyebrow au-dessus du titre, hero dégradé + glow, anneau de progression décoratif, serif Georgia : direction « spa » opposée à « épuré masculin » |

Bugs : date figée après minuit, onglet matin/soir indépendant de l'heure, pas de recalcul au retour dans l'app.

## Après : ~18/20
Mode sombre/clair auto (jetons CSS), un seul accent, SF Pro, zéro emoji (SVG au trait), cibles ≥ 44 px, texte ≥ 12 px (corps 14–16), `100dvh`, safe-areas, `touch-action: manipulation`, hover limité à `(hover:hover)`, feedback `:active`, check animé (ease-out expo), swipe entre jours, matin/soir auto, série (streak), sheet de confirmation, `prefers-reduced-motion`, icône d'accueil iOS générée, recalcul au `visibilitychange`.
Données (étapes, jours niacinamide/HA/huile, produits, glycolique, SPF, disclaimer) et clé `localStorage` `eclat_skincare_v1` inchangées : les coches existantes sont conservées.

## Challenge (points non retenus volontairement)
- taste-skill (sites vitrines, photos, shaders) : hors sujet pour une app d'usage ; seule sa discipline « un système, pas de gadgets » est appliquée.
- Pas de bibliothèque de springs ni d'anneau de progression : barre segmentée plus lisible.
- À valider sur ton iPhone réel (vibration non supportée par Safari iOS ; safe-areas / barre d'état).
