# 5 Porquês — Identificar Causa Raiz

## 📋 **O que é**

Framework da **Toyota** (anos 1950) para identificar causa raiz de problemas.

**Princípio:** Perguntar "Por quê?" 5 vezes até chegar na origem real.

---

## 🎯 **Quando usar**

✅ Problema recorrente  
✅ Sintoma conhecido, causa desconhecida  
✅ Time trata sintoma, problema volta  
✅ Precisa diagnóstico rápido  

❌ **NÃO use para:**
- Problemas com múltiplas causas simultâneas (use Ishikawa)
- Situações sem resposta clara
- Questões comportamentais complexas

---

## 🛠️ **Metodologia**

### **PASSO 1: Defina o problema observável**

Seja específico:
- ❌ "Vendas caíram"
- ✅ "Vendas caíram 30% no Q1 vs Q4"

### **PASSO 2: Pergunte "Por quê?" 5 vezes**

**Exemplo — Projeto que atrasa:**

```
1. Por quê o projeto atrasou?
   → Entregas intermediárias não aconteceram no prazo

2. Por quê as entregas não aconteceram?
   → Membros não sabiam o que entregar

3. Por quê não sabiam?
   → Não existe escopo detalhado por etapa

4. Por quê não existe escopo?
   → Cada gerente define do seu jeito

5. Por quê cada um define do seu jeito?
   → Nunca documentamos processo padrão

CAUSA RAIZ: Falta de processo padronizado
```

### **PASSO 3: Valide com pergunta reversa**

"Se resolver X, problema Y desaparece?"

Se SIM → causa raiz correta ✅  
Se NÃO → refaça os 5 Porquês ❌

---

## 🤖 **PROMPT PARA IA**

### **Copie e cole no ChatGPT ou Claude:**

```
Você é um consultor especializado em Root Cause Analysis usando 5 Porquês.

OBJETIVO:
Identificar causa raiz de problemas através de 5 perguntas consecutivas.

PROCESSO:
1. Recebo descrição do problema
2. Aplico 5 Porquês
3. Identifico causa raiz
4. Valido com pergunta reversa
5. Sugiro ação corretiva

REGRAS:
- Cada resposta baseada em FATOS, não suposições
- Se resposta vaga, peço mais contexto
- Causa raiz deve ser ACIONÁVEL
- Diferencio SINTOMA de CAUSA RAIZ

FORMATO OUTPUT:

═══════════════════════════════════════
    ANÁLISE 5 PORQUÊS
═══════════════════════════════════════

PROBLEMA OBSERVADO:
[descrição]

─────────────────────────────────────

1º POR QUÊ?
[pergunta] → [resposta]

2º POR QUÊ?
[pergunta] → [resposta]

3º POR QUÊ?
[pergunta] → [resposta]

4º POR QUÊ?
[pergunta] → [resposta]

5º POR QUÊ?
[pergunta] → [resposta]

═══════════════════════════════════════

🎯 CAUSA RAIZ:
[descrição]

⚠️ SINTOMAS (não são causa):
✗ [sintoma 1]
✗ [sintoma 2]

✅ CAUSA REAL:
[causa raiz acionável]

═══════════════════════════════════════

VALIDAÇÃO (pergunta reversa):
Se resolvermos [causa raiz], [problema] desaparece?
[SIM/NÃO + justificativa]

═══════════════════════════════════════

💡 AÇÃO CORRETIVA:
[ação específica, mensurável, com prazo]

═══════════════════════════════════════

Pronto. Descreva o problema que quer diagnosticar.
```

---

## 💬 **Exemplo de Uso**

### **INPUT:**
```
Problema: 80% dos projetos da EJ atrasam nas últimas 8 semanas
```

### **OUTPUT:**

```
═══════════════════════════════════════
    ANÁLISE 5 PORQUÊS
═══════════════════════════════════════

PROBLEMA OBSERVADO:
80% dos projetos atrasam (últimas 8 semanas)

─────────────────────────────────────

1º POR QUÊ os projetos atrasam?
→ Entregas intermediárias não acontecem no prazo

2º POR QUÊ entregas não acontecem?
→ Membros não sabem o que precisa ser entregue

3º POR QUÊ não sabem?
→ Não existe escopo detalhado por etapa

4º POR QUÊ não existe escopo?
→ Cada gerente define do seu jeito

5º POR QUÊ cada um define do seu jeito?
→ Nunca documentamos processo padrão

═══════════════════════════════════════

🎯 CAUSA RAIZ:
Ausência de processo padronizado de gestão de projetos

⚠️ SINTOMAS (não são causa):
✗ Membros preguiçosos
✗ Cliente muda escopo
✗ Falta de ferramenta (Trello, etc)

✅ CAUSA REAL:
Falta de metodologia estruturada e documentada

═══════════════════════════════════════

VALIDAÇÃO:
Se criarmos processo padrão, atrasos param?

SIM — alta probabilidade. Processo elimina 
reinvenção da roda em cada projeto.

═══════════════════════════════════════

💡 AÇÃO CORRETIVA:

CRIAR PLAYBOOK (30 dias)

Semana 1-2:
✓ Mapear 3 projetos recentes
✓ Identificar etapas comuns
✓ Documentar gargalos

Semana 3:
✓ Desenhar processo padrão
✓ Template de escopo
✓ Checklist por fase

Semana 4:
✓ Documentar no Notion
✓ Treinar time
✓ Pilotar em 2 projetos

MÉTRICA: Reduzir atrasos de 80% → 30% em 2 meses
```

---

## 🔧 **Setup**

### **ChatGPT (Custom GPT):**
1. [chat.openai.com](https://chat.openai.com) → "Explore GPTs" → "Create"
2. Nome: "5 Porquês - Diagnóstico"
3. Cole o prompt acima
4. Salve

### **Claude (Projects):**
1. [claude.ai](https://claude.ai) → Criar projeto "Diagnóstico 5 Porquês"
2. Cole o prompt nas instruções
3. Adicione docs de contexto (opcional)

---

## ✅ **Checklist de Qualidade**

- [ ] Cada resposta baseada em FATOS
- [ ] Causa raiz é ACIONÁVEL
- [ ] Pergunta reversa retorna SIM
- [ ] Time concorda com diagnóstico
- [ ] Resolver causa é viável

---

## 📚 **Recursos**

**Leitura:**
- Toyota Production System (Taiichi Ohno)
- The Lean Startup (Eric Ries)

**Combine com:**
- SWOT (estratégia pós-diagnóstico)
- Ishikawa (se múltiplas causas)

---

**Próximo passo:** Causa raiz identificada?  
→ Vá para [`../02-mapeamento/bpmn-as-is.md`](../02-mapeamento/bpmn-as-is.md)

---

**Criado por Ana Lindiner | NUCA 2026**  
MIT License
