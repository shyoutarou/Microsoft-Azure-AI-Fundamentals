<p align="center">
    <img  src="../imagens/00_Logo_Bootccamp.jpeg" width="1000"/>  
</p>

<h1 align="center">
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/dc92e499-6ec6-4c82-af3f-00c40538ca80.png"></a>
    <span> Análise de Sentimentos com Language Studio </span>
</h1>

## Criando modelo de previsão - Passo a passo

Neste LAB, exploraremos o uso do Azure Speech Studio e a análise linguística proporcionada pelo Language Studio. Durante a prática, teremos a oportunidade de aprofundar nosso entendimento sobre como aproveitar essas ferramentas avançadas da Microsoft Azure. Estaremos focados em aprimorar nossas habilidades na implementação de soluções de análise de fala e linguagem, abrindo portas para uma compreensão mais ampla e prática das capacidades oferecidas por essas tecnologias inovadoras.


### Como entregar esse projeto?
1. Crie um novo repositório no github com um nome a sua preferência
2. Crie uma pasta chamada 'inputs' e crie um documento de texto com algumas sentenças3. 
3. Crie um arquivo chamado readme.md, deixe alguns prints descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças 
4. Compartilhe conosco o link desse repositório através do botão 'entregar projeto' na plataforma da [DIO](https://web.dio.me/home)



### Instrutora
**Valéria Baptista** - [Linkedin](https://www.linkedin.com/in/valeriabaptista/)
<br>Head of Cloud and Cybersecurity, CloudData Tech & DevOps

### Links Importantes
- [Explorar o Estúdio de Fala](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html)
- [Analise texto com Language Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-análise.html)




## Explorar o Estúdio de Fala

O serviço Azure AI Speech transcreve a fala em texto e o texto em fala audível. Você pode usar o AI Speech para criar um aplicativo que possa transcrever notas de reuniões ou gerar texto a partir da gravação de entrevistas.

Criar um recurso de fala do Azure AI

Você pode usar o serviço de Fala criando um recurso de Fala ou um recurso de serviços de IA do Azure .

Neste exercício, você criará um recurso AI Speech, a menos que já tenha um recurso que possa usar.
1.	Em outra guia do navegador, abra o Azure AI Speech Studio   em https://speech.microsoft.com  entrando com sua conta da Microsoft.
 


2.	Selecione Configurações então Crie um recurso. 
 

3.	Configure-o com as seguintes configurações:
- Nome do novo recurso: Insira um nome exclusivo.
- Assinatura: Sua subscrição Azure .
- Região : Selecione uma região suportada .
- Nível de preços: FO gratuito (se disponível, caso contrário, selecione Padrão S0).
- Grupo de recursos: selecione ou crie um grupo de recursos com um nome exclusivo.
 

4.	Selecione Criar recurso. Aguarde até que o recurso seja criado e selecione Usar recurso. O Obter iniciado com página de fala é exibido .


## Explore a fala em texto no Speech Studio

1.	Selecione https://aka.ms/mslearn-speech-files para baixar o speak.zip . Abra a pasta.
2.	Na página Introdução à fala, em Fala, localize Fala em tempo real para texto. Selecione Experimente a fala em tempo real para texto .
 

3.	No subtítulo Experimente, reconheça a política de uso de recursos lendo e marcando a caixa.

 


4.	Em Escolher arquivos de áudio, selecione Procurar arquivos e navegue até a pasta onde você salvou o arquivo. Selecione WhatAICanDo.m4a e então Abrir.
 
5.	O serviço Speech transcreve e exibe o texto em tempo real. Se você tiver áudio em seu computador, poderá ouvir a gravação enquanto o texto é transcrito.
6.	Revise a saída, que deve ter reconhecido e transcrito com êxito o áudio em texto.


## Analise texto com Language Studio

Neste exercício, você explorará os recursos da linguagem Azure AI analisando alguns exemplos de avaliações de hotéis. Você usará o Language Studio para entender se as avaliações são em sua maioria positivas ou negativas.

O Processamento de Linguagem Natural (PNL) é um ramo da IA que lida com a linguagem escrita e falada. Você pode usar a PNL para construir soluções que extraiam significado semântico de texto ou fala, ou que formulem respostas significativas em linguagem natural.  O Azure AI Language Service inclui análise de texto e recursos de PNL. Isso inclui a identificação de frases-chave no texto e a classificação do texto com base no sentimento.

### Crie um recurso de idioma

Você pode usar muitos recursos do Azure AI Language com um recurso de idioma ou de serviços do Azure AI . Existem alguns casos em que apenas um recurso Idioma pode ser usado. Para o exercício abaixo, utilizaremos um recurso Linguagem. 
 


Se ainda não o fez, crie um recurso de idioma na sua assinatura do Azure.
 

## Configure seu recurso no Azure AI Language Studio

1.	Em outra guia do navegador, abra o Language Studio em https://language.cognitive.azure.com e entre.
2.	Quando solicitado com Select an Azure resource , faça as seguintes configurações:
- Diretório do Azure : diretório padrão, o diretório que você está usando
- Assinatura do Azure : selecione a assinatura que você está usando
- Recurso tipo: Idioma
- Nome do recurso: selecione o recurso de serviço de idioma que você acabou de criar
 

Em seguida, selecione Concluído .
Observação : se você não for solicitado a escolher um recurso de idioma, pode ser porque você possui vários recursos de idioma em sua assinatura; nesse caso:
1.	Na barra na parte superior da página, selecione Configurações ( ⚙ ) .
2.	Na página Configurações , visualize a guia Recursos .
3.	Selecione o recurso que você acabou de criar e selecione Alternar recurso. Verifique se identidade Gerenciada está Habilitado


4.	No topo da página, selecione Language Studio para retornar à página inicial do Language Studio.


## Analisar avaliações em Language Studio

1.	Num navegador web, navegue até Language Studio em https://language.cognitive.azure.com 
2.	Na página inicial Bem-vindo ao Language Studio, selecione a guia Classificar texto e, em seguida, selecione o bloco Analisar sentimento e extrair opiniões.
 

3.	Em Selecionar idioma do texto, selecione Inglês. Em Selecione seu recurso do Azure , selecione seu recurso.
 

4.	Em Digite seu próprio texto, carregue um arquivo ou use um de nossos textos de exemplo, copie e cole a seguinte revisão:
Hotel cansado com mau serviço
The Royal Hotel, Londres, Reino Unido
 5/6/2018 _ _ _ _
Este é um hotel antigo (existe desde 1950 ) e os móveis dos quartos são medianos - tornando-se um pouco antigos agora e precisam ser alterados. A internet não funcionava e tive que ir a uma das salas do escritório para fazer o check- in para o meu voo para casa. O site diz que fica perto do Museu Britânico, mas é muito longe para caminhar.
5.	Marque a caixa para confirmar que a demonstração incorrerá em uso e poderá gerar custos e selecione Executar.
 

6.	Revise a saída. Observe que o documento é analisado quanto ao sentimento, assim como cada frase. Selecione Frase 1 para mostrar a análise de sentimento dessa frase.
 

Observe que há um sentimento geral seguido por pontuações próximas a três categorias: pontuação positiva, pontuação neutra e pontuação negativa. Em cada uma das categorias é atribuída uma pontuação entre 0 e 1. Essas pontuações de confiança indicam a probabilidade do texto fornecido ser um sentimento específico.
 

Selecione a frase 1 novamente para fechar.
1.	Role para cima para selecionar Limpar caixa de texto e copie e cole a seguinte revisão:
Cópia de código
Bom hotel e funcionários
The Royal Hotel, Londres, Reino Unido
 02/03/2018 _ _ _ _
Quartos limpos, bom serviço, excelente localização perto do Palácio de Buckingham e da Abadia de Westminster, e assim por diante . Nós apreciamos completamente a nossa estadia. O pátio é muito tranquilo e fomos a um restaurante que faz parte do mesmo grupo e é indiano ( costa oeste com muitos peixes ) com uma estrela Michelin. Tivemos o menu de degustação que foi fabuloso. Os quartos eram muito bem decorados com cozinha, sala, quarto e banheiro enorme. Completamente recomendado .
2.	Selecione Executar. Revise o resultado e o sentimento e o nível de confiança.
3.	Selecione Limpar caixa de texto novamente e copie e cole a seguinte revisão:
Muito barulhento e os quartos são pequenos The Lombard Hotel, São Francisco, EUA 05/09/2018 O hotel está localizado na rua Lombard, que é uma rua muito movimentada de SEIS pistas, diretamente da Ponte Golden Gate. Tráfego desde o início da manhã até tarde da noite, especialmente nos finais de semana. O ruído não seria tão ruim se os quartos fossem melhor isolados, mas não são. Tive que colocar algodão nos ouvidos para conseguir dormir – estava cansado demais para aproveitar a cidade no dia seguinte. Os quartos são MINÚSCULOS. Escolhi o quarto porque tinha duas camas queen size – mas o quarto mal tinha espaço para acomodá-las. Com uma família de quatro pessoas na sala, era apertado. Com tudo isso dito, os quartos são limpos e eles fizeram um esforço para atualizá-los. O hotel fica no bairro de Marina, com muitos bons lugares para comer, a uma curta caminhada do Presidio. Pode ser um bom hotel para jovens adultos que ficam acordados até tarde com um orçamento limitado
4.	Selecione Executar e analise o sentimento juntamente com o nível de confiança. Dê uma olhada no texto e compare-o com a análise de sentimento que o serviço retornou.





## Excluir Grupo de Recursos 

Se não pretende fazer mais exercícios, exclua todos os recursos que não precisa mais. Esse evita acumulando qualquer desnecessário custos .

1. Acesse a página do portal e clique para abrir o menu lateral esquerdo:
<p align="center">
    <img  src="../imagens/01_41_Limpar_Menu.png" width="60%"/> 
    <br>
</p> 

2. Clique em "Resource Groups":
<p align="center">
    <img  src="../imagens/01_42_Limpar_Menu_Grupo.png" width="30%"/> 
    <br>
</p> 

3. Selecione o grupo que deseja deletar:
<p align="center">
    <img  src="../imagens/01_43_Limpar_Select_Grupo.png" width="100%"/> 
    <br>
</p> 

4. No ambiente do recurso referido, clique em "Delete resource group":
<p align="center">
    <img  src="../imagens/01_44_Limpar_Delete_Grupo.png" width="100%"/> 
    <br>
</p> 

5. Confirme as informações, informe o nome do recurso no campo abaixo e clique em delete:
<p align="center">
    <img  src="../imagens/01_45_Limpar_Modal.png" width="50%"/> 
    <br>
</p> 

6. Confirme a exclusão:

<p align="center">
    <img  src="../imagens/01_46_Limpar_Modal_Confirma.png" width="40%"/> 
    <br>
</p> 

Obs.: A exclusão pode demorar um pouco para acontecer. Aguarde um pouco e confira que o recurso foi excluído dando um refresh (F5) na página para que a lista de grupos de recursos seja atualizada.



## Não encontrou sua resposta aqui? Tente esses repositórios...

### Repos Auxiliares
- [giselle-ferreira](
https://github.com/giselle-ferreira/language-studio-microsoft-azure)
- [alexklenio](
https://github.com/alexklenio/DIO-Microsoft-Azure-AI-Fundamentals/tree/main/DP03%20-%20An%C3%A1lise%20de%20sentimentos)


## 📜 License

O projeto publicado em 2024 sobre a licença [MIT](./LICENSE) ❤️ 

Made with ❤️ by Shyoutarou

Gostou? Deixe uma estrelinha para ajudar o projeto ⭐


