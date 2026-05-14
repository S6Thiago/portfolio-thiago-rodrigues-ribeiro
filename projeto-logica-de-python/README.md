## 🐍 Práticas de Lógica com Python: Algoritmos de Automação
Este repositório contém uma série de exercícios desenvolvidos para consolidar os fundamentos da programação em Python.
O foco principal foi o domínio de estruturas de repetição, controle de fluxo e manipulação de tipos de dados.

Sobre o Projeto
Os algoritmos aqui presentes simulam situações reais do cotidiano — desde a gestão de uma loja até a análise climática — servindo como base para entender como a lógica de programação resolve problemas práticos.

.

 O que esses códigos têm em comum?
Embora resolvam problemas diferentes, todos os scripts utilizam a Tríade da Lógica de Programação:

1 - Estruturas de Repetição (for, while): Usadas para processar múltiplos dados (vários produtos, 7 dias da semana, vários alunos).

2 - Estruturas Condicionais (if, elif, else): Cruciais para a tomada de decisão (aplicar desconto, definir aprovação ou emitir alertas).

3- Tipagem e Entrada de Dados: Prática intensiva com float, int e input, garantindo que os cálculos matemáticos sejam precisos.

Detalhamento dos Scripts
1. Processamento de Vendas com Desconto Progressivo
O que faz: Simula um carrinho de compras que aceita múltiplos produtos, calcula o subtotal e aplica descontos automáticos baseados no valor final.

Destaque Técnico: Uso de acumuladores para somar o total de itens e o valor da compra dentro de um laço for.

Regra de Negócio: Descontos de 5% para compras acima de R$ 200 e 10% para compras acima de R$ 500.

2. Analisador Clímatico Semanal
O que faz: Coleta a temperatura de 7 dias e gera um relatório de integridade climática.

Destaque Técnico: Implementação de flags (sinalizadores) como alerta_extremo (booleano) para identificar condições perigosas.

Regra de Negócio: Identifica picos de calor acima de 35°C e emite alertas de segurança para temperaturas extremas.

3. Gestão Acadêmica (Sistema de Notas)
O que faz: Gerencia uma turma de alunos, calculando médias individuais e definindo o status pedagógico.

Destaque Técnico: Uso de while para validação de entrada (checar se a turma está vazia) e for para iterar sobre a lista de alunos.

Regra de Negócio:Média $\ge$ 7.0: AprovadoMédia entre 5.0 e 6.9: RecuperaçãoMédia < 5.0: Reprovado.

4. Simulador de Investimento (Poupança)
O que faz: Projeta o crescimento de um patrimônio mês a mês, considerando aportes variáveis e juros compostos.

Destaque Técnico: Lógica de juros acumulados sobre o saldo atualizado, não apenas sobre o depósito isolado.

Regra de Negócio: Monitoramento de meta financeira (ex: alerta ao atingir os primeiros R$ 200,00).

Tecnologias e Conceitos Aplicados
Linguagem: Python 3.x

Conceitos:

Funções (def) para organização de blocos de código.

Formatação de strings (f-strings) para exibição de valores monetários.

Cálculos aritméticos e operadores lógicos.

Como executar
Certifique-se de ter o Python instalado.

Clone o repositório.

Execute qualquer um dos arquivos .py no seu terminal:

python nome_do_arquivo.py

Autor: [Thiago Rodrigues Ribeiro]
Estudante de Análise e Desenvolvimento de Sistemas - UNICID
