# Aprendizagem por Projetos Integrados 2020-1
![logo_figma](https://user-images.githubusercontent.com/56441534/138282337-943cad4b-ddad-43b0-a959-aa154fa47837.png)

O desenvolvimento do projeto foi em torno da necessidade da empresa parceira, de realizar uma gestão de informação mais eficaz para garantir a qualidade, o uso adequado e gerar valor através dos dados.
Tendo em vista a mudança do modelo de operação do Cadastro Positivo.


### Parceiro Acadêmico
SPC - Brasil. Uma empresa de tecnologia vinculada à CNDL para processar e armazenar todas as operações de crédito realizadas pelas empresas associadas.

***

### Visão do Projeto
DP Standardize se trata de uma ferramenta no formato Aplicativo Desktop que visa padronizar dados recebidos em remessas. O objetivo da ferramenta é ser utilizada como um Data Preparation, visando auxiliar no tratamento e padronização de uma remessa de dados, poupando um tempo valioso de trabalho antes de se agregar um valor maior a estes dados em futuros projetos.

![marketing_PI_11111](https://user-images.githubusercontent.com/57918707/87260544-dbc5ef80-c488-11ea-8987-faec80939a8b.png)

Preparar os dados é um processo que demanda tempo e esforço e é durante esta etapa que os dados são coletados, tratados e consolidados visando facilitar e auxiliar uma análise precisa dos dados.

DP Standardize trabalha principalmente na padronização dos dados, sendo capaz de analisar qualquer tabela ```xlsx``` e ```csv```. Permite a personalização dos campos, e possibilitando um apontamento de quais tipos de dados não podem conter em cada coluna.

A ferramenta permite também a geração de novos arquivos ```xlsx``` e ```csv``` oriundos dos arquivos originais. Depois de trabalhar na remessa de dados, as novas tabelas podem ser geradas, agora com os dados padronizados.

#### Lista de Requistos 
Por conta de ser o primeiro projeto dentro da meotodologia de Aprendizagem por Projetos Integrados, o cliente das equipes foi a própria FATEC São José dos Campos - Prof. Jessen Vidal. Sendo assim a lista de requistos utilizada para a validação das entregas do projeto foi definida e validada junto ao corpo docente da universidade. 

Os ```Requisitos Funcionais``` foram aplicados tendo em vista as seguintes Métricas de Qualidade disponibilizadas pela empresa parceira:

1. COMPLETUDE:
    - O campo de cadastro do estado referente a um endereço pode estar preenchido ou não, mesmo sendo obrigatório.

2. CONFORMIDADE:
    - Uma vez preenchido, tal preenchimento pode ser feito seguindo ou não as regras de negócio (formato, tamanho, etc)

3. CONSISTÊNCIA:
    - “Estado” é um dado presente em diversas bases, para um mesmo endereço é importante que todas as bases tenham o mesmo estado cadastrado.

4. UNICIDADE:
    - Em cada base que tenha dados geoespaciais é importante que o mesmo endereço, no mesmo estado, não tenha múltiplos registros.

5. ACURÁCIA:
    - Mesmo preenchido (completude) e no formato adequado (validade), o valor pode não se referir a nenhum estado existente na federação 
(ex: “RG” é uma sigla no formato adequado, porém não simboliza um estado)
.
Requisitos não Funcionais:
1. Aplicação Desktop.
2. Análise e tratamento de arquivos no formato ```xlsx``` e ```csv```.

***

#### link do repositório no Github
[Repositório](https://github.com/Mateus-Prestes/Tratamento-de-dados-SPC/tree/master)


### Tecnologias adotadas na solução
Para obter o resultado esperado, a equipe utilizou as seguintes tecnologias:

![tecnologias_PI](https://user-images.githubusercontent.com/56441214/87261156-8c34f300-c48b-11ea-89cf-a96eef22661c.png)

- Linguagem de programação ```Python``` para análise dos dados e alcance dos indicadores propostos.
- Framework ```Electron``` para o desenvolvimento da aplicação desktop GUI (Graphical User Interface).
- ```HTML```, ```CSS``` e ```JavaScript``` para criação e desenvolvimento do design da Interface do usuário.
- Por conta da utilização do Framework Electron, foi necessário migrar de python para ```NodeJS```. 

### Funcionamento

Abaixo alguns gifs de demonstração da utilização da ferramenta DP Standardize em seu resultado final.

A aplicação contém um sistema de login e senha, onde cada Analista pode possuir seu cadastro.

A padronização das tabelas é feita de forma rápida, devendo somente arrastar ou clicar para adicionar a tabela ao local indicado.

A página seguinte já contará com seus metadados, que ao serem clicados, abrirão uma nova janela para inserção da personalização já citada no tópico acima.

Após a escolha das opções, clique em **Baixar Tabela**, assim seus dados padronizados serão gerados e salvos. 

![ezgif com-video-to-gif (4)](https://user-images.githubusercontent.com/57918707/87265117-47fc1f80-c498-11ea-8787-60aab6d6b2e4.gif)

Ao final, sua nova tabela será gerada e salva automaticamente na pasta **GenerateTable** para tomar o destino conveniente.

![ezgif com-video-to-gif (5)](https://user-images.githubusercontent.com/57918707/87265314-dc668200-c498-11ea-9721-fe048f989bf3.gif)

Para padronizar mais campos, volte ao DP Standardize, clique em **Limpar**, adicione as novas personalizações e clique em **Baixar Tabela** novamente.

![ezgif com-video-to-gif (6)](https://user-images.githubusercontent.com/57918707/87265504-5dbe1480-c499-11ea-9b1e-51bab99032d0.gif)

Assim será gerada uma nova tabela com as novas padronizações.

![ezgif com-video-to-gif (7)](https://user-images.githubusercontent.com/57918707/87265568-7c241000-c499-11ea-90f2-1b7276aeaa5b.gif)


### Contribuições Pessoais
Durante o desenvolvimento do projeto atuei em conjunto com os demais membros no tratamento dos dados em arquivos no formato ```xlsx``` e ```csv``` utilizando a linguagem de programação ```python``` em conjunto de algumas bibliotecas como ```xlrd``` e ```matplotlib```.
Foram diversos tratamentos realizados nos dados, dentre eles:
- Verificação de valores nulos e repetidos.
- Geração de gráficos das métricas obtidas com os tratamentos.
![gráficos](https://user-images.githubusercontent.com/57918707/87258902-93ed9b00-c47d-11ea-8016-06595b8f563e.jpeg)

- Inserção, excusão e listagem de dados confidenciais contidos nas remessas de dados.
Um algoritmo é capaz de ler as extensões ```xlsx``` e ```csv``` da base de dados enviadas pela empresa parceira e fazer a verificação em todas as tabelas.

    - Verificação entre os dados cadastrados como confidenciais, para a inserção do nível de restrição: **_Baixo, Médio_** ou **_Alto_**.
![sprint_3_opc_1_1](https://user-images.githubusercontent.com/57918707/83317345-302b4d80-a202-11ea-8b2c-ba5d8db5ce37.gif)

    - Remoção de um metadado específico da configuração, para ser analisado como confidencial.
![sprint_3_opc_2_1](https://user-images.githubusercontent.com/57918707/83317359-594bde00-a202-11ea-9b2d-041e2bda4adb.gif)

    - Adição de metadado, na configuração e marcado para ser analisado como confidencial.
![sprint_3_opc_2_2](https://user-images.githubusercontent.com/57918707/83317378-78e30680-a202-11ea-803a-a9d7c16fc75e.gif)

    - Listagem de todos os metadados marcados como confidenciais.
![sprint_3_opc_2_3](https://user-images.githubusercontent.com/57918707/83317393-a2039700-a202-11ea-8704-ab287e6b240f.gif)

- Também atuei fortemente no estudo e entendimento para com a equipe das regras de negócio e métricas solicitadas pelo cliente a serem atendidas.

### Hard Skills
Dentre as habilidades técnicas, obtive o seguinte avanço:
- Análise de dados com python3 de arquivos ```xlsx``` e ```csv```:
    - Sei fazer com autonomia;
- Geração de gráficos com python3 e a biblioteca matplotlib:
    - Sei fazer com autonomia.
- Desenvolvimento dentro dos padrões da LGPD:
    - Aprendi a utilizar LGPD com acompanhamento de profissionais mais experientes.

### Soft Skills
Dentre as habilidades interpessoais performei minhas habilidades em Regras de negócio, relacionamento com cliente, .
As Habilidades na metodologia ágil também foram muito trabalhadas através do SCRUM, onde tive pela primeira que vez utilizar minhas habilidades e as ferramentas SCRUM com um cliente real. Todo esse desenvolvimento junto ao cliente foi acompanhado pelo corpo docente da FATEC São José dos Campos - Prof. Jessen Vidal.

 