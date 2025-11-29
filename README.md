# -Agente-IA-WhatsApp-Pro
Automação humanizada no WhatsApp com IA. O Agente IA WhatsApp Pro entende áudios, imagens, vídeos e documentos, responde dúvidas, agenda consultas e oferece atendimento 24h personalizado para cada empresa. Ideal para negócios que desejam agilidade, profissionalismo e escala.

## Como ativar envio automático do formulário (Formspree)

O formulário do site suporta envio automático via Formspree. Por padrão o projeto contém um placeholder — siga estes passos para ativar o envio real para seu e‑mail:

1. Acesse https://formspree.io e crie uma conta (ou faça login).
2. Clique em "New Form" e siga os passos. Você poderá escolher seu e‑mail destino na dashboard.
3. Copie o endpoint fornecido por eles. Será algo como: `https://formspree.io/f/abcde123`.
4. No arquivo `index.html`, procure a constante `FORMPSREE_ENDPOINT` (perto do final do arquivo) e substitua o placeholder (`https://formspree.io/f/<YOUR_FORM_ID>`) pelo endpoint copiado.

Exemplo:
```
const FORMPSREE_ENDPOINT = 'https://formspree.io/f/abcde123';
```

5. Salve e redeploy seu site. O formulário agora enviará automaticamente (via Formspree). Se ocorrer algum erro, o formulário fará fallback para `mailto:` e abrirá o cliente de e‑mail do usuário.

Observação: esta solução é simples para sites estáticos e evita criar um backend. Se você preferir suporte por SMTP ou serverless, me diga que eu oriento a configurar.

## Política de Privacidade

As políticas de privacidade do site foram incorporadas ao repositório como arquivos estáticos em `politica-privacidade/index.html`.
Você pode visualizar a página localmente pelo caminho `/politica-privacidade/index.html` ou no GitHub em: https://github.com/MatheusOBS/politica-privacidade

Observação: anteriormente este conteúdo estava vinculado como um submódulo Git; ele foi substituído por arquivos estáticos para simplificar o deploy e garantir disponibilidade sem dependências de submódulos.
