# 🧾 Validador de CPF

Este é um projeto web simples que permite ao usuário validar um número de CPF brasileiro. Desenvolvido com HTML, CSS e JavaScript puro, o sistema verifica os dígitos verificadores do CPF e informa ao usuário se ele é válido ou inválido.

---

## 🔍 Funcionalidades

- Validação completa do CPF segundo a fórmula oficial da Receita Federal.
- Exibição dinâmica de mensagens de sucesso ou erro.
- Interface limpa e moderna.

---

## 💻 Como usar

1. Clone este repositório ou baixe o `.zip`.
2. Abra o arquivo `index.html` em qualquer navegador moderno.
3. Digite um número de CPF no campo.
4. Clique em **Validar**.
5. O sistema exibirá se o CPF é **válido** ou **inválido**.

---

## 📁 Estrutura de Arquivos

📦 validador-cpf
├── index.html # Página principal
├── cpf.css # Estilos do formulário
├── cpf.js # Lógica de validação
├── imagens/ # (Opcional) Capturas de tela do site
└── README.md # Este arquivo

---

## 🧠 Lógica da Validação

A validação segue os passos oficiais:

- Remove caracteres não numéricos.
- Verifica se todos os dígitos são iguais (caso sejam, é inválido).
- Calcula o **1º dígito verificador** com os 9 primeiros números.
- Calcula o **2º dígito verificador** com os 10 primeiros números.
- Compara os dígitos calculados com os fornecidos no CPF.

---

## ✅ Exemplos para Testes

| CPF | Resultado |
|-----|-----------|
| `529.982.247-25` | ✅ Válido |
| `123.456.789-00` | ❌ Inválido |

---

## 🖼️ Capturas de Tela

img("![image](https://github.com/user-attachments/assets/63d6d265-f583-4225-8927-6f0600f6ab08)
")

```markdown
![Formulário de Validação](imagens/formulario.png)
![CPF Válido](imagens/cpf_valido.png)
![CPF Inválido](imagens/cpf_invalido.png)
🎨 Estilo Visual
A interface conta com:

Caixa de formulário centralizada.

Cores diferentes para mensagens de erro (vermelho) e sucesso (verde).

Estilo limpo com foco em usabilidade.

💡 Melhorias Futuras
Adicionar máscara automática para CPF (000.000.000-00)

Validação em tempo real enquanto digita

Adicionar testes automatizados

Adicionar validação no backend com Node.js
