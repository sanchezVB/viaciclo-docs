---
title: Política de Privacidade — ViaCiclo
---

# Política de Privacidade

**Última atualização:** 12 de maio de 2026

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

### 2.4. Contatos de emergência (Crash Detection)

Se você ativar a funcionalidade **Crash Detection** em *Configurações → Contatos de emergência*, coletamos para cada contato cadastrado:

- Nome
- Telefone
- Relacionamento (opcional)

Limite máximo: **3 contatos**. Os contatos só são usados quando você toca em "Chamar contato de emergência" no alerta de queda detectada — o app abre o discador do Android com o número pré-preenchido e **você** confirma a chamada com o botão verde do discador. **O ViaCiclo não disca nem envia mensagens automaticamente** — todas as ligações são iniciadas manualmente por você.

Os números **nunca** são enviados a terceiros nem incluídos em telemetria. Ficam armazenados apenas na sua conta no Supabase (sa-east-1) protegidos por Row Level Security.

### 2.5. Eventos de detecção de queda

Quando a Crash Detection identifica uma possível queda, registramos:

- Localização aproximada do evento
- Pico de aceleração medido
- Sua resposta ao alerta ("estou bem", "chamei contato", "falso alarme", etc.)
- Opcionalmente, o **trace de aceleração** dos 5 segundos anteriores (toggle "Compartilhar trace anônimo" — ligado por padrão para ajudar a calibrar o algoritmo, pode ser desligado a qualquer momento).

O trace é **anônimo** quando agregado para análise de calibração e nunca é compartilhado fora do nosso banco de dados.

### 2.6. Reports de segurança e Modo "Rotas mais seguras"

#### 2.6.1. Reports de segurança (todos os tipos)

Se você reportar uma ocorrência usando o botão de reporte do app (ícone
de aviso), coletamos:

- Localização aproximada do ponto reportado (coordenada geográfica)
- Data e horário do reporte
- Tipo do incidente: **assédio**, **acidente próximo (near-miss)**,
  **pavimento ruim**, **furto/roubo** ou outras categorias declaradas
  no momento do reporte
- Severidade ("leve", "grave", "fatal") quando aplicável
- Descrição livre opcional (até 500 caracteres)
- Flag "anônimo" — **ligada por padrão**

**Visibilidade pública dos reports:**

- Quando o reporte é **anônimo** (padrão), a descrição livre nunca é
  exibida a outros usuários — só o tipo + a localização agregada.
- Quando você desmarca o anônimo, a descrição passa a aparecer na
  visualização pública do report (sem seu nome, mas com a descrição).
- Em ambos os casos, **seu identificador de usuário nunca é exposto**
  publicamente, e o horário exato vira só "mês" na visualização pública.

#### 2.6.2. Flag opt-in "Rotas mais seguras" (Modo Mulher)

Em **Perfil → Segurança** existe um toggle chamado **"Rotas mais seguras"**.
Ele está **desligado por padrão** e armazena uma flag privada no seu
perfil (`prefers_safer_routes`).

Quando você liga este toggle:

- Suas rotas calculadas tentam **evitar áreas com histórico agregado
  de reports de assédio** (mapa interno baseado em §2.6.1).
- A flag em si **nunca é exibida publicamente** — outros usuários, o
  leaderboard e qualquer view agregada **não conseguem ver** que você
  tem essa preferência ativada. É um dado estritamente privado da sua
  conta.

**Como protegemos os dados agregados de assédio:**

- Reports de assédio são tratados de forma **sempre agregada**. Nenhum
  relatório individual é exibido para outros usuários.
- Só exibimos uma área no mapa quando **pelo menos 10 usuários diferentes**
  reportaram aquela região — isso impede que um relatório isolado possa
  identificar a pessoa que o fez.
- A granularidade temporal é mensal (nunca exibimos a hora exata) e a área
  mínima é uma célula de ~110 m × ~110 m — não exibimos o ponto preciso
  do report.
- Dados são considerados para o mapa por uma **janela de 180 dias**;
  reports mais antigos deixam de influenciar o roteamento.

Você pode desativar o Modo "Rotas mais seguras" a qualquer momento no
mesmo toggle (Perfil → Segurança → "Rotas mais seguras"), e pode pedir
exclusão dos seus reports a qualquer momento via o email do DPO (§1).

### 2.7. Dados armazenados localmente no dispositivo

- Cache de blocos de mapa (tiles) para funcionamento offline
- Preferência de tema (claro/escuro/sistema)
- Flag de onboarding já visto
- Token de sessão (para manter você logado)

### 2.8. Eventos internos de uso (analytics privacy-first)

O app registra eventos agregados de uso **dentro do nosso próprio
servidor** (Supabase) para melhorar segurança, calibrar a pontuação de
rotas e detectar problemas de UX. **Não usamos Firebase Analytics,
Google Analytics, Mixpanel nem qualquer ferramenta de terceiros.**

Exemplos de eventos: "rota gerada", "pedalada finalizada", "Modo
seguro ativado". Para cada evento salvamos no máximo:

- Identificador anônimo de sessão (gerado quando o app abre, não
  sobrevive a reinstalações)
- Nome do evento (ex.: `route_completed`)
- Tela onde ocorreu (ex.: `tracking`)
- Métricas numéricas agregadas (ex.: distância em km, score médio
  calculado, perfil de rota escolhido)

**Não salvamos** nesses eventos: coordenadas GPS, trajetos completos,
seu email, telefone, identificador de dispositivo, texto livre digitado
por você ou qualquer dado que permita reidentificação.

### 2.9. Feedback que você envia voluntariamente

Quando você toca em **"Reportar problema"** no Perfil ou responde ao
modal de feedback após uma pedalada, salvamos:

- Sua avaliação (👍/😐/👎) e categoria escolhida
- Mensagem opcional que você digitar (até 2.000 caracteres)
- Identificador da pedalada associada (se aplicável)
- Métricas numéricas agregadas da rota (distância, score calculado,
  perfil), **sem coordenadas GPS**

Esse feedback fica visível apenas para nós (mantenedores do app) e
para você mesmo. Não é compartilhado com outros usuários e não aparece
em nenhum ranking ou mapa público.

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
| Contatos de emergência | Discar manualmente em caso de queda detectada |
| Trace de aceleração (anônimo) | Calibrar o algoritmo de Crash Detection |
| Reports de assédio (localização + data, se "Rotas mais seguras" ativo) | Calcular áreas de avoidance para o roteamento; só exibidos em agregados com ≥ 10 contribuintes distintos |

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

<!--
Doc complementar (não destinado ao usuário final): a especificação técnica
interna da privacidade — princípios, RLS, k-anonymity, defaults — vive em
`docs/PRIVACY_INTERNAL.md`. Toda mudança de coleta/visibilidade deve
aparecer nos dois lugares de forma coerente.
-->

