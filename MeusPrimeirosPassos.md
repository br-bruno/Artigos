
# Meus Primeiros Passos

Eduardo, antes de entrar nesse mundo da programação, trabalhava de motorista de ônibus.
Um dos critérios que a empresa de ônibus lhe pedia, era que carregasse no final do expediente no mínimo 200 passageiros pagantes,
sem contar os passageiros com gratuidades.
Estudando programação em **C#**, percebeu que podia criar um sistema para ajudar a saber quantos
pagantes estava carregando.

Partindo disso, sabemos que em **C#** existe um recurso que usamos para 
guardar valores, qual é esse recurso? Você sabe? 
Se chama variável. 

Então vamos criar aqui uma variável para 
`idadePagante` , mas em C# temos que declarar qual o seu tipo, se é do tipo string, int, double... colocaremos que essa variável é do tipo int, de integer, do português inteiro: 

    int idadePassageiro 

Sabemos também, que a idade mínima para obter gratuidade é de 60 anos, contudo colocaremos que o valor dessa variável é 

    int idadePassageiro = 30 

Bom, já criamos a nossa primeira variável do sistema, agora temos uma variável que indica a idade do passageiro que está entrando no ônibus, mas qual condiçâo temos para que possamos saber `Se` o passageiro é pagante ou gratuidade? 

A condiçâo é que: 

    se ("idadePagante < 60") 
    

Existe um meio em **C#** que nos possibilita implementar uma condição para saber se o passageiro é pagante ou gratuidade, que se chama  `IF` , ou seja:

    if (idadePagante < 60)
    {

    } 

Ele retornará `true` , e o passageiro terá que pagar a passagem. Mas, pera lá, como que o passageiro vai saber se ele é pagante se a condiçâo não lhe retorna nenhuma mensagem? Pensando nisso, em **C#** existe outro meio que nos disponibiliza imprimir uma mensagem para o usuário, sabe qual é? Esse recurso é o `Console.WriteLine`.
Ele nos possibilita enviar a mensagem ao usuário de que o passageiro terá que pagar a passagem,lembrando que essa mensagem terá que ficar entre `()` e `""`:

    int idadePassageiro = 30
    if (idadePassageiro < 60)
    {
        Console.WriteLine("Terá que pagar.");
    }

Olhando o nosso codigo, percebi que podemos aprimorá-lo, e para ajudar, iremos criar uma outra variável para substituir esse número `60` que receberá uma outra variável do tipo `int`:

    int idadeGratuidade = 60
    int idadePassageiro = 30
        if (idadePassageiro < 60)
        {
            Console.WriteLine("Terá que pagar.");
        }
Podemos agora testar o nosso programa para saber se o passageiro terá que pagar a passagem. 

Ops! Como você pôde ver o programa apresentou um erro, e no erro ele diz que 

    ; esperado

Em **C#** ele não nos deixa declarar algo sem que no final da declaração tenha um `;` , e se repararmos, nas declarações das variáveis não colocamos o `;` no final. Então vamos colocar?

        int idadeGratuidade = 60;
        int idadePassageiro = 30;
            if (idadePassageiro < 60)
            {
                Console.WriteLine("Terá que pagar.");
            }