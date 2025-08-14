TUTORIAL_REACT
		Note
			React  ha questo tutorial:
				https://it.reactjs.org/tutorial/tutorial.html

		Panoramica
					@REACT@LIBRERIA@JAVASCRIPT
					@cosa@è@react
					@props
			LIBRERIA DI JAVA SCRIPT DI REACT: Cosa è React? React è una libreria JavaScript per costruire interfacce utente caratterizzata dal fatto che è dichiarativa, efficiente e flessibile. Ti permette di comporre UI complesse a partire da piccoli ed isolati stralci di codice chiamati “componenti”. 
			Quando viene creata una classe viene creata una CLASSE COMPONENT o componenti di questa 
			libreria che serve a react per creare interfaccie dichiarativa efficiente e flessibile con 
			questi componenti (piccoli pezzi di codice) che permettono a React di disegnare sullo schermo.
				es.
					class ShoppingList extends React.Component {
								render() { .....
			la classe è una estensione di um componente di react CHE RICONO PARAMETRI chiamati
					props 	= parametri o proprieta 
					render 	= metodo che ritorna una gerarchia di viste da visualizzare.

					ESEMPIO DI CLASSE COMPLETA 
							class ShoppingList extends React.Component {
								  	render() {
								  		//DESCRITTO PER INTERO
								    	return (
								      	<div className="shopping-list">
								        	<h1>Lista della spesa per {this.props.name}</h1>
								        	<ul>
								          	<li>Instagram</li>
								          	<li>WhatsApp</li>
								          	<li>Oculus</li>
								        	</ul>
								      	</div>
								    	);
								  	}
									}
									
									// Esempio d'utilizzo: <ShoppingList name="Mark" />


						ESENPIO DI UTILIZZO DI JSX
									La sintassi <div /> viene trasformata a build time in React.createElement('div'). L’esempio di prima è equivalente a:
											//CON REACT
											return React.createElement('div', {className: 'shopping-list'},
												  	React.createElement('h1', /* ... h1 children ... */),
												  	React.createElement('ul', /* ... ul children ... */)
													);

			METODO RENDER
					@render
				Il metodo render ritorna una descrizione di cosa vogliamo vedere sullo schermo. React prende questa descrizione e ne visualizza il risultato. In particolare, render ritorna un elemento React, che è una descrizione leggera di cosa bisogna visualizzare. La maggioranza degli sviluppatori React usa una speciale sintassi chamata “JSX” che rende queste strutture più facili da scrivere.

			S
				SLICE
						Metodo di copia per creare la copia dell'array in formato lettura non si puo modificare.
								es 
									 const squares = this.state.squares.slice();







		Introduzione a JSX

		COMPONENTI CONTROLLATI	
			Nell'esempio Board controlla gli Square che non hanno più al loro interno lo status ma viene
			controllato dal componente superiore Board; Board invia valori ai figli (Square) ed i componenti
			Square invia il valore del click che subisce al (padre) Board.



		IMMUTABILITA
			LA MUTAZIONE DIRETTA E' MOLTO DIFFICILE  e  Si ha la mutazione diretta 
			quando RILEVI I CAMBIAMENTI IN OGGETTI MUTABILI facendo il 
					confronto tra OGGETTO MUTATO con LE VERSIONI PRECEDENTI DELL'OGGETTO e quindi
					si deve attraversare l'intero albero dell'oggetto.

			MENTRE L'IMMUTABILITA DEGLI OGGETTI è più semplice gli OGGETTI SONO IMMUTABILI e rilevare 
			i cambiamenti E' PIU FACILE dovendo fare solo il paragone tra l'oggetto immutabile e quello
			precedente.
			Infatti nell'esempio abbiamo usato l'immutabilita con .slice che ci ha permesso di creare
			COMPONENTI PURI  in React avere quindi DATI IMMUTABILI  e capire quando è necessario identificare
			i cambiamenti e fare la renderizzazione del componente.
			Eliminare la MUTAZIONE DIRETTA permette nel futuro di costruire uno storico del gioco. Sara
			utilizzata shouldComponentUpdate per un CONFRONTO SUPERFICIALE del cambiamento.

		COMPONENTI A FUNZIONE
			Sono componenti piu semplici che permettono di evitare di SCRIVERE UNA CLASSE CHE ESTENDE il componente i COMPONENTI A FUNZIONE  sono sempre UN COMPONENTE  che NON HA STATO INTERNO ma che
			rappresentano UNA FUNZIONE  che prende un imput un PROPS e RITORNA  cosa bisonga renderizzare.
					esempio componente a funzione:

							function Square(props) {
							  	return (
							    	<button className="square" onClick={props.onClick}>
							      	{props.value}
							    	</button>
							  	);
								}


TUTORIAL_REACT_CONCETTI_CHIAVE
	



# COMANDI
## D
		l'ATTRIBUTO onclick del COMPONENTE DI FABBRICA DOM Glie evention[Evento] per le props


			