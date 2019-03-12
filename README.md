# Progetto di ML e SII

Repository contente il progetto di Machine Learning e Sistemi Intelligenti per Internet svolto da Bianca Camilla e Valeriani Dalia, studentesse di Ingegneria Informatica presso l'Università degli Studi di RomaTre.
L'obettivo del progetto consiste nell'analisi e nello sviluppo dei cambiamenti dei parametri e degli iper-paraemtri relativi alle reti neurali che realizzano una Generative Adversarial Network.
Inizialmente è stata analizzata una rete base di tipo Vanilla, per poi far riferimento a strutture leggermente più complesse (richiamando la conoscenza di argomenti studiati a lezione): le DCGAN.

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

La Vanllia GAN è ...
Questo tipo di GAN è costitutio da Generatore e Discriminatore con 3 hidden layers:
*3 layers*
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
