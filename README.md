# Projeto 02 — Bug Report e Análise de Qualidade | Realbugz

<p align="center">
  <b>Portfólio de Garantia de Qualidade (QA) — Testes Manuais, Análise de Requisitos e Relatório de Defeitos.</b>
</p>

---

## Objetivo do Projeto
Realizar uma análise de qualidade completa em um formulário web de inscrição registro de participante de uma expedição arqueológica, utilizando os requisitos funcionais como base para planejar cenários de teste, executar testes exploratórios e funcionais, identificar desvios, documentar bugs de forma estruturada e avaliar a severidade e prioridade dos defeitos encontrados.

---

## Tecnologias, Ferramentas e Ambiente
* **Aplicação testada:** Realbugz (Módulo: *Registration Form* — Formulário de registro de expedição arqueológica).
* **Plataforma:** Web / Desktop
* **Navegador:** Google Chrome
* **Sistema Operacional:** Windows
* **Idioma:** Inglês
* **Tipo de Teste:** Manual (Funcional, Exploratório e de Validação de Campos)

---

## Escopo dos Testes (Campos Validados)
O formulário foi submetido a uma bateria de testes cobrindo dados pessoais, regras de negócio e restrições de entrada:

1. **Full Name** (Validação de caracteres especiais, números e limites de caracteres)
2. **Email** (Validação de formato, domínio, extensão e caracteres obrigatórios)
3. **Contact Number** (Validação de formato e números)
4. **Date of Birth** (Validação de faixa etária permitida)
5. **Archaeology Experience** (Seleção de opções)
6. **Preferred Role** (Seleção de função desejada)
7. **Preferred Expedition Region** (Seleção de região)
8. **Desired Salary** (Validação de slider / limites de valores e incrementos)
9. **Preferred Contact Method** (Seleção de método)
10. **Upload Passport/ID** (Validação de anexo de documentos)
11. **Additional Comments** (Validação de limite máximo de caracteres)
12. **Terms and Conditions** (Obrigatoriedade de concordância)

---

## Resumo da Execução dos Testes
Na aba **Exploração e Testes** da planilha de documentação, o escopo foi dividido da seguinte forma:
* **Total de Cenários Mapeados:** 41 cenários
* **✅ Passou (Pass):** 30 cenários comportaram-se estritamente conforme o esperado.
* **❌ Falhou (Fail):** 9 cenários revelaram inconsistências, resultando na abertura de *Bug Reports*.
* **⚠️ Observação:** 2 cenários com pontos de atenção ou refinamento de comportamento.

---

## Defeitos Encontrados (Bug Reports)
Foram identificados e catalogados **9 bugs** na aplicação, detalhados com passos para reprodução, ambiente, evidências e classificação de impacto:

| ID do Bug | Título do Defeito | Severidade | Prioridade |
| :--- | :--- | :---: | :---: |
| **BUG-001** | Sistema permite envio do formulário com números no campo *Full Name* | Média | Média |
| **BUG-002** | Sistema permite envio com caractere especial (`@`) no campo *Full Name* | Média | Média |
| **BUG-003** | Sistema permite mais de 50 caracteres no campo *Full Name* | Média | Média |
| **BUG-004** | Formulário não é limpo (*Clear Form*) automaticamente após envio bem-sucedido | Média | Média |
| **BUG-005** | Sistema permite cadastro de participante menor de 18 anos | Média | **Alta** |
| **BUG-006** | Sistema permite cadastro de participante com idade superior a 70 anos | Média | **Alta** |
| **BUG-007** | Slider de *Desired Salary* permite selecionar valor abaixo do mínimo ($0) | Baixa | Média |
| **BUG-008** | Slider permite incrementos de $1 em vez do intervalo de $10 estipulado | Média | Média |
| **BUG-009** | Campo *Additional Comments* permite inserir e enviar mais de 1.000 caracteres | Média | Média |

*(O detalhamento completo com passos para reprodução, pré-condições, resultados esperados e obtidos de cada bug encontra-se na planilha anexa).*

---

## Estrutura do Repositório
* `Bug Report + Análise de Qualidade.xlsx` — Planilha contendo os cenários de teste e a base de bugs.
* `Evidencias Projeto 2/` — Pasta contendo todas as capturas de tela comprobatórias de cada defeito.

---

##  Autoria
Desenvolvido por **Jhenifer Machado da Silva**  
*Estudante de Analise e desenvolvimento de sistemas* 
[LinkedIn][(https://www.linkedin.com/in/jhenifer-machado-da-silva-03a1782b0?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)
