# Meesterproef

## Leerdoelen
Ik heb tijdens de minor geen moeite gehad met techniek vakken zoals Web App From Scratch, Performance Matters en Realtime Web, daarom heb ik besloten om geen leerdoelen voor deze vakken op te stellen.

Ik vind wel dat mijn front-end skills nog niet op het niveau is dat ik graag wil hebben, dus ga ik mij focussen op de vakken CSS To The Rescue en Web Design.

Mijn leerdoelen voor CSS To The Rescue zijn:
- Leren Sass te gebruiken, omdat ik er nooit eerder mee heb gewerkt
- Leren BEM toe te passen, omdat ik tijdens CSS To The Rescue niet de kans had om deze methodology te leren.
- En tenslotte om beter semantische HTML te schrijven.

Voor Web Design heb ik als leerdoel:
- Een MVP (minimal viable prototype) rapid prototypen om experimenten te doen

Deze leerdoelen heb ik aan Laurens voorgelegd en hij vond het prima maar gaf wel aan dat ik de uitdaging moet zoeken.
Hij gaf ook aan om met Vasilis contact te zoeken, omdat front-end zijn sterke punt is.

## Reflectie

Mijn opgestelde leerdoelen heb ik behaald, maar helaas heb ik mijzelf niet kunnen uitdagen.
Het project vergde te veel inspanning en tijd om uberhaupt meer te doen dan de opgestelde leerdoelen.
Dit heeft te maken met het feit dat ik een groep leidde om de meesterproef te realiseren.
Mijn techniek kennis is namelijk veel hoger dan die van mijn groepsleden, waardoor ik constant dingen ging uitleggen en anderen ging helpen met hun problemen.
Hierdoor had ik weinig tijd over voor mijzelf.
Echter, heb ik geen spijt van mijn keuze om samen te werken.
De groepsleden vulden elkaar goed aan, waardoor wij voor de opdrachtgever iets moois hebben kunnen realiseren.

### Behaalde leerdoelen

#### Sass en BEM
Sass en BEM zijn een ideale combinatie.
Met behulp van Sass kunnen CSS styles in meerdere bestanden gezet worden om ze vervolgens te bundelen voor browsers.
Hoewel Sass veel functionaliteiten bevat, heb ik gebruik gemaakt van Sass variabelen en Sass nesting, omdat ik alleen deze functionaliteiten nodig had.
Sass variabelen kunnen als volgt gedeclareerd worden:

```$gold: #F8D84F;```

Door een dollar teken te gebruiken wordt er een variabele gedeclareerd. 
In dit voorbeeld wordt er een hex kleur bewaard in de variabele $gold.
Deze variabele kan dan in andere Sass bestanden gebruikt worden.

Sass nesting werkt door een ampersand & te gebruiken:

```
.button {
  color: black;
  border: none;
  font-size: 16px;
  padding: 6px 15px;
  border-radius: 10px;

  &--large {
    padding-right: 3.5rem;
    padding-left: 3.5rem;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
    border-radius: 10px;
  }

  &__image {
    float: left;
    width: 15px;
    height: 15px;
    pointer-events: none;
  }

  &__image--smaller {
    width: 15px;
    height: 15px;
  }

  &--gray {
    background-color: #ff1;
  }
}
```

Dit wordt uiteindelijk gecompiled naar: 

```
.button {
	 color: black;
	 border: none;
	 font-size: 16px;
	 padding: 6px 15px;
	 border-radius: 10px;
}
 .button--large {
	 padding-right: 3.5rem;
	 padding-left: 3.5rem;
	 padding-top: 0.5rem;
	 padding-bottom: 0.5rem;
	 border-radius: 10px;
}
 .button__image {
	 float: left;
	 width: 15px;
	 height: 15px;
	 pointer-events: none;
}
 .button__image--smaller {
	 width: 15px;
	 height: 15px;
}
 .button--gray {
	 background-color: #ff1;
}
```
