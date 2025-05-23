# 🌡️ Assignment 2 - Visualização Interativa de Anomalias de Temperatura Global

## 📋 Visão Geral

Este projeto é uma visualização interativa desenvolvida para o Assignment 2, focando na análise e apresentação das anomalias de temperatura média global de 1880 a 2024. Utiliza dados baseados no dataset NASA GISS GISTEMP v4 para criar uma experiência educativa e interativa sobre mudanças climáticas.

### 🎯 Objetivos do Projeto

 - ✅ Análise exploratória de 3 diferentes designs de visualização
 - ✅ Implementação interativa usando tecnologias web modernas
 - ✅ Comparação crítica de ferramentas (Tableau vs D3.js)
 - ✅ Documentação completa do processo de design


### 📁 Estrutura do Projeto
  ```csharp
            assignment2/
            ├── 📄 assignment2
            ├── 📄 README.md                                
            ├── 🌐 interactive_climate_viz.html
            ├── 🎨 design_iterations.html                                
  ```    

### 🚀 Como Executar
#### Pré-requisitos:

  - Navegador moderno (Chrome, Firefox, Safari, Edge)
  -	Conexão à internet (para carregar Plotly.js)
  - Nenhuma instalação adicional necessária

#### Instruções de Execução

```csharp
          open interactive_climate_viz.html
          open design_iterations.html   
  ```

#### Explore as funcionalidades usando os controles interativos


### 🎨 Designs Explorados
#### Design 1: Gráfico de Linha Temporal

   - Conceito: Linha simples mostrando evolução temporal
   - Iterações:
       - v1.1: Dados brutos "ruidosos"
       - v1.2: Suavização + gradiente de cores
   - Resultado: Base sólida, mas limitado para exploração

#### Design 2: Mapa de Calor Temporal

   - Conceito: Heatmap com anos×meses
   - Iterações:
     - v2.1: Grade básica com padrões sazonais
     - v2.2: Divisões por década + tooltips
   - Resultado: Excelente para padrões, mas perde continuidade temporal

#### Design 3: Visualização Interativa (ESCOLHIDO)

  - Conceito: Interface multi-layer com controles
  - Iterações:
    - v3.1: Layout complexo com muitos controles
    - v3.2: Interface simplificada e organizada
  - Resultado: Combina clareza, funcionalidade e usabilidade

## 🛠️ Especificações Técnicas
### Tecnologias Utilizadas

  - HTML5 - Estrutura e markup
  - CSS3 - Estilização e layout responsivo
  - JavaScript ES6+ - Lógica e interatividade
  - Plotly.js v2.26.0 - Renderização de gráficos

### Funcionalidades Implementadas
#### 🎛️ Controles Interativos

  - Períodos Históricos: Botões pré-definidos (Era Industrial, Pós-Guerra, etc.)
  - Sliders Temporais: Seleção customizada de intervalos
  - Opções Visuais: Toggle para suavização e linha de tendência
  - Zoom e Pan: Exploração detalhada dos dados

#### 📊 Visualização de Dados

  - Linha Principal: Anomalias de temperatura com fill
  - Suavização: Média móvel para revelar tendências
  - Linha de Tendência: Regressão linear do período selecionado
  - Cores Significativas: Azul (frio) → Vermelho (quente)

#### 📈 Painel de Estatísticas

  - Anomalia Média: Cálculo dinâmico do período
  - Extremos: Temperaturas máxima e mínima
  - Taxa de Aquecimento: °C por década (calculado automaticamente)


### 📊 Dados e Metodologia
#### Fonte dos Dados

  - Origem: NASA Goddard Institute for Space Studies (GISS)
  - Dataset: GISTEMP v4 - Global Land-Ocean Temperature Index
  - Período: 1880-2024 (145 anos)
  - Baseline: Anomalias relativas ao período 1951-1980

#### Processamento dos Dados

```csharp
javascript// Exemplo da estrutura de dados
{
  year: 2024,
  anomaly: +1.24,  // °C
  date: Date(),
  decade: 2020,
  period: "2000-presente"
}
  ```   

#### Algoritmos Implementados

  - Média Móvel: Janela de 5 anos para suavização
  - Regressão Linear: Cálculo da taxa de aquecimento
  - Filtros Temporais: Seleção dinâmica de períodos

### 🎯 Público-Alvo e Contexto
#### Audiência Primária

  - 🔬 Investigadores em climatologia
  - 📚 Educadores em ciências da Terra

#### Contexto de Utilização

  - Apresentações académicas e conferências
  - Relatórios de investigação e publicações
  - Educação ambiental em escolas e universidades
  - Comunicação pública sobre mudanças climáticas

#### Melhorias Implementadas

- ✅ Contexto histórico expandido com eventos climáticos
- ✅ Performance otimizada para dispositivos móveis
- ✅ Tooltips mais informativos com explicações
- ✅ Modo alto contraste para acessibilidade


### 🛠️ Comparação de Ferramentas
#### Tableau
- ✅ Vantagens:
  
  - Prototipagem rápida e intuitiva
  - Design visual profissional por padrão
  - Integração fácil com múltiplas fontes de dados
  - Dashboards interativos sem programação

- ❌ Desvantagens:

  - Custo elevado para licenças
  - Flexibilidade limitada para customizações
  - Dependência do ecossistema proprietário
  - Curva de aprendizagem para análises complexas

#### D3.js
- ✅ Vantagens:

  - Flexibilidade total e controle granular
  - Performance otimizável para grandes datasets
  - Integração nativa com tecnologias web
  - Open source e gratuito

- ❌ Desvantagens

  - Requer conhecimentos avançados de programação
  - Desenvolvimento demorado para visualizações complexas
  - Necessita manutenção e debugging constante
  - Curva de aprendizagem muito íngreme

### Decisão Final
- Abordagem Híbrida: Tableau para prototipagem inicial + D3.js/Plotly.js para implementação final com máxima customização.

### 📈 Resultados e Impacto
- Métricas de Sucesso:

  - ✅ 100% dos objetivos do assignment atingidos
  - ✅ 3 designs diferentes explorados e documentados
  - ✅ Feedback positivo de todos os utilizadores testados
  - ✅ Interface responsiva funcional em múltiplos dispositivos

- Impacto Educativo Esperado:

  - 📚 Ferramenta de ensino para mudanças climáticas
  - 🔍 Exploração interativa de dados científicos
  - 💡 Consciencialização pública sobre aquecimento global
  - 📊 Exemplo de boas práticas em visualização de dados

### 🔬 Principais Descobertas
#### Sobre os Dados Climáticos

  - 🌡️ Aquecimento acelerado evidente após 1980
  - 📈 Taxa atual: ~+0.18°C por década
  - 🔥 2024: Provavelmente o ano mais quente registado
  - 🌊 Variabilidade natural sobreposta à tendência de longo prazo

- Sobre Design de Visualizações

  - 🔄 Iteração é fundamental para refinamento
  - 👥 Feedback de utilizadores revela problemas não antecipados
  - ⚖️ Balanceamento entre simplicidade e funcionalidade é crucial
  - 🎨 Contexto histórico essencial para dados climáticos

### 🚧 Limitações e Trabalho Futuro
- Limitações Atuais: 

  - 📱 Performance móvel pode ser melhorada
  - 🌍 Dados geoespaciais não incluídos
  - 🔮 Projeções futuras não implementadas
  - 💾 Exportação de dados limitada

- Próximos Desenvolvimentos

  - 🗺️ Mapa mundial interativo com anomalias regionais
  - 📊 Integração com outros indicadores (CO2, nível do mar)
  - 🎮 Elementos de gamificação para educação
  - 📱 App móvel nativo para melhor experiência


### 📚 Referências e Fontes
- Dados Científicos: 

  - GISTEMP Team, 2025: GISS Surface Temperature Analysis (GISTEMP), version 4. NASA Goddard Institute for Space Studies. https://data.giss.nasa.gov/gistemp/
  - Lenssen, N., et al., 2024: A GISTEMPv4 observational uncertainty ensemble. J. Geophys. Res. Atmos., 129, no. 17.
  - Hansen, J., et al., 2010: Global surface temperature change. Rev. Geophys., 48, RG4004.

- Recursos Técnicos

  - Plotly.js Documentation: https://plotly.com/javascript/
  - Our World in Data - Climate: https://ourworldindata.org/climate-change
  - NASA Climate Change: https://climate.nasa.gov/


## 👤 Informações do Autor

  - Estudante: Silvano Rodrigues
  - Email: juniorsilvano242@gmail.com
  - Data: 23 de maio de 2025
  - Assignment: 2 - Análise, Design e Implementação de Visualização
  - Tempo investido: 15+ horas

## 📄 Licença e Uso
Este projeto foi desenvolvido para fins académicos. Os dados são baseados em fontes públicas da NASA. O código pode ser usado para fins educativos com devida atribuição.
Citação Sugerida
Silvano Rodrigues (2025). "Visualização Interativa de Anomalias de Temperatura Global". 

## 🤝 Contribuições e Feedback
- Para questões, sugestões ou melhorias:

  - 📧 Email: juniorsilvano242@gmail.com
  - 💬 Issues: Reportar problemas ou sugestões
  - 🔄 Pull Requests: Contribuições são bem-vindas


## 🏆 Reconhecimentos

  - NASA GISS pelos dados climáticos públicos
  - Plotly.js pela excelente biblioteca de visualização
  - Participantes do feedback pelas valiosas contribuições
  - Comunidade open source pelas ferramentas utilizadas

```csharp
"Visualizar dados climáticos não é apenas sobre gráficos - é sobre comunicar uma das histórias mais importantes da nossa época."
  ```   
