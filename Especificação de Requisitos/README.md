# *ESPECIFICAÇÃO DE REQUISITOS*

## SUMÁRIO

###  HISTÓRICO DE VERSÕES
### 1. INTRODUÇÃO
- ##### 1.1. Objetivo
- ##### 1.2. Descrição do Projeto
- ##### 1.3. Diferenciais do Projeto
- ##### 1.4. Definições, Acrônimos e abreviaturas
### 2.VISÃO GERAL DO SISTEMA
- ##### 2.1. Premissas
- ##### 2.2. Restrições
### 3. SEGURANÇA DE DADOS
- ##### 3.1. Definição
- ##### 3.2. Implementação no projeto
### 4.PÚBLICO-ALVO
- ##### 4.1. Características do Usuário
- ##### 4.2. Dores do Publico-Alvo
- ##### 4.3. Rentabilidade do Negócio
### 5.RESQUISITOS FUNCIONAIS
- ##### 5.1. Requisitos Funcionais Controle de Acesso
- ##### 5.2. Requisitos Funcionais Controle Financeiro
- ##### 5.3. Requisitos Funcionais Controle dos Dashboards
- ##### 5.4. Requisitos Funcionais Controle Acessibilidade
### 6.REQUISITOS NÃO-FUNCIONAIS
- ##### 6.1. Usabilidade
- ##### 6.2. Confiabilidade
- ##### 6.3. Manutenabilidade
- ##### 6.4. Reusabilidade
- ##### 6.5. Acessibilidade
- ##### 6.6. Segurança
### 7.FUTURO DO PROJETO
### CONCLUSÃO


------------

## HISTÓRICO DE REVISÕES

| Data       | Versão | Descrição                                                |
|------------|--------|----------------------------------------------------------|
| 11/05/2021 | 0.0    | Criação do documento de especificação de requisitos.     |
| 11/05/2021 | 0.1    | Estruturação do Esqueleto do documento.                  |
| 12/05/2021 | 0.2    | Ajustes das terminologias.                               |
| 15/05/2021 | 0.3    | Definição da introdução do projeto.                      |
| 16/05/2021 | 0.4    | Definição do público-alvo.                               |
| 26/05/2021 | 0.5    | Definição da visão geral do sistema.                     |
| 26/05/2021 | 0.6    | Definição dos requisitos funcionais.                     |
| 28/05/2021 | 0.7    | Definição dos requisitos funcionais.                     |
| 12/05/2021 | 0.9    | Definição da segurança dos dados.                        |
| 14/05/2021 | 1.0    |Desenvolvimento da implementação de segurança  o projeto. |
|            |        |                                                          |

------------

## 1 - INTRODUÇÃO
###  1.1. Objetivo
A criação da plataforma tem como objetivo principal auxiliar microempreendedores individuais e/ou trabalhadores informais a administrar financeiramente seus produtos/serviços, desde a precificação até o controle de fluxo de caixa, para garantir um controle financeiro de qualidade.
Além disso, para ajudar os usuários a gerirem seus negócios de forma mais dinâmica e profissional, a plataforma disponibiliza links e datas de cursos para capacitação.

###  1.2. Descrição do projeto
A plataforma é um gerenciador contábil de fácil acesso e com layout super intuitivo. Após o cadastro, o usuário insere as informações necessárias nos campos pré-definidos, de acordo com o tipo de usuário (trabalhador informal ou microempreendedor individual) e a plataforma faz os cálculos básicos necessários.
Através do histórico das informações armazenadas, será gerado Dashboards de fácil leitura. Dessa forma, fazendo com que o usuário tenha maior conhecimento sobre questões financeiras do seu negócio.

### 1.3. Diferenciais do projeto
Visando abranger a maior parcela possível do nosso público alvo, além de possuir um layout intuitivo. Além disso, para maior liberdade e privacidade, o aplicativo se adequa a Lei Geral de Proteção de Dados Pessoais (LGPD), assegurando a proteção dos dados coletados dos usuários da plataforma.

### 1.4. Definições, Acrônimos e abreviaturas
Recomenda-se a leitura da definição dos seguintes termos, os quais estão presentes neste documento, visando uma melhor compreensão dos desenvolvedores, usuários e demais leitores:

**RF**: requisito funcional, classificando-se entre essencial, importante e desejável.

**RNF**: requisito não funcional.

**RS**: requisito do sistema (aborda requisitos funcionais e não funcionais de forma mais detalhada).

**UML**: Unified Modeling Language, linguagem de notação para expressar um sistema em forma de diagramas.

**MEI**: Microempreendedor Individual

**PF**: Pessoa física

**LGPD**: Lei Geral de Proteção de Dados

## 2 - VISÃO GERAL DO SISTEMA

### 2.1. Premissas
O usuário da plataforma encontrará um ambiente de fácil acesso e explicativo que vai auxiliá-lo no controle do próprio negócio no âmbito financeiro. Contendo as diretrizes colocadas pela LGPD como conceito de segurança no projeto. 

### 2.2. Restrições
O projeto tem como limitação principal o prazo de conclusão, já que seu desenvolvimento engloba diversos campos tanto na área contábil, quanto da esfera tecnológica, além das diretrizes nos direitos regidos pela LGPD. Diretamente derivado do prazo, temos que o escopo do projeto também se faz como restrição, em que as funcionalidades estabelecidas na análise de requisitos ficam dependentes do processo de desenvolvimento do projeto.

## 3 - SEGURANÇA DE DADOS

### 3.1. Definição

A LGPD trata da segurança e privacidade envolvida durante o processamento de dados pessoais por aplicações ou sistemas que coletam e armazenam os mesmos. Por sua vez, estes são responsáveis pela integridade das informações que foram coletadas ou geradas durante o uso da plataforma ou sistema. O surgimento dessas exigências veio do aumento de casos com vazamentos de dados ou a venda dos mesmos para empresas terceiras, que por sua vez tratavam os dados de forma não consentida pelo usuário de forma direta.
Esse processo visa limitar e assegurar que as informações sejam usadas para outros fins sem ser aqueles já declarados e aceitos pelo usuário. Com essa parametrização a identificação e aplicação de penalidades aos que descumprirem os termos da LGPD se torna mais fácil e ágil.

### 3.2. Implementação no projeto

O projeto desenvolvido foi estruturado utilizando os parâmetros da LGPD, em que os dados dos usuários são armazenados de forma local e individual, onde os administradores da plataforma não possuem mecanismos para a visualização das informações dos usuários, exceto os dados de cadastro ao aplicativo, para que seja feita a validação das informações, em que esse uso será declarado ao usuário e criptografado durante o armazenamento de contas ativas.
Junto ao armazenamento dos dados que são obtidos durante o uso ativo da plataforma, temos que, visando a LGPD, as informações guardadas no aplicativo serão excluídas após a determinação do usuário com o encerramento da conta. Esse processo garante ao titular dos dados que suas informações não serão usadas ou compartilhadas depois da sua experiência com a plataforma.
E por fim, o titular da conta tem a possibilidade de solicitar todas as informações que o controlador de dados detém, sendo essas, os dados de acesso que foram usados para a verificação no cadastro da conta. O não compartilhamento dos dados com terceiros também faz parte da LGDP, já que garante a limitação na exposição dos mesmos com empresas ou sistemas que não tenham os mesmos parâmetros de segurança que os da plataforma primária.

## 4 - PÚBLICO-ALVO

### 4.1. Características do Usuário
As características dos usuários permeiam empreendedores de nível iniciante, já que segundo o Sebrae, grande parte do surgimento de novos negócios têm relação com a necessidade de aumento na receita pessoal, que deriva da falta de espaço no mercado de trabalho e dificuldades com a capacitação que o mercado exige.
Microempreendedores Individuais e/ou trabalhadores informais de classe C e D, com idades entre 18 a 50 anos, da cidade de Araras- SP, que empreendem por necessidade e que tenham baixo acesso a informações sobre como gerir seu próprio negócio e que tenham acesso a um celular smartphone.

### 4.2. Dores do Público-Alvo
Segundo o Sebrae (2016), uma das dificuldades de se manter o próprio negócio é a falta de conhecimento (12%), impostos/tributos (10%) e inadimplência (6%), e, segundo os empresários entrevistados, um melhor planejamento do negócio (18%) e crédito mais facilitado (21%) seriam fatores que seriam úteis para que as empresas obtivessem sucesso.
Levando em consideração as informações acima e o período de pandemia devido a Covid-19, que acarretou na alta no desemprego (14%) e elevação do empreendedorismo no país (20%), a população ararense enfrenta o desemprego e a falta de vagas de emprego e iniciando o próprio negócio devido a necessidade e sem conhecimento de informações básicas sobre gerenciamento e conhecimento do próprio negócio. Além disso, há uma maior concorrência entre esses empreendedores, que, geralmente, empreendem em setores similares (venda de bolos, doces, salgados, pinturas de parede, pedreiro, carreto de mudança, etc).

### 4.3. Rentabilidade do Negócio
A rentabilidade da plataforma será feita através de parcerias com empresas que estejam dentro do mesmo âmbito que o empreendedorismo e o marketing digital, já que os mesmos podem fazer parte do conjunto de recomendações dadas pelo aplicativo. Os parceiros devem estar dentro da mesma proposta que o projeto, contendo funcionalidades de aceleração comercial e gerenciamento de pequenos negócios.
Por fim, nossos anunciantes devem possuir serviços ou conteúdos total ou parcialmente gratuitos, para que possam agregar qualidade de uso ao nosso público-alvo.

## 5 - REQUISITOS FUNCIONAIS
- #### Controle de Acesso
    * Acessar login; 
    * Recuperar senha;
    * Cadastrar usuário;

- #### Controle Financeiro
    * Cadastrar entradas para os cálculos;
    * Consultar vendas;
    * Cadastrar vendas;
    * Consultar saídas;
    * Cadastrar saídas;
    * Consultar fluxo de caixa;

- #### Controle de Dashboards
    * Consultar produtos mais vendidos;
    * Consultar produtos menos vendidos;
    * Consultar produtos com maiores rentabilidades;
    * Consultar produtos com maiores custos;

- #### Controle de Acessibilidade
    * Habilitar modo noturno;
    * Habilitar modo para daltonismo;
    * Alterar tamanho da fonte;
    * Consultar perguntas mais frequentes;
 

## 6- REQUISITOS NÃO-FUNCIONAIS
- ### 6.1. Usabilidade
   * O sistema deverá prover informações sobre os temas mais técnicos para os usuários.

- ### 6.2. Confiabilidade
   * O sistema deverá ter alta disponibilidade de tempo.

- ### 6.3. Manutenabilidade
   * O sistema deverá ter grande facilidade na manutenção do código.

- ### 6.4. Reusabilidade
   * O sistema poderá reutilizar os dados utilizados pelos usuários em diversas outras funcionalidades da plataforma.

- ### 6.5. Acessibilidade
   * O sistema deverá ter funcionalidades que irão facilitar a adequação do sistema visual e usual para determinados grupos de usuários.

- ### 6.6. Segurança
   * O sistema deve criptografar todas as comunicações entre o usuário e o servidor, assim    como deixar explícito qual será o uso e quais dados que o sistema detém do usuário. O sistema também deverá fazer a exclusão de toda e qualquer informação dos usuários quando não houver consentimento do mesmo ou caso este decida parar de fazer uso do nosso sistema. 

## 7 - FUTURO DO PROJETO
O futuro da plataforma se propõe a, além de facilitar os cálculos e o controle de um empreendimento inicial, encaminhar o microempreendedor para a capacitação de gerência do próprio negócio. Para isso, o projeto pretende acrescentar às funcionalidades da plataforma a recomendação de cursos gratuitos disponíveis em sites seguros e consolidados, incentivando os usuários a entrarem em contato com a esfera acadêmica empreendedora e, por sua vez, aumentar seu negócio com métodos e conhecimentos na área.
<br>
Também relacionando o cliente com a apresentação de facilidades já existentes no mercado, a plataforma contará com a integração dos usuários com outras ferramentas de complemento e produtividade para seu negócio. Dentro desse aspecto, será implementado um módulo dedicado ao uso das mídias sociais para impulsionar a divulgação e as vendas dos nossos clientes, contando com o aproveitamento máximo de ferramentas disponíveis nas principais redes sociais, como a  interpretação das estatísticas geradas pelas páginas virtuais ou as melhores formas de alcançar seu público-alvo com publicações.
<br>
E por fim, sendo uma ramificação das propostas anteriores, a divulgação de aplicativos e programas que podem ser usados pelos empreendedores para aumentar a qualidade do seu serviço ou produto, como o uso de ferramentas automáticas de criação publicitária, controle de feed nas redes sociais e planejamento de mídias.


## CONCLUSÃO
a definir

