> _Fork_ deze leertaak en ga aan de slag. 
Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. 
De instructie vind je in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

# Mijn Vinimini - Interactive Website
<!-- Geef je project een titel en schrijf in één zin wat het is -->

## User Story
<!-- Schrijf de user story waar je aan hebt gewerkt  -->
__User Story:__ Als ouder wil ik in een dagboek aantekeningen kunnen maken zodat ik niet vergeet wat er is gebeurd.

## Beschrijving
<!-- In de Beschrijving staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->

📸 - Before TAP/KLIk
![image](https://user-images.githubusercontent.com/112857932/213443968-5857a130-8f06-48d5-8aa2-68b7222729b6.png)

📸 - After TAP/KLIL
![image](https://user-images.githubusercontent.com/112857932/213443984-3d92cdb4-fd6e-4a56-9c63-094b19b0acd3.png)

🌐 - Interactie - url: https://ibadr49.github.io/fix-the-flow-interactive-website/agenda.html

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met JS gedaan en hoe? -->
De interactie die ik had ontworpen en getest was een "fieldset" gemaakt en als je ergens binnen die "fieldset" klikt wordt de fieldset height grooter en de "hidden" content wordt zichtbaar voor de gebruiker. <br>
Hoe heb ik deze intercatie gemaakt? __Check__ hieronder:

💬 Html
```html
      <fieldset class="input1">
        <div class="inputForm">
          <input class="input" type="checkbox" />
          <label class="container">10-11-2022</label>
          <span class="checkmark"></span>
        </div>
        <p> Vandaag heeft Ali een pinda zakje genomen.</p>
        <legend><span>1</span></legend>
        <label for="question"></label>
        <textarea id="question" placeholder="Vul hier hoe het ging?">
        </textarea> 
        <input type="submit" value="Submit">
        <p class="test">Dit zie je nu!</p>
      </fieldset>
```

💬 JavaScript 

```js
const input1 = document.querySelector('.input1');
const inputOn = document.querySelector('.inputOn');
input1.addEventListener("click", inputClick);

// selecteer p element
const paragraph = document.querySelector('.test');

function inputClick(){
    input1.classList.toggle('inputOn');
    paragraph.classList.toggle('test');
}
```

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
