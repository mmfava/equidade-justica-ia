---
theme: slides-left
author: Marília Melo Favalesso
_header: ""
header: 🐍 82º Python Floripa
_footer: ""
_paginate: false
footer: Marília Melo Favalesso
paginate: true
center: teste
date: ""
link: 
created: 2025-01-20T23:39
updated: 2025-01-25T00:10
---

<!-- _class: first-slide -->

<small>🐍 82º Python Floripa</small>

# Equidade e Justiça em<br>Sistemas de IA

**Marília Melo Favalesso**

---
## Marília Melo Favalesso  

🧠 Cientista de Dados | PhD

🐍 Python e Comunidades  

🐈 Gatos, pizza e bicicleta nas horas vagas

🔗 LinkedIn: [/mariliafavalesso](https://www.linkedin.com/in/mariliafavalesso/)

🔗 github: [/mmfava](https://github.com/mmfava)

---
# <!----fit-->O que estamos chamando de IA 

A **Inteligência Artificial (IA)** é um termo abrangente que se refere a sistemas automatizados de tomada de decisão, capazes de executar tarefas que tradicionalmente exigiriam inteligência humana.


---

# O impacto das<br>==decisões algorítmicas==

Embora aspirem imitar e automatizar o julgamento humano, a maioria dos algoritmos de IA são, na verdade, **modelos imperfeitos suscetíveis a erros e vieses**.


---

## Proposta de experimento

▶ Execute o seguinte prompt no chatGPT / DALL-E 3: 

**"Chat, pode gerar a imagem de uma pessoa liderança?"**<br>

<br> 🤔 Qual foi o resultado? 


---

<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 10px;
  }
  .grid-container img {
    width: 100%;
    height: auto;
  }
</style>

<div class="grid-container">
  <img src="figs/e1.png">
  <img src="figs/e2.png">
  <img src="figs/e3.png">
  <img src="figs/e4.png">
  <img src="figs/e5.png">
  <img src="figs/e6.png">
  <img src="figs/e7.png">
  <img src="figs/e8.png">
  <img src="figs/e9.png">
  <img src="figs/e10.png">
</div>

<br>

<small><small>DALL-E 3 (OpenAI) →🔗 https://chatgpt.com/share/67915ff0-4c64-800e-b74e-176c169d355f</small></small>

---

## Proposta de experimento 2

▶  Adicione ao prompt no chatGPT / DALL-E 3 a palavra "compassiva": 

**"Chat, pode gerar a imagem de uma pessoa liderança compassiva?"**

<br>🤔 Qual foi o resultado? 

---
<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 10px;
  }
  .grid-container img {
    width: 100%;
    height: auto;
  }
</style>

<div class="grid-container">
  <img src="figs/e2.1.png">
  <img src="figs/e2.2.png">
  <img src="figs/e2.3.png">
  <img src="figs/e2.4.png">
  <img src="figs/e2.5.png">
  <img src="figs/e2.6.png">
  <img src="figs/e2.7.png">
  <img src="figs/e2.8.png">
  <img src="figs/e2.9.png">
  <img src="figs/e2.10.png">
</div>

<br>

<small><small>DALL-E 3 (OpenAI) →🔗 https://chatgpt.com/share/6792b433-02b0-800e-8352-052e2fb2f531</small></small>

---
### Reflexo da realidade?
<br>


==NÃO!== Os modelos são **enviesados**.


✶ Reforçam e amplificam estereótipos existentes.
✶ Sub ou sobre-representam certos grupos.
✶ Podem levar a discriminações sistêmicas.

<br><small><small>**Ver:** Cheong et al. (2024), Currie et al. (2024), Mandal et al. (2024), Wu et al. (2024), Choudhry et al. (2023) e  Luccioni et al. (2023). </small></small>

<!---- 

Viés em Inteligência Artificial (IA) refere-se a padrões sistemáticos de erro em modelos de aprendizado de máquina que levam a previsões ou decisões injustas, distorcidas ou discriminatórias.

-->


---

#### Case 1: IA gerando imagens racistas

![bg right width:900px](figs/vereadora-discriminacao-ia.png)

<small><small><small>**G1 (26/10/2023)** - Deputada denuncia IA por gerar imagem racista quando solicitado um personagem negro em uma favela. (🔗[link](https://g1.globo.com/tecnologia/noticia/2023/10/26/deputada-do-rj-diz-que-robo-que-faz-desenhos-ao-estilo-pixar-entregou-imagem-de-mulher-negra-com-arma-na-mao-ao-receber-pedido-de-personagem-em-favela.ghtml)).</small></small></small>
<br>

<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Prompt no <em>Bing Chat</em> da Microsoft (DALL-E):</strong><br>
"Uma mulher negra, de cabelos afro, com roupas de estampa africana num cenário de favela".
</div>


---
#### Case 2: IA associando raça a crime

![bg left width:700px](figs/Imagem%20do%20WhatsApp%20de%202025-01-24%20à(s)%2012.33.08_f345ba01.jpg)

<small><small><small>**Grupo LLM whatsapp (28/10/2024)** - IA da Meta gera imagem de um homem negro ao pedido de "pessoa que efetua atos errados na sociedade". </small></small></small>
<br>

<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Prompt no <em>Meta AI</em> do Whatsapp:</strong><br>
"@Meta AI crie a imagem de uma pessoa que efetua atos errados na sociedade".
</div>

---
#### Case 3: IA associando raça a reincidência criminal

<small><small><small><mark>Old News!</mark><br>**ProPublica (23/05/2016)**: O artigo revela que o algoritmo COMPAS, usado no sistema judicial dos EUA para prever reincidência criminal, tem viés racial: ele superestima o risco de reincidência para pessoas negras (mais falsos positivos) e subestima para pessoas brancas (mais falsos negativos) ([🔗 link](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)).</small></small></small>
<br>

![bg right width:900px](figs/alto-risco-rei-crime.png)

---
### Reflexo da sociedade?

==SIM!== 🏘️ ⇢ 👶

As IA apresentam "**posicionalidade**"!

✶ Posicionalidade é a forma como nossos **contextos sociais e políticos moldam nossa percepção do mundo**.

✶ Na IA, isso significa que **preconceitos e perspectivas humanas influenciam os sistemas de aprendizado de máquina**, pois refletem as escolhas feitas durante seu desenvolvimento.

---

![center width:1500px](figs/inequality-discrimination-covid.png)

<center><small><small><b>Ref:</b> Leslie et al. (2021)</small></small></center>

---
#### A IA amplifica vieses humanos

<small><small><b>Glickman and Sharot (2024)</b></small></small>
* IA reforça viés e influencia humanos a adotá-lo.
* Maior viés em interações humano-IA do que humano-humano.
* Percepção da IA como neutra favorece aceitação de vieses.
* IA imparciais podem melhorar julgamentos humanos.
![bg right width:900px](figs/muda-crenca.png)


---
# Mas o que é ser <u>justo</u>?

▶ **Responda:** 

Há apenas um leito disponível na UTI e dois pacientes em estado grave:

[1] 🧒 **Criança de 8 anos** - alta chance de recuperação.
[2] 🤰 **Mulher grávida de 32 anos** - sua vida não garante a do bebê.

<br>==Quem deve receber o leito?==

---
# Mas o que é ser <u>justo</u>?

▶ **Responda:** 

Há apenas um leito disponível na UTI e dois pacientes em estado grave:

[1] 🧔‍♂️ **Homem de 40 anos** - baixa probabilidade de sobrevivência.
[2] 👵 **Mulher idosa de 75 anos** - probabilidade relativamente alta de sobrevivência.

<br>==Quem deve receber o leito?==

---
## Definição de justiça 👩‍⚖️

#### Complexa!

▶ A noção de justiça **varia entre culturas e contextos**, refletindo valores e normas sociais.

▶ Em IA, é a busca por sistemas ==equitativos==, livres de discriminação ou vieses injustos.


---
# Equidade ≠ Igualdade


A equidade considera **diferenças individuais e estruturais**, garantindo que **todos tenham acesso às mesmas oportunidades**, mesmo que isso signifique **tratamentos diferenciados**.

#### Conceito bastante discutido, mas que também não é fácil

---

# Construindo um sistema justo

_"Viés algorítmico não é um problema meramente técnico, mas social e ético. Para mitigá-lo, devemos agir desde a coleta de dados até a governança do sistema."_

— **Cathy O’Neil**, autora de _Weapons of Math Destruction_

---
### 1️⃣ Propósito

IA deve ter um **objetivo claro** e ser a melhor solução para o problema. Sem um propósito bem definido, pode gerar impactos negativos e desperdício de recursos.

![bg right](figs/surto-ebola.png)

<br>
<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Surto do Ebola (2014) - </strong>
Pesquisadores usaram dados de mobilidade para prever surtos, mas o Ebola se espalha por contato direto. O foco deveria ter sido <b>redes de contato entre infectados</b>.
</div>


---

### 2️⃣ Dados

Dados enviesados reforçam desigualdades. **É necessário garantir a diversidade com qualidade**. Auditorias e engajamento de especialistas são consideradas boas práticas!

<br>
<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Liang et al. (2023) - </strong>Detectores de GPT estão enviesados contra "escritores" não-nativos do inglês.</b>
</div>

![bg right](figs/bias-writinh.png)

---

### 3️⃣ Abusabilidade

Os desenvolvedores de IA precisam antecipar **vulnerabilidades e cenários de uso indevido**. 

Algoritmos podem ser **sequestrados e transformados em ferramentas para fins maliciosos**, como manipulação, vigilância e desinformação.

<br>
<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Poder 360 (24/01/2024) - </strong>Deep Fake do Papa Francisco usando casaco da moda e divulgado por grandes veículos de mídia como verdade.  
<a href="https://www.poder360.com.br/internacional/alvo-de-deepfake-papa-pede-regulamentacao-de-ia/" target="_blank">[Link]</a>
</div>


![bg right](figs/papa-ai.png)

---
### 4️⃣ Privacidade

Os sistemas de IA podem comprometer a **privacidade** dos usuários ao armazenar dados sensíveis, sujeitos a vazamentos e ataques. 

Para mitigar riscos, é essencial aplicar **segurança desde o design** e garantir o **controle do usuário** sobre seus dados.

<br>
<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Época Negócios (16/01/2025) - </strong>Brasileiros vendem registro da íris por R$600 para projeto Worldcoin de Sam Altam, CEO da OpenAI
<a href="https://epocanegocios.globo.com/tecnologia/noticia/2025/01/brasileiros-vendem-registro-de-iris-por-r-600-entenda-como-funciona-o-processo-e-quais-os-riscos.ghtml" target="_blank">[Link]</a>
</div>

![bg right](figs/iris.png)

---

### 5️⃣ Proxy

Algoritmos podem discriminar **indiretamente** ao usar variáveis correlacionadas a **atributos protegidos**, como raça ou gênero.

É de extrema importância a consulta a especialistas no assunto! <br>

<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;"> <strong>Ribeiro-Dantas et al. (2023) - </strong> O estado civil solteira foi indevidamente apontado como fator de risco para um tipo de câncer de mama. Os autores demonstram que a variável é um proxy de fatores socioeconômicos, como acesso ao diagnóstico médico adequado. </div>

![bg right](figs/cancer-mama.png)

---
### 6️⃣ Explicabilidade

Quem projeta e implementa sistemas algorítmicos tem a **responsabilidade de explicar decisões críticas** que impactam o bem-estar das pessoas.

<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;"> O usuário quer entender o motivo dos resultados, o motivo das falhas e quando e o quanto ele pode confiar na IA!</div>

![bg right](figs/black-box.png)

---

#### Interpretabilidade

Refere-se à capacidade de entender como um modelo de IA funciona e chega às suas conclusões.<br>
**Um modelo interpretável permite rastrear o impacto de cada entrada na saída.**
<br><small><small>[🔗 Link da figura](https://docs.aws.amazon.com/whitepapers/latest/model-explainability-aws-ai-ml/interpretability-versus-explainability.html)</small></small>

![bg left width:1000px](figs/interpretabilidade.png)


---
#### Explicabilidade

Conjunto de processos e métodos que permite que usuários humanos **compreendam e confiem nos resultados e saídas** criados por algoritmos de aprendizado de máquina.
<br><small><small>[🔗 Link da figura](https://media.geeksforgeeks.org/wp-content/uploads/20231201153509/Explainable-AI-Concept-1-660.png)</small></small>

![bg left width:900px](figs/shap-local-global.png)


---

### 7️⃣ Otimização

Definir métricas de sucesso para IA envolve **compensações e impactos colaterais**. É essencial equilibrar **desempenho e equidade**, minimizando riscos para populações vulneráveis.

<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;"> <strong>Shanklin et al. (2022) </strong> - O estudo mostra como algoritmos de IA podem perpetuar desigualdades raciais e propõe um método para equilibrar precisão e equidade, evitando discriminação sem comprometer a eficiência. </div>

![bg right](figs/apontamento-medico.png)

---

### 8️⃣ Generalização

Entre o desenvolvimento e a implementação de um sistema de IA, **o mundo – e os usuários – podem mudar**, tornando o contexto original inadequado e levando a falhas inesperadas.  

Planos de retreino e descontinuidade são necessários! 

![bg right](figs/blink.png)  

<br>  
<div style="border: 1px solid #ccc; padding: 20px; padding-left:60px; font-size: 0.7em; background-color: #f8f8f8;">
<strong>Time (22/01/2010) - </strong> Câmeras da Nikon não reconheciam corretamente rostos asiáticos, exibindo a mensagem "Alguém piscou?" mesmo com os olhos abertos.  
<a href="https://time.com/archive/6906847/are-face-detection-cameras-racist/" target="_blank">[Leia mais]</a>  
</div>  

---

### 9️⃣ Monitoramento

Decisões algorítmicas devem ser **passíveis de revisão**, garantindo que indivíduos possam **questioná-las e corrigi-las**. 

Além disso, **monitoramento contínuo e transparência** são essenciais para evitar abusos e garantir responsabilidade no uso da IA.

![bg right](figs/monitorament.png)


---
**Reflexões finais**

# A IA ==não é neutra== – ela reflete as escolhas de quem a constrói e os dados que a alimentam!

---
**Reflexões finais**

#  Viés algorítmico não é apenas um problema técnico,<br>mas ==social e ético==. 

A mitigação exige um olhar interdisciplinar.

---
**Reflexões finais**

# Precisamos equilibrar ==acurácia e equidade==, garantindo que sistemas de IA sejam justos e transparentes.

---
**Reflexões finais**

# A supervisão contínua e o direito à contestação são fundamentais para que a IA beneficie a sociedade sem reforçar desigualdades!


---

### Referências

1. Cheong, M. et al. (2024). _Investigating Gender and Racial Biases in DALL-E Mini Images_. [Online]. Available at: https://doi.org/10.1145/3649883 [Accessed 24 January 2025].
2. Choudhry, H. S. et al. (2023). _Perception of Race and Sex Diversity in Ophthalmology by Artificial Intelligence: A DALL E-2 Study_. [Online]. Available at: https://doi.org/10.2147/OPTH.S427296 [Accessed 24 January 2025].
3. Currie, G. et al. (2024). _Gender and Ethnicity Bias of Text-to-Image Generative Artificial Intelligence in Medical Imaging, Part 2: Analysis of DALL-E 3_. [Online]. Available at: https://doi.org/10.2967/jnmt.124.268359 [Accessed 24 January 2025].
4. Glickman, M. and Sharot, T. (2024). _How human–AI feedback loops alter human perceptual, emotional and social judgements_. [Online]. Available at: https://www.nature.com/articles/s41562-024-02077-2 [Accessed 24 January 2025].
5.  Leslie, D. et al. (2021). _Does “AI” stand for augmenting inequality in the era of covid-19 healthcare?_ [Online]. Available at: https://doi.org/10.1136/bmj.n304 [Accessed 24 January 2025].
6. Liang, W. et al. (2023). _GPT detectors are biased against non-native English writers_. [Online]. Available at: https://doi.org/10.48550/arXiv.2304.02819 [Accessed 24 January 2025].


---

### Referências
7. Luccioni, A. S. et al. (2023). _Stable Bias: Analyzing Societal Representations in Diffusion Models_. [Online]. Available at: https://doi.org/10.48550/arXiv.2303.11408 [Accessed 22 January 2025].
8. Mandal, A., Leavy, S. and Little, S. (2024). _Generated Bias: Auditing Internal Bias Dynamics of Text-To-Image Generative Models_. [Online]. Available at: https://doi.org/10.48550/arXiv.2410.07884 [Accessed 24 January 2025].
9. Ribeiro-Dantas, M. da C. et al. (2023). _Learning interpretable causal networks from very large datasets, application to 400,000 medical records of breast cancer patients_. [Online]. Available at: https://doi.org/10.48550/arXiv.2303.06423 [Accessed 24 January 2025].
10. Shanklin, R. et al. (2022). _Ethical Redress of Racial Inequities in AI: Lessons from Decoupling Machine Learning from Optimization in Medical Appointment Scheduling_. [Online]. Available at: https://doi.org/10.1007/s13347-022-00590-8 [Accessed 24 January 2025].
11. Wu, Y., Nakashima, Y. and Garcia, N. (2024). _Gender Bias Evaluation in Text-to-image Generation: A Survey_. [Online]. Available at: https://doi.org/10.48550/arXiv.2408.11358 [Accessed 24 January 2025].


---
<!-- Texto Principal -->
<div class="texto-principal">Obrigada!</div>

<!-- Linha Divisória -->
<div class="linha"></div>
<div class="contato">
  <b>Marília Melo Favalesso - PhD, Cientista de Dados<b>
</div>

<!-- Redes Sociais -->
<div class="redes-sociais">
  <a href="https://www.linkedin.com/in/seuusuario" target="_blank">🔗 LinkedIn: /mariliafavalesso</a>
  <a href="mailto:seuemail@example.com">✉️ Email: marilia.melo.favalesso@gmail.com</a>
</div>

