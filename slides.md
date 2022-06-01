---
title: 'Conference Creative coding in your web browser'
theme: seriph

# fonts:
  # sans: '"DM Sans"'

download: true
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://user-images.githubusercontent.com/5133074/171389401-91d93a9c-b483-4479-ba1d-d7b85f80cc6f.svg

drawings:
  enabled: dev
# Photo by <a href="https://unsplash.com/@heytowner?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">JOHN TOWNER</a> on <a href="https://unsplash.com/s/photos/mountains?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
colorSchema: 'dark'
---

# Creative coding 🎨

Soyons tous ensemble de Mesh !

<!-- This is a page note btw -->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171328387-5991c10c-b383-4307-aa7a-369e3ff79173.svg
---

## Comment en suis-je arrivé là ?

<!--
commencé à coder il y a de cela 4ans environ, fullstack et maintenant front

avant de coder en pro, j'ai commencé avec pas mal de CSS, avec 0 Bootstrap donc

avec le temps, on se lasse de faire: call HTTP à une API, itérer sur une liste d'éléments, on loop dessus niveau couleurs

besoin de fraîcheur et d'expression
-->


---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

<div class="flex">
  <img src="/images/game2.png" alt="Netlify actual game progress" class="w-auto h-96" />

  <img src="/images/game1.png" alt="Netlify game" class="pt-34 pl-18 h-96" />
</div>

[Petit jeu wall-e codé par Sarah Drasner](https://codepen.io/sdras/full/YZBGNp/)

<!--
des couleurs bien cools donc

on peut aussi créer un jeu sympa, comme ici sur Netlify lors d'un build pour passer le temps

ou créer toute sorte d'animation avec Greensock, pour faire patienter les utilisateurs

c'est astucieux et les gens supportent bien mieux l'attente ainsi

l'endgame serait tout de même d'avoir un peu de 3D!
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

## Pour de la 3D, WebGL donc ?

<div class="text-left pt-8">
<v-clicks>

- une API qui permet de render des polygones (triangles) très rapidement grâce à la carte graphique
- millions de points générés en quelques millisecondes
- le cumul de tous ces points formera l'image
- standard quand il s'agit de Web
- la documentation sera toute relative par contre... 😭
- une solution simple pour créer un truc fun ?

</v-clicks>
</div>

<!--
cela semble être une bonne idée en soit, pour les raisons suivantes
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

## ThreeJS pour éviter ceci surtout !

<br />
<br />
<div class="flex">
  <img src="https://user-images.githubusercontent.com/5133074/171332004-9c0f5f7f-271e-47cc-a80e-0e7f8e6b7689.png" alt="Triangle render en WebGL" class="h-84" />
  <img src="https://user-images.githubusercontent.com/5133074/171332757-99a29512-f29a-4b5f-b135-03d74204477d.gif" alt="Triangle render en WebGL" class="h-84 pl-8" />
</div>

120 lignes de WebGL juste pour un triangle donc ? 🤔

<!--
c'est cool et sympa mais 3h pour cela ca fait beaucoup

pas très fun et obligera d'apprendre le fonctionnement interne des choses très tôt
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171333288-d0ec9368-58c3-4799-a1f3-a44ab153e118.svg
---

## Quelques exemples de ce qui est faisable avec ThreeJS

<br/>

<div class="text-left pl-36">

[Site de Nuxt, framework VueJS](https://v3.nuxtjs.org/)

[Petite animation cool pour son portfolio](https://www.craftz.dog/)

[Render réaliste d'une maison](https://twitter.com/rocha_ycaro/status/1529205485731299335/photo/1)

[Customization à la volée d'objets](https://infinitemirai.files.wordpress.com/2015/08/vlcsnap-00025.png)

[Pinbal game basé sur OUIGO](http://letsplay.ouigo.com/)

[Le CV interactif de Bruno Simon](https://bruno-simon.com/)

Site pour custom ses chaussures Nike

</div>

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

## ThreeJS nous permet ceci

<div class="text-left pt-8">
<v-clicks>

- beaucoup de choses directement prêtes à l'emploi
- pas besoin d'être un expert en 3D pour s'amuser
- éviter d'avoir à écrire 300 lignes de code pour quelque chose de simple
- une documentation et des exemples SUPER complets

</v-clicks>
</div>

<!--
des formes (simples ou moins), des lumières, des caméras, des matériaux etc...

permet d'åvoir du fun rapidement

passer 3 jours à coder une fonction pour pouvoir faire une rotation dans l'espace c'est pas le plus fun

la plupart des principes requirènt des connaissances mathématiques sur les inversions de matrices etc, pas le + friendly non plus quand on doit le faire à la mano
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

## Des pré-requis pour commencer avec ThreeJS?

<div class="text-left pt-8">
<v-clicks>

- les bases en JavaScript
- comprendre quelques principes en 3D (représentation spatiale, aliasing, optimisation etc...)
- les bases de la trigonométrie peuvent être utiles (`sin`, `cos`)
- des connaissances en gaming + hardware en _nice to have_

</v-clicks>
</div>

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171334746-70ecbd5d-5acd-47d1-977a-062762ce7e95.svg
---

## Que nous faut-il pour avoir un visuel ?

<div class="text-left pt-8">
<v-clicks>

- une scène
- une [géométrie](https://www.mathsisfun.com/geometry/images/vertex-edge-face.svg) (tous les vertices + toutes les faces)
- un matériau sera aussi nécessaire
- la combo de `géometrie + matériau` nous donnera la surface
- (parfois) une lumière pour éclairer tout cela
- une caméra simple
- on call la méthode `render` (du renderer)

</v-clicks>
</div>

<!--
scène -> espace virtuel où on va mettre tous nos éléments

géometrie + matériau: ø

combo: surface se dit d'ailleurs _Mesh_ en anglais

lumière: le besoin de lumière dépend du matériau utilisé, elle n'est pas toujours obligatoire

camera: il y en a une dizaine de différentes, avec chacune ses spécificités, en plus du champ de vision, l'angle etc

on fait attention à que tout soit dans le champ de vision de la caméra
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171349616-5d84267a-0eef-4781-9ba6-9eff6172ad6d.svg
---

<h2 class="absolute right-24">Du concret SVP ! 🙏🏻</h2>

<!--
je vais vous montrer 3 renders maintenant

regardons comment avoir un objet simple tout d'abord (cône)

ensuite une petite galaxie bien sympa

bon, pouvoir coder un petit cube c'est bien, mais comment on render quelque chose de + complexe ?

découvrons ensemble Blender
-->

---
layout: cover
background: https://user-images.githubusercontent.com/5133074/171331451-8e66c500-b7d1-48ad-a222-08a5ba71a3d5.svg
---

## Resources intéressantes pour approfondir le sujet

<div class="text-left pt-8">

- Bruno Simon avec [three.js journey](https://threejs-journey.com/)
- Andrew Price aka "Blender Guru" avec [sa playlist Youtube](https://www.youtube.com/watch?v=OqMLfMXVhhI&list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD&index=16)
- Roman Klčo aka Polygon Runway avec [ses cours](https://polygonrunway.com/courses) + [chaîne YouTube](https://www.youtube.com/c/PolygonRunway/featured)

</div>

---
layout: cover
preload: false
background: https://user-images.githubusercontent.com/5133074/171355214-f6e54836-6bd5-4c4e-8216-fe4098dea7b9.svg
---

<div class="absolute top-12 left-14 text-left">
  <h2 class="!text-white underline decoration-wavy decoration-1 underline-offset-4 underline-grey-100">Qui suis-je ?</h2>

  <h3 class="mt-2">Konstantin BIFERT ~ <a href="https://twitter.com/kissu_io" target="_blank" class="text-transparent bg-clip-text bg-gradient-to-tl from-blue-400 to-teal-500 font-bold" alt="konstantin's twitter">@kissu_io</a> (twitter)
</h3>
</div>

<div class="flex mt-4">
  <img v-motion :initial="{ x: -200, y: 0, scale: 1, rotate: 0 }" :enter="final"
    class="h-64 w-48 rounded-lg" src="https://user-images.githubusercontent.com/5133074/171390829-56ff3280-c326-4fd8-ae6b-bed1bdd7238b.jpg"
    alt="photo of konstantin" />

  <section class="ml-6 text-left">
    <p class="!m-0">
      <logos-vue/> Consultant frontend <a href="https://twitter.com/passionpeopleNL">@passionpeopleNL</a> (boîte 🇳🇱)
    </p>
    <p class="my-2">
      <logos-nuxt-icon class="inline h-6" />
      <a href="https://nuxtjs.org/teams" class="ml-2">Ambassadeur Nuxt.js</a>
    </p>
    <p class="my-2">
      <logos-stackoverflow-icon class="inline mr-2" />
      <a href="https://stackoverflow.com/users/8816585/kissu">Helper au quotidien sur Stackoverflow</a>
      <p>🎤  Créateur de contenu + speaker</p>
      <p>✨ Je kiffe le gaming, les mécas, la tech et le DIY</p>
      <p><logos-twitter class="h-4" /> Je communique sur Vue, la perf et la 3D !</p>
    </p>
  </section>
</div>

<script setup lang="ts">
  const final = {
    x: 0,
    y: 0,
    scale: 1,
    transition: {
      type: 'spring',
      damping: 10,
      stiffness: 20,
      mass: 2
    }
  }
  const melon = {
    x: 50,
    y: -50,
    rotate: 0,
    scale: 1,
    transition: {
      type: 'spring',
      damping: 10,
      stiffness: 20,
      mass: 2
    }
  }
</script>
