# DIO Agent — Mentor de Cibersegurança

##  Especialização
Transformei o DIO Agent num especialista em análise de vulnerabilidades. Em vez de dar respostas prontas, ele:
1. Coleta o contexto completo
2. Identifica a falha e sua origem
3. Avalia impacto, probabilidade e severidade
4. Orienta pelos princípios defensivos, sem entregar soluções copiáveis
5. Sugere como validar a correção

Isso foi criado para praticar o pensamento de um profissional de AppSec e segurança defensiva.

##  Arquivos criados e alterados

| Caminho | O que é |
|---|---|
| `skills/vulnerability-analysis/SKILL.md` | Roteiro passo a passo que o agente segue |
| `skills/vulnerability-analysis/README.md` | Explicação da skill para pessoas |
| `agent/knowledge/security-basics.md` | Conceitos: vulnerabilidade, ameaça, risco, tríade CIA e boas práticas |
| `agent/persona.md` | Adicionado perfil de mentor de cibersegurança |
| `AGENTS.md` | Skill registrada na tabela de uso |
| `app.py` | Código de teste — versão vulnerável e versão corrigida |

##  Como rodar o agente

1. Instale o **Git for Windows** (necessário no Windows)
2. Instale o Hermes:
   ```powershell
   pip install hermes-agent
   ```
   ## Abra o terminal dentro da pasta do projeto:
   cd "C:\Users\DoriaN\Desktop\Projetos Github\lab-ai agent cyber\dio-agent-main" (Este é o caminho usado no meu computador)
```bash
hermes 
```
Conecte com a conta gratuita e comece a interagir com o agente  

# Evidências dos Testes  

## 1. Análise do código vulnerável  
O agente identificou a concatenação de strings na consulta SQL, explicou o risco de SQL Injection e orientou os princípios de defesa sem dar código pronto.  



## 2. Validação após correção  
Substituí a concatenação por consulta parametrizada (? como marcadores). O agente confirmou que a falha foi mitigada e explicou por que separar comando de dados é seguro.   


## 3. Coleta de contexto — servidor Ubuntu  
Ao perguntar sobre um servidor exposto, o agente não entregou comandos prontos. Primeiro perguntou detalhes sobre serviços, portas, dados e acessos — provando que a persona está ativa.  

## Melhoria escolhida  
A análise sempre segue o formato profissional: Contexto → Identificação → Avaliação de Risco → Orientação → Validação, com classificação de impacto e severidade. Assim é possível comparar diferentes vulnerabilidades com a mesma régua.  

## Entrega  
Repositório público: https://github.com/seu-usuario/dio-agent
