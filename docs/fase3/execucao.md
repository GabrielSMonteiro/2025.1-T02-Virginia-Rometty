# Fase 3 – Projeto da Avaliação de Qualidade  
### Focos: Portabilidade & Conformidade da Plataforma **AgroMart**

## 1 ▪ Introdução

Nessa fase, será documentado todo o trabalho de execução da avaliação do projeto, incluindo a análise de requisitos, a implementação da avaliação e a coleta de dados, no qual ao seu final , será possível identificar os pontos de melhoria para a plataforma **AgroMart**, o que será melhor documentado e apresentado na fase 04, no qual irei abordar a conclusão sobre os resultados obtidos.

<br>
**Com essa execução, será abordado:**

- Os procedimentos do teste e quais instrumentos e métodos foram usados para a coleta de dados
- O cronograma de execução
- Os recursos utilizados
- Os critérios de aceitação e os resultados obtidos

## 2 ▪ Escopo da avaliação

| Característica | Sub-característica ISO/IEC 25010 | Prioridade | Unidades de análise |
|----------------|----------------------------------|-----------|----------------------|
| **Portabilidade** | Adaptabilidade e instalabilidade| Alta | Web e aplicativo |
| **Conformidade** | Padrões de código e de API | Alta | Repositórios do GitHub, documentação e interface Web |

## 3 ▪ Método

| Etapa | Objetivo | Técnica | Ferramenta|
|-------|----------|---------|-----------------------|
| **Configuração** | Preparar ambiente  | Script da documentação e ajuda do monitor | GitHub e VSCode |
| **Coleta de Portabilidade** | Verificar instalação e execução | Instalação nos diferentes dispositivos e navegadores | Computador e celudar |
| **Coleta de Conformidade** | Verificar códigos e documentação | ESLint e observação segundo a ISO | SonarQube e documentação |
| **Relatórios com dados** | Escrever os resultados obtidos | Planilhas e documentar | VSCode + MkDocs |
| **Análise** | Ver os resultados de acordo com os critérios | Análise e confronto de resultados | Miro + Google Sheets |
| **Relato final** | Documentar resultador e recomendações | Relatório Markdown| MkDocs + VSCode|

## 4 ▪ Métricas e critérios de Aaeitação

### 4.1 Portabilidade  

| Métrica | Descrição | Forma de Cálculo | Aceitável | Esperado |
|--------------|-----------|------------------|------------------|--------------|
| 01 | Taxa de compatibilidade de navegador | Nº testes bons / Nº testes × 100 | ≥ 95% | 100% |
| 02 | Sucesso de instalação mobile | Nº instalações bons / dispositivos × 100 | ≥ 90% | ≥ 95% |
| 03 | Tempo médio de build para nova plataforma | Média (min) | ≤ 6 horas | ≤ 4 horas min |
| 04 | Bugs de plataforma | Bugs / sessões × 100 | ≤ 30% | ≤ 1% |

### 4.2 Conformidade  

| Métrica (ID) | Descrição | Forma de Cálculo | Aceitável | Esperado |
|--------------|-----------|------------------|------------------|--------------|
| 05 | Endpoints em conformidade | Endpoints conformes / total × 100 | ≥ 90% | ≥ 95% |
| 06 | Violações ESLint | Violações / 1 000  | ≤ 3 | ≤ 1 |
| 07 | Não conformidades graves| Contar | 0–2 | 0 |
| 08 | Documentação completa | Seções completas / total × 100 | ≥ 85% | ≥ 95% |

## 5 Ferramentas necessárias

* **Análise estática:** ESLint e SonarQube    
* **Testes mobile:** Celular 
* **Documentação:** Github 

## 6 ▪ Cronograma

| Dia | Entregável  | Atividades |
|--------|------------------|-----------|
| 11/07 | Ambiente pronto | Configurar sonarQube e navegadores |
| 11/07 | Relatório de portabilidade preliminar | Testes de navegador e no celular |
| 11/07 | Relatório de conformidade preliminar | Execução do SonarQube, análise do ESLint e da documentação do Github |
| 12/07 | Juntar resultados | Análise comparativa |
| 12/07 | Relatório final | Documento concluído com recomendação de correções |

## 7 ▪ Critérios de aceitação

A avaliação será considerada boa se:  

* ≥ 80% das métricas atingirem ao menos o nível “Aceitável”  
* Não houver alguma não conformidade crítica que não possas ser resolvida

## 8 ▪ Riscos

| Risco | Prob. | Impacto | Ação de Mitigação |
|-------|-------|---------|-------------------|
| Ambientes demorarem para configurar | Média | Alto | Fazer o quanto antes para buscar ajuda se necessário |
| Perca do acesso ao Github | Baixa | Médio | Basear em repositórios anteriores |
| Falta de tempo | Alto | Alto | Reprovação |

## 9 ▪ Entregáveis

1. **Github e Gitpages completo** 
2. **Apresentação final (slides e/ou gitpages completo)**

## 11 ▪ Histórico de Versões

| Versão | Data | Descrição | Autor(es) | 
|--------|------|-----------|-----------|
| 1.0 | 12/07/2025 | Criação inicial da Fase 03 | Gabriel Monteiro |