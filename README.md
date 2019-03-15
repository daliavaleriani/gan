# Progetto ML/SII

Il repository contiene il progetto di Machine Learning e Sistemi Intelligenti per Internet svolto da Bianca Camilla e Valeriani Dalia, studentesse di Ingegneria Informatica presso l'Università degli Studi di RomaTre.
L'obettivo del progetto consiste nell'analisi e nello sviluppo dei cambiamenti dei parametri e degli iper-parametri relativi alle reti neurali che realizzano una Generative Adversarial Network. In particolare, l'attenzione è rivolta all'evoluzione della GAN partendo da un'implementazione semplice, fino ad arrivare ad una struttura più complessa. Infatti, inizialmente è stata analizzata una rete base di tipo Vanilla, per poi far riferimento all'utilizzo di operatori convolutivi tipici di una DCGAN, richiamando la conoscenza di argomenti studiati a lezione.

## GAN

“The coolest idea in deep learning in the last 20 years.” — Yann LeCun on GANs.
Le GAN (Reti avversarie generative) sono una combinazione di vari modelli di Deep Learning che cercano di competere l'uno contro l'altro.

L'architettura della GAN presa in oggetto è la seguente:

![GAN](https://cdn-images-1.medium.com/max/1600/0*2Smzp-1MDx2TTwU6.png)

La GAN è costituita da due reti neurali che sono in competizione tra di loro, che prendono il nome di:
- Generatore: il suo compito è generare nuovi dati simili a quelli del dataset di riferimento, partendo da rumore casuale;
- Discriminatore: il suo obiettivo è riconoscere se un dato di input è "reale" (appartenente al set di dati originale) o se è "falso" (generato dal Generatore).

Competendo l'uno contro l'altro, questi due modelli forniranno i migliori dati possibili, nuovi e mai visti.

## Codice
Il codice riportato in questo repository è scritto con l'utilizzo della libreria pyTorch, ed è stato eseguito tramite l'ausilio di Google Colaboratory; esso comprende:
- [VanillaGAN.ipynb](https://github.com/daliavaleriani/gan/blob/master/VanillaGAN.ipynb) (dataset MNIST);
- [DCGAN.ipynb]() (dataset MNIST, fashionMNIST e celebA).

## Risultati finali
Per completezza si riporta il confronto tra i risultati migliori delle due GAN esaminate:
*immagini*
Nello studio svolto le DCGAN si sono dimostrate reti più stabili in termini di addestramento e sono in grado di generare campioni di qualità superiore.
