<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sistema de Decisión Diario — BTC/SOL Futures</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{background:#0f1117;color:#e8e6e0;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;padding:16px;min-height:100vh}
h1{font-size:17px;font-weight:600;color:#e8e6e0;margin-bottom:4px}
.sub{font-size:12px;color:#898781;margin-bottom:20px}
.step{background:#1a1d27;border:.5px solid #2a2d3a;border-radius:12px;padding:14px 16px;margin-bottom:10px}
.step-title{font-size:11px;font-weight:600;color:#5a9cf5;text-transform:uppercase;letter-spacing:.08em;margin-bottom:10px}
.opts{display:flex;gap:6px;flex-wrap:wrap}
.opt{padding:7px 14px;border-radius:20px;border:.5px solid #2a2d3a;background:#232633;color:#898781;cursor:pointer;font-size:12px;font-weight:500;transition:all .15s;user-select:none}
.opt:hover{border-color:#5a9cf5;color:#c8c6c0}
.opt.sel-bull{background:#0f3d2a;border-color:#1D9E75;color:#4dcca0}
.opt.sel-bear{background:#3d1212;border-color:#E24B4A;color:#f08080}
.opt.sel-grey{background:#2a2d3a;border-color:#555;color:#aaa}
.opt.sel-blue{background:#0d2a4a;border-color:#5a9cf5;color:#7ab8ff}
.opt.sel-amber{background:#3a2a08;border-color:#EF9F27;color:#f5c265}
.opt.sel-green{background:#0f3d2a;border-color:#1D9E75;color:#4dcca0}
.opt.sel-red{background:#3d1212;border-color:#E24B4A;color:#f08080}
.combo-title{font-size:11px;color:#898781;margin:10px 0 6px;font-weight:500}
.combo-table{width:100%;border-collapse:collapse;font-size:11px}
.combo-table th{padding:5px 8px;text-align:left;color:#555;font-weight:500;border-bottom:.5px solid #2a2d3a}
.combo-table td{padding:5px 8px;border-bottom:.5px solid #1a1d27;color:#898781}
.combo-table .hl{background:#0f3d2a}
.combo-table .hl td{color:#4dcca0}
.result{border-radius:12px;padding:16px 18px;margin-top:12px;border:.5px solid #2a2d3a;display:none}
.r-long{background:#0a2a1a;border-color:#1D9E75}
.r-short{background:#2a0a0a;border-color:#E24B4A}
.r-caution{background:#2a1f08;border-color:#EF9F27}
.r-skip{background:#1a1d27;border-color:#444}
.r-notrend{background:#1a1d27;border-color:#555}
.r-title{font-size:20px;font-weight:600;margin-bottom:4px}
.r-sub{font-size:13px;line-height:1.5;margin-bottom:12px;color:#c8c6c0}
.sig-row{display:flex;align-items:center;gap:8px;padding:5px 0;border-bottom:.5px solid rgba(255,255,255,0.05);font-size:12px}
.sig-row:last-child{border-bottom:none}
.sig-name{color:#898781;min-width:110px}
.sig-val{flex:1;color:#c8c6c0}
.sig-score{font-size:11px;font-weight:600;padding:2px 8px;border-radius:20px;min-width:32px;text-align:center}
.sp{background:#0f3d2a;color:#4dcca0}
.sn{background:#3d1212;color:#f08080}
.s0{background:#2a2d3a;color:#898781}
.sb{background:#0d2a4a;color:#7ab8ff}
.score-bar{height:6px;border-radius:3px;background:#2a2d3a;margin:10px 0;overflow:hidden}
.score-fill{height:6px;border-radius:3px;transition:width .4s,background .4s}
.ins{padding:8px 12px;border-left:3px solid;font-size:12px;color:#898781;line-height:1.5;margin-top:8px;border-radius:0 6px 6px 0;background:#1a1d27}
.ig{border-left-color:#1D9E75}.ir{border-left-color:#E24B4A}.ia{border-left-color:#EF9F27}.ib{border-left-color:#5a9cf5}
.ref-section{margin-top:20px}
.ref-title{font-size:11px;font-weight:600;color:#5a9cf5;text-transform:uppercase;letter-spacing:.08em;margin-bottom:8px}
.ref-card{background:#1a1d27;border:.5px solid #2a2d3a;border-radius:10px;padding:12px 14px;margin-bottom:8px}
.ref-card h4{font-size:12px;font-weight:600;color:#c8c6c0;margin-bottom:6px}
.ref-row{display:flex;align-items:flex-start;gap:8px;padding:4px 0;font-size:12px;color:#898781;border-bottom:.5px solid #22253a}
.ref-row:last-child{border-bottom:none}
.ref-key{min-width:200px;font-weight:500;color:#c8c6c0}
.ref-badge{font-size:10px;font-weight:600;padding:1px 7px;border-radius:20px;flex-shrink:0}
.decision-table{width:100%;border-collapse:collapse;font-size:12px;margin-top:6px}
.decision-table th{padding:6px 10px;text-align:left;color:#555;font-size:11px;font-weight:500;border-bottom:.5px solid #2a2d3a}
.decision-table td{padding:6px 10px;border-bottom:.5px solid #1a1d27;color:#898781}
.decision-table .best td{background:#0f3d2a;color:#4dcca0}
.decision-table .ok td{background:#3a2a08;color:#f5c265}
.decision-table .bad td{background:#3d1212;color:#f08080}
</style>
</head>
<body>

<h1>Sistema de Decisión Diario</h1>
<div class="sub">BTC / SOL Futures — usar cada mañana en 2 minutos antes de la sesión 8AM CR</div>

<!-- PASO 1: DAILY -->
<div class="step">
  <div class="step-title">Paso 1 — Daily Trend (filtro absoluto)</div>
  <div class="opts">
    <div class="opt" onclick="sel('trend','bull',this,'sel-bull')">📈 Bullish — HH + HL</div>
    <div class="opt" onclick="sel('trend','bear',this,'sel-bear')">📉 Bearish — LH + LL</div>
    <div class="opt" onclick="sel('trend','range',this,'sel-grey')">↔ Sin tendencia / Rango</div>
  </div>
</div>

<!-- PASO 2: 4H -->
<div class="step">
  <div class="step-title">Paso 2 — 4H Alignment</div>
  <div class="opts">
    <div class="opt" onclick="sel('h4','aligned',this,'sel-green')">✅ Alineado con Daily</div>
    <div class="opt" onclick="sel('h4','neutral',this,'sel-grey')">➡ Neutral / Rango en 4H</div>
    <div class="opt" onclick="sel('h4','against',this,'sel-amber')">⚠ Contra el Daily (pullback)</div>
  </div>
</div>

<!-- PASO 3: ETF -->
<div class="step">
  <div class="step-title">Paso 3 — ETF Flows (revisar en farside.co.uk cada mañana)</div>
  <div class="opts">
    <div class="opt" onclick="sel('etf','pos',this,'sel-green')">🟢 Positivos — más de +$100M (comprando)</div>
    <div class="opt" onclick="sel('etf','neu',this,'sel-grey')">⚪ Neutros — entre -$100M y +$100M</div>
    <div class="opt" onclick="sel('etf','neg',this,'sel-red')">🔴 Negativos — menos de -$100M (vendiendo)</div>
  </div>
</div>

<!-- PASO 4: OI -->
<div class="step">
  <div class="step-title">Paso 4 — Open Interest (coinglass.com)</div>
  <div class="opts">
    <div class="opt" onclick="sel('oi','rising',this,'sel-blue')">📊 Subiendo — posiciones nuevas entrando</div>
    <div class="opt" onclick="sel('oi','stable',this,'sel-grey')">➡ Estable</div>
    <div class="opt" onclick="sel('oi','falling',this,'sel-amber')">📉 Bajando — posiciones cerrando</div>
  </div>
</div>

<!-- PASO 5: FUNDING -->
<div class="step">
  <div class="step-title">Paso 5 — Funding Rate (coinglass.com o Binance Futures)</div>
  <div class="opts" style="flex-direction:column;gap:5px">
    <div class="opt" onclick="sel('fr','vpos',this,'sel-red')" style="border-radius:8px">🔴 Muy positivo &gt; +0.05% — longs pagando fuerte (mercado sobreapalancado alcista)</div>
    <div class="opt" onclick="sel('fr','spos',this,'sel-amber')" style="border-radius:8px">🟡 Positivo +0.01% a +0.05% — longs pagando normalmente</div>
    <div class="opt" onclick="sel('fr','neu',this,'sel-grey')" style="border-radius:8px">⚪ Neutro — entre -0.01% y +0.01%</div>
    <div class="opt" onclick="sel('fr','sneg',this,'sel-green')" style="border-radius:8px">🟢 Negativo -0.01% a -0.05% — shorts pagando moderadamente</div>
    <div class="opt" onclick="sel('fr','vneg',this,'sel-blue')" style="border-radius:8px">🔵 Muy negativo &lt; -0.05% — shorts pagando fuerte (mercado sobreapalancado bajista)</div>
  </div>
</div>

<!-- RESULTADO -->
<div id="result" class="result">
  <div class="r-title" id="rTitle"></div>
  <div class="r-sub" id="rSub"></div>
  <div class="score-bar"><div class="score-fill" id="rBar"></div></div>
  <div style="font-size:11px;color:#555;margin-bottom:10px" id="rScore"></div>
  <div style="font-size:11px;font-weight:600;color:#555;text-transform:uppercase;letter-spacing:.06em;margin-bottom:6px">Detalle de señales</div>
  <div id="rSignals"></div>
  <div id="rInsight"></div>
</div>

<!-- REFERENCIA PERMANENTE -->
<div class="ref-section">
  <div class="ref-title">Referencia permanente — siempre visible</div>

  <div class="ref-card">
    <h4>Funding Rate — qué significa según el Daily</h4>
    <div class="ref-row"><div class="ref-key">Muy positivo + Daily bullish</div><div>Longs sobreapalancados → riesgo flush antes de subir</div><span class="ref-badge" style="background:#3d1212;color:#f08080">-1</span></div>
    <div class="ref-row"><div class="ref-key">Positivo + Daily bullish</div><div>Sentimiento alcista sano → confirma dirección</div><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></div>
    <div class="ref-row"><div class="ref-key">Neutro</div><div>Sin señal adicional</div><span class="ref-badge" style="background:#2a2d3a;color:#898781">0</span></div>
    <div class="ref-row"><div class="ref-key">Negativo + Daily bullish</div><div>Shorts bajo presión → eventualmente cubren → alcista</div><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></div>
    <div class="ref-row"><div class="ref-key">Muy negativo + Daily bullish</div><div>Shorts muy sobreapalancados → squeeze inminente → muy alcista</div><span class="ref-badge" style="background:#0d2a4a;color:#7ab8ff">+2</span></div>
    <div class="ref-row" style="margin-top:6px;border-top:.5px solid #2a2d3a;padding-top:6px"><div class="ref-key" style="color:#898781;font-style:italic">Para Daily bearish: invierte todos los signos</div><div style="color:#555">Positivo→-1, Muy positivo→-2, Negativo→+1, Muy negativo→+2</div></div>
  </div>

  <div class="ref-card">
    <h4>OI + Funding combinados — para Daily Bullish</h4>
    <table class="combo-table">
      <thead><tr><th>OI</th><th>Funding</th><th>Score</th><th>Por qué</th></tr></thead>
      <tbody>
        <tr><td>Sube</td><td>Muy positivo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-1</span></td><td>Longs sobreapalancados entrando — riesgo flush</td></tr>
        <tr><td>Sube</td><td>Positivo</td><td><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+2</span></td><td>Nuevo dinero largo entrando sano — fuerte confirmación</td></tr>
        <tr><td>Sube</td><td>Neutro</td><td><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></td><td>Nuevo dinero, sin exceso de sentimiento</td></tr>
        <tr><td>Sube</td><td>Negativo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-1</span></td><td>Nuevos shorts entrando contra ti</td></tr>
        <tr><td>Sube</td><td>Muy negativo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-2</span></td><td>Shorts pesados entrando — peligroso</td></tr>
        <tr style="border-top:.5px solid #333"><td>Estable</td><td>Muy positivo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-1</span></td><td>Overleverage sin nuevo dinero — alerta</td></tr>
        <tr><td>Estable</td><td>Positivo</td><td><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></td><td>Sentimiento alcista sano</td></tr>
        <tr><td>Estable</td><td>Neutro</td><td><span class="ref-badge" style="background:#2a2d3a;color:#898781">0</span></td><td>Sin señal adicional</td></tr>
        <tr><td>Estable</td><td>Negativo</td><td><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></td><td>Shorts bajo presión — squeeze en formación</td></tr>
        <tr><td>Estable</td><td>Muy negativo</td><td><span class="ref-badge" style="background:#0d2a4a;color:#7ab8ff">+2</span></td><td>Shorts muy sobreapalancados — squeeze fuerte</td></tr>
        <tr style="border-top:.5px solid #333"><td>Baja</td><td>Muy positivo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-2</span></td><td>Longs cerrando desde posición sobreapalancada — bajista</td></tr>
        <tr><td>Baja</td><td>Positivo</td><td><span class="ref-badge" style="background:#3d1212;color:#f08080">-1</span></td><td>Longs tomando ganancias — momentum debilitando</td></tr>
        <tr><td>Baja</td><td>Neutro</td><td><span class="ref-badge" style="background:#2a2d3a;color:#898781">0</span></td><td>Reducción normal, sin señal</td></tr>
        <tr><td>Baja</td><td>Negativo</td><td><span class="ref-badge" style="background:#0f3d2a;color:#4dcca0">+1</span></td><td>Shorts cubriendo — precio sube</td></tr>
        <tr><td>Baja</td><td>Muy negativo</td><td><span class="ref-badge" style="background:#0d2a4a;color:#7ab8ff">+2</span></td><td>Shorts cubriendo masivamente — squeeze activo</td></tr>
      </tbody>
    </table>
    <div style="font-size:11px;color:#555;margin-top:6px;padding-top:6px;border-top:.5px solid #2a2d3a">Para Daily bearish: invierte todos los signos y swap positivo/negativo en el funding.</div>
  </div>

  <div class="ref-card">
    <h4>Score total → Decisión final</h4>
    <table class="decision-table">
      <thead><tr><th>Score total</th><th>Decisión</th><th>Tamaño</th><th>Exigencia técnica</th></tr></thead>
      <tbody>
        <tr class="best"><td>+4 o +5</td><td>LONG / SHORT — máxima convicción</td><td>1% completo</td><td>Setup normal H1/M15</td></tr>
        <tr class="best"><td>+3</td><td>LONG / SHORT — buena confirmación</td><td>1% completo</td><td>Setup limpio</td></tr>
        <tr class="ok"><td>+2</td><td>LONG / SHORT — moderado</td><td>0.75%</td><td>Setup limpio con volumen</td></tr>
        <tr class="ok"><td>+1</td><td>LONG / SHORT — cautela</td><td>0.5%</td><td>Setup muy limpio — sweep claro + vela fuerte</td></tr>
        <tr><td>0</td><td>Señales mixtas</td><td>0.25% o skip</td><td>Solo setup perfecto con todo alineado</td></tr>
        <tr class="bad"><td>-1</td><td>SKIP hoy</td><td>No operas</td><td>Espera mañana con mejores condiciones</td></tr>
        <tr class="bad"><td>-2 o menos</td><td>SKIP absoluto</td><td>No operas</td><td>Macro contradice fuertemente el Daily</td></tr>
      </tbody>
    </table>
  </div>

  <div class="ref-card">
    <h4>Reglas absolutas que nunca cambian</h4>
    <div class="ref-row"><div class="ref-key">Sin Daily trend claro</div><div>No operas, sin importar macro. Fin del análisis.</div></div>
    <div class="ref-row"><div class="ref-key">4H contra Daily</div><div>-1 al score. Solo entras en AOI Daily esperando reversión.</div></div>
    <div class="ref-row"><div class="ref-key">Score negativo</div><div>Nunca cambias dirección contra el Daily por macro. Solo skipeas.</div></div>
    <div class="ref-row"><div class="ref-key">TP máximo</div><div>36–45% del Daily ATR. Si no hay nivel H1 en ese rango con R:R ≥ 1:2.7 → skip.</div></div>
    <div class="ref-row"><div class="ref-key">Time stops</div><div>10AM → SL a BE / 10:30AM → cierre 50% / 11AM → cierre total</div></div>
  </div>
</div>

<script>
const state={trend:null,h4:null,etf:null,oi:null,fr:null};

function sel(key,val,el,cls){
  state[key]=val;
  document.querySelectorAll(`[onclick*="'${key}',"]`).forEach(b=>{
    b.className='opt';
  });
  el.classList.add(cls);
  compute();
}

function oifrScore(oi,fr,dir){
  const tbl={
    rising: {vpos:-1,spos:2,neu:1,sneg:-1,vneg:-2},
    stable: {vpos:-1,spos:1,neu:0,sneg:1,vneg:2},
    falling:{vpos:-2,spos:-1,neu:0,sneg:1,vneg:2}
  };
  let score=tbl[oi]?.[fr]??0;
  return dir==='bear'?-score:score;
}

function etfScore(etf,dir){
  const s=etf==='pos'?1:etf==='neg'?-1:0;
  return dir==='bear'?-s:s;
}

function h4Score(h4){
  return h4==='aligned'?1:h4==='against'?-1:0;
}

function frLabel(fr){
  return{vpos:'Muy positivo >+0.05%',spos:'Positivo +0.01–0.05%',neu:'Neutro ±0.01%',sneg:'Negativo -0.05–-0.01%',vneg:'Muy negativo <-0.05%'}[fr]||'—';
}
function oiLabel(oi){return{rising:'Subiendo',stable:'Estable',falling:'Bajando'}[oi]||'—';}
function etfLabel(etf){return{pos:'Positivos (comprando)',neu:'Neutros',neg:'Negativos (vendiendo)'}[etf]||'—';}
function h4Label(h4){return{aligned:'Alineado con Daily',neutral:'Neutral / Rango',against:'Contra Daily (pullback)'}[h4]||'—';}

function frInterp(fr,dir,oiScore){
  if(dir==='bull'){
    if(fr==='vneg')return'Shorts muy sobreapalancados → squeeze inminente → alcista';
    if(fr==='sneg')return'Shorts bajo presión → cubren eventualmente → alcista';
    if(fr==='neu') return'Sin sesgo adicional';
    if(fr==='spos')return'Longs con sentimiento alcista sano → confirma';
    if(fr==='vpos')return'Longs sobreapalancados → riesgo de flush antes de continuar';
  }else{
    if(fr==='vpos')return'Longs muy sobreapalancados → squeeze bajista inminente';
    if(fr==='spos')return'Longs bajo presión → cubren eventualmente → bajista';
    if(fr==='neu') return'Sin sesgo adicional';
    if(fr==='sneg')return'Shorts con sentimiento bajista sano → confirma';
    if(fr==='vneg')return'Shorts sobreapalancados → riesgo de rebote alcista';
  }
  return'—';
}

function compute(){
  const {trend,h4,etf,oi,fr}=state;
  if(!trend||!h4||!etf||!oi||!fr){document.getElementById('result').style.display='none';return;}

  const rEl=document.getElementById('result');
  rEl.style.display='block';

  if(trend==='range'){
    rEl.className='result r-notrend';
    document.getElementById('rTitle').innerHTML='<span style="color:#898781">⏸ NO OPERAS HOY</span>';
    document.getElementById('rSub').textContent='Sin tendencia clara en Daily, no hay trade sin importar qué digan los macro indicadores. Espera a que se forme estructura clara (HH+HL o LH+LL).';
    document.getElementById('rBar').style.cssText='width:0%;background:#555';
    document.getElementById('rScore').textContent='';
    document.getElementById('rSignals').innerHTML='';
    document.getElementById('rInsight').innerHTML='<div class="ins ia" style="margin-top:8px">El Daily es el primer filtro absoluto. Sin tendencia, cualquier entrada es especulación pura.</div>';
    return;
  }

  const dir=trend;
  const h4s=h4Score(h4);
  const es=etfScore(etf,dir);
  const ofs=oifrScore(oi,fr,dir);
  const total=h4s+es+ofs;

  let action,cls,size,req,titleColor,emoji;
  if(total>=4){action='Máxima convicción — entra';size='1% completo';req='Setup normal H1/M15';cls=dir==='bull'?'r-long':'r-short';titleColor=dir==='bull'?'#4dcca0':'#f08080';emoji=dir==='bull'?'📈':'📉';}
  else if(total===3){action='Buena confirmación — entra';size='1% completo';req='Setup limpio';cls=dir==='bull'?'r-long':'r-short';titleColor=dir==='bull'?'#4dcca0':'#f08080';emoji=dir==='bull'?'📈':'📉';}
  else if(total===2){action='Señales moderadas — entra';size='0.75% de riesgo';req='Setup limpio con volumen alto';cls=dir==='bull'?'r-long':'r-short';titleColor=dir==='bull'?'#4dcca0':'#f08080';emoji=dir==='bull'?'📈':'📉';}
  else if(total===1){action='Cautela — posición reducida';size='0.5% de riesgo';req='Setup muy limpio — sweep claro + vela fuerte en M15';cls=dir==='bull'?'r-long':'r-short';titleColor=dir==='bull'?'#7ab8ff':'#f5c265';emoji=dir==='bull'?'📈':'📉';}
  else if(total===0){action='Señales mixtas — alta exigencia';size='0.25% o skip';req='Solo si el setup en H1/M15 es perfecto';cls='r-caution';titleColor='#f5c265';emoji='⚠';}
  else{action='SKIP — macro contradice el Daily';size='No operas hoy';req='Espera mañana con mejores condiciones';cls='r-skip';titleColor='#898781';emoji='⏸';}

  const dirLabel=dir==='bull'?'LONG (compra)':'SHORT (venta)';
  rEl.className='result '+cls;
  document.getElementById('rTitle').innerHTML=`<span style="color:${titleColor}">${emoji} ${dirLabel} — ${action}</span>`;
  document.getElementById('rSub').textContent=`Tamaño: ${size}   ·   Exigencia: ${req}`;

  const barW=Math.max(0,Math.min(100,(total+3)/6*100));
  const barCol=total>=3?'#1D9E75':total>=1?'#EF9F27':total===0?'#555':'#E24B4A';
  document.getElementById('rBar').style.cssText=`width:${barW}%;background:${barCol}`;
  document.getElementById('rScore').textContent=`Score de confirmación: ${total>0?'+':''}${total} / +5   (mínimo +1 para entrar, +3 para tamaño completo)`;

  const h4Interp=h4==='aligned'?'Confirma dirección del Daily'
    :h4==='against'?'Pullback dentro del Daily — espera AOI + reversión'
    :'Sin señal adicional de 4H';

  const etfInterp=dir==='bull'
    ?(etf==='pos'?'Instituciones comprando → confirma':etf==='neg'?'Instituciones vendiendo → contra Daily':'Sin señal')
    :(etf==='neg'?'Instituciones vendiendo → confirma':etf==='pos'?'Instituciones comprando → contra Daily':'Sin señal');

  document.getElementById('rSignals').innerHTML=`
    <div class="sig-row"><div class="sig-name">Daily trend</div><div class="sig-val">${dir==='bull'?'Bullish — HH+HL':'Bearish — LH+LL'}</div><div class="sig-score sb">Base</div></div>
    <div class="sig-row"><div class="sig-name">4H alignment</div><div class="sig-val">${h4Label(h4)} — ${h4Interp}</div><div class="sig-score ${h4s>0?'sp':h4s<0?'sn':'s0'}">${h4s>0?'+'+h4s:h4s}</div></div>
    <div class="sig-row"><div class="sig-name">ETF Flows</div><div class="sig-val">${etfLabel(etf)} — ${etfInterp}</div><div class="sig-score ${es>0?'sp':es<0?'sn':'s0'}">${es>0?'+'+es:es}</div></div>
    <div class="sig-row"><div class="sig-name">OI + Funding</div><div class="sig-val">${oiLabel(oi)} + ${frLabel(fr)} → ${frInterp(fr,dir,ofs)}</div><div class="sig-score ${ofs>0?'sp':ofs<0?'sn':'s0'}">${ofs>0?'+'+ofs:ofs}</div></div>
  `;

  let insight='';
  if(total>=3)insight=`<div class="ins ig" style="margin-top:8px">Señales macro alineadas con el Daily. Aplica tu checklist técnico normal y entra cuando H1/M15 confirme en el AOI.</div>`;
  else if(total===1||total===2)insight=`<div class="ins ia" style="margin-top:8px">Hay señales en conflicto. Puedes entrar pero con riesgo reducido. El setup técnico debe ser impecable — sweep claro, vela de confirmación fuerte, volumen alto.</div>`;
  else if(total===0)insight=`<div class="ins ia" style="margin-top:8px">Las señales se cancelan. Si decides entrar, usa el mínimo posible (0.25%) y exige el setup más perfecto que hayas visto. Lo más probable es que hoy no haya trade.</div>`;
  else insight=`<div class="ins ir" style="margin-top:8px">El macro contradice el Daily. No cambias de dirección — simplemente no operas hoy. El Daily seguirá siendo bullish/bearish mañana cuando las condiciones macro mejoren.</div>`;

  document.getElementById('rInsight').innerHTML=insight;
}
</script>
</body>
</html>
