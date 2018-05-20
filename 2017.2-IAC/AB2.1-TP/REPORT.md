# Identificação

* Página do repositório do trabalho ([link GitHub](TODO)) 

* Discente 1
	* Nome: Lucas Alves de Barros
	* Matrícula: 16110949
	* Distribuição da nota (%): ___
* Discente 2
	* Nome: Dayvisson Nelson Mendes
	* Matrícula: 16110744
	* Distribuição da nota (%): ___
* Discente 3
	* Nome: Jefersson Ricardo
	* Matrícula: 17210973
	* Distribuição da nota (%): ___		
	
# Resultados




# Discussão

## Utilização intensa da UCP

No teste UCP foi observado uma utilização entre 90-100% do processamento, mesmo assim o processo foi executado até o fim dos 10 segundos sem causar nenhum efeito perceptível na máquina. O resultado foi como esperado, já que a UCP controla e revesa os processos, afim de fazer com que todos sejam terminados em algum momento. Também foi possível observar que o processo era substituído. Por outros, provamelmente com mais prioridade.
A principal dificuldade foi encontrar uma função para monitorar a utilização da UCP, uma vez que nenhuma fonte na internet possuia informações específicas sobre o assunto, somente alguns comandos do Linux, como por exemplo: ps, top, etc. Dessa forma resolvemos utilizar estes comandos juntamente com alguns filtros, afim de mostrar somente os resultados do programa em questão. Estes comando e filtros foram executados através da função “system”, que é responsável por executar comandos no terminal durante a execução do software.

## Utilização intensa da UCP e memória

Com relação ao teste de  UCP-MEM, o programa utilizou também entre 90-100% do processamento, porém o consumo de memória aumentou gradativamente nos primeiros 5 segundos e em seguida causou um travamento na maquina. O resultado esperado era que o processo fosse morto automaticamente após alguns segundos de travamento, mas isso não aconteceu, uma vez que o programa estava utilizando praticamente todos os recursos do computador e sua morte dependeria do início de outro processo responsável, como esse processo não teve recurso para ser iniciado, aconteceu o travamento da máquina, o que levou à necessidade de reiniciar.
Em um exemplo de programa postado nos comentários dessa atividades, percebemos a presença da função “popen”, pesquisamos sobre a mesma e verificamos que ela pode executar comando “no terminal” sem que o usuário veja, porém tentamos executar o código e não obtivemos resultado, assim, resolvemos fazer todo o prcesso através da função “system”, e já mostrar na tela todo o processo printado a cada segundo decorrido.
