# Neural Network vs Prophet

In questo notebook vedremo come <b><i> spesso un modello più semplice può ottenere dei buoni risultati equiparabili e delle reti neurali </i></b>.
Per realizzare questo lavoro abbiamo utilizzato un dataset denominato <b><i>alchol_sales</i></b>, codesto dataset è una Times Series che riguarda le vendite di alcolici mese per mese in un periodo che va dal 1992/01/01 al 2019/12/01. Il dataset lo si può trovare presso il seguente link:
*	https://rdrr.io/cran/TSA/man/beersales.html
*	In ogni caso il dataset lo troverete anche in una cartella denominata 'data' di questo lavoro su github.

Nella fattispecie in questo lavoro abbiamo messo a confronto <b><i>Prophet</i></b> (<i>di facebook</i>) con diverse reti neurali e nello specifico le seguenti:
* <b><i>SimpleRNN</i></b>
*	<b><i>LSTM</i></b>
*	<b><i>LSTM multistrato</i></b>
*	<b><i>GRU</i></b>

La metrica scelta per confrontare le predizioni dei vari modelli è stata quella della RSME. 
Nel caso in cui si voglia mandate in esecuzione il notebook si consiglia di utilizzare la piattaforma Colab di Google, in quanto, il train delle reti neurali richiede una discreta quantità di tempo. Se si decide di adoperare Colab, come ulteriore suggerimento vi consigliamo di andare su Modifica-> Impostazioni blocco-> Accelerazione hardware-> settare su GPU, tutto ciò perché Colab mette a disposizione degli utenti gratuitamente una GPU NVIDIA Tesla K80 da 12 GB che può funzionare fino a 12 ore consecutive gratuitamente.
