# Àlgebra Master - 2n ESO 📐

Una aplicació web interactiva dissenyada per ajudar els estudiants de 2n d'ESO a dominar l'àlgebra. El projecte inclou generadors d'exercicis infinits, feedback instantani i un mode examen per posar a prova els coneixements.

## 🌟 Característiques

- **Generació d'Exercicis Infinits**: Mai et quedaràs sense problemes per practicar; el motor matemàtic genera noves preguntes cada vegada.
- **Nivells de Dificultat**: Fàcil, Mitjà i Difícil per a cada tipus d'exercici.
- **Feedback Immediat**: Correcció automàtica amb explicació dels errors.
- **Sistema de Pistes**: Ajuda progressiva per resoldre els dubtes sense donar la solució directament.
- **Mode Examen**: Una prova contrarellotge de 15 minuts amb 10 preguntes aleatòries i resultats detallats.
- **Disseny Modern**: Interfície neta, responsive i adaptada a dispositius mòbils utilitzant Tailwind CSS.

## 📚 Continguts Matemàtics

L'aplicació cobreix el temari estàndard d'introducció a l'àlgebra:

1.  **Monomis**
    - Identificació de parts (coeficient, part literal, grau).
    - Operacions bàsiques (suma, resta, multiplicació).
2.  **Identitats Notables**
    - Desenvolupament: $(a+b)^2$, $(a-b)^2$, $(a+b)(a-b)$.
    - Factorització: $a^2 + 2ab + b^2 \rightarrow (a+b)^2$.
3.  **Polinomis**
    - Valor numèric d'un polinomi $P(x)$.

## 🛠️ Tecnologies Utilitzades

Aquest projecte està construït amb tecnologies web modernes utilitzant un enfocament *no-build* (sense necessitat de compiladors complexos per al desenvolupament local):

- **React 19**: Llibreria per a la interfície d'usuari.
- **TypeScript**: Per a garantir la seguretat de tipus i un codi robust.
- **Tailwind CSS**: Per al disseny i estils (via CDN).
- **Lucide React**: Per a la iconografia.
- **ES Modules (esm.sh)**: Càrrega de dependències directament al navegador.

## 🚀 Com executar el projecte

Aquest projecte no requereix `npm install` ni `node_modules` pesats per executar-se, ja que utilitza Import Maps.

1.  **Clona el repositori** o descarrega els fitxers.
2.  **Obre una terminal** a la carpeta del projecte.
3.  **Inicia un servidor web local**. Com que l'aplicació utilitza mòduls ES6, necessita servir-se a través d'HTTP i no obrint directament el fitxer (`file://`).
    *   Si tens Python instal·lat:
        ```bash
        python3 -m http.server
        ```
    *   Si tens Node.js (utilitzant `npx`):
        ```bash
        npx http-server
        ```
    *   O utilitza l'extensió "Live Server" de VS Code.
4.  Obre el navegador a l'adreça local (normalment `http://localhost:8000` o `http://localhost:8080`).

## 📂 Estructura del Codi

- `/components`: Components reutilitzables de la interfície (Barra de navegació, Targetes d'exercicis, etc.).
- `/pages`: Vistes principals (Inici, Exercici, Examen).
- `/utils`:
    - `generators.ts`: El cor de l'aplicació. Conté la lògica per generar problemes matemàtics aleatoris i verificar-ne les respostes.
    - `mathUtils.ts`: Funcions auxiliars per formatar expressions (superíndexs, normalització de text, càlculs bàsics).
- `types.ts`: Definicions de tipus globals.
- `index.html`: Punt d'entrada de l'aplicació i configuració de Tailwind/Import Maps.

## 📝 Llicència

Aquest projecte és de codi obert i està disponible per a fins educatius.

---

Creat amb ❤️ per a l'aprenentatge de les matemàtiques.
