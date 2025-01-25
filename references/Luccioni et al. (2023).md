---
created: 2025-01-22T18:26
updated: 2025-01-24T10:39
group: papers
title: "Stable Bias: Evaluating Societal Representations in Diffusion Models"
authors:
  - Alexandra Sasha Luccioni
  - Christopher Akiki
  - Margaret Mitchell
  - Yacine Jernite
publisher: Neural Information Processing Systems (NeurIPS) 2023 – Datasets and Benchmarks Track
year: 2023
journal: NeurIPS 2023 – Datasets and Benchmarks Track
institution:
  - Hugging Face, Canada
  - Leipzig University and ScaDS.AI
  - Hugging Face, USA
doi: https://doi.org/10.48550/arXiv.2303.11408
abstract: |
  O estudo avalia os vieses sociais embutidos em modelos de difusão para geração de imagens a partir de texto (*text-to-image*). A abordagem compara imagens geradas com variação em atributos de identidade, como gênero e etnia, e analisa a representatividade dos modelos Stable Diffusion v1.4, v2 e DALL·E 2. Os resultados indicam sub-representação de mulheres e minorias raciais, com implicações para equidade e transparência em IA.
tags:
  - Bias
  - in
  - AI
  - Text-to-Image
  - Models
  - Stable
  - Diffusion
  - DALL·E
  - Machine
  - Learning
  - Ethics
  - Representation
  - in
  - AI
link: https://openreview.net/pdf?id=qVXYU3F017
---


### **Métodos**

O estudo propõe uma abordagem para quantificar vieses sociais nos modelos de geração de imagens por difusão, analisando a variação das imagens geradas com base em atributos de identidade como gênero e etnia. O método segue os seguintes passos:

1. **Geração de Dataset**
    
    - Foram usados prompts padronizados no formato _"Photo portrait of a [X] [Y] at work"_, onde _X_ representa etnia e _Y_ representa gênero.
    - Foram utilizados 68 combinações de gênero (homem, mulher, não-binário, e neutro) e etnia (baseado no censo dos EUA).
    - Os modelos analisados foram:
        - **Stable Diffusion v1.4**
        - **Stable Diffusion v2**
        - **DALL·E 2**
    - Além disso, foi criada uma segunda base de dados com imagens geradas para 146 profissões, baseadas na classificação do Bureau of Labor Statistics (BLS) dos EUA.
2. **Análise dos Vieses nas Imagens**
    
    - Foram utilizadas **duas abordagens principais** para avaliação das imagens:
        1. **Análise baseada em texto**:
            - Uso de modelos de _Image Captioning_ e _Visual Question Answering (VQA)_ para gerar descrições das imagens.
            - Foram analisadas palavras-chave associadas a gênero e etnia.
        2. **Análise baseada em imagens**:
            - Uso de **técnicas de clustering** para agrupar imagens em espaços de representação multimodal, permitindo avaliar a distribuição de diferentes grupos.
            - Para isso, utilizaram embeddings extraídos pelo modelo BLIP VQA.
3. **Comparação com Dados Demográficos**
    
    - Os resultados foram comparados com as estatísticas de gênero e etnia para cada profissão segundo os dados do BLS.
    - Isso permitiu avaliar se os modelos reproduziam ou distorciam as proporções reais dessas categorias no mercado de trabalho.
4. **Exploração Interativa**
    
    - Foram desenvolvidas ferramentas para facilitar a análise interativa dos dados:
        - _Diffusion Bias Explorer_: compara as imagens geradas pelos diferentes modelos.
        - _Average Face Comparison Tool_: gera uma média visual das faces representadas em cada profissão.
        - _k-NN Explorer_: permite explorar imagens por similaridade visual.

### **Principais Resultados**

Os resultados mostram que os modelos apresentam vieses sistemáticos em suas representações de gênero e etnia. Algumas descobertas importantes:

1. **Sub-representação de Mulheres e Grupos Raciais Minoritários**
    
    - Em todos os modelos, a proporção de imagens de mulheres e de pessoas negras geradas para profissões específicas é menor do que os dados reais do mercado de trabalho.
    - O modelo **DALL·E 2** apresentou os maiores desvios, enquanto o **Stable Diffusion v1.4** teve os desvios menos acentuados.
2. **Diferenças entre Modelos**
    
    - O **Stable Diffusion v1.4** gerou distribuições mais próximas das estatísticas reais do BLS.
    - O **DALL·E 2** teve um viés maior, frequentemente gerando imagens majoritariamente masculinas e brancas.
    - O **Stable Diffusion v2** apresentou uma tendência intermediária entre os dois modelos anteriores.
3. **Profissões mais Afetadas por Viés de Gênero**
    
    - Algumas profissões que, segundo o BLS, possuem alta presença feminina (como enfermeiras e professores) foram sub-representadas nos modelos.
    - Profissões tradicionalmente masculinas (como CEO e engenheiro) tiveram representações ainda mais dominadas por imagens masculinas.
4. **Análises Quantitativas dos Vieses**
    
    - Cerca de **97,66% das legendas geradas por modelos de Image Captioning** continham marcadores de gênero, demonstrando que os modelos incorporam fortemente categorias sociais em suas representações.
    - A distribuição de gênero nas imagens geradas ficou **9% a 27% abaixo** dos valores reais do BLS, dependendo do modelo analisado.
5. **Distribuição Visual de Gênero e Etnia**
    
    - Usando a abordagem de _clustering_, foi possível identificar que imagens de **homens brancos** eram dominantes nas representações geradas.
    - Regiões associadas a **mulheres** e **pessoas negras** eram sistematicamente menos representadas, especialmente em profissões onde esses grupos são historicamente minoritários.

### **Conclusão e Implicações**

- O estudo evidencia que os modelos de geração de imagens baseados em difusão apresentam vieses que refletem e amplificam desigualdades sociais.
- Esses vieses podem ter impactos significativos quando os modelos são utilizados em contextos profissionais, artísticos e comerciais, contribuindo para a marginalização de grupos sub-representados.
- Os autores disponibilizaram ferramentas para permitir a auditoria de vieses em outros modelos de geração de imagens.

## **Implicações Práticas do Estudo**

### **1. Impacto na Indústria de Inteligência Artificial e Empresas de Tecnologia**

- **Melhoria na Transparência e Auditoria de Modelos**: Empresas que desenvolvem modelos de _text-to-image_ (TTI) podem usar a metodologia proposta para identificar e mitigar vieses em seus modelos antes de disponibilizá-los para o público.
- **Tomada de Decisão na Escolha de Modelos**: Empresas que utilizam modelos como _Stable Diffusion_ ou _DALL·E 2_ para gerar imagens comerciais podem usar a abordagem do estudo para escolher modelos menos enviesados ou aplicar técnicas de correção.
- **Evolução de Ferramentas de Controle de Viés**: A pesquisa reforça a necessidade de novas abordagens para reduzir a perpetuação de estereótipos e desigualdades na geração de imagens.

### **2. Impacto em Aplicações Comerciais e Criativas**

Os modelos de geração de imagens são amplamente utilizados em diversas aplicações, e os vieses descobertos podem ter impactos negativos nesses contextos:

- **Publicidade e Marketing**:
    
    - Se os modelos geram predominantemente imagens de homens brancos para certas profissões, isso pode reforçar estereótipos e afetar campanhas publicitárias que buscam representar a diversidade do público-alvo.
    - Empresas podem precisar ajustar manualmente as imagens geradas ou desenvolver estratégias para garantir maior representatividade.
- **Indústria de Entretenimento e Design Gráfico**:
    
    - Profissionais de criação podem depender desses modelos para gerar arte conceitual, ilustrações e conteúdo visual.
    - O viés nos modelos pode limitar a diversidade nas criações, reforçando uma visão de mundo homogênea e pouco representativa.
- **Educação e Mídia**:
    
    - Plataformas educacionais e veículos de comunicação que utilizam IA para criar conteúdo visual podem, sem querer, propagar representações estereotipadas de gênero e etnia.

### **3. Riscos para Inclusão e Representatividade**

- **Sub-representação de Grupos Marginalizados**:
    
    - O estudo mostrou que mulheres e pessoas negras são menos representadas nas imagens geradas, especialmente em profissões onde elas já são minoritárias.
    - Isso pode impactar a autoimagem e a percepção de oportunidades de carreira para pessoas pertencentes a esses grupos.
- **Amplificação de Discriminação e Estereótipos**:
    
    - Se os modelos continuam a reforçar estereótipos de gênero e raça (por exemplo, associando profissões de alta renda a homens brancos), podem contribuir para a normalização desses padrões na sociedade.

### **4. Implicações Reguladoras e Éticas**

- **Necessidade de Normas e Padrões para Modelos de IA**:
    
    - Reguladores podem usar essa pesquisa como base para estabelecer padrões de transparência e mitigação de viés para modelos de IA.
    - Ferramentas de auditoria baseadas na metodologia do estudo podem se tornar um requisito legal em setores como publicidade, contratação e educação.
- **Desafios na Regulação de Modelos de Código Aberto**:
    
    - Enquanto modelos fechados como o _DALL·E 2_ podem ser ajustados pelos desenvolvedores para reduzir viés, modelos abertos como _Stable Diffusion_ podem ser treinados ou ajustados por qualquer pessoa, tornando a mitigação de viés mais difícil.
    - Políticas públicas podem precisar considerar como balancear inovação e responsabilidade social no uso de modelos abertos.

### **5. Desenvolvimento de Novas Ferramentas e Métodos de Mitigação**

- **Adoção de Técnicas de Ajuste e Fine-Tuning**:
    
    - Empresas e pesquisadores podem desenvolver ajustes nos modelos para balancear melhor as representações de gênero e etnia.
    - Técnicas de _prompt engineering_ podem ser refinadas para melhorar a diversidade nas imagens geradas.
- **Ferramentas de Auditoria e Monitoramento**:
    
    - As ferramentas desenvolvidas no estudo, como _Diffusion Bias Explorer_ e _Average Face Comparison Tool_, podem ser usadas por desenvolvedores e reguladores para monitorar vieses em novos modelos de IA.



### **Viés Estável: Avaliando Representações Sociais em Modelos de Difusão**

Esta pesquisa foca na avaliação das representações sociais em sistemas de **Texto para Imagem (TTI)** para compreender e mitigar vieses em tecnologias de aprendizado de máquina. O estudo introduz um método inovador para analisar vieses nesses sistemas, examinando as variações nas imagens geradas com base em **gênero, marcadores étnicos e profissões**, permitindo a identificação de tendências específicas de viés e fornecendo escores comparativos de diversidade. Os resultados revelam que os principais sistemas de TTI apresentam correlações com a demografia do mercado de trabalho dos EUA, mas sub-representam consistentemente **identidades marginalizadas**, ressaltando a importância de abordar o viés em modelos de inteligência artificial para melhorar a inclusão social.

---

### **Introdução**

A introdução discute o avanço dos modelos baseados em difusão no **Aprendizado de Máquina (ML)**, principalmente na geração de imagens a partir de texto, destacando modelos como **Stable Diffusion, Make-a-Scene, Imagen e DALL·E 2**, que ganharam popularidade rapidamente. Os principais pontos abordados são:

- Modelos de difusão são inspirados em princípios da **termodinâmica fora de equilíbrio** e treinados para reduzir gradualmente o ruído em imagens.
- Sua **função de perda baseada em verossimilhança** torna o treinamento mais simples e os resultados mais diversos.
- A análise do **espaço latente** desses modelos é difícil devido ao seu treinamento iterativo.
- Modelos TTI incluem **múltiplas fases de processamento de texto e imagem**.
- Esses sistemas estão se tornando **onipresentes em várias aplicações**, podendo **perpetuar vieses sociais**.
- Há **pouca documentação detalhada** sobre os vieses nos sistemas TTI, dificultando sua auditoria.
- O artigo introduz ferramentas para **auditar vieses sociais**, comparando saídas de modelos baseadas em prompts específicos.
- A pesquisa compara os vieses sociais incorporados nos modelos **Stable Diffusion v1.4, v2 e DALL·E 2** em relação a diferentes profissões e palavras-chave de gênero/etnia.
- São fornecidas ferramentas para explorar outros sistemas TTI e analisar conjuntos de dados gerados para profissões.
- A conclusão aborda **as implicações da pesquisa e sugere direções futuras para investigações adicionais**.

---

### **Contextualização**

O viés em aprendizado de máquina (ML) envolve:

- Diferenças no desempenho do modelo para diferentes categorias;
- Propagação de estereótipos sociais;
- Representações problemáticas nos conjuntos de dados que influenciam as saídas do modelo e as percepções dos usuários.

Principais aspectos abordados:

- Estudos anteriores analisaram vieses em ML, com contribuições de diversas áreas, incluindo **ciências sociais, cognitivas, direito e políticas públicas**.
- O projeto se baseia nesses trabalhos para expandir os conhecimentos sobre viés em ML.
- Três dimensões principais são consideradas:
    1. **Diferença de desempenho dos modelos entre categorias sociais**;
    2. **Propagação de estereótipos**;
    3. **Problemas de representatividade em datasets usados para treinar os modelos**.

---

### **Avaliação de Viés em Modelos Multimodais**

A pesquisa explora vieses em modelos **multimodais**, que combinam **texto e imagem**. Os principais pontos são:

- **Desafios na compreensão do viés**: Estudos anteriores focaram separadamente em modelos de texto e imagem, mas o crescimento dos modelos multimodais superou o desenvolvimento de métodos para análise de viés.
- **Amplificação de viés**: Ainda não está claro se os vieses de diferentes modalidades se somam ou amplificam um ao outro.
- **Exemplo de viés composto**: Um modelo pode representar “pessoas” e “pessoas brancas” de maneira visualmente distinta, ao mesmo tempo que associa “pessoas” a termos positivos e “pessoas negras” a termos negativos.
- **Evidências de viés**: Pesquisas anteriores mostraram que modelos multimodais tendem a perpetuar **estereótipos sociais sobre raça, gênero e aparência**.
- **Exemplos práticos**:
    - Modelos de IA associam **mulheres a compras** e **homens a esportes radicais**.
    - Modelos geram descrições de menor qualidade para **pessoas de pele escura**.
    - Algoritmos de busca de imagens reforçam vieses ao mostrar **mais imagens de homens brancos** para profissões prestigiadas.

---

### **Sistemas Texto-para-Imagem e seus Vieses**

Os sistemas TTI se tornaram populares, motivando pesquisas sobre:

- Filtros de segurança e seu funcionamento;
- Estrutura semântica dos modelos;
- Geração de **representações estereotipadas** de diferentes grupos demográficos;
- Memorização e reprodução de exemplos específicos do conjunto de treinamento.

Algumas das principais descobertas incluem:

- Modelos como **CLIP**, que orientam a difusão, já codificam **vieses raciais e culturais**.
- Dados de treinamento são retirados da internet e **contêm conteúdo problemático, como pornografia e informações incorretas**.
- Aplicação de **filtros de segurança** pode **exacerbar vieses**, como foi observado no DALL·E 2.

---

### **Metodologia: Auditoria de Vieses Sociais em Sistemas TTI**

Os pesquisadores propõem uma nova abordagem para medir vieses nos modelos TTI. Os passos são:

1. **Definir características de identidade**: O estudo foca em **gênero e etnia**.
2. **Gerar imagens com variações nesses atributos**: Utilizam prompts padronizados como:
    - _"Retrato fotográfico de um [etnia] [gênero] no trabalho."_
3. **Criar conjuntos de dados**:
    - **Dataset de identidades**: 68 combinações de etnia e gênero.
    - **Dataset de profissões**: 146 profissões baseadas no Bureau of Labor Statistics (BLS).
4. **Analisar as imagens geradas**:
    - **Análise baseada em texto** (usando modelos de _Visual Question Answering_ e _Image Captioning_).
    - **Análise baseada em imagens** (técnicas de _clustering_ para agrupar imagens com características similares).

---

### **Principais Resultados**

1. **Sub-representação de mulheres e grupos raciais marginalizados**:
    
    - Todos os modelos analisados geraram **menos imagens de mulheres e pessoas negras** do que os dados reais do mercado de trabalho.
    - O **DALL·E 2** apresentou o maior viés, enquanto o **Stable Diffusion v1.4** foi o mais balanceado.
2. **Discrepâncias nas profissões**:
    
    - Algumas profissões com alta presença feminina no mercado de trabalho, como **enfermeiras e professoras**, foram **sub-representadas** nos modelos.
    - Profissões como **CEO e engenheiro** apresentaram uma **proporção ainda maior de homens brancos** do que os dados reais indicam.
3. **Impacto dos filtros de segurança**:
    
    - A tentativa de **remover conteúdos explícitos** do treinamento do DALL·E 2 **ampliou desigualdades de representação**, reduzindo a presença de **mulheres e grupos raciais minoritários**.

---

### **Conclusões e Implicações Práticas**

- **Regulamentação e transparência**: As empresas devem desenvolver estratégias para auditar e reduzir vieses em IA.
- **Impacto em publicidade e mídia**: Modelos enviesados podem reforçar **estereótipos de gênero e raça**.
- **Evolução de ferramentas de IA**: Novas técnicas devem ser desenvolvidas para tornar os modelos mais representativos.
- **Padrões éticos**: O estudo destaca a necessidade de diretrizes para que a IA seja mais **justa e inclusiva**.

