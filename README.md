# 🚀 PedMoto

**PedMoto** é uma plataforma SaaS multi-tenant de logística focada em **corridas rápidas**, **entregas** e **gestão de frotas** para pequenas e médias empresas sob o modelo White-Label.

A plataforma conecta clientes, motoristas (via App nativo) e operadores de frota em um ecossistema unificado, oferecendo funcionalidades de marketplace sob demanda (táxi/mototáxi) com suporte a negociação de preços (leilão/bids) e frotas próprias.

**Versão Atual:** `1.0.1-Stable`

---

## 🏗️ Arquitetura do Ecossistema

O ecossistema PedMoto é composto por três pilares de software integrados:

1. **Next.js WebApp (Este Repositório):** Portal administrativo multi-tenant, dashboard de frotas, painel do cliente web e APIs públicas de integração.
2. **Native Flutter App (v4.0.0):** Aplicativo móvel nativo de alta performance para os motoristas (`/Motok/App`), garantindo rastreamento geográfico em segundo plano em tempo real e entrega resiliente de notificações de novas corridas via FCM.
3. **Distribution Daemon:** Microsserviço responsável pela inteligência de distribuição de pedidos baseada em lotes geográficos, fila de prioridade por proximidade, suporte a broadcasts de leilão e regras de categorias de veículos.
