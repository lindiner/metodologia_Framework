# ICE Score — Validação Rápida de Ideias

## 📋 **O que é**

Framework criado por **Sean Ellis** (Growth Hacking) para priorizar ideias.

**ICE = Impact × Confidence × Ease**

Cada dimensão: nota 1-10  
Score final: média das 3

---

## 🎯 **Quando usar**

✅ Várias ideias, precisa priorizar  
✅ Recurso limitado (tempo/gente)  
✅ Decisão em 1-2 dias  

❌ **NÃO use para:**
- Ideias complexas multi-área (use RICE)
- Projetos estratégicos de longo prazo
- Quando já decidiu fazer

---

## 🛠️ **Metodologia**

### **As 3 Dimensões**

**IMPACT (Impacto):**  
"Se der certo, qual o resultado?"

- 10 = Transformacional (dobra métrica)
- 7-9 = Grande impacto
- 4-6 = Moderado
- 1-3 = Pequeno

**CONFIDENCE (Confiança):**  
"Quão certo que vai funcionar?"

- 10 = Certeza (validado)
- 7-9 = Alta confiança
- 4-6 = Média
- 1-3 = Achismo

**EASE (Facilidade):**  
"Quão fácil implementar?"

- 10 = Muito fácil (1 pessoa, 1 dia)
- 7-9 = Fácil (2-3 pessoas, 1 semana)
- 4-6 = Médio (time, 2-4 semanas)
- 1-3 = Difícil (meses)

### **Cálculo**

```
ICE Score = (I + C + E) / 3
```

**Interpretação:**
- **8-10** → FAZER AGORA ✅
- **6-7.9** → CONSIDERAR ⚠️
- **4-5.9** → BACKLOG 📋
- **< 4** → DESCARTAR ❌

---

## 🤖 **PROMPT PARA IA**

```
Você é estrategista de priorização usando ICE Score.

OBJETIVO:
Avaliar ideias em Impact, Confidence, Ease (1-10).

PROCESSO:
1. Recebo descrição da ideia
2. Faço perguntas pra contexto
3. Avalio cada dimensão
4. Calculo score
5. Recomendo ação

DIMENSÕES:

IMPACT: "Qual tamanho do resultado?"
- 10 = Transformacional
- 7-9 = Grande
- 4-6 = Moderado
- 1-3 = Pequeno

CONFIDENCE: "Certeza de que funciona?"
- 10 = Validado
- 7-9 = Alta confiança
- 4-6 = Média
- 1-3 = Achismo

EASE: "Facilidade de implementar?"
- 10 = Muito fácil (1 pessoa, 1 dia)
- 7-9 = Fácil (2-3, 1 semana)
- 4-6 = Médio (time, 2-4 semanas)
- 1-3 = Difícil (meses)

FORMATO OUTPUT:

═══════════════════════════════════════
    ICE SCORE
═══════════════════════════════════════

IDEIA: [descrição]
CONTEXTO: [info coletada]

─────────────────────────────────────

📊 AVALIAÇÃO:

IMPACT: [nota]/10
[justificativa]

CONFIDENCE: [nota]/10
[justificativa]

EASE: [nota]/10
[justificativa]

─────────────────────────────────────

🎯 ICE SCORE: [score]
Cálculo: ([I] + [C] + [E]) / 3

═══════════════════════════════════════

💡 RECOMENDAÇÃO:
[FAZER AGORA / CONSIDERAR / BACKLOG / DESCARTAR]
[ação específica]

═══════════════════════════════════════

🚀 PRÓXIMOS PASSOS (se aprovado):
1. [passo 1]
2. [passo 2]
3. [passo 3]

Métrica de sucesso: [como medir]
Prazo: [tempo]

Pronto. Descreva a ideia.
```

---

## 💬 **Exemplo de Uso**

**INPUT:**
```
Ideia: Programa de mentoria sênior → júnior na EJ

Contexto:
- 30 membros (10 sênior, 20 júnior)
- Alta rotatividade (18-24 meses)
- Júnior demora 3-4 meses pra produzir
```

**OUTPUT:**
```
═══════════════════════════════════════
    ICE SCORE
═══════════════════════════════════════

IDEIA: Programa de mentoria estruturado

─────────────────────────────────────

📊 AVALIAÇÃO:

IMPACT: 8/10
Reduz ramp-up 50% (4→2 meses)
Retém conhecimento
Aumenta engajamento

CONFIDENCE: 7/10
Mentoria validada em outras EJs
Sem dados internos ainda
Depende de engajamento sênior

EASE: 6/10
Setup 2-3 semanas
Precisa buy-in de 10 pessoas
Não é plug-and-play

─────────────────────────────────────

🎯 ICE SCORE: 7.0

═══════════════════════════════════════

💡 RECOMENDAÇÃO:
⚠️ CONSIDERAR — Prioridade média-alta

Ação: PILOTAR grupo pequeno antes de escalar

Por quê? Score bom, mas risco em Ease
Reduzir risco: começar pequeno

═══════════════════════════════════════

🚀 PRÓXIMOS PASSOS:

PILOTO (8 semanas):
1. Selecionar 3 duplas interessadas
2. Estrutura mínima: 1x/semana, 30min
3. 3 tópicos: onboarding, projeto, soft skills
4. Medir: tempo até 1ª entrega solo

DECISÃO: Escalar se ramp-up < 2.5 meses
```

---

## 🔧 **Setup**

**ChatGPT:** Custom GPT com prompt acima  
**Claude:** Projects com prompt nas instruções

---

## 📊 **ICE vs RICE**

| Aspecto | ICE | RICE |
|---------|-----|------|
| Dimensões | 3 | 4 (+Reach) |
| Tempo | 5min | 15min |
| Use para | Decisão rápida | Investimento grande |

---

## ✅ **Checklist**

- [ ] Notas baseadas em DADOS
- [ ] Justificativas claras
- [ ] Ease considera recursos reais
- [ ] Impact é mensurável

---

**Próximo passo:** Score > 7?  
→ Vá para [`../02-mapeamento/customer-journey-map.md`](../02-mapeamento/customer-journey-map.md)

---

**Criado por Ana Lindiner | NUCA 2026**  
MIT License
