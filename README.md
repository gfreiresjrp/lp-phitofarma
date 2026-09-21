# LP Phitofarma — Farmácia de Manipulação

Landing page estática (HTML/CSS/JS sem build) da Phitofarma São Bernardo, gerada no padrão da skill `lp-farmacia-manipulacao`.

- `index.html` — página principal
- `privacidade.html`, `termos.html` — páginas legais
- `assets/` — logo e imagens

## Rodar localmente

```bash
python3 -m http.server 5173
```

Abra http://localhost:5173.

## Configuração

- **GTM:** `GTM-MN99C777` (head + noscript nas três páginas).
- **Webhook de lead:** constante `LEAD_WEBHOOK` no script do `index.html`. Recebe POST JSON com nome, whatsapp, UTMs, gclid e data a cada envio do formulário.
- **Eventos no dataLayer:** `lead_form_submit` e `whatsapp_click` (sem dados pessoais).
