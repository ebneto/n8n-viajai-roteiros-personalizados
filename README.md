# n8n-viajai-roteiros-personalizados
# 🌍 Automação de Roteiros de Viagem (Entrega de PDF Personalizado)

Um projeto que demonstra a aplicação de IA (Gemini) e automação No-Code/Low-Code (n8n) para criar uma experiência de usuário altamente personalizada: o usuário recebe um roteiro de viagem customizado em formato PDF diretamente no seu e-mail.

## 🎯 Destaques do Produto e Valor

* **Personalização em Escala:** Utiliza a inteligência artificial para gerar conteúdo único com base nas preferências de viagem do usuário.
* **Entrega Automatizada:** O *workflow* completo (da submissão do formulário ao envio do PDF) é 100% automatizado, garantindo agilidade.
* **Decisões Orientadas por Dados (PO Mindset):** Um painel de métricas rastreia as preferências de viagem mais solicitadas, guiando futuras otimizações do produto.

## ⚙️ Tecnologias e Ferramentas

| Categoria | Tecnologia | Uso e Função no Workflow |
| :--- | :--- | :--- |
| **Frontend/UX** | Lovable | Criação da interface de usuário e coleta de preferências de forma ágil. |
| **Motor de Automação** | n8n (Low-Code/Orquestrador) | Gerencia o *workflow* complexo: Webhook → Wikipedia → Gemini → HTML → PDF → Gmail. |
| **Inteligência Artificial** | Google Gemini | Geração do conteúdo do roteiro de viagem. |
| **Conteúdo de Apoio** | Wikipedia Node | Obtenção de informações factuais para contextualização do roteiro (prompt engineering). |
| **Geração de Documentos** | API de Conversão PDF.co | Conversão do HTML gerado em um PDF profissional e estilizado. |
| **Dados da Interface** | Airtable | Fonte das imagens ou dados para composição do PDF. |

## 📝 O Workflow (N8N)

1.  **Webhook:** Recebe os dados de preferência do Lovable.
2.  **Wikipedia:** Consulta informações sobre o destino escolhido.
3.  **Gemini:** Gera o roteiro de viagem usando os dados do usuário + Wikipedia.
4.  **Code/Set:** Converte o retorno em texto em um código HTML estruturado (com a URL das imagens do Airtable).
5.  **Conversor PDF:** Transforma o HTML em arquivo PDF binário com o PDF.co.
6.  **Gmail:** Envia o PDF como anexo para o e-mail do usuário.

## 🔗 Links

* **Demo Online:** https://viajai-roteiros-personalizados.lovable.app/
* **Workflow N8N:** 
***
*Desenvolvido com 💛 por ebneto*
