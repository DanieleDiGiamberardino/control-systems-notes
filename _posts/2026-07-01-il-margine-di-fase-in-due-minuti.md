---
title: "Il margine di fase in due minuti"
tags: [controlli-classici, bode]
---

**Cos'è.** Il margine di fase (PM) misura quanto "spazio di sicurezza" ha un
sistema in retroazione prima di diventare instabile. Si legge sul diagramma
di Bode alla pulsazione di attraversamento $\omega_c$, dove il modulo di
$L(j\omega)$ vale 1 (0 dB):

$$
PM = 180° + \angle L(j\omega_c)
$$

**Perché conta.** Un PM basso (es. sotto i 30-40°) è il sintomo tipico di un
sistema che oscilla parecchio prima di assestarsi — poli dominanti vicini
all'asse immaginario, $\zeta$ basso. Un PM alto è più robusto ma più lento a
reagire.

**Relazione pratica.** Per sistemi dominati da una coppia di poli complessi
coniugati del secondo ordine, vale l'approssimazione:

$$
PM \approx 100 \cdot \zeta
$$

Non è esatta, ma è la prima stima "ad occhio" da tenere in tasca in un
colloquio.

**Nota a margine.** Il margine di fase da solo non basta: un sistema può
avere PM ottimo ma margine di guadagno pessimo (o viceversa) se la curva di
fase attraversa più volte i -180°. Vale sempre la pena guardare entrambi.
