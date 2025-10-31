<!doctype html>
<html lang="ru">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
<title>Сыромания — Мини-приложение</title>
<link rel="preconnect" href="https://telegram.org" />
<script src="https://telegram.org/js/telegram-web-app.js"></script>
<style>
:root{
  --bg: #ffffff;
  --text: #111111;
  --muted: #6b7280;
  --card: #f8f9fb;
  --accent: #2563eb;
  --accent-contrast: #ffffff;
  --border: #e5e7eb;
  --danger: #b91c1c;
  --ok: #166534;
  --shadow: 0 2px 10px rgba(0,0,0,.08);
  --radius: 16px;
  --gap: 12px;
  --focus: 2px solid #2563ebaa;
}
html,body{height:100%}
body{
  margin:0; font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, 'Helvetica Neue', Arial, 'Noto Sans', 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  background: var(--bg); color: var(--text);
}
header{
  position: sticky; top: 0; z-index: 5;
  padding: 12px; background: var(--bg); border-bottom: 1px solid var(--border);
  display:grid; gap: var(--gap);
}
.header-row{display:grid; grid-template-columns: 1fr auto; gap: var(--gap); align-items:center}
.filters{display:grid; grid-template-columns: 1fr 1fr auto; gap: var(--gap)}
.search{
  display:flex; align-items:center; gap:8px; background: var(--card);
  padding:10px 12px; border-radius: var(--radius); border:1px solid var(--border);
}
.search input{flex:1; border:none; outline:none; background:transparent; color:var(--text)}
select, button, input[type="number"], input[type="text"], textarea{
  border:1px solid var(--border); background:var(--bg); color:var(--text);
  border-radius: 10px; padding:10px 12px; font-size: 14px;
}
button{cursor:pointer}
button.primary{
  background: var(--accent); color: var(--accent-contrast); border-color: transparent;
}
button.ghost{background: var(--card)}
button.danger{ background: #fee2e2; border-color: #fecaca; color: var(--danger) }
kbd.badge{
  font-family: inherit; font-weight: 600; border:1px solid var(--border);
  background: var(--card); color: var(--muted); padding:3px 8px; border-radius: 999px; font-size:12px;
}
main{ padding: 12px; padding-bottom: 100px; }
.grid{
  display:grid; gap: var(--gap);
  grid-template-columns: repeat( auto-fit, minmax(240px, 1fr) );
}
.card{
  background: var(--card); border:1px solid var(--border); border-radius: var(--radius);
  box-shadow: var(--shadow); padding: 12px; display:flex; flex-direction: column; gap: 8px;
}
.card h3{margin:0; font-size: 16px}
.card .muted{color:var(--muted); font-size: 12px}
.card .price{font-weight:700}
.card .pic{
  width: 64px; height:64px; display:grid; place-items:center; font-size:32px; border-radius: 12px;
  background: var(--bg); border:1px solid var(--border);
}
.card footer{ display:flex; gap:8px; align-items:center; justify-content: space-between; margin-top:auto }

.tags{display:flex; gap:6px; flex-wrap:wrap}
.tag{font-size:12px; background: var(--bg); border:1px solid var(--border); color:var(--muted); padding:4px 8px; border-radius:999px}

/* floating cart bar */
.cart-bar{
  position: fixed; left: 12px; right: 12px; bottom: 12px; z-index: 10;
  display:flex; align-items:center; justify-content:space-between; gap: 10px;
  background: var(--bg); border:1px solid var(--border); border-radius: 14px; box-shadow: var(--shadow);
  padding: 10px 12px;
}
.cart-bar .summary{ display:flex; align-items:center; gap:10px; font-weight:600 }
.cart-bar .summary .chip{
  background: var(--card); border:1px solid var(--border); padding:3px 8px; border-radius:999px; font-size:12px; color:var(--muted)
}

dialog{ border: none; border-radius: 16px; padding:0; box-shadow: 0 20px 60px rgba(0,0,0,.2); width:min(720px, 95vw) }
dialog::backdrop{ background: rgba(0,0,0,.4) }
.modal{
  background: var(--bg); color: var(--text); border:1px solid var(--border); border-radius: 16px; padding: 16px; max-height: 85vh; overflow:auto
}
.modal header{ position: sticky; top: -16px; background: var(--bg); border-bottom:1px solid var(--border); margin:-16px; margin-bottom:16px; padding:16px; border-top-left-radius:16px; border-top-right-radius:16px }
.modal footer{ position: sticky; bottom:-16px; background: var(--bg); border-top:1px solid var(--border); margin:-16px; margin-top:16px; padding:16px; border-bottom-left-radius:16px; border-bottom-right-radius:16px; display:flex; gap:8px; align-items:center; justify-content:space-between; flex-wrap:wrap }
.modal .row{ display:grid; gap:12px; grid-template-columns: 1fr 1fr; align-items: end }
.modal .row .full{ grid-column: 1 / -1 }

.table{ width:100%; border-collapse: collapse; }
.table th, .table td{ padding: 10px; border-bottom:1px solid var(--border); text-align:left; vertical-align:middle }
.table th{ font-size:12px; color: var(--muted); font-weight:600 }
.table .qty{ display:flex; align-items:center; gap:6px }
.table .qty input{ width:70px }

hr{ border: none; height:1px; background: var(--border); margin: 8px 0 }

.notice{ font-size: 12px; color: var(--muted) }
.muted{ color: var(--muted) }
.right{ margin-left:auto }
.center{ text-align:center }

/* focus */
:focus-visible{ outline: var(--focus); outline-offset: 2px }

/* dark mode from Telegram theme */
.tg-dark{
  --bg: #0e1621;
  --text: #f5f7fb;
  --muted: #a9b4c2;
  --card: #17212b;
  --accent: #5ea1ff;
  --accent-contrast: #0b1220;
  --border: #253241;
  --danger: #fca5a5;
  --ok: #34d399;
  --shadow: 0 8px 24px rgba(0,0,0,.4);
}

/* small helpers */
.hidden{ display:none !important }
</style>
</head>
<body>
<header>
  <div class="header-row">
    <div class="search" role="search">
      <span aria-hidden="true">🔎</span>
      <input id="q" type="search" placeholder="Поиск по названию…" autocomplete="off" />
    </div>
    <button id="resetFilters" class="ghost" title="Сбросить фильтры">Сброс</button>
  </div>
  <div class="filters">
    <select id="catFilter" aria-label="Фильтр по категории">
      <option value="">Все категории</option>
      <option value="Сыры">Сыры</option>
      <option value="Молочная продукция">Молочная продукция</option>
      <option value="Сладости и выпечка">Сладости и выпечка</option>
    </select>
    <label style="display:flex;align-items:center;gap:8px">
      <input id="onlyCheese" type="checkbox" />
      Только сыры
    </label>
    <div class="tags" aria-live="polite" id="activeFilters"></div>
  </div>
</header>

<main>
  <div class="grid" id="grid" aria-live="polite"></div>
</main>

<!-- Product modal -->
<dialog id="productDialog">
  <div class="modal">
    <header>
      <div style="display:flex; gap:12px; align-items:center">
        <div class="pic" id="prodPic" aria-hidden="true">🧀</div>
        <div>
          <div id="prodCat" class="muted"></div>
          <h2 id="prodName" style="margin:4px 0 6px 0; font-size:20px">—</h2>
          <div id="prodSku" class="muted"></div>
        </div>
        <button id="closeProduct" class="right ghost">Закрыть</button>
      </div>
    </header>

    <div id="prodDesc" class="notice" style="margin-bottom:8px"></div>

    <div class="row">
      <label class="full">Вариант
        <select id="variantSelect"></select>
      </label>
      <label>Кол-во
        <input id="variantQty" type="number" value="1" min="1" step="1" />
      </label>
      <div class="full">
        <div id="variantPrice" class="price">— ₽</div>
        <div id="variantPriceNote" class="notice"></div>
      </div>
    </div>

    <footer>
      <div>
        <div id="discountHint" class="notice"></div>
      </div>
      <div style="display:flex;gap:8px">
        <button id="addToCart" class="primary">Добавить в корзину</button>
      </div>
    </footer>
  </div>
</dialog>

<!-- Cart modal -->
<dialog id="cartDialog" aria-label="Корзина">
  <div class="modal">
    <header style="display:flex;align-items:center;gap:8px">
      <h2 style="margin:0">Корзина</h2>
      <span class="right notice" id="cartDiscountFlag"></span>
      <button id="closeCart" class="ghost">Закрыть</button>
    </header>

    <div id="cartEmpty" class="center muted hidden">Корзина пуста</div>

    <table class="table" id="cartTable" aria-label="Содержимое корзины">
      <thead>
        <tr><th>Товар</th><th>Вариант</th><th>Цена</th><th>Кол-во</th><th>Сумма</th><th></th></tr>
      </thead>
      <tbody></tbody>
    </table>

    <div id="orderExtras" class="hidden">
      <hr />
      <div class="row">
        <label class="full">Комментарий к заказу
          <textarea id="orderComment" rows="2" placeholder="Например: доставить к 18:00, не звонить"></textarea>
        </label>
      </div>
    </div>

    <footer>
      <div>
        <div class="notice" id="cartNote"></div>
      </div>
      <div style="display:flex;gap:8px;align-items:center;flex-wrap:wrap">
        <button id="clearCart" class="danger">Очистить</button>
        <div style="font-weight:700">Итого: <span id="cartTotal">0 ₽</span> <kbd class="badge" id="cartCount">0 поз.</kbd></div>
        <button id="sendCart" class="primary">Отправить</button>
      </div>
    </footer>
  </div>
</dialog>

<!-- Floating bar -->
<div class="cart-bar" id="cartBar" role="button" tabindex="0" aria-label="Открыть корзину">
  <div class="summary">
    <span>🧺</span>
    <span id="barText">0 позиций</span>
    <span class="chip" id="barSum">0 ₽</span>
  </div>
  <button class="primary" id="barSend">Отправить</button>
</div>

<script>
/* =========================
   Конфигурация
========================= */
const CONFIG = {
  CURRENCY: 'RUB',
  ROUND: Math.round,
  DISCOUNT_THRESHOLDS: [ {g:1000, rate:0.15}, {g:700, rate:0.10}, {g:500, rate:0.05} ],
  ONLY_CHEESE_FILTER_DEFAULT: false,
  PAYLOAD_SCHEMA_VERSION: 'v1',
  SHOW_COMMENT_FIELD: true,        // флаг: поле "Комментарий к заказу" в корзине
  ENABLE_CITY_SELECT: false,       // флаг: выбор города (не используется по умолчанию)
  BAKERY_STEP_G: 250,              // шаг для выпечки/печенья по кг
  MAX_G_DEFAULT: 1000,             // максимум, если не указано иное
  PUZZLEBOT_HINT: true,            // положим подсказку в payload.meta
  WEBHOOK_HINT: 'srv-d42e1s3ipnbc73c8tgeg', // исключительно как подсказка в meta
};
/* =========================
   Телеграм окружение (без падений)
========================= */
const tg = (function(){
  const env = (window.Telegram && Telegram.WebApp) ? Telegram.WebApp : null;
  const fallback = {
    ready(){ console.log('[preview] ready'); },
    expand(){},
    close(){ console.log('[preview] close requested'); },
    colorScheme: window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light',
    themeParams: {},
    MainButton: {
      isVisible:false,
      text:'Отправить',
      show(){ this.isVisible=true; console.log('[preview] MainButton show') },
      hide(){ this.isVisible=false; console.log('[preview] MainButton hide') },
      onClick(cb){ this._cb = cb },
      offClick(){ this._cb=null },
      setText(txt){ this.text=txt },
      enable(){}, disable(){}, color:'#2481cc', textColor:'#fff'
    },
    sendData(payload){
      alert('Предпросмотр: данные отправлены в бота (симуляция). См. консоль.');
      console.log('sendData payload:', payload);
    }
  };
  return env || fallback;
})();
document.body.classList.toggle('tg-dark', tg.colorScheme === 'dark');
document.body.classList.toggle('tg-light', tg.colorScheme !== 'dark');
applyThemeParams(tg.themeParams||{});
tg.ready(); tg.expand();

/* ============ Тема из Telegram ============ */
function applyThemeParams(params){
  if(!params) return;
  const map = {
    bg_color:'--bg', text_color:'--text', secondary_bg_color:'--card', hint_color:'--muted',
    button_color:'--accent', button_text_color:'--accent-contrast'
  };
  for(const k in map){
    if(params[k]){
      document.documentElement.style.setProperty(map[k], params[k]);
    }
  }
}

/* =========================
   Справочник товаров и правила вариантов
========================= */
/** Категории */
const CAT = {
  CHEESE: 'Сыры',
  DAIRY: 'Молочная продукция',
  SWEETS: 'Сладости и выпечка',
};
/** Иконки по категориям/товарам (заглушки) */
const ICO = { [CAT.CHEESE]:'🧀', [CAT.DAIRY]:'🥛', [CAT.SWEETS]:'🍪' };

/** PRODUCTS: id, name, cat, pricePerKg|pricePerL|pricePerUnit, description?, ico? */
const PRODUCTS = [
  // ===== СЫРЫ (цены за кг) =====
  {id:'paneer_classic', name:'Панир / Адыгейский — классический', cat:CAT.CHEESE, pricePerKg:1200, ico:'🧀'},
  {id:'paneer_herbs', name:'Панир / Адыгейский — с зеленью', cat:CAT.CHEESE, pricePerKg:1300, ico:'🧀'},
  {id:'paneer_spice', name:'Панир / Адыгейский — с пряностями', cat:CAT.CHEESE, pricePerKg:1350, ico:'🧀'},
  {id:'paneer_smoked', name:'Панир / Адыгейский — копчёный', cat:CAT.CHEESE, pricePerKg:1400, ico:'🧀'},

  {id:'suluguni', name:'Сулугуни', cat:CAT.CHEESE, pricePerKg:1400},
  {id:'suluguni_smoked', name:'Сулугуни копчёный', cat:CAT.CHEESE, pricePerKg:1550},

  {id:'imeretinsky', name:'Имеретинский', cat:CAT.CHEESE, pricePerKg:1300},
  {id:'imeretinsky_dill_garlic', name:'Имеретинский с укропом и чесноком', cat:CAT.CHEESE, pricePerKg:1400},

  {id:'halloumi_classic', name:'Халлуми — классический', cat:CAT.CHEESE, pricePerKg:1650},
  {id:'halloumi_spicy_mix1', name:'Халлуми — паприка и орегано', cat:CAT.CHEESE, pricePerKg:1800},
  {id:'halloumi_mix_tbg', name:'Халлуми — томат, базилик, чеснок', cat:CAT.CHEESE, pricePerKg:1800},
  {id:'halloumi_sundried', name:'Халлуми — с вялеными помидорами и паприкой', cat:CAT.CHEESE, pricePerKg:1800},

  {id:'kosichka', name:'Косичка', cat:CAT.CHEESE, pricePerKg:1600},
  {id:'kosichka_smoked', name:'Косичка копчёная', cat:CAT.CHEESE, pricePerKg:1750},

  {id:'spicy_ball', name:'Пряный клубок', cat:CAT.CHEESE, pricePerKg:1680},

  {id:'mozzarella', name:'Моцарелла', cat:CAT.CHEESE, pricePerKg:1700},
  {id:'burrata', name:'Буратта', cat:CAT.CHEESE, pricePerKg:1800},

  {id:'stracciatella', name:'Страчателла', cat:CAT.CHEESE, pricePerKg:1850},

  {id:'ricotta', name:'Творожный сыр (рикотта)', cat:CAT.CHEESE, pricePerKg:1100},
  {id:'ricotta_herbs', name:'Творожный сыр (рикотта) с укропом и зеленью', cat:CAT.CHEESE, pricePerKg:1200},

  {id:'caciotta', name:'Качотта', cat:CAT.CHEESE, pricePerKg:2150},
  {id:'caciotta_fenugreek', name:'Качотта с пажитником', cat:CAT.CHEESE, pricePerKg:2250},

  {id:'hard_rural', name:'Твёрдый по-деревенски', cat:CAT.CHEESE, pricePerKg:1400},
  {id:'hard_smoked', name:'Твёрдый копчёный', cat:CAT.CHEESE, pricePerKg:1600},

  {id:'cheese_roll_olives_walnut', name:'Сырный рулет (маслины и грецкий орех)', cat:CAT.CHEESE, pricePerKg:1550},
  {id:'cheese_roll_apricot_pine', name:'Сырный рулет (курага и кедровые)', cat:CAT.CHEESE, pricePerKg:1550},

  // ===== МОЛОЧНАЯ ПРОДУКЦИЯ =====
  {id:'milk', name:'Молоко', cat:CAT.DAIRY, pricePerL:100, ico:'🥛'},
  {id:'baked_milk', name:'Топлёное молоко', cat:CAT.DAIRY, pricePerL:200},
  {id:'yogurt', name:'Йогурт классический', cat:CAT.DAIRY, pricePerL:230},
  {id:'ryazhenka', name:'Ряженка', cat:CAT.DAIRY, pricePerL:250},
  {id:'whey', name:'Сыворотка', cat:CAT.DAIRY, pricePerL:50},

  {id:'cream', name:'Сливки', cat:CAT.DAIRY, pricePerL:1200},
  {id:'curd', name:'Творог', cat:CAT.DAIRY, pricePerKg:500},

  {id:'butter', name:'Масло сливочное', cat:CAT.DAIRY, pricePerKg:1800, description:'Доступен фикс-пак 1 шт (200 г) = 360 ₽' },
  {id:'ghee', name:'Топлёное масло (ГХИ)', cat:CAT.DAIRY, pricePerKg:2300},

  {id:'condensed', name:'Сгущёнка', cat:CAT.DAIRY, pricePerKg:850},
  {id:'curd_mass_apricot', name:'Творожная масса — курага', cat:CAT.DAIRY, pricePerKg:700},
  {id:'curd_mass_raisins', name:'Творожная масса — изюм', cat:CAT.DAIRY, pricePerKg:700},
  {id:'curd_mass_prunes', name:'Творожная масса — чернослив', cat:CAT.DAIRY, pricePerKg:700},
  {id:'curd_mass_dates', name:'Творожная масса — финики', cat:CAT.DAIRY, pricePerKg:700},

  {id:'mishti_dahi', name:'Мистхи Дахи', cat:CAT.DAIRY, /* TODO_PRICE */ },

  // ===== СЛАДОСТИ И ВЫПЕЧКА =====
  // Печенье (цена за кг, продавать кратно 250 г)
  {id:'cookie_curd', name:'Печенье творожное', cat:CAT.SWEETS, pricePerKg:600, ico:'🍪'},
  {id:'cookie_oat', name:'Печенье овсяное', cat:CAT.SWEETS, pricePerKg:600},
  {id:'cookie_nut_fingers', name:'Ореховые пальчики', cat:CAT.SWEETS, pricePerKg:700},
  {id:'cookie_carob', name:'Печенье кэрбовое', cat:CAT.SWEETS, pricePerKg:600},
  {id:'cookie_shortbread', name:'Печенье песочное', cat:CAT.SWEETS, pricePerKg:600},

  // Кексы (цена за кг, шаг 250 г)
  {id:'muffin_plain', name:'Кексы обычные', cat:CAT.SWEETS, pricePerKg:500, ico:'🧁'},
  {id:'muffin_carob', name:'Кексы кэробовые', cat:CAT.SWEETS, pricePerKg:550},
  {id:'muffin_raisins', name:'Кексы с изюмом', cat:CAT.SWEETS, pricePerKg:550},

  // Кексы микс — фикс-паки
  {id:'muffin_mix_plain_raisins', name:'Кексы микс (обычные+изюм)', cat:CAT.SWEETS, pricePerUnit:280, description:'Пакет 0.5 кг', _fixed:{label:'0.5 кг', price:280}},
  {id:'muffin_mix_plain_carob', name:'Кексы микс (обычные+кэроб)', cat:CAT.SWEETS, pricePerUnit:300, description:'Пакет 0.5 кг', _fixed:{label:'0.5 кг', price:300}},
  {id:'muffin_mix_raisins_carob', name:'Кексы микс (изюм+кэроб)', cat:CAT.SWEETS, pricePerUnit:300, description:'Пакет 0.5 кг', _fixed:{label:'0.5 кг', price:300}},

  // Индийские сладости / выпечка (фикс-пакеты)
  {id:'sandesh_orange', name:'Сандеш — апельсин', cat:CAT.SWEETS, pricePerUnit:250, description:'5 шт / пакет', _countPack:{count:5, label:'5 шт', price:250}},
  {id:'sandesh_walnut', name:'Сандеш — грецкий орех', cat:CAT.SWEETS, pricePerUnit:250, description:'5 шт / пакет', _countPack:{count:5, label:'5 шт', price:250}},
  {id:'sandesh_carob', name:'Сандеш — кэроб', cat:CAT.SWEETS, pricePerUnit:250, description:'5 шт / пакет', _countPack:{count:5, label:'5 шт', price:250}},

  {id:'burfi_classic', name:'Бурфи — классический', cat:CAT.SWEETS, pricePerUnit:300, description:'5 шт / пакет', _countPack:{count:5, label:'5 шт', price:300}},
  {id:'burfi_hazelnut', name:'Бурфи — фундук', cat:CAT.SWEETS, pricePerUnit:300, description:'5 шт / пакет', _countPack:{count:5, label:'5 шт', price:300}},
  {id:'burfi_sesame', name:'Бурфи — кунжутный', cat:CAT.SWEETS, pricePerUnit:420, description:'7 шт / пакет', _countPack:{count:7, label:'7 шт', price:420}},

  {id:'halva', name:'Халва', cat:CAT.SWEETS, pricePerUnit:200, description:'0.2 кг фикс-пак', _fixed:{label:'0.2 кг', price:200}},
  {id:'potato_pastry', name:'Пирожное «Картошка»', cat:CAT.SWEETS, pricePerUnit:330, description:'5 шт или 2 шт', _multiPacks:[{label:'5 шт', price:330}, {label:'2 шт', price:155}]},
  {id:'cottage_casserole_plain', name:'Запеканка творожная', cat:CAT.SWEETS, pricePerUnit:260, description:'250 г фикс-пак', _fixed:{label:'250 г', price:260}},
  {id:'cottage_casserole_raisins', name:'Запеканка творожная с изюмом', cat:CAT.SWEETS, pricePerUnit:260, description:'250 г фикс-пак', _fixed:{label:'250 г', price:260}},
  {id:'crazy_cake', name:'Крейзи-кейк', cat:CAT.SWEETS, pricePerUnit:600, _countPack:{count:1, label:'1 шт', price:600}},
  {id:'coconut_kuchen', name:'Кокосовый кухен', cat:CAT.SWEETS, pricePerUnit:1800, _multiPacks:[{label:'1 кг', price:1800}, {label:'0.5 кг', price:1000}]},
  {id:'napoleon', name:'Торт «Наполеон»', cat:CAT.SWEETS, pricePerUnit:1300, description:'Пакеты: 1+ кг / 0.5+ кг', _multiPacks:[{label:'1+ кг', price:1300}, {label:'0.5+ кг', price:750}]},
  {id:'apple_pie', name:'Яблочный пирог', cat:CAT.SWEETS, pricePerUnit:560, _fixed:{label:'900 г', price:560}},
  {id:'pancakes_10', name:'Блины — 10 шт', cat:CAT.SWEETS, pricePerUnit:330, _countPack:{count:10, label:'10 шт', price:330}},
  {id:'pancakes_5', name:'Блины — 5 шт', cat:CAT.SWEETS, pricePerUnit:220, _countPack:{count:5, label:'5 шт', price:220}},
  {id:'pancakes_curd', name:'Блины с творогом', cat:CAT.SWEETS, pricePerUnit:300, _countPack:{count:5, label:'5 шт', price:300}},
  {id:'pancakes_curd_raisins', name:'Блины творог-изюм', cat:CAT.SWEETS, pricePerUnit:300, _countPack:{count:5, label:'5 шт', price:300}},
  {id:'syrniki_10', name:'Сырники — 10 шт', cat:CAT.SWEETS, pricePerUnit:520, _countPack:{count:10, label:'10 шт', price:520}},
  {id:'syrniki_5', name:'Сырники — 5 шт', cat:CAT.SWEETS, pricePerUnit:280, _countPack:{count:5, label:'5 шт', price:280}},
  {id:'chapati_10', name:'Чапати — 10 шт', cat:CAT.SWEETS, pricePerUnit:270, _countPack:{count:10, label:'10 шт', price:270}},
  {id:'chapati_wg_10', name:'Чапати (ц/з мука) — 10 шт', cat:CAT.SWEETS, pricePerUnit:320, _countPack:{count:10, label:'10 шт', price:320}},
];

/** Правила генерации вариантов */
const VARIANT_RULES = {
  // Панир/Адыгейский — фиксированные граммы
  paneer_classic:          {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  paneer_herbs:            {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  paneer_spice:            {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  paneer_smoked:           {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  // Сулугуни / Имеретинский — шаг 100 г
  suluguni:                {type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:100},
  suluguni_smoked:         {type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:100},
  imeretinsky:             {type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:100},
  imeretinsky_dill_garlic: {type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:100},
  // Халлуми — 1 шт 200/250 г
  halloumi_classic:        {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200,250]},
  halloumi_spicy_mix1:     {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200,250]},
  halloumi_mix_tbg:        {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200,250]},
  halloumi_sundried:       {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200,250]},
  // Косички/клубок/моцарелла/буратта
  kosichka:                {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200]},
  kosichka_smoked:         {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200]},
  spicy_ball:              {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[150]},
  mozzarella:              {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[200]},
  burrata:                 {type:'COUNT_FIXED_WEIGHT_CHOICES', gramsPerUnit:[250]},
  // Страчателла — перечисление
  stracciatella:           {type:'WEIGHT_CHOICES', grams:[200,250,300,500]},
  // Рикотта — перечисление
  ricotta:                 {type:'WEIGHT_CHOICES', grams:[200,250,300,450]},
  ricotta_herbs:           {type:'WEIGHT_CHOICES', grams:[200,250,300,450]},
  // Качотта — от 200 г шаг 100 г
  caciotta:                {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  caciotta_fenugreek:      {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  // Твёрдые — перечисление
  hard_rural:              {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  hard_smoked:             {type:'WEIGHT_CHOICES', grams:[200,300,400,500,1000]},
  // Рулеты — от 100 г шаг 50 г
  cheese_roll_olives_walnut:{type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:50},
  cheese_roll_apricot_pine: {type:'WEIGHT_STEP', minG:100, maxG:1000, stepG:50},

  // МОЛОЧКА
  milk:        {type:'LITER_CHOICES', liters:[0.5,1]},
  baked_milk:  {type:'LITER_CHOICES', liters:[0.5,1]},
  yogurt:      {type:'LITER_CHOICES', liters:[0.5,1]},
  ryazhenka:   {type:'LITER_CHOICES', liters:[0.5,1]},
  whey:        {type:'LITER_CHOICES', liters:[1]},

  cream:       {type:'LITER_CHOICES', liters:[0.2,0.5,1]},
  curd:        {type:'WEIGHT_CHOICES', grams:[500,1000,1500,2000]},
  butter:      {type:'WEIGHT_CHOICES_PLUS_FIXED', grams:[200,300,400,500,1000], fixed:{label:'1 шт (200 г)', price:360}},
  ghee:        {type:'WEIGHT_CHOICES', grams:[200,500,1000]},
  condensed:   {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  curd_mass_apricot: {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  curd_mass_raisins: {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  curd_mass_prunes:  {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  curd_mass_dates:   {type:'WEIGHT_STEP', minG:200, maxG:1000, stepG:100},
  mishti_dahi: {type:'HIDE_NO_PRICE'},

  // СЛАДОСТИ/ВЫПЕЧКА
  cookie_curd:         {type:'BAKERY_BY_KG_250G'},
  cookie_oat:          {type:'BAKERY_BY_KG_250G'},
  cookie_nut_fingers:  {type:'BAKERY_BY_KG_250G'},
  cookie_carob:        {type:'BAKERY_BY_KG_250G'},
  cookie_shortbread:   {type:'BAKERY_BY_KG_250G'},

  muffin_plain:        {type:'BAKERY_BY_KG_250G'},
  muffin_carob:        {type:'BAKERY_BY_KG_250G'},
  muffin_raisins:      {type:'BAKERY_BY_KG_250G'},

  muffin_mix_plain_raisins: {type:'FIXED_PACK'},
  muffin_mix_plain_carob:   {type:'FIXED_PACK'},
  muffin_mix_raisins_carob: {type:'FIXED_PACK'},

  sandesh_orange: {type:'COUNT_PACK'},
  sandesh_walnut: {type:'COUNT_PACK'},
  sandesh_carob:  {type:'COUNT_PACK'},

  burfi_classic: {type:'COUNT_PACK'},
  burfi_hazelnut:{type:'COUNT_PACK'},
  burfi_sesame:  {type:'COUNT_PACK'},

  halva: {type:'FIXED_PACK'},
  potato_pastry: {type:'MULTI_PACKS'},
  cottage_casserole_plain: {type:'FIXED_PACK'},
  cottage_casserole_raisins:{type:'FIXED_PACK'},
  crazy_cake: {type:'COUNT_PACK'},
  coconut_kuchen: {type:'MULTI_PACKS'},
  napoleon: {type:'MULTI_PACKS'},
  apple_pie: {type:'FIXED_PACK'},
  pancakes_10: {type:'COUNT_PACK'},
  pancakes_5: {type:'COUNT_PACK'},
  pancakes_curd: {type:'COUNT_PACK'},
  pancakes_curd_raisins: {type:'COUNT_PACK'},
  syrniki_10: {type:'COUNT_PACK'},
  syrniki_5: {type:'COUNT_PACK'},
  chapati_10: {type:'COUNT_PACK'},
  chapati_wg_10: {type:'COUNT_PACK'},
};

/* =========================
   Утилиты
========================= */
const fmtRub = (v)=> `${CONFIG.ROUND(v).toLocaleString('ru-RU')} ₽`;
const clamp = (n, a, b)=> Math.max(a, Math.min(b, n));

/** Генератор вариантов для карточки */
function buildVariants(product){
  const rule = VARIANT_RULES[product.id];
  if(!rule){
    console.warn('Нет правила вариантов:', product.id);
    return [];
  }
  const variants = [];
  const addWeight = (g)=> variants.push({key:`g${g}`, label:`${g} г`, type:'weight', grams:g});
  const addVolume = (l)=> variants.push({key:`l${l}`, label:`${l} л`, type:'volume', liters:l});
  const addUnitWeight = (g)=> variants.push({key:`u${g}`, label:`1 шт (${g} г)`, type:'unit_weight', grams:g, units:1});
  const addFixed = (label, price)=> variants.push({key:`f${label}`, label, type:'fixed', fixedPrice:price});
  switch(rule.type){
    case 'WEIGHT_CHOICES':
      rule.grams.forEach(addWeight); break;
    case 'WEIGHT_STEP':{
      const max = rule.maxG ?? CONFIG.MAX_G_DEFAULT;
      for(let g = rule.minG; g <= max; g += rule.stepG) addWeight(g);
      break;
    }
    case 'COUNT_FIXED_WEIGHT_CHOICES':
      rule.gramsPerUnit.forEach(addUnitWeight); break;
    case 'WEIGHT_CHOICES_PLUS_FIXED':
      rule.grams.forEach(addWeight);
      if(rule.fixed) addFixed(rule.fixed.label, rule.fixed.price);
      break;
    case 'LITER_CHOICES':
      rule.liters.forEach(addVolume); break;
    case 'BAKERY_BY_KG_250G':{
      for(let g = CONFIG.BAKERY_STEP_G; g <= 2000; g += CONFIG.BAKERY_STEP_G) addWeight(g);
      break;
    }
    case 'FIXED_PACK':{
      const f = product._fixed; if(f) addFixed(f.label, f.price); break;
    }
    case 'MULTI_PACKS':{
      const arr = product._multiPacks||[]; arr.forEach(p=> addFixed(p.label, p.price)); break;
    }
    case 'COUNT_PACK':{
      const c = product._countPack; if(c) addFixed(c.label, c.price); break;
    }
    case 'HIDE_NO_PRICE':
      return [];
    default:
      console.warn('Неизвестный тип правил:', rule.type);
  }
  return variants;
}

/** Цена за 1 единицу выбранного варианта до скидки */
function unitBasePrice(product, variant){
  if(variant.type === 'fixed') return CONFIG.ROUND(variant.fixedPrice);
  if(product.pricePerKg && (variant.type === 'weight' || variant.type === 'unit_weight')){
    const grams = (variant.type === 'unit_weight') ? variant.grams : variant.grams;
    return CONFIG.ROUND(product.pricePerKg * (grams/1000));
  }
  if(product.pricePerL && variant.type === 'volume'){
    return CONFIG.ROUND(product.pricePerL * variant.liters);
  }
  if(product.pricePerUnit && variant.type === 'count'){ // не используем сейчас
    return CONFIG.ROUND(product.pricePerUnit);
  }
  if(product.pricePerUnit && variant.type === 'fixed'){
    return CONFIG.ROUND(variant.fixedPrice ?? product.pricePerUnit);
  }
  // Если дошли сюда — невозможно определить цену
  return NaN;
}

/** Определение участия в «скидке на сыр» */
function isCheeseDiscountEligible(product, variant){
  if(product.cat !== CAT.CHEESE) return false;
  // Скидка применяется к позициям, у которых есть вес в граммах (включая 1 шт (N г))
  return (variant.type === 'weight' || variant.type === 'unit_weight');
}

/** Карточка корзины: структура хранимых данных */
function makeCartKey(pid, vkey){ return `${pid}__${vkey}` }

/* =========================
   Состояние (сохранение в localStorage)
========================= */
const LS = {
  load(){
    try{
      const raw = localStorage.getItem('syromania_cart_v1');
      return raw ? JSON.parse(raw) : {lines:{}, createdAt: Date.now()};
    }catch(e){ console.warn('localStorage load error', e); return {lines:{}, createdAt: Date.now()} }
  },
  save(state){
    try{ localStorage.setItem('syromania_cart_v1', JSON.stringify(state)); }catch(e){ console.warn('localStorage save error', e) }
  }
};
let CART = LS.load(); // { lines: { [key]: {pid, vkey, qty} }, createdAt }

/* =========================
   Рендер каталога
========================= */
const grid = document.getElementById('grid');
const qInput = document.getElementById('q');
const catFilter = document.getElementById('catFilter');
const onlyCheese = document.getElementById('onlyCheese');
const activeFilters = document.getElementById('activeFilters');
document.getElementById('resetFilters').addEventListener('click', ()=>{
  qInput.value=''; catFilter.value=''; onlyCheese.checked=CONFIG.ONLY_CHEESE_FILTER_DEFAULT; renderCatalog();
});

onlyCheese.checked = CONFIG.ONLY_CHEESE_FILTER_DEFAULT;

// Фильтруем и скрываем позиции без цены (TODO_PRICE)
const CATALOG = PRODUCTS.filter(p=>{
  const hasPrice = (typeof p.pricePerKg === 'number') || (typeof p.pricePerL === 'number') || (typeof p.pricePerUnit === 'number') || p._fixed || p._multiPacks || p._countPack;
  if(p.id === 'mishti_dahi' || !hasPrice){
    console.warn('TODO_PRICE:', p.id);
    return false;
  }
  return true;
});

function iconFor(product){ return product.ico || ICO[product.cat] || '🛍️' }

function minDisplayPrice(product){
  const vs = buildVariants(product);
  let min = Infinity;
  for(const v of vs){
    const base = unitBasePrice(product, v);
    if(Number.isFinite(base)) min = Math.min(min, base);
  }
  if(min === Infinity) return null;
  return fmtRub(min);
}

function renderCatalog(){
  // активные фильтры UI
  activeFilters.innerHTML = '';
  if(qInput.value.trim()) activeFilters.appendChild(tag(`Поиск: “${qInput.value.trim()}”`));
  if(catFilter.value) activeFilters.appendChild(tag(`Категория: ${catFilter.value}`));
  if(onlyCheese.checked) activeFilters.appendChild(tag('Только сыры'));
  // список
  grid.innerHTML = '';
  const query = qInput.value.trim().toLowerCase();
  const list = CATALOG.filter(p=>{
    if(onlyCheese.checked && p.cat !== CAT.CHEESE) return false;
    if(catFilter.value && p.cat !== catFilter.value) return false;
    if(query && !(`${p.name} ${p.cat}`.toLowerCase().includes(query))) return false;
    const variants = buildVariants(p);
    return variants.length > 0;
  });
  for(const p of list){
    const card = document.createElement('article');
    card.className = 'card';
    const minP = minDisplayPrice(p);
    card.innerHTML = `
      <div class="pic" aria-hidden="true">${iconFor(p)}</div>
      <h3>${escapeHtml(p.name)}</h3>
      <div class="muted">${p.cat}</div>
      <div class="tags">${priceBadge(p)}</div>
      ${p.description ? `<div class="notice">${escapeHtml(p.description)}</div>` : ''}
      <footer>
        <span class="price">${minP ? `от ${minP}` : ''}</span>
        <button class="primary" data-open="${p.id}">Подробнее</button>
      </footer>
    `;
    grid.appendChild(card);
  }
  // focusable cards
  grid.querySelectorAll('button[data-open]').forEach(btn=>{
    btn.addEventListener('click', ()=> openProduct(btn.getAttribute('data-open')));
  });
}
function priceBadge(product){
  let badge = '';
  if(product.pricePerKg) badge = `<span class="tag">тариф: ${fmtRub(product.pricePerKg)} / кг</span>`;
  else if(product.pricePerL) badge = `<span class="tag">тариф: ${fmtRub(product.pricePerL)} / л</span>`;
  else if(product.pricePerUnit) badge = `<span class="tag">${fmtRub(product.pricePerUnit)} / пакет</span>`;
  return badge;
}
function tag(text){ const k=document.createElement('kbd'); k.className='badge'; k.textContent=text; return k }
function escapeHtml(s){ return String(s).replace(/[&<>"']/g, m=>({ '&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;' })[m]) }

qInput.addEventListener('input', renderCatalog);
catFilter.addEventListener('change', renderCatalog);
onlyCheese.addEventListener('change', renderCatalog);

/* =========================
   Модал товара
========================= */
const productDialog = document.getElementById('productDialog');
const closeProductBtn = document.getElementById('closeProduct');
const prodPic = document.getElementById('prodPic');
const prodCat = document.getElementById('prodCat');
const prodName = document.getElementById('prodName');
const prodSku = document.getElementById('prodSku');
const prodDesc = document.getElementById('prodDesc');
const variantSelect = document.getElementById('variantSelect');
const variantQty = document.getElementById('variantQty');
const variantPrice = document.getElementById('variantPrice');
const variantPriceNote = document.getElementById('variantPriceNote');
const discountHint = document.getElementById('discountHint');
const addToCartBtn = document.getElementById('addToCart');

let CURRENT_PRODUCT = null;
let CURRENT_VARIANTS = [];
function openProduct(pid){
  const p = CATALOG.find(x=>x.id===pid);
  if(!p) return;
  CURRENT_PRODUCT = p;
  CURRENT_VARIANTS = buildVariants(p);
  prodPic.textContent = iconFor(p);
  prodCat.textContent = p.cat;
  prodName.textContent = p.name;
  prodSku.textContent = `Артикул: ${p.id}`;
  prodDesc.textContent = p.description || '';
  variantSelect.innerHTML = '';
  CURRENT_VARIANTS.forEach(v=>{
    const opt = document.createElement('option');
    opt.value = v.key; opt.textContent = v.label;
    variantSelect.appendChild(opt);
  });
  variantQty.value = 1;
  updateVariantPriceUI();
  productDialog.showModal();
  addToCartBtn.disabled = false;
}
function currentVariant(){
  const key = variantSelect.value;
  return CURRENT_VARIANTS.find(v=>v.key===key);
}
variantSelect.addEventListener('change', updateVariantPriceUI);
variantQty.addEventListener('input', ()=>{ variantQty.value = Math.max(1, parseInt(variantQty.value||'1',10)); updateVariantPriceUI(); });
closeProductBtn.addEventListener('click', ()=> productDialog.close());

function updateVariantPriceUI(){
  const p = CURRENT_PRODUCT; if(!p) return;
  const v = currentVariant(); if(!v){ variantPrice.textContent='—'; addToCartBtn.disabled = true; return; }
  const qty = parseInt(variantQty.value||'1', 10);
  const base = unitBasePrice(p, v);
  if(!Number.isFinite(base)){ variantPrice.textContent='Ошибка цены'; addToCartBtn.disabled = true; return; }
  const rates = computeDiscountRatesPreviewWithItem(p, v, qty);
  const rate = rates[p.id] || 0;
  const up = CONFIG.ROUND(base * (1 - rate));
  variantPrice.textContent = `${fmtRub(up)} × ${qty} = ${fmtRub(up * qty)}`;
  const note = [];
  if(p.pricePerKg && (v.type==='weight'||v.type==='unit_weight')) note.push('Цена расчётная из тарифа /кг');
  if(p.pricePerL && v.type==='volume') note.push('Цена расчётная из тарифа /л');
  variantPriceNote.textContent = note.join(' • ');
  if(rate>0){
    discountHint.textContent = `Скидка на этот вид сыра: ${(rate*100)|0}%`;
  }else{
    // Подсказка до какой границы осталось
    if(isCheeseDiscountEligible(p,v)){
      const curG = currentCheeseGramsById(p.id);
      const vG = (v.type==='unit_weight'||v.type==='weight') ? v.grams : 0;
      const totalG = curG + vG*qty;
      const next = CONFIG.DISCOUNT_THRESHOLDS.slice().reverse().find(th=> totalG < th.g);
      if(next){
        discountHint.textContent = `Добавьте ещё ${(next.g - totalG)} г этого сыра для скидки ${(CONFIG.DISCOUNT_THRESHOLDS.find(x=>x.g===next.g).rate*100)|0}%`;
      }else{
        discountHint.textContent = '';
      }
    }else{
      discountHint.textContent = '';
    }
  }
}
addToCartBtn.addEventListener('click', ()=>{
  const p = CURRENT_PRODUCT; const v = currentVariant();
  if(!p || !v){ variantSelect.focus(); return; }
  const qty = clamp(parseInt(variantQty.value||'1', 10), 1, 999);
  const key = makeCartKey(p.id, v.key);
  if(!CART.lines[key]) CART.lines[key] = {pid:p.id, vkey:v.key, qty:0};
  CART.lines[key].qty += qty;
  LS.save(CART);
  productDialog.close();
  renderCartBar();
});

/* =========================
   Скидки на сыр: расчёт по корзине
========================= */
function currentCheeseGramsById(pid){
  let grams = 0;
  for(const k in CART.lines){
    const line = CART.lines[k];
    if(line.pid !== pid) continue;
    const product = CATALOG.find(p=>p.id===line.pid);
    if(!product) continue;
    const variant = buildVariants(product).find(v=>v.key===line.vkey);
    if(!variant) continue;
    if(isCheeseDiscountEligible(product, variant)){
      const gPerUnit = variant.grams;
      grams += gPerUnit * line.qty;
    }
  }
  return grams;
}
function computeDiscountRates(){
  // группируем граммы по id продукта, только для сыров
  const gramsById = {};
  for(const k in CART.lines){
    const line = CART.lines[k];
    const p = CATALOG.find(x=>x.id===line.pid); if(!p) continue;
    const v = buildVariants(p).find(v=>v.key===line.vkey); if(!v) continue;
    if(isCheeseDiscountEligible(p, v)){
      gramsById[p.id] = (gramsById[p.id]||0) + (v.grams * line.qty);
    }
  }
  const rates = {};
  for(const pid in gramsById){
    const g = gramsById[pid];
    let rate = 0;
    for(const th of CONFIG.DISCOUNT_THRESHOLDS){
      if(g >= th.g){ rate = Math.max(rate, th.rate); }
    }
    rates[pid] = rate;
  }
  return rates;
}
// превью с учётом потенциального добавления текущей позиции
function computeDiscountRatesPreviewWithItem(product, variant, qty){
  const tmp = JSON.parse(JSON.stringify(CART));
  const key = makeCartKey(product.id, variant.key);
  if(!tmp.lines[key]) tmp.lines[key] = {pid:product.id, vkey:variant.key, qty:0};
  tmp.lines[key].qty += qty;
  const gramsById = {};
  for(const k in tmp.lines){
    const line = tmp.lines[k];
    const p = CATALOG.find(x=>x.id===line.pid); if(!p) continue;
    const v = buildVariants(p).find(v=>v.key===line.vkey); if(!v) continue;
    if(isCheeseDiscountEligible(p, v)){
      gramsById[p.id] = (gramsById[p.id]||0) + (v.grams * line.qty);
    }
  }
  const rates = {};
  for(const pid in gramsById){
    const g = gramsById[pid];
    let rate = 0;
    for(const th of CONFIG.DISCOUNT_THRESHOLDS){
      if(g >= th.g){ rate = Math.max(rate, th.rate); }
    }
    rates[pid] = rate;
  }
  return rates;
}

/* =========================
   Корзина — расчёт и UI
========================= */
const cartBar = document.getElementById('cartBar');
const barText = document.getElementById('barText');
const barSum = document.getElementById('barSum');
const barSend = document.getElementById('barSend');
const cartDialog = document.getElementById('cartDialog');
const cartTableBody = document.querySelector('#cartTable tbody');
const cartEmpty = document.getElementById('cartEmpty');
const cartTotalEl = document.getElementById('cartTotal');
const cartCountEl = document.getElementById('cartCount');
const cartNote = document.getElementById('cartNote');
const cartDiscountFlag = document.getElementById('cartDiscountFlag');
const orderExtras = document.getElementById('orderExtras');
const orderComment = document.getElementById('orderComment');

document.getElementById('closeCart').addEventListener('click', ()=> cartDialog.close());
document.getElementById('clearCart').addEventListener('click', ()=>{
  CART.lines = {}; LS.save(CART); renderCartBar(); if(cartDialog.open) renderCartModal();
});
cartBar.addEventListener('click', ()=> { renderCartModal(); cartDialog.showModal(); });
cartBar.addEventListener('keydown', (e)=>{ if(e.key==='Enter' || e.key===' '){ e.preventDefault(); cartBar.click(); }});
barSend.addEventListener('click', ()=> { renderCartModal(); sendCart(); });
document.getElementById('sendCart').addEventListener('click', sendCart);

function enrichLine(line){
  const p = CATALOG.find(x=>x.id===line.pid);
  if(!p) return null;
  const v = buildVariants(p).find(v=>v.key===line.vkey);
  if(!v) return null;
  const baseUnit = unitBasePrice(p, v);
  const rates = computeDiscountRates();
  const rate = isCheeseDiscountEligible(p, v) ? (rates[p.id]||0) : 0;
  const unit = CONFIG.ROUND(baseUnit * (1 - rate));
  const total = unit * line.qty;
  return { ...line, product:p, variant:v, unitBase: baseUnit, discountRate: rate, unitPrice: unit, lineTotal: total };
}
function cartSummary(){
  const items = [];
  for(const k in CART.lines){
    const e = enrichLine(CART.lines[k]);
    if(e) items.push(e);
  }
  const total = items.reduce((s,i)=> s + i.lineTotal, 0);
  const count = items.reduce((s,i)=> s + i.qty, 0);
  const anyDiscount = items.some(i=> i.discountRate>0);
  return {items, total, count, anyDiscount};
}
function renderCartBar(){
  const {total, count} = cartSummary();
  barText.textContent = count ? `${count} поз.` : '0 позиций';
  barSum.textContent = fmtRub(total);
  updateMainButton(count, total);
}
function renderCartModal(){
  orderExtras.classList.toggle('hidden', !CONFIG.SHOW_COMMENT_FIELD);
  const {items, total, count, anyDiscount} = cartSummary();
  cartEmpty.classList.toggle('hidden', items.length>0);
  cartTableBody.innerHTML = '';
  for(const it of items){
    const tr = document.createElement('tr');
    tr.innerHTML = `
      <td style="min-width:160px"><div style="font-weight:600">${escapeHtml(it.product.name)}</div><div class="muted">${it.product.cat}</div></td>
      <td>${escapeHtml(it.variant.label)}</td>
      <td><div>${fmtRub(it.unitPrice)}</div><div class="notice">${it.discountRate>0 ? `скидка ${(it.discountRate*100)|0}%` : ''}</div></td>
      <td class="qty">
        <button class="ghost" data-dec="${it.pid}__${it.vkey}" aria-label="Уменьшить">−</button>
        <input type="number" min="1" value="${it.qty}" data-qty="${it.pid}__${it.vkey}">
        <button class="ghost" data-inc="${it.pid}__${it.vkey}" aria-label="Увеличить">+</button>
      </td>
      <td>${fmtRub(it.lineTotal)}</td>
      <td><button class="ghost" data-del="${it.pid}__${it.vkey}" aria-label="Удалить">✕</button></td>
    `;
    cartTableBody.appendChild(tr);
  }
  cartTotalEl.textContent = fmtRub(total);
  cartCountEl.textContent = `${count} поз.`;
  cartDiscountFlag.textContent = anyDiscount ? 'Применены скидки на сыр' : '';
  cartNote.textContent = 'Скидки на сыр: ≥500 г — 5%, ≥700 г — 10%, ≥1000 г — 15% (по одному виду).';

  // handlers
  cartTableBody.querySelectorAll('button[data-dec]').forEach(b=> b.addEventListener('click', onDec));
  cartTableBody.querySelectorAll('button[data-inc]').forEach(b=> b.addEventListener('click', onInc));
  cartTableBody.querySelectorAll('button[data-del]').forEach(b=> b.addEventListener('click', onDel));
  cartTableBody.querySelectorAll('input[data-qty]').forEach(inp=>{
    inp.addEventListener('input', ()=>{
      const key = inp.getAttribute('data-qty');
      const n = clamp(parseInt(inp.value||'1',10), 1, 999);
      CART.lines[key].qty = n; LS.save(CART); renderCartModal(); renderCartBar();
    });
  });
}
function onDec(e){ const key = e.currentTarget.getAttribute('data-dec'); if(!CART.lines[key]) return; CART.lines[key].qty = Math.max(1, CART.lines[key].qty-1); LS.save(CART); renderCartModal(); renderCartBar(); }
function onInc(e){ const key = e.currentTarget.getAttribute('data-inc'); if(!CART.lines[key]) return; CART.lines[key].qty = Math.min(999, CART.lines[key].qty+1); LS.save(CART); renderCartModal(); renderCartBar(); }
function onDel(e){ const key = e.currentTarget.getAttribute('data-del'); delete CART.lines[key]; LS.save(CART); renderCartModal(); renderCartBar(); }

/* =========================
   Отправка в бота (Telegram.WebApp.sendData)
========================= */
function buildPayload(){
  const {items, total} = cartSummary();
  const itemsOut = items.map(it=>({
    id: it.product.id,
    name: it.product.name,
    cat: it.product.cat,
    variant: it.variant.label,
    qty: it.qty,
    unit_price_base: it.unitBase,
    discount_rate: it.discountRate,
    unit_price: it.unitPrice,
    line_total: it.lineTotal
  }));
  const meta = {
    ts: Date.now(),
    schema_ver: CONFIG.PAYLOAD_SCHEMA_VERSION,
    puzzlebot_hint: CONFIG.PUZZLEBOT_HINT ? { target:'inline_button->bot', webhook_hint: CONFIG.WEBHOOK_HINT } : undefined,
  };
  const comment = CONFIG.SHOW_COMMENT_FIELD ? (orderComment.value||'') : '';
  const payload = {
    type: 'cart',
    source: 'miniapp',
    currency: 'RUB',
    items: itemsOut,
    total,
    comment,
    meta
  };
  return payload;
}
function sendCart(){
  const {count} = cartSummary();
  if(count===0){ alert('Корзина пуста'); return; }
  const payload = JSON.stringify( buildPayload() );
  try{
    tg.sendData(payload);
  }catch(err){
    alert('Ошибка отправки. Смотрите консоль.'); console.error(err); console.log('payload:', payload);
  }
  // Закрываем мини-приложение
  try{ tg.close(); }catch(e){ /* preview mode */ }
}

/* =========================
   Telegram MainButton
========================= */
function updateMainButton(count, total){
  const text = count ? `Отправить • ${fmtRub(total)}` : 'Корзина пуста';
  try{
    tg.MainButton.setText(text);
    if(count){ tg.MainButton.show(); } else { tg.MainButton.hide(); }
    tg.MainButton.offClick?.();
    tg.MainButton.onClick(()=> sendCart());
  }catch(e){ /* preview fallback */ }
}

/* =========================
   Инициализация
========================= */
renderCatalog();
renderCartBar();

/* =========================
   Юнит-тесты (консоль)
   — проверка кейсов (4)
========================= */
(function runTests(){
  const clone = (x)=> JSON.parse(JSON.stringify(x));
  function add(pid, vkey, qty){ const k = makeCartKey(pid, vkey); if(!CART.lines[k]) CART.lines[k]={pid, vkey, qty:0}; CART.lines[k].qty+=qty }
  const original = clone(CART);

  // Кейс A — Качотта 2150 ₽/кг; 200 г ×1 и 300 г ×1 -> итог 1022 ₽
  CART.lines = {};
  const caciotta = CATALOG.find(p=>p.id==='caciotta'); const v200 = buildVariants(caciotta).find(v=>v.grams===200);
  const v300 = buildVariants(caciotta).find(v=>v.grams===300);
  add('caciotta', v200.key, 1); add('caciotta', v300.key, 1);
  let sumA = cartSummary().total;
  console.log('[TEST A] ожидаемо 1022 ₽ ->', sumA, 'OK?', sumA===1022);

  // Кейс B — Сулугуни 1400 ₽/кг; 250 г ×2 и 300 г ×1 -> 1008 ₽
  CART.lines = {};
  const sul = CATALOG.find(p=>p.id==='suluguni');
  const v250s = buildVariants(sul).find(v=>v.grams===200) ? null : null; // ensure search below
  const v250 = buildVariants(sul).find(v=>v.grams===250);
  const v300b = buildVariants(sul).find(v=>v.grams===300);
  add('suluguni', v250.key, 2); add('suluguni', v300b.key, 1);
  let sumB = cartSummary().total;
  console.log('[TEST B] ожидаемо 1008 ₽ ->', sumB, 'OK?', sumB===1008);

  // Кейс C — Халлуми классический (1 шт, 250 г) -> 413 ₽
  CART.lines = {};
  const hal = CATALOG.find(p=>p.id==='halloumi_classic');
  const v250u = buildVariants(hal).find(v=>v.type==='unit_weight' && v.grams===250);
  add('halloumi_classic', v250u.key, 1);
  let sumC = cartSummary().total;
  console.log('[TEST C] ожидаемо 413 ₽ ->', sumC, 'OK?', sumC===413);

  // Кейс D — Йогурт 0.5 л -> 115 ₽
  CART.lines = {};
  const yog = CATALOG.find(p=>p.id==='yogurt');
  const v05 = buildVariants(yog).find(v=>v.type==='volume' && v.liters===0.5);
  add('yogurt', v05.key, 1);
  let sumD = cartSummary().total;
  console.log('[TEST D] ожидаемо 115 ₽ ->', sumD, 'OK?', sumD===115);

  CART = original; LS.save(CART); renderCartBar();
})();

/* =========================
   Доступность: фокус на Esc — закрытие модалок
========================= */
document.addEventListener('keydown', (e)=>{
  if(e.key==='Escape'){
    if(productDialog.open) productDialog.close();
    if(cartDialog.open) cartDialog.close();
  }
});
</script>
</body>
</html>
