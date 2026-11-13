<img src="logo.svg" alt="Ferro" width="196">

# Ferro Gym

Webapp personal per programar i seguir rutines de gimnàs. Pensada per al mòbil: s'obre amb Safari i s'afegeix a la pantalla d'inici.

## Què fa

- Rutines editables (cos sencer, tors i cama, o empenta, tracció i cama) amb fotos de cada exercici.
- Calendari amb un programa de 12 setmanes; les sessions es poden afegir, treure i moure arrossegant-les.
- Registre de pes i repeticions, temporitzador de descans i progressió automàtica.
- Gràfiques d'evolució i rècords per exercici.

## Com funciona

És una sola pàgina (`index.html`) sense dependències ni servidor. Les dades es desen al navegador del dispositiu (`localStorage`); a Ajustos hi ha un botó per copiar-ne una còpia de seguretat.

## Sincronització amb GitHub (opcional)

A Ajustos es pot connectar un repositori **privat** amb un token d'accés limitat (Contents: Read and write només sobre aquell repositori). L'app hi desa un fitxer `ferro-gym-dades.json` després de cada canvi i el llegeix en obrir-se, de manera que les dades es comparteixen entre dispositius. El token es queda al navegador de cada dispositiu i no s'inclou al fitxer sincronitzat.

## Crèdits

Fotos dels exercicis: [Free Exercise DB](https://github.com/yuhonas/free-exercise-db), de domini públic.
