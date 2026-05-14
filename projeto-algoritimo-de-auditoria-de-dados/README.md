Auditoria de Vendas Semanais 📊
Script em Python desenvolvido para análise de integridade e detecção de anomalias em fluxos de vendas.

📝 Descrição do Projeto
Este projeto automatiza o processo de conferência de vendas semanais. Ele calcula a média de transações e aplica regras de negócio para identificar valores atípicos (outliers) ou volumes de vendas que excedam parâmetros de segurança pré-estabelecidos.

🚀 Funcionalidades
O código executa quatro etapas principais:

Entrada de Dados: Coleta três valores de vendas (float) e permite a atualização de um LIMITE_SEGURANÇA global.

Cálculo de Média: Processa a média aritmética através de uma função dedicada (analisar_vendas).

Lógica de Auditoria (Checklist):

Quarentena: Bloqueio preventivo caso a média das vendas supere o limite de segurança.

Revisão Manual: Alerta gerado se qualquer venda individual for 5x superior à média calculada (identificação de picos isolados).

Funcionamento Normal: Confirmação de que os dados estão dentro da conformidade.

Validação de Tipagem: Exibe o tipo de cada variável no console para garantir que os cálculos financeiros mantenham a precisão necessária.

🛠️ Tecnologias Utilizadas
Python 3.x

Conceitos aplicados: Funções, Estruturas Condicionais, Escopo de Variáveis Globais e Manipulação de Inputs.

📖 Como Usar
Execute o script em um ambiente Python.

Insira os valores das três vendas quando solicitado.

Defina o novo limite de segurança para a verificação do sistema.

O sistema imprimirá o status da auditoria e o log de tipos de dados.

💻 O Código
Python

# AUDITORIA DE VENDAS SEMANAIS #
# Thiago Rodrigues Ribeiro #

LIMITE_SEGURANÇA = 10000

venda1 = float (input("Digite o valor da 1º venda: "))
venda2 = float (input("Digite o valor da 2º venda: "))
venda3 = float (input("Digite o valor da 3º venda: "))

def analisar_vendas():
    mediavendas = (venda1 + venda2 + venda3) / 3
    print("A média de vendas é: ", mediavendas)
    return mediavendas

mediavendas = analisar_vendas()

# Atualização de limite via escopo global
global LIMITE_SEGURANÇA
LIMITE_SEGURANÇA = int(input("\nDigite o novo limite de segurança: "))

# Verificação de condições de segurança
if mediavendas > LIMITE_SEGURANÇA:
    print("\nSISTEMA EM QUARENTENA!")
elif venda1 > mediavendas * 5 or venda2 > mediavendas * 5 or venda3 > mediavendas * 5:
    print("REVISÃO MANUAL")
else:
    print("FUNCIONAMENTO NORMAL")

# Log de depuração (Tipos de variáveis)
print(f"\nTipo de variável de vendas1: {type(venda1)}")
print(f"Tipo de variável de mediavendas: {type(mediavendas)}")
print(f"Tipo de variável de LIMITE_SEGURANÇA: {type(LIMITE_SEGURANÇA)}")
👤 Autor
Thiago Rodrigues Ribeiro - Desenvolvedor
