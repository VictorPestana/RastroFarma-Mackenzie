# PROJETO RASTROFARMA: RASTREIO E CONTROLE DE QUALIDADE FARMACÊUTICA

## 1. IDENTIFICAÇÃO DO PROJETO
* **Instituição:** Universidade Presbiteriana Mackenzie
* **Curso:** Curso de Sistemas de Informação
* **Disciplina:** Modelagem de Sistemas
* **Local e Ano:** Barueri, SP - 2026
* **Integrantes do Grupo:**
  * Victor Gouveia Pestana
  * Yan Ambrosio Gralha
  * Patrick Piloto
  * David Ventura

---

## 2. RESUMO DO PROJETO
O projeto RastroFarma apresenta o desenvolvimento de um sistema integrado para a indústria farmacêutica, focando na rastreabilidade e na gestão eficiente dos dados. A solução proposta utiliza a modelagem UML para estruturar processos que garantam que os processos sigam todas as normas da ANVISA e de fabricação. 

O sistema abrange a Gestão de Produção, como controle de lotes, processos de fabricação e rastreabilidade, além da Gestão de Estoque e Logística, voltada para o monitoramento de matérias-primas e produtos finais. Através da solução proposta, busca-se eliminar erros operacionais e elevar a segurança dos pacientes.

---

## 3. ALINHAMENTO COM AS ODS (ONU)
O projeto está alinhado com os Objetivos de Desenvolvimento Sustentável (ODS) da ONU:
* **ODS 3 (Saúde e Bem-Estar):** Garante que o consumidor final, o paciente, tenha acesso a medicamentos seguros e verificados, reduzindo riscos à saúde pública.
* **ODS 9 (Indústria, Inovação e Infraestrutura):** Foca no uso da tecnologia para modernizar a infraestrutura logística e os processos industriais do setor.

---

## 4. OBJETIVOS
* **Objetivo Geral:** Desenvolver a modelagem de um sistema integrado para a indústria farmacêutica que conecte os módulos de gestão de produção e logística, utilizando diagramas UML para estruturar o controle de qualidade e a rastreabilidade de lotes.
* **Objetivos Específicos:** * Levantamentos de requisitos necessários para o controle de produção e movimentação de estoque, seguindo as exigências da ANVISA.
  * Construção de diagramas de Casos de Uso, Classes, Sequência, Atividade e Estados para validar a lógica do software.
  * Propor um fluxo de dados onde o Controle de Qualidade valide a liberação de lotes para a logística de forma autorizada.
  * Definir mecanismos de verificação (como ID's) que asseguram a eficácia e a credibilidade dos medicamentos entregues aos pacientes.

---

## 5. ESPECIFICAÇÃO DO SISTEMA

### 5.1 Requisitos Funcionais (RF)
* **RF01:** O sistema precisa permitir o cadastro de lotes de medicamentos;
* **RF02:** Ele deve registrar todas as etapas da produção;
* **RF03:** Deve permitir o cadastro das matérias-primas usadas;
* **RF04:** Controlar o estoque de insumos e produtos acabados;
* **RF05:** Permitir o rastreamento completo de cada lote;
* **RF06:** Permitir que o controle de qualidade avalie os lotes;
* **RF07:** Liberar a distribuição apenas de lotes aprovados;
* **RF08:** Registrar as movimentações logísticas;
* **RF09:** Gerar relatórios de rastreabilidade;
* **RF10:** Permitir a consulta do histórico de cada lote;
* **RF11:** O sistema deve permitir que o ponto de venda (farmácia) consulte o status do lote antes de finalizar a venda ao cliente.

### 5.2 Requisitos Não Funcionais (RNF)
* **RNF01:** O sistema deve garantir a segurança das informações;
* **RNF02:** Ter alta disponibilidade;
* **RNF03:** Acesso restrito a usuários autenticados;
* **RNF04:** Estar em conformidade com as normas da ANVISA;
* **RNF05:** Ter uma interface intuitiva;
* **RNF06:** Registrar logs de todas as operações.

### 5.3 Regras de Negócio (RN)
* Um lote só pode ser distribuído após aprovação do controle de qualidade;
* Cada lote deve ter um identificador único;
* Lotes reprovados não podem ser enviados para logística;
* Todas as etapas devem ser registradas no sistema;
* A rastreabilidade deve identificar a origem e o destino do medicamento;
* Um medicamento só pode ter a venda autorizada se o lote estiver com o status "Aprovado" no Controle de Qualidade.

---

## 6. ARQUITETURA DO SISTEMA
A arquitetura proposta para o sistema RastroFarma segue o modelo em camadas, estruturado em:
* **Camada de Apresentação:** responsável pela interface com o usuário;
* **Camada de Aplicação:** responsável pelas regras de negócio;
* **Camada de Dados:** responsável pelo armazenamento das informações.
