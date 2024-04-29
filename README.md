# Gerador automático de horários (Novo projeto)

## Introdução

A UFERSA tem com atual demanda no final de cada período o planejamento do cadastro e com as atualização dos horários dos componentes curriculares e assoaciação aos devidos professores. É de conhecimento das coordenadorias acadêmicas e chefias de departamento que este período é um momento crítico para ser resolvidos, por diversos fatores. 

## Restrições conhecidas

O sistema atual é gerido pelas coordenações através de troca de planilhas que por muitas vezes pode ser cadastrado de forma equivocada. Isto ocorre, dentre outros fatores pela quantidade extensa de restrições que o sistema possui. A conhecer alguns:

+ Restrição de tempo
  + Existe um fluxo necessário para o cadastro, começando pela coordenação de C&T e BTI e seguindo pelas coordenações de segundo ciclo.
+ Restrição de horários: 
  + Há um acordo não escrito que os professores devem estar em três dias específicos para facilitar a locomoção para suas residências que normalmente estão fora do *campus*.
+ Restrições de período: 
  + As disciplinas devem ser posicionadas de forma que os disciplinas de um mesmo período não estejam com conflitos de horários.
+ Restrição de espaço físico:
  + A depender do agrupamento da alocação dos componentes de laboratórios, seria necessário re-alocar estes componentes de forma há não haver *choque* de horário/local.
  + A reserva do espaço físico deve comportar a capacidade máxima cadastrada da turma.
+ Retrição de turno:
  + Existem componentes que devem ser colocados em um turno específico. Isto ocorre por dois motivos: aproveitamento melhor da estadia dos alunos no campus e necessidade da característica do curso ao qual pertence o componente.
+ Restrição de professores:
  + As turmas de um mesmo professor não podem conflitar com os horários;

## Trabalhos iniciais

Recentemente a UFERSA campus Pau dos Ferros desenvolveu dois trabalhos iniciais para para o ambiente de Smart Campus. Os trabalhos dos alunos Leonardo Dantas e Luan Paiva desenvolveram um sistema para cadastro dos componentes curriculares de forma a não haver choques entre disciplinas do mesmo período e com os mesmo professores. O sistema que foi desenvolvido com o *backend* por Leonardo e *frontend* por Luan realiza a verificação componente a componente da existência de conflitos.


## Proposta

Com base nos trabalhos iniciais e demanda antiga dos coordenadores, proponho uma nova proposta a ser explorada pelo nosso grupo *smart campus*: Gerador automático de horários (nome provisório e pretencioso).

Este sistema seria responsável, como o nome sugere, por conduzir a construção de horários factíveis para o planejamento de um semestre. Uma vez que todos reconheçam e descrevam suas restrições, o sistem propõe uma geração sistemática da elaboração de horários. 

Os benefícios para o nosso grupo surgiria das propostas multidisciplinares que os alunos e professores poderiam contribuir. Abordarei algumas tarefas necessárias para um bom desenvolvimento:

### Lógica proposicional e Banco de Regras

As regras lógicas estariam presentes a todo momento, uma vez que a escolha das disciplinas seriam baseadas nas restrições inicialmente propostas pelo coordenadores, chefias e professores envolvidos.

Uma nova sugestão seria incluir um ambiente para cadastro de novas regras. Este sistema que poderia ser chamado de **Banco de Regras** responderia pela inclusão de situações que não estavam previstas no projeto inicial. Podem ocorrer restrições distintas em cada período que não é possível ser observado *a priori*.

### Estrutura de Dados

É previsto que a avaliação de situações factíveis seria implementado por um grande esforço computacional. Por isso se faz necessário escolher adequadamente as estruturas do sistema, prever a complexidade algorítmica, verificar se a solução pode ser resolvida por completo (avaliação de todas as situações) ou resolvida de forma estocástica: apresentar uma(s) solução(ões) que atende(m) a maior parte das restrições.

Outra avaliação da disciplina de Estrutura de Dados é verificar se podemos *abrir mão* da complexidade de espaço em contrapartida da melhoria na complexidade de tempo. Isto realizado na escolha das características dos objetos envilvidos.

### Engenharia de Software

Para planejamento da execução do sistema seria interessante incluir os conhecimentos deste componente para criar um fluxo de entrega regular dos produtos de software. Aos poucos o projeto irá ganhando forma e em etapas destacadas poderíamos gerar trabalhos científicos (artigos, TCC), Registros de Software ou Patentes.

Inclui-se também neste conteúdo:

+ Identficação dos Stakeholders: Quais serão os responsáveis pelo projeto;
+ Levantamento de requisitos: Realização de entrevistas com os interessados para elicitar as reais necessidades do sistema;
+ Análise e priorização: Analisar as necessidades prioritárias para ter um fluxo contínuo de entregas;
+ Documentação: Geração dos diagramas de Engenharia de Software para conduzir o trabalho;
+ Validação: Avaliar se os requisitos foram cumpridos em concordância do que é solicitado pelos usuários finais.

### PROGRAMAÇÃO CONCORRENTE E DISTRIBUÍDA (PCD)

Não há uma garantia que os desenvolvimentos com estrutura de dados retornem a tempo soluções factíveis. Uma tentativa inicial foi realizada pelo professor Italo em linguagem Java mas como era de se esperar, o tempo necessário para que o algoritmo convirja era superior ao esperado. O PCD será útil para aumentar as chances da resolução do problema, ou então que a solução seja avaliada em tempos menores a tempo de averiguação da corretude das soluções.

## Integrantes do projeto

Vários perfis podem ser observados na execução desta proposta. 

+ Um primeiro perfil poderia ser algum aluno com habilidade em análise de dados. Provavelmente este aluno teria concluído a disciplina de estatística.
+ Alunos de Engeharia de Computação ou Engenharia de Software: Alunos neste perfil estariam habilitados a desenvolver suas habilidades na produção deste sistema tendo em vista os disciplinas listadas
