## Portabilidade  

| **Categoria** | **Descrição** |
|---------------|---------------|
| **Objeto** | Sistema AgroMart |
| **Propósito** | Avaliar a possibilidade de instalar e executar a plataforma AgroMart em diferentes ambientes|
| **Foco de qualidade** | Portabilidade |
| **Ponto de Vista** | -  Desenvolvedores e  Usuários finais |
| **Fatores de Variação** | -  Sistemas operacionais mobile (IOS e Android) <br> - Navegadores web (Chrome, Firefox, Edge e Brave) <br> |
| **Hipóteses de Base** | - **H1:** A plataforma na web funciona em 100% dos navegadores <br> - **H2:** É possível intalar em 90% dos dispositivos<br> - **H3:** O tempo médio de build para uma nova plataforma não excede 6 horas <br> - **H4:** Taxa de bugs específicos de plataforma ≤ 30% por uso |
| **Impacto dos Fatores de Variação** | -  Versões antigas de sistema operacional podem aumentar falhas de instalação e mudanças de arquitetura podem acabar estendendo o tempo de build |

## Conformidade  

| **Categoria** | **Descrição** |
|---------------|---------------|
| **Objeto** | Arquitetura de software do AgroMart|
| **Propósito** | Ver se está conforme os requisitos de qualidade da ISO/IEC 25010 |
| **Foco da Qualidade** | ISO/IEC 25010 – Conformidade|
| **Ponto de Vista** | -  Desenvolvedor e ISO/IEC |
| **Fatores de Variação** | -  Mudanças de requisitos na ISO analisada <br> -  Atualizações de bibliotecas do React e do Strapi|
| **Hipóteses de Base** | - **H1:** ≥ 90% dos endpoints estão em conformidade <br> - **H2:** Violação do ESLint ≤ 3 por mil linhas <br> - **H3:** Nenhuma não conformidade grave de acessibilidade <br> -  Mudanças em regulamentos podem criar não-conformidades de acessibilidade |
 **Hipóteses de Base** | - **H1:** A plataforma na web funciona em 100% dos navegadores <br> - **H2:** É possível intalar em 90% dos dispositivos<br> - **H3:** O tempo médio de build para uma nova plataforma não excede 6 horas <br> - **H4:** Taxa de crashes específicos de plataforma ≤ 1% por sessão |
| **Impacto dos Fatores de Variação** | - Bibliotecas descontinuadas podem gerar erros no ESLint <br> - Mudanças em regulamentos podem gerar novos erros |

## 📝 Histórico de Versões  

| Versão | Data | Descrição | Autor(es) |
|--------|------|-----------|-----------|
| 1.0 | 12/07/2025 | Criação dos abstraction sheets de Portabilidade e Conformidade detalhados. | [Gabriel Monteiro](https://github.com/GabrielSMonteiro) |