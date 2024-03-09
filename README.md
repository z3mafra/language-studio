# Desafio: Language Studio do Azure
## Repositório: language-studio  

> 1. Crie um novo repositório no github com um nome a sua preferência;  
> 2. Crie uma pasta chamada 'inputs' e crie um documento de texto com algumas sentenças;  
> 3. Crie um arquivo chamado readme.md, deixe alguns prints descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças;  
> 4. Compartilhe conosco o link desse repositório através do botão 'entregar projeto'.  
  
-------

## 1. Criar um novo repositório no github com um nome a sua preferência  

Na maquina local foi crido o diretório 'language-studio'  

~~~bash
$ mkdir language-studio
~~~

Depois, entrei no diretório criado e iniciei o diretório como um repositório no Git.

~~~bash
$ CD language-studio
$ git init
~~~

No GItHub foi criado o repositório 'language-studio'

> Comandos/configurações:  
> 
> - "Novo repositório".  
> - Nome para o repositório: 'language-studio'.  
> - Descrição: "Desafio: conhecendo o Language Studio do Azure".  
> - Visibilidade: "pública".  
> - Opção: README.  
> - Cliquei em "Criar repositório".  
> 

-------

## 2. Crie uma pasta chamada 'inputs' e crie um documento de texto com algumas sentenças;    

No GItHub foi criado o diretório 'inputs' no repositório 'language-studio'

> Comandos/configurações:  
> 
> - Botão: "Add File".  
> - Opção: + Create new file.  
> - Preenchi: inputs/algumas-sentences.txt  
> - Opção: Commit changes.  

-------

## 3. Crie um arquivo chamado readme.md, deixe alguns prints descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças    

-------

### 3.1. Criar um arquivo readme.md  

No GitHub na raiz do repositório 'language-studio', foi crido o arquivo 'readme.md', no ato da criação do repositório (Ver etapa 1. Criar um novo repositório no github).  
Nesta etapa, o procedimento foi o de editar o arquivo "readme.md". E, para isso:

>>  No repositório 'language-studio', no GitHub:
> - Botão: :pencil2: "lápis"  
> - Abre o editor de texto no GitHub.

Após a edição do arquivo, no diretório local foi feito o git pull do repositório.  
O arquivo foi editado no editor do GitHub e com o auxílio do VSCode no diretório local.  
-------

### 3.2. Prints e descrição do processo no Language Studio  

O primeiro passo é criar um recurso de linguagem (Create a Language resource), no Azure AI services, com sua inscrição Azure.  

*Configurando para o Visio Studio*:
>
>- 1. Entrar no portal Azure [https://portal.azure.com](https://portal.azure.com/?azure-portal=true).  
>- 2. Clicar no botão ＋Create a resource e procure por serviço de idiomas (*Language Service*). Selecionei "create a Language service plan". Direcionado a uma página para **Select additional features**. Mantenha a seleção padrão e clique em **Continue to create your resource**.  
>- 3. Na página **Create Language** (Criar Idioma), configure-o com as seguintes configurações:
>     >> - Subscription: Azure subscription 1.  
>     >> - Resource group: LabLang.  
>     >> - Region: East US.  
>     >> - Name: DioFalaLab.  
>     >> - Pricing tier: Standard S0.  
>     >> - Selecinei o check box: "I acknowledge that I have read and understood all the terms below.  
>
>- 4. Selecionei Review + create then Create e aguardei a implantação se completar.

Configure your resource in Azure AI Language Studio

In another browser tab, open Language Studio at https://language.cognitive.azure.com and sign in.

When prompted with Select an Azure resource, make the following configurations:

Azure directory: Default Directory, the directory you are using
Azure subscription: Select the subscription you are using
Resource type: Language
Resource name: select the Language service resource you just created
Then select Done.


Analyze reviews in Language Studio
1. In a web browser, navigate to Language Studio at https://language.cognitive.azure.com.

2. On the Welcome to Language Studio landing page, select the Classify text tab, then select the Analyze sentiment and mine opinions tile.

3. Under Select text language, select English.

4. Under Select your Azure resource, select your resource. LabFala-texto-fiat-uno.txt

5. Under Enter your own text, upload a file, or use one of our sample texts, copy and paste the following review:

>> Porque o Fiat Uno é tão bom?  
>> É um carro simples e robusto, com bom valor de revenda e liquidez, mesmo já fora de linha. Tem no acabamento simples sua maior fragilidade, mas no geral não apresenta falhas graves e custosas de reparar. E deve permanecer ainda “bom de mercado” por um bom tempo pela frente. É uma opção a ser considerada.  
>

6. Check the box to acknowledge that the demo will incur usage and may incur costs, and then select Run.


<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat1-titulo.jpg" width="50%">

7. Review the output. Notice that the document is analyzed for sentiment, as well as each sentence. Select Sentence 1 to show the sentiment analysis for that sentence.


<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat2-titulo.jpg" width="50%">

  
<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat3-titulo.jpg" width="50%">


run and run (prints)

In this exercise you used Language Studio to either create a new Language resource or use an existing Language resource. You enabled the resource in Settings before trying out the Sentiment and opinion mining service. You then tested the service with three pieces of text.


-------

### 3.3. alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças; 

O Processamento de Linguagem Natural (PNL) é fundamental para compreender e interagir com a linguagem escrita e falada, possibilitando a extração de significado semântico e a formulação de respostas em linguagem natural.  

Agências de Viagens podem usar o Azure Language Studio para analisar avaliações de hotéis, identificando sentimentos e entidades mencionadas, melhorando a experiência do cliente.  

O Azure Language Studio é uma ferramenta poderosa oferecida pela Microsoft para análise de texto e compreensão de linguagem natural. Uma das aplicações mais significativas do Language Studio é a análise de sentimentos, onde ele pode ser utilizado para determinar se as avaliações de produtos, serviços ou qualquer outro tipo de conteúdo são predominantemente positivas ou negativas. Isso é essencial para empresas que desejam entender o feedback dos clientes e a reputação de sua marca. Ao empregar técnicas de processamento de linguagem natural avançadas, o Language Studio é capaz de identificar nuances no texto, capturando não apenas palavras-chave, mas também o contexto e o tom geral das avaliações.  

Através do uso de algoritmos de aprendizado de máquina e modelos de linguagem pré-treinados, o Language Studio é capaz de analisar grandes volumes de avaliações de forma rápida e eficiente. Ele pode detectar palavras e frases que indicam sentimentos positivos ou negativos, levando em consideração aspectos como sarcasmo, ironia e ambiguidade. Isso permite uma avaliação mais precisa e detalhada do sentimento expresso no texto, proporcionando insights valiosos para as empresas.  

Uma das vantagens do Azure Language Studio é sua capacidade de personalização. As empresas podem ajustar os modelos de análise de sentimento de acordo com suas necessidades específicas e o domínio de seu negócio. Isso permite uma análise mais precisa e relevante das avaliações, levando em consideração termos e expressões específicas da indústria ou do público-alvo. Além disso, o Language Studio oferece integração com outras ferramentas e serviços do Azure, permitindo uma implementação suave em diferentes sistemas e plataformas.  

No entanto, é importante reconhecer que nenhuma ferramenta de análise de sentimento é perfeita. O Azure Language Studio pode enfrentar desafios ao lidar com textos complexos ou ambíguos, onde o contexto pode influenciar significativamente o sentimento expresso. Além disso, como qualquer tecnologia baseada em machine learning, o desempenho do Language Studio pode variar dependendo da qualidade dos dados de treinamento e das configurações específicas utilizadas. Portanto, é fundamental complementar a análise automatizada com revisão humana e outras formas de feedback para obter uma compreensão abrangente das avaliações.  


-------

## 4. Compartilhar o link do repositório através do botão 'entregar projeto'  

Antes de finalizar o desafio, uma providência importate é limpar (Clean up) o Language Studio, deletando os recrusos para não gerar custos desnecessários.

### **Clean up**  
Como é recomendado na documentção, senão se pretende fazer mais exercícios, excluir todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.  
‑
>    1. Abra o portal do Azure (<https://portal.azure.com/>) e selecione o grupo de recursos que contém o recurso que você criou.  
>    2. Selecione o recurso e selecione Excluir e depois Sim para confirmar. O recurso é então excluído.
>
>>  - **Observação:** Uma curiosidade que, nesta etapa, a plataforma informou que não houve consumo de recursos, restando ainda um crédito de R$ 988,18, na assinatura gratuita.


### **Postar link do repositório**
Como é recomendado na documentção, senão se pretende fazer mais exercícios, excluir todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.  
>    1. Abra o portal da DIO (<https://www.dio.me/>), com as credenciais e selecione o [Bootcamp Microsoft AZure AI Fundamentals](https://web.dio.me/track/microsoft-azure-ai-fundamentals).
>    2. Entra na Atividade Desafio de projeto: "Reconhecimento Facial e transformação de imagens em Dados no Azure ML"
>    3. Clica no botão "ENTREGAR PROJETO" 
>    4. Cola o link do projeto na caixa de texto "Repositório do Projeto"; Cola a descrição do repositório; Ler e marcar o Check box "Termos de uso", concordando com os termos o recurso; e,
>    5. Selecione Entregar. O Desafio é então entregue.
>

-------

-------
