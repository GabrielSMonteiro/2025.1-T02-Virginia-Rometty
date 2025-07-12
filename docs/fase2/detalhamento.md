# Fase de definição dos objetivos

## 1. O que o Agromart pode fazer

### 1.1 Funcionalidades principais observadas

- Gerenciar conta
- Acesso às lojas e produtos
- Gerenciar endereços de entrega
- Acesso ao suporte e contato com agricultores
- Visualizar e alterar carrinho de compras

**Funcionalidades importantes para a avaliação:**

1. **Compras:** Adicionar ao carrinho e fazer as compras
2. **Comunicação:** Sistema de notificações
4. **Autenticação:** Sistema de login

### 1.2 Tipos de usuários

- **Agricultores** 
- **Consumidores** 
- **Administradores** 

### 1.3 Ambientes

- **Dispositivos:** Celulares e computadores
- **Navegadores:** Chrome, Firefox, Brave e Edge
- **Conectividade:** Funcionamento em diferentes condições de rede
- **Contexto:** Regiões com acesso tecnológico limitado

## 2. Critérios de Avaliação Específicos

### 2.1 Portabilidade - Subcaracterísticas (ISO/IEC 25010)

**Adaptabilidade:**

- Capacidade de adaptação a diferentes sistemas operacionais
- Facilidade de personalizar para diferentes CSAs

**Instalabilidade:**

- Facilidade de instalar o aplicativo
- Facilidade de fazer o deploy do modelo web
- Documentação clara

### 2.2 Conformidade

**Padrões de Código:**

- Estar conforme as boas práticas do JavaScript/React
- Uso do ESLint para padronização e detecção de problemas
- Aplicação de boas práticas de desenvolvimento

**Padrões de API:**

- Documentação adequada
- Versionamento apropriado de APIs

**Padrões de Acessibilidade:**

- Conformidade com as ISOs
- Usabilidade para pessoas com deficiência
- Compatibilidade com tecnologias assistivas

## 3. Objetivo do AgroMart

A ideia fundamental do Agromart é facilitar o comércio de produtos agroecológicos, conectando os pequenos agricultores familiares aos consumidores por meio de uma plataforma de fácil uso e com bastante eficiência, considerando pessoas com baixa familiaridade tecnológica e que, em seu contexto inicial de pandemia, precisavam manter um distanciamento social.

## 3.1 Objetivo de medição de Portabilidade

**Analisar:** o sistema AgroMart   
**Para o propósito de:** avaliar a capacidade de instalar, executar e manter a plataforma em diferentes ambientes tecnológicos  
**Com respeito a:** adaptabilidade e instalabilidade entre diferentes ambientes  
**Do ponto de vista de:** desenvolvedores e usuários finais  
**No contexto de:** sistemas operacionais móveis (iOS e Android) e navegadores web (Chrome, Firefox, Edge e Brave)

### 3.1.1 Questões do do objetivo da medição de Portabilidade

- **Q1:** A plataforma web funciona corretamente em todos os navegadores principais?  
  **Hipótese Q1:** A plataforma na web funciona em 100% dos navegadores testados (Chrome, Firefox, Edge, Brave)

- **Q2:** É possível instalar e executar o aplicativo móvel em diferentes dispositivos?  
  **Hipótese Q2:** É possível instalar em 90% dos dispositivos móveis testados (iOS e Android)

- **Q3:** Qual é o tempo necessário para adaptar a plataforma para uma nova arquitetura ou ambiente?  
  **Hipótese Q3:** O tempo médio de build para uma nova plataforma não excede 6 horas

- **Q4:** A plataforma apresenta estabilidade consistente entre diferentes ambientes?  
  **Hipótese Q4:** Taxa de bugs da plataforma ≤ 30% por  uso

## 3.2 Objetivo de da medição de Conformidade

**Analisar:** a arquitetura de software do AgroMart
**Para o propósito de:** verificar a conformidade da qualidade de acordo com ISO/IEC 25010
**Com respeito a:** conformidade funcional e da documentação 
**Do ponto de vista de:** desenvolvedores e da ISO/IEC 25010  
**No contexto de:** mudanças das normas e atualizações das bibliotecas React/Strapi

### 3.2.1 Questões do objetivo de Conformidade

- **Q1:** Os endpoints da API estão em conformidade com os padrões REST e documentação OpenAPI?  
  **Hipótese Q1:** ≥ 90% dos endpoints estão em conformidade com os padrões estabelecidos

- **Q2:** O código-fonte atende aos padrões de qualidade definidos pelo ESLint?  
  **Hipótese Q2:** Violação do ESLint ≤ 3 por mil linhas de código

- **Q3:** A plataforma atende aos requisitos básicos de acessibilidade e usabilidade?  
  **Hipótese Q3:** Nenhuma não conformidade grave de acessibilidade é identificada em auditorias

- **Q4:** A documentação técnica está completa e atualizada conforme os padrões?  
  **Hipótese Q4:** ≥ 85% da documentação técnica está completa e atualizada

## Relação entre Objetivos de Medição, Questões e Métricas

### Objetivo de Medição 1 – Portabilidade

| Questão | Métrica |
|---------|---------|
| Q1: A plataforma web funciona corretamente em todos os navegadores principais? | M1: Taxa de compatibilidade com navegadores (%) |
| Q2: É possível instalar e executar o aplicativo móvel em diferentes dispositivos? | M2: Taxa de sucesso de instalação em dispositivos móveis (%) |
| Q3: Qual é o tempo necessário para adaptar a plataforma para uma nova arquitetura? | M3: Tempo médio de build para nova plataforma (horas) |
| Q4: A plataforma apresenta estabilidade consistente entre diferentes ambientes? | M4: Taxa de crashes específicos de plataforma (%) |

### Objetivo de Medição 2 - Conformidade

| Questão | Métrica |
|---------|---------|
| Q1: Os endpoints da API estão em conformidade com os padrões REST e documentação OpenAPI? | M1: Percentual de endpoints em conformidade (%) |
| Q2: O código-fonte atende aos padrões de qualidade definidos pelo ESLint? | M2: Número de violações ESLint por mil linhas de código |
| Q3: A plataforma atende aos requisitos básicos de acessibilidade e usabilidade? | M3: Número de não conformidades graves de acessibilidade |
| Q4: A documentação técnica está completa e atualizada conforme os padrões? | M4: Percentual de completude da documentação técnica (%) |

## Bibliografia

- **ISO/IEC 25010:2011.** *Systems and Software Engineering — Systems and Software Quality Requirements and Evaluation (SQuaRE) — System and Software Quality Models*. International Organization for Standardization, 2011.

## 📝 Histórico de Versões

| Versão | Data | Descrição | Autor(es) |
| ------ | ---- | --------- | --------- |
| 1.0    | 12/07/2025 | Criação documento da fase 01 | [Gabriel Monteiro](https://github.com/GabrielSMonteiro) 