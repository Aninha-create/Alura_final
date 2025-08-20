# 📊 Análise Preditiva de Evasão de Clientes

Este projeto tem como objetivo identificar os principais fatores que influenciam a evasão de clientes e comparar o desempenho de dois modelos preditivos: **Regressão Logística** e **Random Forest**.

---

## 🎯 Objetivo

Prever a probabilidade de evasão de clientes com base em dados demográficos, contratuais e de uso de serviços, além de entender os fatores que mais contribuem para essa evasão.

---

## 📈 Distribuição de Clientes

Abaixo está o gráfico que mostra a proporção de clientes ativos e evadidos:

![Gráfico de distribuição de evasão](./distribuicao_evasao.png)

- **Clientes Ativos**: 73.5%  
- **Clientes Evadidos**: 26.5%

Essa distribuição mostra que, embora a maioria dos clientes permaneça ativa, há uma parcela significativa que abandona o serviço.

---

## ⚖️ Comparativo de Modelos

| Métrica                     | Regressão Logística | Random Forest      |
|----------------------------|---------------------|--------------------|
| Acurácia                   | 74%                 | 79%                |
| Recall (Evasão)            | 81%                 | 48%                |
| Precisão (Evasão)          | 51%                 | 63%                |
| F1-score (Evasão)          | 0.62                | 0.54               |
| AUC                        | —                   | 0.69               |

- A **Regressão Logística** é mais eficaz para identificar clientes que vão evadir (recall alto).
- O **Random Forest** tem melhor acurácia geral, mas menor sensibilidade à evasão.

---

## 🔍 Fatores que Influenciam a Evasão

### 🔺 Aumentam a chance de evasão:
- Tipo de internet: *Fiber Optic*
- Serviços digitais: *Streaming TV*, *Filmes*, *Fatura digital*
- Método de pagamento: *Electronic Check*
- Perfil demográfico: *Idosos*, *Múltiplas linhas*

### 🔻 Reduzem a chance de evasão:
- Tipo de contrato: *One year*, *Two year*
- Presença de dependentes
- Serviços adicionais: *Segurança online*, *Backup online*
- Menor cobrança mensal e maior tempo de empresa

---

## 🌟 Variáveis Mais Relevantes (Random Forest)

1. **Meses com a empresa**
2. **Cobrança total**
3. **Cobrança mensal**
4. **Conta diária**
5. **Contrato de dois anos**

Essas variáveis quantitativas tiveram maior impacto na previsão de evasão.

---
## 🚀 Melhorias Futuras para o Projeto

Para aumentar a precisão e aplicabilidade dos modelos, sugerimos as seguintes melhorias:

- **Aprimoramento dos dados**:
  - Incluir dados de atendimento ao cliente (tempo de resposta, satisfação).
  - Incorporar histórico de reclamações e solicitações de suporte.
  - Adicionar variáveis de engajamento com campanhas de marketing.

- **Modelagem avançada**:
  - Testar modelos como XGBoost e LightGBM para maior performance.
  - Implementar técnicas de balanceamento como SMOTE para lidar com classes desbalanceadas.
  - Aplicar validação cruzada estratificada para maior robustez.

- **Monitoramento contínuo**:
  - Criar dashboards em tempo real para acompanhar métricas de evasão.
  - Automatizar alertas para clientes com alto risco de evasão.

---

## 💡 Estratégias de Retenção para a TelecomX

Com base nos insights obtidos, a TelecomX pode adotar as seguintes ações para reduzir a evasão:

### 🎁 Incentivos e benefícios
- Oferecer **descontos progressivos** para contratos de longo prazo.
- Criar **programas de fidelidade** com recompensas por tempo de permanência.

### 📞 Atendimento personalizado
- Identificar clientes com alto risco de evasão e realizar **ações proativas** (ligações, ofertas).
- Treinar equipes de suporte para lidar com perfis mais vulneráveis (ex: idosos).

### 📊 Transparência e controle
- Melhorar a **comunicação de cobranças** e oferecer simulações de planos.
- Criar um **painel do cliente** com visualização clara de uso e benefícios.

### 📲 Experiência digital
- Investir em **apps intuitivos** e canais digitais para facilitar o autoatendimento.
- Oferecer **conteúdos personalizados** com base no perfil de consumo.

### 🔄 Feedback contínuo
- Implementar pesquisas de satisfação após interações.
- Usar análise de sentimentos em comentários e redes sociais para detectar insatisfações precoces.

---

## 🧠 Conclusão Final

A TelecomX pode transformar dados em decisões estratégicas com impacto direto na retenção. Ao unir modelagem preditiva com ações práticas, é possível antecipar comportamentos e construir uma relação mais duradoura com seus clientes.



---
