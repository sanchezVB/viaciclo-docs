---
title: Política de Privacidade — ViaCiclo
---

# Política de Privacidade

**Última atualização:** 30 de setembro de 2026

Esta Política explica, em linguagem direta, quais dados pessoais o aplicativo
**ViaCiclo** trata, para quê, com quem compartilha, por quanto tempo guarda e
como você exerce seus direitos. Ela segue a **Lei Geral de Proteção de Dados
Pessoais (LGPD — Lei 13.709/2018)** e as regras da Google Play.

Um resumo antes do detalhe:

- **Não vendemos dados pessoais** e não usamos seus dados para publicidade.
- **Sua localização só é usada em segundo plano durante uma pedalada que você
  iniciou**, com uma notificação permanente na tela enquanto isso acontece.
- **Tudo o que protege você na rua é gratuito**, e usar esses recursos não
  depende de você aceitar usos extras dos seus dados.
- **Você pode excluir sua conta dentro do app**, a qualquer momento.

---

## 1. Quem é o responsável

O ViaCiclo é mantido por **Vinicius Brasil Sanchez**, CNPJ
**65.139.333/0001-41**, que é o **controlador** dos dados tratados pelo app.

**Encarregado de dados (DPO) e contato:** viaciclo.app@gmail.com

Dúvidas, pedidos e o exercício de qualquer direito previsto na LGPD vão para
esse e-mail.

---

## 2. Quais dados tratamos

### 2.1. Conta

Você pode entrar de duas formas:

- **Com o Google:** recebemos seu nome, e-mail, foto e o identificador da sua
  conta Google. Não recebemos sua senha do Google.
- **Com e-mail e senha:** guardamos seu e-mail e a senha em forma de *hash*
  (nunca em texto). Os e-mails de confirmação e de troca de senha são
  enviados pelo nosso provedor de banco de dados e autenticação (Supabase).

No perfil você pode ainda definir um **nome de exibição**, uma **foto** e uma
**bio** curta.

### 2.2. Localização

O app usa a localização do aparelho de duas formas, e só com a permissão que
você concedeu:

**Com o app aberto na tela (primeiro plano).** Para mostrar onde você está no
mapa, buscar ciclovias e alertas perto de você, sugerir resultados de busca
próximos e calcular rotas a partir da sua posição. Nesse uso a posição **não
é guardada** nos nossos servidores; ela é enviada apenas aos serviços que
fazem cada uma dessas tarefas (seção 4).

**Durante uma pedalada (inclusive em segundo plano).** Quando você toca em
"Iniciar", o app registra latitude, longitude, altitude, velocidade e horário
de cada ponto, e calcula distância, tempo e velocidade média. O registro
continua com a tela bloqueada ou o app em segundo plano — senão a rota ficaria
cortada toda vez que o celular fosse para o bolso. Nesse período o Android
mostra uma **notificação permanente** avisando que o ViaCiclo está usando sua
localização. Ao encerrar a pedalada, a notificação some e o registro para.

**Fora de uma pedalada ativa, o app não usa sua localização em segundo
plano.**

Se não houver internet ao terminar, a pedalada fica guardada no aparelho e é
enviada sozinha quando a conexão voltar.

### 2.3. Pedaladas, rotas compartilhadas, curtidas e ranking

- **Pedaladas:** o traçado completo e os números de cada pedalada que você
  salva. São **privadas**: só você as vê. Você pode apagar uma pedalada no
  histórico.
- **Rotas compartilhadas:** quando você escolhe compartilhar uma pedalada na
  aba Social, ela fica **visível para os outros usuários logados**, com o
  traçado completo, o nome da rota e seu nome de exibição. **O traçado mostra
  onde a pedalada começou e terminou** — evite compartilhar trajetos que
  saem ou chegam na sua casa. Você pode apagar a rota a qualquer momento.
- **Curtidas:** o registro de que você curtiu uma rota.
- **Ranking:** seu nome de exibição, foto, pontos, quilômetros e número de
  pedaladas aparecem no ranking para os outros usuários logados.

### 2.4. Relatos de segurança

Quando você usa o botão de reportar, guardamos: o tipo do relato (quase
acidente, assédio, pavimento ruim, iluminação ruim, motorista perigoso,
obstrução, área de furto), a gravidade, a localização, a data e a hora, uma
descrição opcional (até 500 caracteres) e a opção "anônimo" (**ligada por
padrão**).

**Como os outros usuários veem seus relatos:**

- **Nunca** mostramos quem fez o relato.
- A **descrição** só aparece se você desligou o "anônimo".
- Relatos recentes aparecem como **alertas no mapa e durante a pedalada**,
  com a posição e uma faixa de tempo aproximada ("agora", "há poucas horas",
  "hoje", "esta semana") — nunca o horário exato.
- **Relatos de assédio nunca aparecem individualmente.** Eles só entram no
  mapa de forma agregada: uma área (célula de cerca de 110 m × 110 m) só é
  exibida quando **pelo menos 10 pessoas diferentes** relataram assédio ali,
  considerando os últimos 180 dias.

### 2.5. Modo "Rotas mais seguras" (Modo Mulher)

Em **Perfil → Segurança**, o ajuste "Rotas mais seguras" vem **desligado**.
Ligado, suas rotas passam a evitar as áreas agregadas de relatos de assédio
descritas acima. A escolha fica guardada no seu perfil e é **visível só para
você** — outros usuários, o ranking e as telas públicas não a veem.

### 2.6. Detecção de queda e contatos de emergência

A detecção de queda é **opcional** e vem desligada. Para ativá-la você
cadastra de 1 a 3 contatos de emergência (nome, telefone e, se quiser,
relação com você).

Quando o celular percebe uma possível queda, o app pergunta se você está bem
e oferece ligar para o seu contato ou para o SAMU (192). **O app não disca nem
manda mensagem sozinho**: ele abre o discador com o número, e é você quem
confirma a ligação. O alerta é gerado dentro do próprio aparelho.

De cada evento guardamos a localização, o pico de aceleração, a sua resposta
("estou bem", "liguei", "falso alarme") e, se a opção **"Compartilhar trace
para calibração"** estiver ligada (padrão ligado, pode ser desligada), os
dados do acelerômetro dos 5 segundos anteriores. Esse trace fica ligado à sua
conta no nosso banco e só é analisado em conjunto com outros, para melhorar a
detecção.

Os telefones dos seus contatos **não** são enviados a terceiros nem entram em
relatórios técnicos.

Um evento de queda pode revelar algo sobre a sua saúde. Por isso esse
tratamento só acontece com o seu consentimento, dado ao ativar o recurso, e
pode ser revogado desligando-o.

### 2.7. Avaliações e feedback

Depois de uma pedalada o app pode perguntar como foi a rota. Se você
responder, guardamos a nota, as categorias escolhidas, uma mensagem opcional
(até 2.000 caracteres), a pedalada a que se refere e números da rota
(distância, duração, perfil, nota de segurança calculada, hora do dia e dia
da semana). **Sem coordenadas.** O mesmo vale para "Reportar problema" no
Perfil.

Essas respostas são o que usamos para **calibrar o Safety Score** —
comparar o que o app estimou com o que quem pedalou sentiu. Elas ficam
visíveis **apenas para você e para a equipe do ViaCiclo**; não aparecem para
outros usuários.

### 2.8. CoPiloto (assistente de IA)

O CoPiloto é um assistente opcional sobre pedalar com segurança. Ele só
recebe dados quando você envia uma mensagem. Nesse momento são transmitidos
ao nosso serviço de IA:

- o **texto** que você escreveu;
- sua **localização aproximada**, quando disponível, para a resposta
  considerar onde você está;
- a rota em questão, quando a conversa parte de uma rota.

**As conversas ficam guardadas**, ligadas à sua conta, para o assistente
manter o contexto e para melhorarmos as respostas. Sua localização é usada
para responder e não é guardada junto da conversa. Se você avaliar uma
resposta (útil / não útil), guardamos essa avaliação.

O texto é processado por modelos de linguagem de **provedores contratados**
(seção 4). Para perguntas que dependem de informação atual, o assistente pode
fazer buscas na web; nesse caso, só os **termos da busca** são enviados ao
serviço de busca, sem dados da sua conta.

**Não escreva no CoPiloto dados sensíveis** — documentos, senhas, dados de
saúde ou informações de outras pessoas.

Se você nunca usar o CoPiloto, nada é enviado a esse serviço.

### 2.9. ViaCiclo Explorers

O Explorers é um programa **opcional** em que ciclistas aprovados recebem
para percorrer trajetos definidos e avaliá-los. Quem participa tem dados
tratados além dos já descritos:

- **Candidatura:** região, texto de motivação (até 500 caracteres) e o seu
  consentimento para o uso das pedaladas e avaliações do programa na
  calibração do Safety Score.
- **Situação no programa:** status (candidato, aprovado, pausado), nível e
  uma nota de qualidade das entregas, usados para organizar as missões.
- **Missões:** quais você aceitou, a pedalada que você vinculou a cada uma,
  o resultado da validação e a **avaliação por fator** (notas de 0 a 10 para
  espaço, trânsito, motoristas, pavimento, iluminação e movimento).
- **Pagamento:** sua **chave Pix**, o tipo da chave e o **nome do titular**.
  Guardamos também o registro de cada repasse: valor, data, situação e o
  identificador da transação Pix. Não guardamos comprovantes em imagem.

**Quem vê esses dados:** você e a **equipe de operação** do programa, que
aprova candidaturas, valida missões e faz os pagamentos. Quando alguém se
candidata, a operação recebe um aviso por e-mail com o e-mail, a região e a
motivação da candidatura.

**Separação:** a chave Pix e os dados de contato ficam **separados** dos
dados de análise. Eles não entram em estatística, mapa ou base de
calibração.

### 2.10. Eventos de uso do app

O app registra eventos de uso **no nosso próprio banco** — por exemplo
"rota gerada", "pedalada finalizada", "detecção de queda ativada" — para
melhorar a segurança, calibrar as notas e achar problemas de uso. Cada
evento traz: sua conta, um identificador da sessão de uso, o nome do evento,
a tela e números agregados (como distância em km, nota média da rota, perfil
escolhido).

**Não** registramos nesses eventos coordenadas, trajetos, textos que você
digitou, e-mail ou telefone. **Não** usamos ferramentas de analytics,
publicidade ou atribuição de terceiros (nem Firebase Analytics, Google
Analytics, Mixpanel ou equivalentes).

### 2.11. Relatórios técnicos de falhas e de desempenho

Quando o app apresenta um erro, enviamos um relatório técnico ao Sentry:
tipo do erro, versão do app, modelo e sistema do aparelho e a sequência de
ações técnicas que antecedeu o problema (por exemplo, o nome das telas
abertas). Também medimos, por amostragem, se as telas estão rodando sem
travar. O envio de dados pessoais está **desligado** na configuração: esses
relatórios não levam seu nome, e-mail, localização ou endereços.

### 2.12. Notificações

O app pode enviar notificações (por exemplo, quando alguém interage com uma
rota sua). A permissão é pedida **quando você abre a aba Social pela
primeira vez**; recusar não afeta o resto do app.

Com a permissão, o Firebase Cloud Messaging (Google) gera no aparelho um
**identificador de entrega**. Guardamos esse identificador no seu perfil,
apenas para endereçar as notificações. Ele não contém nome, e-mail, telefone
nem localização, e é **apagado ao sair da conta**.

### 2.13. Área de transferência e destinos vindos de outros apps

- **Área de transferência:** quando você toca no campo de busca, o app
  confere se o que você copiou parece um endereço e, se parecer, oferece
  usá-lo como destino. Isso acontece **só quando você toca na busca**, e o
  conteúdo não sai do aparelho a menos que você escolha usá-lo.
- **Compartilhar para o ViaCiclo:** você pode enviar um endereço ou link de
  mapa de outro app para o ViaCiclo. O conteúdo recebido é lido no aparelho
  para achar o destino. **Não guardamos** esses endereços nos nossos
  servidores nem os registramos em relatórios técnicos ou eventos de uso.

### 2.14. Câmera e galeria

Para trocar a foto do perfil, o app pede acesso à galeria ou à câmera **só na
hora** em que você toca para escolher a foto, e envia apenas a imagem
escolhida. A foto fica num endereço público de imagem, para aparecer no
ranking.

### 2.15. Dados guardados no aparelho

- Sessão de login (para você não precisar entrar toda vez)
- Preferências (tema, estilo do mapa, perfil de rota e ajustes de
  navegação)
- Mapas baixados para uso sem internet
- Cópia das ciclovias da sua região, para o mapa abrir rápido e funcionar sem
  rede
- Pedaladas ainda não enviadas por falta de conexão

Tudo isso sai ao desinstalar o app ou limpar os dados dele nas configurações
do Android.

---

## 3. Para que usamos, e com que base legal

| Finalidade | Dados | Base legal (LGPD) |
|---|---|---|
| Criar e manter sua conta | conta, perfil | execução do contrato (art. 7º, V) |
| Mostrar o mapa, calcular rotas, buscar destinos | localização em primeiro plano, texto da busca | execução do contrato |
| Registrar e mostrar suas pedaladas | localização durante a pedalada, pedaladas | execução do contrato |
| Rotas compartilhadas, curtidas e ranking | rotas, nome, foto, pontos | execução do contrato, a partir da sua escolha de compartilhar |
| Alertas de segurança e mapa de assédio agregado | relatos | consentimento, dado ao enviar o relato (art. 7º, I) |
| Detecção de queda e contatos de emergência | eventos de queda, contatos | consentimento, dado ao ativar o recurso (art. 11, I) |
| Calibrar o Safety Score e a detecção de queda | avaliações, eventos de queda, pedaladas do Explorers | legítimo interesse em tornar as rotas mais seguras (art. 7º, IX) e, no Explorers, consentimento |
| Responder no CoPiloto | mensagens, localização aproximada | execução do contrato, quando você usa o recurso |
| Operar e pagar o Explorers | candidatura, missões, chave Pix | execução do contrato (art. 7º, V) |
| Guardar os registros de pagamento | repasses do Explorers | cumprimento de obrigação legal (art. 7º, II) |
| Achar erros e melhorar o app | eventos de uso, relatórios técnicos | legítimo interesse (art. 7º, IX) |
| Enviar notificações | identificador de entrega | consentimento, dado na permissão do Android |

**Não usamos seus dados para publicidade**, não os vendemos e não traçamos
perfis de você para terceiros.

**Estatísticas anonimizadas.** Podemos publicar ou compartilhar com
prefeituras, órgãos públicos, pesquisadores e parceiros **estatísticas
agregadas e anonimizadas** — por exemplo, a nota de segurança de um trecho
de rua ou o volume de ciclistas numa região. Esses conjuntos não permitem
identificar ninguém e, por isso, deixam de ser dados pessoais (art. 12 da
LGPD).

**Decisões automatizadas.** A nota de segurança das ruas e a ordem das rotas
sugeridas são calculadas automaticamente. Elas são uma sugestão: você sempre
pode escolher outra rota. Se quiser entender como uma nota foi calculada ou
pedir revisão, escreva para o encarregado (art. 20 da LGPD).

---

## 4. Com quem compartilhamos

Compartilhamos só o necessário para cada serviço funcionar:

| Serviço | O que recebe | Para quê | Onde |
|---|---|---|---|
| **Supabase** | todos os dados da sua conta descritos acima | banco de dados, autenticação e arquivos | Brasil (São Paulo) |
| **Google** (login) | o vínculo com sua conta Google | entrar com o Google | EUA |
| **Firebase Cloud Messaging** (Google) | identificador de entrega e conteúdo da notificação | entregar notificações | EUA |
| **Google Cloud** | mensagens do CoPiloto em trânsito | hospedar o serviço de IA | Brasil (São Paulo) |
| **Groq** | texto das mensagens do CoPiloto | gerar as respostas do assistente | EUA |
| **Serviços de busca na web** (como Tavily ou Brave) | termos de busca, quando o CoPiloto precisa pesquisar | informação atual para a resposta | EUA |
| **Mapbox** | áreas do mapa visualizadas, texto de busca com posição aproximada, origem e destino de rotas | mapa, busca de endereços e cálculo de rotas | EUA |
| **HERE** | texto de busca e posição aproximada | busca de endereços | União Europeia |
| **openrouteservice** (HeiGIT) | origem e destino de rotas; texto de busca | cálculo de rotas e busca de endereços | Alemanha |
| **OpenStreetMap** (Fundação OSM) | áreas do mapa visualizadas; texto de busca com posição aproximada | mapa e busca de endereços | Reino Unido / UE |
| **Overpass API** (servidores públicos do OpenStreetMap) | a área de cerca de 20 km em volta da sua posição | baixar as ciclovias da região | Alemanha e outros |
| **Sentry** | relatórios técnicos, sem dados pessoais | achar e corrigir falhas | EUA |
| **Resend** | e-mail, região e motivação de quem se candidata ao Explorers | avisar a operação por e-mail | EUA |

Nenhum desses serviços recebe seu nome junto com a sua localização, exceto o
Supabase, onde sua conta está guardada.

**Telemetria do Mapbox.** O mapa 3D da pedalada usa o SDK do Mapbox, que por
padrão envia ao Mapbox dados de uso e de localização **anônimos** para
melhorar os mapas dele. Você pode desligar isso tocando no ícone **ⓘ** no
canto do mapa e escolhendo desativar a telemetria. Veja a [política do
Mapbox](https://www.mapbox.com/legal/privacy).

**Transferência internacional.** Parte desses serviços fica fora do Brasil.
Essas transferências são feitas porque são necessárias para prestar o
serviço que você pediu (art. 33, IX da LGPD) e com fornecedores que adotam
padrões de proteção de dados compatíveis com a LGPD.

**Autoridades.** Podemos fornecer dados quando a lei ou uma ordem judicial
exigir, limitados ao que foi pedido.

---

## 5. O que os outros usuários veem

| Dado | Quem vê |
|---|---|
| Suas pedaladas | só você |
| Rotas que você compartilhou | usuários logados — traçado, nome da rota, seu nome de exibição |
| Nome de exibição, foto, pontos, km e nº de pedaladas | usuários logados, no ranking |
| Seus relatos (exceto assédio) | usuários logados, como alerta — sem autoria; descrição só se não for anônimo |
| Relatos de assédio | ninguém individualmente; só áreas agregadas com 10+ pessoas |
| "Rotas mais seguras", bio, e-mail, contatos, avaliações, conversas do CoPiloto, chave Pix | só você (e, nos dados do Explorers, a operação) |

Nada disso é aberto para quem não tem conta.

---

## 6. Segurança

- Conexões criptografadas (HTTPS/TLS) com todos os serviços
- Senhas guardadas só em *hash*
- **Regras de acesso no banco (Row Level Security)**: cada pessoa só consegue
  ler os próprios dados privados, e o que é público sai por consultas que
  devolvem apenas os campos públicos
- Dados de pagamento do Explorers separados dos dados de análise
- Banco de dados hospedado no Brasil

Nenhum sistema é totalmente seguro. Se acontecer um incidente de segurança que
possa causar risco ou dano relevante a você, avisaremos você e a Autoridade
Nacional de Proteção de Dados (ANPD), como a lei determina.

---

## 7. Por quanto tempo guardamos

| Dado | Por quanto tempo |
|---|---|
| Conta, perfil, pedaladas, rotas, curtidas, relatos, avaliações, eventos de queda, contatos, eventos de uso e conversas do CoPiloto | enquanto sua conta existir |
| Relatos de assédio | enquanto sua conta existir; só os dos últimos 180 dias influenciam as rotas |
| Registros de pagamento do Explorers | pelo prazo exigido pela legislação fiscal e contábil (em regra, 5 anos), mesmo após a exclusão da conta |
| Relatórios técnicos (Sentry) | até 90 dias |
| Identificador de notificação | até você sair da conta |
| Dados no aparelho | até desinstalar o app ou limpar os dados dele |

**Ao excluir sua conta**, apagamos na hora: perfil, foto, pedaladas, rotas
compartilhadas (que saem do feed), curtidas, relatos, contatos, eventos de
queda, avaliações, eventos de uso, conversas do CoPiloto e os dados do
Explorers — exceto os registros de pagamento acima. Cópias de segurança do
banco são sobrescritas em até 30 dias. Estatísticas já anonimizadas não
identificam ninguém e não precisam ser apagadas.

---

## 8. Seus direitos

A qualquer momento você pode pedir:

1. **confirmação** de que tratamos seus dados, e **acesso** a eles;
2. **correção** de dados incompletos, errados ou desatualizados;
3. **anonimização, bloqueio ou eliminação** de dados desnecessários ou
   tratados em desacordo com a LGPD;
4. **portabilidade** dos seus dados;
5. **eliminação** dos dados tratados com base no seu consentimento;
6. **informação** sobre com quem compartilhamos seus dados;
7. **informação** sobre a possibilidade de não consentir, e o que acontece
   se você não consentir;
8. **revogação do consentimento**;
9. **revisão** de decisões tomadas só com base em tratamento automatizado;
10. **oposição** a um tratamento feito sem consentimento, se ele descumprir a
    LGPD.

**Muita coisa você faz direto no app:**

- **Excluir a conta:** Perfil → Apagar conta
- **Corrigir** nome, foto e bio: Perfil → Editar
- **Exportar** suas pedaladas em GPX: no histórico
- **Apagar** uma pedalada ou uma rota compartilhada
- **Revogar consentimentos:** desligar a detecção de queda, o
  compartilhamento do trace, o Modo "Rotas mais seguras" e as notificações;
  apagar contatos de emergência

Para o resto, escreva para **viaciclo.app@gmail.com** com o assunto
"LGPD — [seu pedido]". Respondemos em até **15 dias**. Você também pode
reclamar à **ANPD** (gov.br/anpd).

---

## 9. Crianças e adolescentes

O ViaCiclo não é destinado a menores de **13 anos**. Se soubermos de uma conta
de um menor de 13 anos sem consentimento dos responsáveis, ela será excluída.
O **ViaCiclo Explorers** é só para maiores de **18 anos**.

---

## 10. Mudanças nesta política

Quando esta política mudar de forma relevante, avisaremos por e-mail ou no app
com pelo menos **15 dias** de antecedência. A data da última atualização fica
no topo desta página.

---

## 11. Lei aplicável

Esta política segue as leis do Brasil.

---

### O que mudou em 30 de setembro de 2026

- Novas seções sobre o **ViaCiclo Explorers** (candidatura, missões e dados de
  pagamento) e sobre o **armazenamento das conversas do CoPiloto** e o
  provedor que gera as respostas.
- Descrevemos o uso da localização **com o app aberto**, fora de uma
  pedalada, que a versão anterior não detalhava.
- Lista completa dos serviços que recebem dados — inclusive busca de
  endereços, cálculo de rotas, ciclovias, telemetria do Mapbox e o aviso por
  e-mail do Explorers — com o país de cada um.
- Bases legais, transferência internacional, estatísticas anonimizadas e
  decisões automatizadas.
- Login com **e-mail e senha**, bio no perfil, área de transferência e
  destinos compartilhados por outros apps.
- Eventos de uso **ligados à sua conta** (a versão anterior falava só em
  identificador de sessão).
- **Exclusão de conta pelo app**, o que é apagado e o que a lei manda guardar.
- Correções no banco de dados para cumprir o que esta política promete:
  relatos de assédio nunca mais aparecem um a um; o ajuste "Rotas mais
  seguras" e o identificador de notificação deixaram de ser legíveis por
  outros usuários; avaliações ficaram visíveis só para você e para a equipe;
  a exclusão de conta passou a apagar pedaladas e rotas compartilhadas.

*Primeira versão: 20 de abril de 2026.*

<!--
Doc complementar (não destinado ao usuário final): a especificação técnica
interna da privacidade — princípios, RLS, k-anonymity, defaults — vive em
`docs/PRIVACY_INTERNAL.md` no repositório do app. Toda mudança de
coleta/visibilidade deve aparecer nos dois lugares de forma coerente, e no
resumo in-app (`lib/screens/about/privacy_policy_screen.dart`).
-->
