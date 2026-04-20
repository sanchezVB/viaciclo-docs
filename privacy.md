---
title: Política de Privacidade — ViaCiclo
---

# Política de Privacidade

**Última atualização:** 20 de abril de 2026

Esta Política de Privacidade descreve como o aplicativo **ViaCiclo** coleta, usa, armazena e protege os dados pessoais dos seus usuários. Ao criar uma conta e usar o aplicativo, você concorda com as práticas descritas abaixo.

Esta política está em conformidade com a **Lei Geral de Proteção de Dados Pessoais (LGPD — Lei 13.709/2018)** e com as políticas da Google Play Store.

---

## 1. Quem somos

O **ViaCiclo** é mantido por:

**Vinicius Brasil Sanchez**
Microempreendedor Individual (MEI)
CNPJ: **65.139.333/0001-41**
Email de contato e encarregado de dados (DPO): **viniciusbrasil.30@gmail.com**

Qualquer dúvida, solicitação ou exercício de direitos previstos na LGPD deve ser enviada para este email.

---

## 2. Dados que coletamos

### 2.1. Dados fornecidos pelo login com Google (OAuth)

Quando você entra com sua conta Google, recebemos do Google os seguintes dados básicos:

- Nome completo
- Endereço de email
- Foto de perfil (avatar)
- Identificador único da conta Google

Não recebemos sua senha do Google em nenhum momento.

### 2.2. Dados de localização (GPS)

Enquanto você utiliza a funcionalidade **"Pedalar"** (rastreamento de pedaladas), o aplicativo coleta:

- Coordenadas geográficas (latitude e longitude) em tempo real
- Altitude (quando disponível), velocidade e timestamp de cada ponto
- Distância percorrida, tempo total, velocidade média

A coleta de GPS **só ocorre enquanto o tracking está ativo** e você **pode parar a qualquer momento**. Em nenhum outro momento o app coleta sua localização em segundo plano.

### 2.3. Dados de uso do aplicativo

- Pedaladas registradas (rotas completas em formato de pontos geográficos)
- Rotas compartilhadas publicamente (se você optar por compartilhá-las)
- Curtidas em rotas de outros usuários
- Pontos, nível e estatísticas de uso (quilômetros acumulados, número de pedaladas)

### 2.4. Dados armazenados localmente no dispositivo

- Cache de blocos de mapa (tiles) para funcionamento offline
- Preferência de tema (claro/escuro/sistema)
- Flag de onboarding já visto
- Token de sessão (para manter você logado)

---

## 3. Para que usamos seus dados

| Dado | Finalidade |
|------|-----------|
| Nome, email, foto do Google | Criar sua conta, exibir seu perfil |
| GPS em tempo real | Calcular distância, velocidade e traçar sua rota no mapa |
| Pedaladas salvas | Mostrar seu histórico pessoal e calcular pontos/nível |
| Rotas compartilhadas | Exibir rotas na aba Social para outros ciclistas |
| Pontos e estatísticas | Exibir ranking (leaderboard) e gamificação |
| Cache de mapa local | Permitir uso do app sem rede |

**Não utilizamos seus dados para publicidade, venda ou marketing de terceiros.**

---

## 4. Com quem compartilhamos

Seus dados pessoais **não são vendidos**. Compartilhamos apenas o estritamente necessário com os seguintes serviços:

- **Google (autenticação OAuth)** — Para permitir login com sua conta Google. Veja a [Política de Privacidade do Google](https://policies.google.com/privacy).
- **Supabase (banco de dados)** — Hospedagem segura dos dados de conta, pedaladas e rotas, na região **sa-east-1 (São Paulo)**. Veja a [Política de Privacidade do Supabase](https://supabase.com/privacy).
- **OpenRouteService** — Recebe apenas coordenadas de origem e destino quando você calcula uma rota. Não recebe dados de identificação.
- **OpenStreetMap** — Serve os blocos de mapa. Não recebe dados pessoais, apenas as coordenadas das áreas visualizadas.

Nenhum desses serviços recebe dados além do necessário para sua função.

---

## 5. Visibilidade dos dados dentro do app

- Seu **histórico pessoal** de pedaladas é **privado** e só você pode ver.
- Seu **nome, foto, pontos, nível e quilômetros totais** são **públicos** dentro do app (aparecem no leaderboard para outros usuários).
- **Rotas compartilhadas** por você são **públicas** por sua escolha ativa (aparecem na aba Social). Você pode deletar a qualquer momento.
- **Curtidas** são públicas (aparecem no contador da rota).

---

## 6. Segurança

Utilizamos as seguintes medidas de segurança:

- Comunicação criptografada via HTTPS/TLS com todos os serviços
- Autenticação baseada em tokens JWT (OAuth 2.0 + PKCE)
- **Row Level Security (RLS)** no banco Supabase, garantindo que cada usuário só acessa seus próprios dados privados
- Dados hospedados em servidores em solo brasileiro (sa-east-1)

Apesar das medidas, nenhum sistema é 100% seguro. Em caso de incidente de segurança que afete seus dados, você será notificado por email.

---

## 7. Retenção de dados

- **Enquanto sua conta estiver ativa:** todos os dados ficam armazenados.
- **Após exclusão da conta:** todos os dados pessoais são removidos em até 30 dias, exceto quando a lei exigir retenção.
- **Cache local no celular:** removido ao desinstalar o app ou limpar manualmente nas configurações.

---

## 8. Seus direitos (LGPD)

Você tem direito a, a qualquer momento:

1. **Acessar** seus dados pessoais
2. **Corrigir** dados incorretos ou desatualizados
3. **Exportar** seus dados em formato legível (ex: GPX das suas pedaladas — já disponível diretamente no app)
4. **Excluir** sua conta e todos os dados associados
5. **Revogar consentimento** para coleta de novos dados
6. **Obter informação** sobre com quem seus dados foram compartilhados
7. **Opor-se** a tratamentos específicos

Para exercer qualquer desses direitos, envie um email para **viniciusbrasil.30@gmail.com** com o assunto "LGPD — [seu pedido]". O prazo de resposta é de **até 15 dias**.

---

## 9. Crianças e adolescentes

O ViaCiclo não é direcionado a menores de 13 anos. Se tomarmos conhecimento de que uma conta pertence a um menor de 13 anos sem consentimento dos responsáveis, a conta será removida.

---

## 10. Alterações nesta política

Podemos atualizar esta Política de Privacidade periodicamente. Alterações significativas serão comunicadas por email ou notificação dentro do app, com no mínimo 15 dias de antecedência. A data da última atualização aparece no topo desta página.

---

## 11. Lei aplicável e foro

Esta política é regida pelas leis da República Federativa do Brasil. Fica eleito o foro da comarca de São Paulo/SP para dirimir eventuais conflitos.

---

*Documento vigente a partir de 20 de abril de 2026.*
