# Dr. Luciano Fonseca — Programa Viver Livre

Páginas estáticas do funil Viver Livre. Cada etapa tem seu próprio `index.html`; a identidade visual compartilhada está em `assets/site.css`.

| Rota | Função |
| --- | --- |
| `/viver-livre-l01/` | Apresentação principal e oferta |
| `/gatilhos-ocultos-up01/` | Oferta complementar |
| `/down01/` | Oferta alternativa |
| `/black/` | Oferta sazonal com cartão de desconto |
| `/obrigado/` | Confirmação e acesso ao grupo |

`/` redireciona para a apresentação principal, mantendo parâmetros de URL.

## Desenvolvimento local

```sh
python3 -m http.server 8765
```

Abra `http://localhost:8765/`. Não há etapa de build nem dependências de desenvolvimento.

## Integrações

As páginas usam VTurb/ConverteAI para vídeo, Hotmart para checkout, Meta Pixel e VK Metrics para atribuição. IDs, links e scripts são mantidos nas páginas de cada etapa. Antes de publicar em outro domínio, confirme as configurações desses serviços e teste a revelação das ofertas no player.

O conteúdo das ofertas e condições comerciais deve ser revisado pelo responsável antes de cada campanha. A página de obrigado informa a data da aula pelo grupo, evitando divulgar uma data passada.
