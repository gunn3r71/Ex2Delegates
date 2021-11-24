# Exercício 2 - Delegates

1º Crie uma classe chamada Clock, que irá representar um cronômetro. Esta classe possui o 
método Start(), que inicia um loop infinito. A cada 1 segundo passado, este método chama 
métodos de callback registrados informando quantos segundos se passaram desde o início da 
contagem (a contagem inicia quando Start() é chamado). 

#
2º - Para implementar este comportamento, você precisa de um delegate, que você chamará de 
SecondsHandler. Ele referencia métodos que recebem um parâmetro do tipo long (número 
de segundos) e retornam void. 
#
3º - Crie um método chamado OnSecond() na sua aplicação, que é chamado via delegate pelo 
objeto Clock a cada segundo. Imprima na tela o valor do segundo fornecido. 
Dica: Utilize a chamada Thread.Sleep(1000) para fazer a aplicação pausar por 1 segundo. A 
classe Thread pertence ao namespace System.Threading. 
