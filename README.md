# Progetto di ML e SII

Repository contente il progetto di Machine Learning e Sistemi Intelligenti per Internet svolto da Bianca Camilla e Valeriani Dalia, studentesse di Ingegneria Informatica presso l'Università degli Studi di RomaTre.
L'obettivo del progetto consiste nell'analisi e nello sviluppo dei cambiamenti dei parametri e degli iper-paraemtri relativi alle reti neurali che realizzano una Generative Adversarial Network. In particolare, l'attenzione è rivolta all'evoluzione della GAN partendo da un'implementazione semplice, fino ad arrivare ad una struttura più complessa. Infatti, inizialmente è stata analizzata una rete base di tipo Vanilla, per poi far riferimento all'utilizzo di operatori convolutivi tipici di una DCGAN, richiamando la conoscenza di argomenti studiati a lezione.

# GAN

“The coolest idea in deep learning in the last 20 years.” — Yann LeCun on GANs.
Le GAN (Reti avversarie generative) sono una combinazione di vari modelli di Deep Learning che cercano di competere l'uno contro l'altro.

L'architettura della GAN presa in oggetto è la seguente:

![GAN](https://cdn-images-1.medium.com/max/1600/0*2Smzp-1MDx2TTwU6.png)

La GAN è costituita da due reti neurali che sono in competizione tra di loro, che prendono il nome di:
- Generatore: il suo compito è generare nuovi dati simili a quelli del dataset di riferimento;
- Discriminatore: il suo obiettivo è riconoscere se un dato di input è "reale" (appartenente al set di dati originale) o se è "falso" (generato dal Generatore).

Competendo l'uno contro l'altro, questi due modelli forniranno i migliori dati possibili, nuovi e mai visti.

## Vanilla GAN

La Vanllia GAN è definita la "GAN originale", infatti rappresenta una delle prime versioni funzionanti mai realizzate. È il tipo più semplice di GAN, in cui entrambe le reti che la compongono sono semplicemente percettroni multistrato. Infatti la GAN in oggetto presenta 3 hidden layers sia per il Generatore che per il Discriminatore, ciascuno dei quali è seguito da una funzione di attivazione non lineare Leaky-ReLU e da un livello Dropout, utilizzato per evitare l'overfitting.
Una funzione Sigmoid viene applicata all'output con valore reale del Discriminatore per ottenere un valore nell'intervallo aperto (0,1).
Nel generatore, invece lo strato di output avrà una funzione di attivazione di TanH, che mappa i valori risultanti nell'intervallo (-1, 1), che è lo stesso intervallo in cui le nostre immagini MNIST pre-elaborate sono limitate.
La LeakyReLU utilizzata è una variante della ReLU, una funzione di attivazione molto usata. La LeakyReLU ha una piccola pendenza per i valori negativi, invece che 0. Questa pendenza è la "negative slope". La Leaky ReLU è utile per risolvere il "dying ReLU problem".

Viene utilizzata BCE, che è ...
Per entrambe le reti sono stati svolti dei test utilizzando come funzione di ottimizzazione sia Adam che SGD per studiare l'impatto che tali funzioni hanno sull'addestramento della rete.

### Adam

Adam è ...
Nelle prove svolte si è analizzato il comportamento della GAN al variare del LR e del numero di epoche.

#### Epoche = 50; LR = 0.00000000000000001

### SGD

Cos'è SGD
Momentum
Nelle prove svolte si è analizzato il comportamento della GAN al variare del LR e del numero di epoche.

## Risultati finali
Per completezza si riporta il confronto tra i risultati migliore delle due GAN esaminate:
*immagini*
