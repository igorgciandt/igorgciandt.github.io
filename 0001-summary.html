<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>SmartContracts → App Standalone · Resumo da ADR 0001</title>
<style>
  /* Palette = B2O / Sodexo Design System (chakraThemes.ts): sodexo-blue #283897, red.600 #DA2020, green.600 #2A8652, gold #BD8E39 */
  :root{
    --bg:#eef1f9; --panel:#ffffff; --panel2:#f6f8fd; --ink:#16181d; --muted:#5c5c5c;
    --line:#e4e4e7; --line2:#e7e9f7;
    --accent:#283897; --accent-dark:#1a3478; --ultra-light:#e7e9f7;
    --ok:#2a8652; --ok-bg:#d3f1e0; --warn:#a9772a; --warn-bg:#feefd3;
    --crit:#da2020; --crit-bg:#fdeaea; --crit-line:#f3b6b6;
    --blue-soft:#d1ebf8; --blue-line:#173da6;
  }
  *{box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{margin:0;background:var(--bg);color:var(--ink);
    font:15px/1.55 -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;}
  .wrap{max-width:1040px;margin:0 auto;padding:32px 20px 80px}
  a{color:var(--accent);text-decoration:none}
  header.hero{border:1px solid var(--line2);border-left:5px solid var(--accent);border-radius:18px;padding:28px 28px 24px;
    background:radial-gradient(1100px 320px at 0% 0%,rgba(40,56,151,.10),transparent),var(--panel);
    box-shadow:0 4px 16px rgba(40,56,151,.06)}
  .eyebrow{letter-spacing:.14em;text-transform:uppercase;font-size:12px;color:var(--accent);font-weight:700}
  h1{margin:.35em 0 .15em;font-size:30px;line-height:1.15;color:var(--accent)}
  .sub{color:var(--muted);font-size:15px;max-width:70ch}
  .badges{display:flex;gap:8px;flex-wrap:wrap;margin-top:16px}
  .badge{font-size:12px;font-weight:600;padding:5px 11px;border-radius:999px;border:1px solid var(--line2);background:var(--panel2);color:var(--muted)}
  .badge.status{background:var(--ultra-light);border-color:#c7cdf0;color:var(--accent-dark)}
  .stats{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin:22px 0 6px}
  .stat{border:1px solid var(--line2);border-radius:14px;padding:16px;background:var(--panel);box-shadow:0 2px 8px rgba(0,0,0,.04)}
  .stat .n{font-size:30px;font-weight:800;line-height:1;color:var(--ink)}
  .stat .n.crit{color:var(--crit)} .stat .n.ok{color:var(--ok)} .stat .n.acc{color:var(--accent)}
  .stat .l{color:var(--muted);font-size:12.5px;margin-top:6px}
  section{margin-top:34px}
  h2{font-size:19px;margin:0 0 6px;display:flex;align-items:center;gap:9px;color:var(--accent-dark)}
  h2 .k{font-size:12px;color:#fff;background:var(--accent);border-radius:6px;padding:2px 7px;font-weight:800}
  .lead{color:var(--muted);margin:.2em 0 16px;max-width:78ch}
  .card{border:1px solid var(--line2);border-radius:14px;background:var(--panel);padding:18px 20px;box-shadow:0 2px 10px rgba(0,0,0,.04)}
  code{background:var(--ultra-light);color:var(--accent-dark);padding:1px 5px;border-radius:5px;font-size:.92em}
  table{width:100%;border-collapse:collapse;font-size:14px}
  th,td{text-align:left;padding:10px 12px;border-bottom:1px solid var(--line);vertical-align:top}
  th{color:var(--accent-dark);font-weight:700;font-size:12.5px;text-transform:uppercase;letter-spacing:.04em}
  tr:last-child td{border-bottom:none}
  .pill{font-size:11.5px;font-weight:700;padding:3px 9px;border-radius:999px;white-space:nowrap}
  .copy{background:var(--ok-bg);color:#1f653d}
  .rebuild{background:var(--warn-bg);color:#8a5e18}
  .share{background:var(--blue-soft);color:var(--blue-line)}
  .keep{background:#eceef4;color:#505874}
  .dot{display:inline-block;width:9px;height:9px;border-radius:50%;margin-right:7px;vertical-align:middle}
  .d-crit{background:var(--crit)} .d-high{background:#e0a52e}
  .callout{border:1px solid var(--crit-line);border-left:5px solid var(--crit);border-radius:16px;padding:20px 22px;margin-top:6px;
    background:linear-gradient(180deg,var(--crit-bg),#fff);box-shadow:0 4px 14px rgba(218,32,32,.06)}
  .callout h3{margin:0 0 6px;font-size:16px;color:var(--crit)}
  .callout p{margin:.5em 0;color:#5a2222}
  .callout p code{background:#fbdcdc;color:#a01717}
  .callout .tag{font-size:11px;font-weight:800;letter-spacing:.1em;color:var(--crit);text-transform:uppercase}
  .today{color:var(--crit);font-weight:500}.tmrw{color:var(--ok);font-weight:600}
  ol.timeline{list-style:none;counter-reset:ph;padding:0;margin:8px 0 0}
  ol.timeline li{counter-increment:ph;position:relative;padding:14px 0 14px 52px;border-bottom:1px solid var(--line)}
  ol.timeline li:last-child{border-bottom:none}
  ol.timeline li::before{content:counter(ph);position:absolute;left:0;top:12px;width:34px;height:34px;
    border-radius:10px;background:var(--ultra-light);border:1px solid #c7cdf0;color:var(--accent);
    font-weight:800;display:grid;place-items:center}
  ol.timeline li.p0::before{background:var(--warn-bg);border-color:#eacf96;color:var(--warn)}
  .ph-t{font-weight:700;color:var(--ink)} .ph-d{color:var(--muted);font-size:13.5px}
  ul.q{margin:6px 0 0;padding-left:18px} ul.q li{margin:7px 0;color:#333}
  ul.q li b{color:var(--accent-dark)}
  footer{margin-top:40px;color:var(--muted);font-size:12.5px;text-align:center;border-top:1px solid var(--line2);padding-top:20px}
  .made{border:1px dashed #c7cdf0;border-radius:12px;padding:12px 16px;color:var(--muted);font-size:13px;background:var(--panel2);margin-top:18px}
  @media(max-width:760px){.stats{grid-template-columns:repeat(2,1fr)}h1{font-size:24px}}
  @media print{body{background:#fff}.card,.stat,header.hero{box-shadow:none}}
</style>
</head>
<body>
<div class="wrap">

  <header class="hero">
    <div class="eyebrow">SmartContracts · Decisão de Arquitetura</div>
    <h1>De módulo do MyApps → Aplicação Standalone</h1>
    <p class="sub">Resumo de uma página da <b>ADR 0001</b>. O SmartContracts deixa de ser um web
    component embutido no MyApps e passa a ser um app próprio. Este é o plano de migração — reusando
    o máximo possível do MyApps, com os pontos de falha já mapeados.</p>
    <div class="badges">
      <span class="badge status">Status: Proposta (decisão de ir standalone já fechada)</span>
      <span class="badge">2026-07-06</span>
      <span class="badge">Base: varredura do container B2OContainerApp</span>
    </div>
  </header>

  <div class="stats">
    <div class="stat"><div class="n acc">4</div><div class="l">pilares que o SC passa a ter que ter sozinho</div></div>
    <div class="stat"><div class="n ok">6</div><div class="l">fases, verde e deployável a cada passo</div></div>
    <div class="stat"><div class="n crit">14</div><div class="l">pontos de falha pegos na revisão adversarial</div></div>
    <div class="stat"><div class="n">1</div><div class="l">gotcha crítico que quebraria o login</div></div>
  </div>

  <section>
    <h2><span class="k">1</span> A ideia em 30 segundos</h2>
    <p class="lead">MyApps é o <b>shopping</b>; SmartContracts é uma <b>loja dentro dele</b>. Hoje a
    loja usa a porta (login), os corredores (navegação), a placa (header/menu) e o banheiro
    (toasts/dialogs) do shopping. Virar standalone é abrir uma <b>loja de rua</b>: agora precisa de
    tudo isso por conta própria. A boa notícia: por dentro, o SC já tem Chakra, telemetria, i18n e
    cliente de API próprios. Só faltam quatro coisas — e são o trabalho inteiro.</p>
    <div class="card">
      <table>
        <thead><tr><th>#</th><th>Hoje recebe de graça do MyApps</th><th>Standalone precisa ter</th></tr></thead>
        <tbody>
          <tr><td>1</td><td class="today">Auth — recebe <code>accessToken</code>/<code>idToken</code> como props</td><td class="tmrw">Login próprio via MSAL (Azure AD)</td></tr>
          <tr><td>2</td><td class="today">Roteamento — MyApps decide a página</td><td class="tmrw">Router próprio para as 6 features</td></tr>
          <tr><td>3</td><td class="today">Chrome — reusa header + menu do MyApps</td><td class="tmrw">Header, menu e layout próprios</td></tr>
          <tr><td>4</td><td class="today">UI compartilhada — MyApps dona dos toasts/dialogs</td><td class="tmrw">Camada de toaster/dialog própria</td></tr>
        </tbody>
      </table>
    </div>
  </section>

  <section>
    <h2><span class="k">2</span> O gotcha que teria nos mordido</h2>
    <div class="callout">
      <div class="tag">◆ Crítico · apontado por 3 revisores independentes</div>
      <h3>Config do MSAL não pode usar o modelo de runtime do SC</h3>
      <p>O SC escolhe config <b>em tempo de execução</b> (os <code>env.*.json</code>). Tentador usar
      isso pro login também — mas o MSAL cria seu cliente <code>new PublicClientApplication()</code>
      <b>no carregamento do módulo</b>, antes do React renderizar. Não há como entregar o JSON a
      tempo.</p>
      <p><b>Resultado do erro:</b> quem copiar sem saber hardcoda o <code>clientId</code> de dev e
      <b>quebra o login silenciosamente em todos os outros ambientes</b> (erros <code>AADSTS</code>
      difíceis de debugar).</p>
      <p><b>Decisão:</b> os 4 valores <code>VITE_ENTRA_*</code> são <b>build-time</b>, um build por
      ambiente — exatamente como o MyApps já faz. Todo o resto continua em runtime.</p>
    </div>
  </section>

  <section>
    <h2><span class="k">3</span> Reusar vs. reconstruir</h2>
    <p class="lead">A regra: <span class="pill copy">copiar</span> arquivos pequenos e puros ·
    <span class="pill rebuild">reconstruir</span> o que está acoplado às entranhas do MyApps ·
    <span class="pill share">pacote</span> o que já é dependência · <span class="pill keep">manter</span> o que o SC já faz bem.</p>
    <div class="card">
      <table>
        <thead><tr><th>Peça</th><th>Decisão</th><th>Motivo (resumido)</th></tr></thead>
        <tbody>
          <tr><td>Setup MSAL (<code>msalConfig.ts</code>)</td><td><span class="pill copy">copiar</span></td><td>Estrutura genérica; valores vêm da infra, não do código</td></tr>
          <tr><td>Ciclo do token (<code>AuthContext</code>)</td><td><span class="pill rebuild">reconstruir</span></td><td>Monolito de 310 linhas acoplado ao router → dividir em <code>useMsalSession</code> + <code>AuthGuard</code></td></tr>
          <tr><td>Router + rotas</td><td><span class="pill rebuild">reconstruir</span></td><td>Já especificado no <code>docs/routing.md</code> do próprio SC</td></tr>
          <tr><td>Header / Navbar</td><td><span class="pill rebuild">reconstruir</span></td><td>Embutem módulos de outros times; manter só o esqueleto visual</td></tr>
          <tr><td>Componentes puros (mobile, mediaQuery)</td><td><span class="pill copy">copiar</span></td><td>Sem acoplamento — mas adicionar os tokens de tema antes</td></tr>
          <tr><td>FeedbackDialog (toasts)</td><td><span class="pill copy">copiar</span></td><td>Autocontido; exige tokens de cor no tema (senão fica invisível)</td></tr>
          <tr><td>Pipeline SWA, staticwebapp.config</td><td><span class="pill copy">copiar</span></td><td>Mesmo template DevOps; trocar o identificador do app</td></tr>
          <tr><td><code>@sdx/b2o-fe-tools</code> (permissões, flags, Piano)</td><td><span class="pill share">pacote</span></td><td>Já é dependência; <code>PermissionGate</code> depende do módulo <code>smartcontracts</code> ser publicado</td></tr>
          <tr><td>Telemetria, env config, cliente de API do SC</td><td><span class="pill keep">manter</span></td><td>Já prontos para standalone (a telemetria é melhor que a do MyApps)</td></tr>
          <tr><td>Camada r2wc (<code>web-components/</code>)</td><td><span class="pill rebuild">deletar</span></td><td>Vira peso morto — remover só quando o MyApps largar o pacote npm</td></tr>
        </tbody>
      </table>
    </div>
  </section>

  <section>
    <h2><span class="k">4</span> Plano em 6 fases</h2>
    <p class="lead">Cada fase deixa <code>typecheck</code> + <code>test</code> + <code>build</code> verdes. A URL de verdade sobe já na Fase 1.</p>
    <div class="card">
      <ol class="timeline">
        <li class="p0"><div class="ph-t">Fase 0 — Infra &amp; decisões (sem código, em paralelo)</div>
          <div class="ph-d">Registro no Azure AD por ambiente · backend aceitar o novo audience · 3 Static Web Apps · 3 App Insights separados · decidir native/Capacitor · neutralizar os pipelines antigos de npm · <b>decidir o repo antes de qualquer ticket</b>.</div></li>
        <li><div class="ph-t">Fase 1 — Virar SPA de verdade + router</div>
          <div class="ph-d">Reescrever <code>vite.config.ts</code> (SPA), criar rotas + páginas stub das 6 features, subir pipeline SWA no <b>dev</b> com token temporário. Agora existe link pra demonstrar.</div></li>
        <li><div class="ph-t">Fase 2 — Autenticação MSAL</div>
          <div class="ph-d"><code>VITE_ENTRA_*</code> build-time · <code>useMsalSession</code> (puro) + <code>AuthGuard</code> · timer de refresh proativo (sessões longas do Copilot) · <code>useAxios</code> re-tenta 1× no 401 · deletar o backdoor de token.</div></li>
        <li><div class="ph-t">Fase 3 — Chrome + UI compartilhada</div>
          <div class="ph-d">Copiar componentes puros, adicionar tokens de tema (com teste), construir Header/Navbar/layout próprios, FeedbackDialog + provider, Piano + consentimento.</div></li>
        <li><div class="ph-t">Fase 4 — Aposentar a casca antiga</div>
          <div class="ph-d">Depois que o MyApps confirmar que não importa mais o pacote: deletar <code>web-components/</code>, remover pipelines antigos, limpar o <code>package.json</code>.</div></li>
        <li><div class="ph-t">Fase 5 — Features de domínio + permissões</div>
          <div class="ph-d">Implementar as 6 features · <code>useFeatureFlags</code> · preferência de idioma · <code>PermissionGate</code> (bloqueado no <code>fe-tools</code>) · breadcrumbs com eventos escopados.</div></li>
      </ol>
    </div>
  </section>

  <section>
    <h2><span class="k">5</span> Falhas pegas na revisão (as principais)</h2>
    <p class="lead">O plano acima já as absorve. Aqui pra mostrar o rigor da revisão adversarial.</p>
    <div class="card">
      <table>
        <thead><tr><th>Sev.</th><th>Ponto de falha</th><th>Como o plano trata</th></tr></thead>
        <tbody>
          <tr><td><span class="dot d-crit"></span>Crít.</td><td>Config MSAL não roda com JSON de runtime</td><td>Build-time, 1 build por ambiente</td></tr>
          <tr><td><span class="dot d-crit"></span>Crít.</td><td>Novo <code>clientId</code> → token com audience que a API rejeita (401)</td><td>Ticket de backend na Fase 0</td></tr>
          <tr><td><span class="dot d-crit"></span>Crít.</td><td>3 pipelines no <code>main</code> publicam pacote meio-migrado</td><td><code>publishPackage:false</code> na Fase 0</td></tr>
          <tr><td><span class="dot d-crit"></span>Crít.</td><td>Config de build SPA é só um stub</td><td>Reescrita completa na Fase 1</td></tr>
          <tr><td><span class="dot d-high"></span>Alta</td><td><code>AuthContext</code> acoplado ao router</td><td>Dividir em <code>useMsalSession</code> + <code>AuthGuard</code></td></tr>
          <tr><td><span class="dot d-high"></span>Alta</td><td>SC ficaria "não-entregável" até a Fase 3</td><td>Deploy no dev já na Fase 1</td></tr>
          <tr><td><span class="dot d-high"></span>Alta</td><td>Sem refresh proativo → Copilot expira token</td><td>Timer ~12min + retry</td></tr>
          <tr><td><span class="dot d-high"></span>Alta</td><td>App Insights compartilhado mistura dev e prod</td><td>3 recursos separados na Fase 0</td></tr>
          <tr><td><span class="dot d-high"></span>Alta</td><td>Decisão do repo tardia invalida toda a infra</td><td>Forçar decisão na Fase 0</td></tr>
        </tbody>
      </table>
    </div>
  </section>

  <section>
    <h2><span class="k">6</span> Perguntas em aberto (decisão do time / tech lead)</h2>
    <div class="card">
      <ul class="q">
        <li><b>Native/Capacitor:</b> o SC precisa de app mobile? (Esforço grande e separado.)</li>
        <li><b>Compatibilidade na transição:</b> o SC precisa continuar embutível no MyApps durante a migração?</li>
        <li><b>Registro Azure AD:</b> qual time provisiona e qual o prazo? (Maior bloqueio da Fase 2.)</li>
        <li><b>Header <code>app-code</code>:</b> a API do SmartContracts espera algum valor específico do SC?</li>
        <li><b>Navegação desktop:</b> montar o <code>b2o-navigation-module</code> ou construir uma nav própria (mais confiável)?</li>
        <li><b>Deploy same-origin:</b> o SC vai dividir origem com o MyApps? (Impacta isolamento de cookie/localStorage.)</li>
      </ul>
    </div>
  </section>

  <div class="made">
    🛠️ <b>Como foi feito:</b> gerado por um agente (Claude Code) a partir de uma varredura completa
    do container MyApps — 8 leitores em paralelo mapearam auth, rotas, chrome, UI, env e build; a
    estratégia passou por uma revisão adversarial com 3 lentes (segurança, arquitetura, entrega)
    antes de virar plano. Documento completo: <code>docs/adr/0001-smartcontracts-standalone-app.md</code>.
  </div>

  <footer>
    Resumo da ADR 0001 · SmartContracts · atualizado em 2026-07-06 ·
    verifique <code>arquivo:linha</code> contra o código atual antes de citar em reunião
  </footer>

</div>
</body>
</html>
