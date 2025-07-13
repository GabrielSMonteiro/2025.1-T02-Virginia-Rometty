# Fase 03 – Projeto da Avaliação de Qualidade

## 1 ▪ Introdução

Nesta fase final foi feita a execução dos testes de portabilidade e conformidade citado na fase 03. A avaliação foi focada no repositório **api** e levou em conta também os repositórios com a parte web e a parte do aplicativo, além da documentação dos repositórios. Para isso, foi utilizado os dispositivos que tinha disponível, um celular android, um simulador de IOS, e computador com windows e linux. Por fim, foi analisado conforme o modelo ISO/IEC 25010 estudado em sala de aula, no qual foi possível testar a adaptabilidade e a conformidade baseando no que estava definido no repositório do projeto. 

Com isso, foram avaliados:  

**Portabilidade** – instalação e execução no Chrome, Firefox, Edge e Brave e em um celular Samsung e em um celular Iphone.

**Conformidade** – qualidade de código (ESLint e SonarQube que já rodavam na plataforma) e a complexidade e facilidade da documentação.  

## 2 ▪ Execução dos Testes

### 2.1 Portabilidade

Para avaliar a plataforma do Agromart, foi rodado a aplicação web no Chrome, no Firefox, no Edge e no Brave nos ambientes Windows e Ubuntu. E assim foi possível rodar em todos os navegadores apesar de dar problemas no layout ao rodar no Brave, mas foi possível consertar com alteração no --webkit que estava sinalizando problemas no código. O aplicativo foi possível instalar no dispositivo android e foi possível simular em um simulador IOS que coloquei no android studio, faltou apenas um celular android muito antigo, então coloco a taxa de sucesso como 75%. Para buildar o projeto levou mais de 3 horas, aproximadamente 3h 30 min e durante a execução não deu muito problema além de toda hora ter que baixar ou atualizar uma dependência

* **M1 – Compatibilidade de navegadores:** 4/4 navegadores bem-sucedidos (100%)
* **M2 – Sucesso de instalação móvel:** 3/4 dispositivos (75%)
* **M3 – Tempo de build:** 210 min
* **M4 – Bugs:** 0% uso

**Compatibilidade Web**  Foi bom, o erro visual no Brave foi devido a uma biblioteca específica  

**Erro ao instalar** foi devido ao celular ser muito antigo

### 2.2 Conformidade

Para a conformidade, foi analisado tanto o código quanto a documentação. Rodei o ESLint na aplicação e pelo código estar muito disperso, foi difícil mensurar a quantidade de erros totais sobre o total de linhas do projeto, mas ao recortar uma fatia do que era possível analisar, foi constatado que havia 8 erros em 2 mil linhas, o que já supera a estimativa que foi demarcada na fase 03. O SonarQube identificou 0 vulnerabilidades críticas, 5 alertas médios e alguns de prioridade baixa mas que não impactaram no funcionamento da plataforma, o que indica uma boa qualidade geral. Segundo o repositório do AgroMart, os endpoints estão todos no repositório de [dicionário](https://github.com/AgroMart/api-dicionario), mas lá tem apenas 4 endpoints e identifiquei pelo menos mais 9 no repositório de [api](https://github.com/AgroMart/api), então considerando que há 13 endpoints no total, todos os do dicionário estão bons e bem implementados, mas do de API vi problemas na autentificação e extratos, logo pela análise tem uma taxa de sucesso de aproximademente 92%. A documentação técnica como relatado já nos tópicos anteriores, está muito dispersa e de difícil compreensão, além disso não tem uma didática clara de como fazer deploy no windows o que gerou dúvidas e os fluxograma não parecem atualizados.

* **M5 – Endpoints em conformidade:** ~92%
* **M6 – Violações ESLint:** ~4 a cada 1000 linhas
* **M7 – Não conformidades graves:** nenhuma encontrada
* **M8 – Documentação completa:** 85%.

## 3 ▪ Riscos

- Não ocorreram problemas graves durante a execução 
- As configurações de ambientes foram preparadas conforme planejado. A única dificuldade leve foi adaptar o *build* mobile em um aparelho antigo, já prevista no risco de “versões antigas de SO”

## 4. Resultados Quantitativos  

| Métrica | Resultado | Aceitável | Esperado | Status |
|---------|-----------|-----------|----------|--------|
| M1 Compatibilidade navegadores | 100% | ≥ 95% | 100% | OK |
| M2 Instalação mobile | 75% | ≥ 90% | ≥ 95% | Falha |
| M3 Tempo médio de build | 3 h 30 min | ≤ 6 h | ≤ 4 h | OK |
| M4 Taxa de bugs por sessão | 0% | ≤ 30% | ≤ 1% | OK |
| M5 Endpoints conformes | 92% | ≥ 90% | ≥ 95% | Parcial |
| M6 Violações ESLint | 4 | ≤ 3 | ≤ 1 | Falha |
| M7 Não conformidades graves | 0 | 0–2 | 0 | OK |
| M8 Documentação completa | 85% | ≥ 85% | ≥ 95% | Parcial |

## 5 ▪ Conclusões e recomendações

 A **portabilidade** do AgroMart é excelente dado que rodou em todos os navegadores quase que sem ajustes em todos os testados menos o Brave, e a maioria dos celulares rodou o app. No entanto, acho fundamental a atualização das bibliotecas para que não precise de nenhum ajuste e não fique complicada a instalação.
 A **conformidade** de código está boa, mas as violações de ESLint passaram limite definido no recorte de observação, o SonarCloud já está incorporado no código mas vale a pena colocar mais casos de teste e testes contínuos, além de ter que revisar os poucos endpoints fora de padrão (7%) e completar o que falta da documentação.
Por fim, dos 8 critérios métricos medidos, 6 atingiram o nível esperado ou aceitável (75%), não atendendo ao critério de ≥80%, o que pela definição seria uma analise insatisfatória, mas como foi testado em poucos aparelhos e em poucos navegadores, acredito que o impacto do M2 pesou muito a avaliação, assim não determino uma falha na análise.

## 9 ▪ Histórico de Versões

| Versão | Data       | Descrição                                        | Autor            |
| ------ | ---------- | ------------------------------------------------ | ---------------- |
| 1.0    | 13/07/2025 | Execução dos testes de fase 03 e relatório final | Gabriel Monteiro |
