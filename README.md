# Prodotto
Descrizione degli attributi:
nome (String): Rappresenta il nome del prodotto. È dichiarato private per garantire l'incapsulamento.
peso (double): Indica il peso del singolo pezzo in chilogrammi. È private e viene impostato tramite il costruttore.
prezzo (double): Rappresenta il costo di vendita in Euro del prodotto. È private ed è modificabile tramite il metodo setter.
numero Pezzi (int): Gestisce la quantità di pezzi del prodotto presenti in magazzino. È private e viene aggiornato solo tramite i metodi di vendita e rifornimento.


Descrizione dei metodi (get e set):
Prodotto(String nome, double peso, double prezzo, int numeroPezzi): Costruttore della classe. Inizializza tutti gli attributi del prodotto garantendo che non vengano inseriti valori negativi per peso, prezzo e numero pezzi.
getNome(), getPeso(), getPrezzo(), getNumeroPezzi(): Metodi getter che restituiscono rispettivamente il valore degli attributi privati.
setPrezzo(double nuovoPrezzo): Metodo setter per aggiornare il prezzo del prodotto. Accetta il cambio solo se il nuovo prezzo è maggiore o uguale a 0.
vendiProdotto(int quantita): Riduce il numero di pezzi presenti in magazzino della quantità specificata. Restituisce true se la quantità è positiva e sono presenti abbastanza pezzi; restituisce false se i pezzi sono insufficienti o l'input non è valido. 
rifornisci(int quantita): Aumenta il numero di pezzi presenti in magazzino aggiungendo la quantità fornita in ingresso. Restituisce true se l'operazione ha successo (quantità >0), altrimenti false.
confronta(Prodotto altro): Confronta il prodotto attuale con un altro oggetto Prodotto passato come parametro per verificare se sono uguali (stesso nome e stesso peso). Restituisce true se sono uguali, false altrimenti.
equals(Object obj) e toString(): equals verifica l'uguaglianza profonda tra oggetti, mentre toString restituisce lo stato del prodotto in formato testuale.
