# 🤖 Agente Github MCPilot para Cursor IDE

Este projeto disponibiliza uma regra estruturada para uso como agente de IA no Cursor IDE, permitindo operações reais no Github via protocolo MCP, com logging estruturado e experiência CLI interativa.

## 🎯 Objetivo

Fornecer uma regra pronta para ser utilizada no Cursor IDE, transformando o assistente em um agente Github MCPilot, capaz de:
- Executar comandos reais no Github (via MCP)
- Exibir menus interativos com ícones
- Gerar logs estruturados das interações
- Validar ambiente e permissões
- Guiar o usuário passo a passo

## 🚀 Instalação

1. **Clone ou baixe este repositório**

2. **Copie a regra para seu projeto**

   No terminal, execute:
   ```bash
   mkdir -p .cursor/rules
   cp cursor-ide-rule/agente-github-mcpilot.mdc .cursor/rules/
   ```

3. **Abra seu projeto no Cursor IDE**

4. **Certifique-se de que o modo Agent está ativado**
   - Vá em Settings > Agent > Ative a opção "Enable Agent"
   - Permita execução de comandos

5. **Pronto!**
   - O assistente seguirá as regras do agente Github MCPilot automaticamente.

## 💡 Como usar

- Ao iniciar o Cursor IDE, o agente irá:
  1. Saudar você pelo nome
  2. Exibir a arte de apresentação
  3. Perguntar se deseja gerar logs e onde salvar
  4. Guiar a configuração do ambiente MCP
  5. Exibir um menu numerado com ícones para operações Github reais
- Todas as operações são executadas de fato no Github, com logs estruturados.

## 📁 Estrutura do Projeto

- `cursor-ide-rule/agente-github-mcpilot.mdc`: Arquivo de regra principal para o agente
- `README.md`: Este guia de uso

## 📝 Logging estruturado

Os logs seguem o padrão:

```
[2024-06-07T10:00:00.000Z] [INFO] [request-id:uuid] {"llm":"gpt-4","tokens":123,"command":"listar_repositorios","user":"seu_usuario","result":"success","duration_ms":1200,"details":{}}
```

## 🤝 Contribuição

1. Faça um fork do repositório
2. Crie um branch para sua feature ou ajuste
3. Envie um Pull Request

Sugestões, melhorias e exemplos de uso são bem-vindos!

## 📄 Licença

MIT
