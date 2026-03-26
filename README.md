Otimização de Roteamento de Vans com Algoritmo Genético
Este projeto apresenta uma solução para o Problema de Roteamento de Veículos (VRP) aplicada ao transporte escolar. A implementação utiliza um Algoritmo Genético (AG) para encontrar rotas otimizadas entre uma garagem central e diversos pontos de parada (alunos), visando a minimização da distância total percorrida.

Descrição do Projeto
O sistema simula o processo evolutivo para resolver um problema de otimização combinatória. Através de sucessivas gerações, a população de rotas candidatas sofre processos de seleção, cruzamento e mutação para convergir em uma solução de baixo custo computacional e logístico.

Componentes do Algoritmo
Codificação: Cada indivíduo é representado por uma sequência (permutação) de IDs que identificam os alunos.

Função de Aptidão (Fitness): O cálculo é baseado na distância Euclidiana acumulada, iniciando na garagem, passando por todos os pontos de parada e retornando ao ponto de origem.

Seleção: Implementação de mecanismos de torneio ou roleta para garantir que as melhores rotas tenham maior probabilidade de reprodução.

Operadores Genéticos: Utilização de Crossover de Ordem (OX) ou similares para evitar duplicidade de paradas e mutação por troca (swap) para manter a variabilidade.

Tecnologias Utilizadas
Python 3

NumPy (Processamento matricial e geração de números aleatórios)

Matplotlib (Visualização de dados e gráficos de convergência)

Google Colab (Ambiente de execução)

Estrutura dos Arquivos
AG_VANS_Versao_2.ipynb: Versão modificada do algoritmo, contendo ajustes nos hiperparâmetros e visualização detalhada da convergência entre o melhor, o pior e o custo médio da população. Também possui a rota em formato grafico.

RoteamentoGenetico.ipynb: Versão um do projeto, contendo a fundamentação da lógica de roteamento e as primeiras implementações da fase de avaliação.

Instruções de Uso
Carregue os notebooks em um ambiente compatível com Jupyter (.ipynb).

Configure as coordenadas da garagem e dos alunos na célula de parâmetros iniciais, se necessário.

Execute o algoritmo para observar a evolução do fitness ao longo das gerações.

O resultado final apresentará a melhor rota encontrada e o respectivo gráfico de desempenho.
