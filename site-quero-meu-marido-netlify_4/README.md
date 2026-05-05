# 🚀 Quero Meu Marido de Volta — Deploy Final

✅ Pixel já configurado: **4356731727899519**

## 📁 Arquivos
- `index.html` → quiz (página inicial)
- `oferta.html` → página de vendas (acessada em /oferta)
- `_redirects` → URL limpa /oferta no Netlify

---

## ⚠️ ÚNICA COISA QUE FALTA TROCAR:

### Link do Checkout Kiwify

Em `oferta.html`, busca por:
```
https://pay.kiwify.com.br/SEU_LINK_AQUI
```
Troca pelo link real quando a Kiwify desbugar.

(Pode subir hoje mesmo sem isso — o botão só não vai funcionar até você trocar)

---

## 🌐 Deploy no Netlify (3 minutos):

1. Vai em **app.netlify.com** → cria conta grátis (pode usar Google)
2. Clica em **"Add new site"** → **"Deploy manually"**
3. **Arrasta a pasta inteira** pra dentro do quadrado de upload
4. Pronto! Vai gerar uma URL tipo: `seu-site-xxxxx.netlify.app`

### Renomear a URL:
- Site settings → Change site name
- Coloca: `queromeumarido` ou `qmmv-quiz`
- Vai virar: `queromeumarido.netlify.app`

---

## 🔗 URLs finais:

- **Quiz (URL do anúncio):** `https://seu-site.netlify.app/`
- **Página de vendas:** `https://seu-site.netlify.app/oferta`
- **Checkout:** o que a Kiwify gerar

---

## 📊 Eventos rastreados pelo Pixel:

| Página | Evento |
|---|---|
| Quiz | PageView |
| Oferta | PageView + ViewContent |
| Botão de compra | InitiateCheckout (R$37) |

O evento **Purchase** vem direto da Kiwify quando configurar a integração com Pixel lá.

---

## ✅ Como confirmar que o Pixel está funcionando:

1. Instala a extensão **Meta Pixel Helper** no Chrome
2. Abre seu site no Netlify
3. Clica no ícone da extensão
4. Tem que aparecer: ✅ Pixel ativo + eventos PageView/ViewContent
