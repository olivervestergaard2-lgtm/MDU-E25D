# En herosektion til Bjarnesburger

I dag øver vi os på:

* Et traditionelt website med menu
* Undersider - hvordan laver vi dem?
* En herosektion
* Responsiv visning til forskellige enheder: mobil, tablet og større skærm.

## Undersider

## Navigationsmenu

"Menuer" placeres i `<nav>` elementer og styles passende i CSS. I dag bruger vi helt enkelt. Sådanne elementer kan placeres overalt; men det skal være nemt at finde dem. Som regel lægges navigationen øverst.

Tip: prøv at gøre navigationen "sticky", så den bliver i toppen når du scroller på siden.

## Herosektioner

En hero-sektion på et website er det øverste og mest iøjnefaldende område på en webside – typisk lige under navigationen. Den fungerer som en slags visuel introduktion og har til formål at fange brugerens opmærksomhed med det samme.

Her er de vigtigste kendetegn:

* Stor visuel flade: Ofte med et billede, video eller grafik i baggrunden.
* Kort og klar tekst: En overskrift (headline), evt. en underoverskrift og en call-to-action (CTA) som fx en knap.
* Formål: At kommunikere det vigtigste budskab eller værditilbud hurtigt – fx hvad virksomheden tilbyder, eller hvad brugeren skal gøre som næste skridt.

Hero-sektionen er altså både æstetisk og funktionel – den sætter tonen for resten af siden og guider brugeren videre.

~~~~~
/* Brug enten en class eller en id, her er det en id */
#hero {
    background-image: url('../images/hero.png');
    /* tip: brug "../" når din CSS er i en undermappe */
}
~~~~~

### Baggrundsbilleder

### Tekst over baggrundsbilledet

### Hvordan du giver herosektionen fuld bredde og højde

## Responsiv visning (aka "media breakpoints")

Et breakpoint i CSS er et punkt, hvor layoutet på en webside ændrer sig for at tilpasse sig forskellige skærmstørrelser – fx mobil, tablet og desktop. Det bruges i responsivt design, så indholdet ser godt ud uanset hvilken enhed brugeren benytter.

Breakpoints defineres typisk med media queries, som fortæller browseren: “Når skærmen er mindre eller større end X pixels, så brug fx disse CSS-regler:

~~~~~
/* Mobil (op til 600px) */
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}

/* Tablet (601px til 1024px) */
@media (min-width: 601px) and (max-width: 1024px) {
  body {
    background-color: lightgreen;
  }
}

/* Desktop (fra 1025px og op) */
@media (min-width: 1025px) {
  body {
    background-color: lightcoral;
  }
}
~~~~