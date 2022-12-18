# Progetto FESI
### Automatic de-noiser based on sampled noise analysis and noise profiling in Fourier
#
#### **Autore:** Francesco Spezia
#### **Collaboratori:** Roberto Lazzarini
#
## **Obiettivo:**
Creare un tool in grado di ridurre vari tipi di rumore da un file audio, basandosi su un'analisi di una porzione di rumore, effettuando una divisione in varie bande di frequenze, calcolando l'ampiezza media del volume di ogni banda, allo scopo di creare un profilo del rumore.

Il profilo ottenuto verrà poi utilizzato come filtro, da sommare al file audio completo, in modo da ridurre il rumore in punti specifici sull'intero spettro delle frequenze, senza intaccare troppo il segnale da ripulire.


Il programma è ispirato da strumenti avanzati di riduzione del rumore (come "Edison", riportato per esempio qui sotto), dove viene analizzato inizialmente il rumore per crearne un profilo, per poi applicarlo alla parte di segnale da ripulire, selezionando alcuni parametri di sensibilità dei filtri da applicare.
