# 🏥 Sistema de Atendimento de Pacientes

## 📖 Sobre o Projeto

Este projeto foi criado em Python com o objetivo de simular um sistema simples de atendimento e triagem de pacientes.

O programa coleta algumas informações do paciente, como:

* Temperatura
* Pressão arterial
* Dor no peito
* Sangramentos
* Convulsões
* Tosse
* Fraqueza
* Outros sintomas

Depois disso, o sistema analisa os dados e decide qual é o nível de prioridade do atendimento.

---

# 🎯 Objetivo do Sistema

A ideia principal do código é ajudar na organização do atendimento de pacientes.

O sistema tenta identificar se o paciente:

* Está em estado grave
* Precisa de atendimento rápido
* Possui sintomas leves
* Pode aguardar atendimento

Isso funciona como uma pequena simulação de triagem hospitalar.

---

# ⚙️ Como o Código Funciona

O programa funciona em etapas.

## 1️⃣ Coleta das Informações

Primeiro, o sistema pergunta várias informações ao usuário.

Exemplo:

```python
Temperatura = float(input("Digite a temperatura"))
```

Aqui o usuário digita a temperatura do paciente.

O mesmo acontece com:

* Pressão
* Dor
* Tosse
* Sangramentos
* Convulsões
* Fraqueza

Algumas perguntas são respondidas usando:

* S = Sim
* N = Não

---

## 2️⃣ Armazenamento dos Dados

Depois que o usuário responde, o programa guarda essas informações em variáveis.

Exemplo:

```python
dor = int(input("De 0 a 10, qual a intensidade da dor?"))
```

A variável `dor` guarda o número digitado.

---

# 🧠 Parte Mais Importante: As Condições

O sistema usa estruturas chamadas:

```python
if
elif
else
```

Essas estruturas servem para tomar decisões.

---

## 🚨 Casos Graves

Se o paciente tiver sintomas perigosos, o sistema mostra uma mensagem de urgência.

Exemplo de situações graves:

* Temperatura muito alta
* Pressão muito alta ou muito baixa
* Dor intensa
* Sangramento forte
* Convulsões
* Paciente inconsciente

Nesse caso o sistema exibe algo parecido com:

```python
ATENÇÃO! Paciente com sintomas graves.
```

---

## ⚠️ Casos Médios

Se os sintomas não forem tão graves, mas ainda precisarem de atenção rápida, o sistema envia o paciente para atendimento prioritário.

---

## ✅ Casos Leves

Quando os sintomas são mais simples, o paciente pode aguardar atendimento.

---

# 🖥️ Impressão do Resultado

Depois da análise, o programa mostra todas as informações coletadas.

Exemplo:

```python
print(f"Temperatura: {temperatura}°C")
```

O sistema também mostra:

* Pressão
* Dor
* Tosse
* Fraqueza
* Outros sintomas

Assim o usuário consegue visualizar um pequeno relatório do paciente.

---

# 📌 Conceitos de Python Utilizados

Este projeto utiliza vários conceitos básicos importantes para quem está aprendendo programação.

## 🔹 Variáveis

Servem para guardar informações.

Exemplo:

```python
temperatura = 39
```

---

## 🔹 Entrada de Dados (`input`)

Permite que o usuário digite informações.

Exemplo:

```python
input("Digite seu nome")
```

---

## 🔹 Conversão de Dados

O código usa:

* `int()` → números inteiros
* `float()` → números com vírgula

Exemplo:

```python
float(input())
```

---

## 🔹 Estruturas Condicionais

Usadas para o sistema tomar decisões.

Exemplo:

```python
if temperatura > 39:
```

---

## 🔹 Operadores Lógicos

O programa utiliza operadores como:

* `or` → OU
* `and` → E

Esses operadores ajudam a verificar várias condições ao mesmo tempo.

---

# 📊 O Que Esse Projeto Simula

Esse sistema simula uma pequena triagem médica.

Na vida real, hospitais usam sistemas parecidos para organizar a fila de atendimento e identificar pacientes que precisam de ajuda imediata.

Claro que este projeto é apenas educacional e simplificado.

---

# 🧾 Exemplo de Funcionamento

## Entrada do Usuário

```text
Digite a temperatura: 39
Paciente está consciente? S
Paciente está com dor no peito? S
```

## Resultado

```text
ATENÇÃO! Paciente com sintomas graves.
Encaminhar imediatamente.
```

---

# 📈 Fluxo do Sistema

O funcionamento do programa segue esta sequência:

1. Coletar informações do paciente
2. Guardar os dados
3. Analisar sintomas
4. Verificar gravidade
5. Mostrar resultado final

---

# 🎓 O Que Foi Aprendido com Esse Projeto

Com este projeto é possível praticar:

* Lógica de programação
* Uso de variáveis
* Entrada e saída de dados
* Estruturas condicionais
* Organização de informações
* Criação de sistemas simples

---

# ✅ Conclusão

Este projeto é um sistema simples de triagem hospitalar desenvolvido em Python.

Ele consegue coletar sintomas do paciente, analisar a gravidade e informar qual deve ser o tipo de atendimento.

Mesmo sendo um projeto iniciante, ele já utiliza vários conceitos importantes da programação e ajuda bastante no aprendizado da lógica.

---

# 👨‍💻 Autor: Thiago Rodrigues Ribeiro 

Projeto desenvolvido para fins educacionais e aprendizado em programação Python.
