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

## Comptes d'usuari

A Ajustos es pot entrar o crear un compte amb correu i contrasenya. Cada usuari té les seves rutines, calendari i historial desats en un projecte de [Supabase](https://supabase.com), i els troba a qualsevol dispositiu on entri. L'app també es pot fer servir sense compte, amb les dades només al dispositiu.

La clau que hi ha al codi és la clau publicable del projecte: només permet que un usuari amb la sessió iniciada llegeixi i escrigui la seva pròpia fila (taula `ferro_data`, protegida amb Row Level Security).

## Crèdits

Fotos dels exercicis: [Free Exercise DB](https://github.com/yuhonas/free-exercise-db), de domini públic.
