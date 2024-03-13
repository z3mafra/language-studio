# Desafio: Desafio: Conhecendo o Language Studio do Azure com Análise de Sentimentos
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
>

O arquivo foi editado no editor do GitHub.  
Após a edição do arquivo, para atualizar o repositório local foi dado o comando git pull <endereço do repositório remoto>  

>- No repositório local;  
>  Clica no botão direito do mouse; e
>- Opção: "Open Git Bash here"
> No terminal digita o comando Git Pull <endereço do repositório remoto>

~~~bash
$ git pull https://github.com/z3mafra/language-studio.git
~~~

No GitHub foi criado o diretório 'contents' no repositório language-studio, para armazenar os prints dos resultados das análises.  

> Comandos/configurações:  
> 
> - Botão: "Add File".  
> - Opção: + Create new file.  
> - Preenchi: contents/image-list.txt  
> - Opção: Commit changes.  
> - Dentro do diretório 'inputs': "Add File".  
> - Opção: Upload files 
> - Cliquei em "Choose your files".  
> - Carregou o conjunto de imagens.
>


-------

### 3.2. Prints e descrição do processo no Language Studio  

O primeiro passo é criar um recurso de linguagem (Create a Language resource), no Azure AI services, com sua inscrição Azure.  

#### *Configurando para o Visio Studio*:
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

#### *Configure seu recurso em* **Azure AI Language Studio**

Em outra aba do navegador, abra o **Language Studio** em https://language.cognitive.azure.com e faça login.

Quando solicitado com **Select an Azure resource**, faça as seguintes configurações:

>- **Azure directory**: Default Directory, the directory you are using
>- **Azure subscription**: Select the subscription you are using
>- **Resource type**: Language
>- **Resource name**: select the Language service resource you just created
>- Em seguida, selecione **Done**.


#### *Analise as avaliações em* **Language Studio**  

>  1. Em um navegador da web, navegue até **Language Studio** em https://language.cognitive.azure.com.
>  2. Na página inicial **Welcome to Language Studio**, selecione a guia **Classify text** e, em seguida, selecione o bloco **Analyze sentiment and mine opinions**.
>  3. Em Selecionar idioma do texto, selecione **English**.
>  4. Em **Select your Azure resource**, selecione o seu recurso.
>  5. Em **Enter your own text**, carregue o arquivo (LabFala-texto-fiat-uno.txt), com o seguinte comentário:

>> Porque o Fiat Uno é tão bom?  
>> É um carro simples e robusto, com bom valor de revenda e liquidez, mesmo já fora de linha. Tem no acabamento simples sua maior fragilidade, mas no geral não apresenta falhas graves e custosas de reparar. E deve permanecer ainda “bom de mercado” por um bom tempo pela frente. É uma opção a ser considerada.  
>

>  6. Marque a caixa para reconhecer que a demonstração incorrerá em uso e poderá incorrer em custos e, em seguida, selecione **Run**.


<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat1-titulo.jpg" width="50%">

>  7. Revise a saída. Observe que o documento é analisado quanto ao sentimento, assim como cada frase. Selecione a frase 1 para mostrar a análise de sentimento dessa frase.


<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat2-titulo.jpg" width="50%">

  
<img src="https://github.com/z3mafra/language-studio/blob/main/contents/LabFala-fiat3-titulo.jpg" width="50%">

> [Note]  
> É interessante notar como a análise liga emtdades e enunciados à intensões, criando um sentido ponderado de uma avaliação. Com o Language Studio pode-se fazer mineração de sentimentos e opiniões, com três trechos de texto...  


-------

### 3.3. Alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças; 

O Processamento de Linguagem Natural (PNL) é fundamental para compreender e interagir com a linguagem escrita e falada, possibilitando a extração de significado semântico e a formulação de respostas em linguagem natural.  

Agências de Viagens, entre outros serviçoes, podem usar o Azure Language Studio para analisar avaliações de hotéis, identificando sentimentos e entidades mencionadas, melhorando a experiência do cliente.  

O Azure Language Studio é uma ferramenta poderosa oferecida pela Microsoft para análise de texto e compreensão de linguagem natural. Uma das aplicações mais significativas do Language Studio é a análise de sentimentos, onde ele pode ser utilizado para determinar se as avaliações de produtos, serviços ou qualquer outro tipo de conteúdo são predominantemente positivas ou negativas. Isso é essencial para empresas que desejam entender o feedback dos clientes e a reputação de sua marca. Ao empregar técnicas de processamento de linguagem natural avançadas, o Language Studio é capaz de identificar nuances no texto, capturando não apenas palavras-chave, mas também o contexto e o tom geral das avaliações.  

Através do uso de algoritmos de aprendizado de máquina e modelos de linguagem pré-treinados, o Language Studio é capaz de analisar grandes volumes de avaliações de forma rápida e eficiente. Ele pode detectar palavras e frases que indicam sentimentos positivos ou negativos, levando em consideração aspectos como sarcasmo, ironia e ambiguidade. Isso permite uma avaliação mais precisa e detalhada do sentimento expresso no texto, proporcionando insights valiosos para as empresas.  

Uma das vantagens do Azure Language Studio é sua capacidade de personalização. As empresas podem ajustar os modelos de análise de sentimento de acordo com suas necessidades específicas e o domínio de seu negócio. Isso permite uma análise mais precisa e relevante das avaliações, levando em consideração termos e expressões específicas da indústria ou do público-alvo. Além disso, o Language Studio oferece integração com outras ferramentas e serviços do Azure, permitindo uma implementação suave em diferentes sistemas e plataformas.  

No entanto, é importante reconhecer que nenhuma ferramenta de análise de sentimento é perfeita. O Azure Language Studio pode enfrentar desafios ao lidar com textos complexos ou ambíguos, onde o contexto pode influenciar significativamente o sentimento expresso. Além disso, como qualquer tecnologia baseada em machine learning, o desempenho do Language Studio pode variar dependendo da qualidade dos dados de treinamento e das configurações específicas utilizadas. Portanto, é fundamental complementar a análise automatizada com revisão humana e outras formas de feedback para obter uma compreensão abrangente das avaliações.  

Um outro aspecto importante, que também deve ser consdierado, é a integração dessas ferramentas com os ambientes de navegação na internet, tais como plataformas, sites e aplicativos.  
  
-------

## 4. Compartilhar o link do repositório através do botão 'entregar projeto'  

Antes de finalizar o desafio, uma providência importate é limpar (Clean up) o Language Studio, deletando os recrusos para não gerar custos desnecessários.

### **Clean up**  
Como é recomendado na documentção, senão se pretende fazer mais exercícios, excluir todos os recursos que não precisa mais. Isso evita acumular custos desnecessários.  
‑
>    1. Abra o portal do Azure (<https://portal.azure.com/>) e selecione o grupo de recursos que contém o recurso que você criou.  
>    2. Selecione o recurso e selecione Excluir e depois Sim para confirmar. O recurso é então excluído.
>
>>  - **Observação:** Uma curiosidade que, nesta etapa, a plataforma informou que não houve consumo de recursos, restando ainda um crédito de R$ 988,18, na assinatura gratuita. Foi a mesma posição do último desafio no Azura, Vision Studio: Detect faces; Read text; e, Analyze images.  

Após completar o Desafio, fiz a atualização no repositório local com o comando git pull.  

>- No repositório local;  
>  Clica no botão direito do mouse; e
>- Opção: "Open Git Bash here"
> No terminal digita o comando Git Pull <endereço do repositório remoto>

~~~bash
$ git pull https://github.com/z3mafra/language-studio.git
~~~

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
