<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LEVEL X | GAMES STORE</title>
<style>
*{box-sizing:border-box}body{margin:0;background:#05070d;color:#f5f5f5;font-family:Arial,Helvetica,sans-serif}
.top{background:#8b5cf6;padding:9px 16px;text-align:center;font-weight:800;font-size:14px;white-space:nowrap;overflow:hidden}
.header{padding:22px 22px 18px;display:flex;align-items:center;gap:14px;border-bottom:1px solid #1d2a3d;background:#03050a}
.logo{width:58px;height:58px;border-radius:50%;background:#05070d;display:grid;place-items:center;overflow:hidden;flex:none}.logo img{width:100%;height:100%;object-fit:cover;display:block}
.brand h1{font-size:21px;margin:0 0 5px}.brand p{margin:0;color:#8d9bb0;font-size:14px}
.actions{margin-left:auto;display:flex;gap:10px}.currency-divider{opacity:.6;margin:0 3px}.currency,.cart{background:#0b1220;border:1px solid #24344d;border-radius:16px;padding:13px 15px}.cart{font-size:22px;position:relative}.badge{position:absolute;right:-5px;top:-7px;background:#8b5cf6;border-radius:50%;font-size:12px;padding:5px 8px}
main{max-width:760px;margin:auto;padding:48px 22px}.pill{display:inline-block;border:1px solid #2a2a31;border-radius:30px;padding:11px 20px;color:#dbe3ed;margin-bottom:28px}
h2{font-size:46px;line-height:1.05;margin:0 0 20px}.red{color:#8b5cf6}.lead{color:#aeb9c9;font-size:18px;line-height:1.7;max-width:650px}
.buttons{display:flex;gap:18px;margin:30px 0 42px}.btn{border:1px solid #2b2b34;background:#15151a;color:white;border-radius:18px;padding:18px 27px;font-size:17px;font-weight:800;cursor:pointer}.primary{background:#8b5cf6;border-color:#8b5cf6;box-shadow:0 10px 30px #8b5cf633}
.search{background:#15151a;border:1px solid #20314a;border-radius:18px;padding:19px;color:#8d9bb0;width:100%;font-size:16px;outline:none}.tags{display:flex;gap:10px;overflow:auto;margin:18px 0 28px}.tag{white-space:nowrap;border:1px solid #20314a;background:#080e18;border-radius:22px;padding:10px 16px;color:#d2dae5}
.tabs{display:flex;background:#0b1220;border:1px solid #20314a;border-radius:18px;padding:5px;margin-bottom:25px}.tab{flex:1;padding:15px;text-align:center;border-radius:14px;color:#8d9bb0;font-weight:700}.tab.active{background:#8b5cf6;color:white}
.site-section{display:none}.site-section.active{display:block}.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:16px}.card{background:#0b1220;border:1px solid #20314a;border-radius:20px;overflow:hidden}.cover{aspect-ratio:2/3;height:auto;display:flex;align-items:end;padding:0;font-size:25px;font-weight:900;background-size:cover;background-position:center;background-repeat:no-repeat};}.cover.game-image{overflow:hidden;display:block;padding:0}.cover.game-image img{width:100%;height:100%;object-fit:contain;object-position:center;display:block;background:#05070d}.gta{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/1174180/library_600x900.jpg");background-size:cover;background-position:center;background-repeat:no-repeat}.fc{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/2215430/library_600x900.jpg");background-size:cover;background-position:center center;background-repeat:no-repeat}.gta5{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/271590/library_600x900.jpg");background-size:cover;background-position:center;background-repeat:no-repeat};.mirage{background-image:url("https://media.gamestop.com/i/gamestop/20000926-3b0dde13");background-size:cover;background-position:center;background-repeat:no-repeat}.gow{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/2322010/library_600x900.jpg");background-size:cover;background-position:center;background-repeat:no-repeat}
    .wayout{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/1222700/library_600x900.jpg");background-size:cover;background-position:center;background-repeat:no-repeat}
.wwe{background-image:url("https://media.gamestop.com/i/gamestop/20032440-f4095b2b?fmt=auto&h=768&w=768");background-size:cover;background-position:center;background-repeat:no-repeat}
.info{padding:16px}.info h3{margin:0 0 8px}.price{color:#8b5cf6;font-weight:900}.buy{width:100%;margin-top:14px;padding:12px;border:0;border-radius:12px;background:#8b5cf6;color:white;font-weight:800}
@media(max-width:600px){main{padding:38px 18px}h2{font-size:38px}.grid{grid-template-columns:1fr}.currency{display:flex}.buttons{gap:10px}.btn{flex:1;padding:15px 10px}.brand h1{font-size:18px}}

.plus-section{margin-top:55px}.psplus-title{font-size:32px;color:#8b5cf6;margin:0 0 8px}.psplus-note{color:#8d9bb0;margin:0 0 20px}.psplus-card-img{width:100%;height:230px;object-fit:contain;object-position:center;display:block;border-bottom:1px solid #20314a;background:#05070d;padding:8px;box-sizing:border-box} .edition-img{width:calc(100% + 36px);height:250px;object-fit:cover;display:block;margin:-18px -18px 16px;border-bottom:1px solid #20314a;background:#05070d}.edition-img.fc-standard{object-position:center}.edition-img.fc-ultimate{object-position:center}.edition-img.gta-standard{object-position:center}.edition-img.gta-ultimate{object-position:center}.ps-group{background:#0b1220;border:1px solid #20314a;border-radius:20px;overflow:hidden;margin:16px 0}.ps-group h3,.ps-group .region,.ps-group .ps-row{margin-left:16px;margin-right:16px}.ps-group h3{margin-top:16px}
.ps-group{margin:18px 0;background:#0b1220;border:1px solid #20314a;border-radius:20px;padding:18px}.ps-group h3{margin:0 0 5px;color:#8b5cf6}.region{color:#8d9bb0;font-size:13px;margin-bottom:12px}
.ps-row{display:flex;justify-content:space-between;align-items:center;gap:12px;padding:12px 0;border-bottom:1px solid #1d2a3d}.ps-row:last-child{border-bottom:0}.ps-name{font-weight:700}.ps-type{color:#8d9bb0;font-size:13px}
.ps-actions{display:flex;align-items:center;gap:8px}.ps-price{color:#8b5cf6;font-weight:900;white-space:nowrap}.add{border:0;border-radius:9px;padding:8px 11px;background:#8b5cf6;color:#05070d;font-weight:900;cursor:pointer}
.modal{display:none;position:fixed;inset:0;background:#000b;z-index:20;align-items:center;justify-content:center;padding:20px}.modal.show{display:flex}.modal-box{width:min(430px,100%);background:#0b1220;border:1px solid #8b5cf6;border-radius:22px;padding:25px;position:relative}.modal-box strong{color:#8b5cf6}.close{border:0;background:none;color:#fff;font-size:28px;cursor:pointer}.modal-box .close{position:absolute;right:14px;top:8px}
.cart-panel{position:fixed;right:-390px;top:0;width:min(390px,100%);height:100vh;background:#070c15;border-left:1px solid #24344d;z-index:30;padding:20px;transition:.25s;overflow:auto}.cart-panel.open{right:0}.cart-head{display:flex;justify-content:space-between;align-items:center}.cart-item{padding:14px 0;border-bottom:1px solid #20314a}.cart-item b{color:#8b5cf6}.cart-total{padding:20px 0;font-size:20px}.checkout{margin-top:8px;background:#25D366!important;color:#fff}
@media(max-width:600px){.ps-row{align-items:flex-start}.ps-actions{flex-direction:column;align-items:flex-end}}
.spiderman2{background-image:url("https://cdn.akamai.steamstatic.com/steam/apps/2651280/library_600x900.jpg");background-size:cover;background-position:center;background-repeat:no-repeat}
.plus-details-btn{margin:10px 12px 0 !important;width:calc(100% - 24px) !important}
.plus-detail-card .plus-details-only{display:none;margin-top:14px;padding:14px;border:1px solid rgba(126,92,255,.35);border-radius:14px;background:rgba(8,10,22,.72)}
.plus-detail-card .plus-details-title{font-weight:900;color:#9bdcff;margin-bottom:10px;font-size:16px}
.plus-detail-line{display:flex;justify-content:space-between;gap:12px;padding:9px 0;border-bottom:1px solid rgba(255,255,255,.08);font-size:14px}
.plus-detail-line:last-child{border-bottom:0}
.plus-detail-line b{color:#fff}.plus-detail-line span{color:#aeb8ca;text-align:left}
</style>

<style id="compact-site-scale">
  body { zoom: 0.90; }
  @media (max-width: 700px) {
    body { zoom: 0.94; }
  }
</style>


<style>
.whatsapp-btn{display:inline-flex;align-items:center;gap:8px;padding:12px 18px;border-radius:12px;background:#25D366;color:#071b10;font-weight:900;text-decoration:none;border:0;cursor:pointer;transition:.2s;box-shadow:0 0 0 rgba(37,211,102,0)}
.whatsapp-btn:active{transform:scale(.94);box-shadow:0 0 24px rgba(37,211,102,.8);}
</style>
<style id="whatsapp-icon-style">
.whatsapp-icon{width:42px;height:42px;border:1px solid #20314a;border-radius:12px;background:#0b1220;color:#25D366;display:inline-flex;align-items:center;justify-content:center;font-size:22px;text-decoration:none;margin-left:8px;transition:.2s;vertical-align:middle}.whatsapp-icon:hover{transform:scale(1.05);box-shadow:0 0 14px rgba(37,211,102,.25)}
</style><style id="whatsapp-top-icon-fix">.whatsapp-top-icon{display:flex;width:46px;height:46px;margin:0 auto 12px;align-items:center;justify-content:center;border:1px solid #20314a;border-radius:14px;background:#0b1220;color:#25D366;text-decoration:none;font-size:24px;box-shadow:0 0 12px rgba(37,211,102,.15);transition:.2s}.whatsapp-top-icon:hover{transform:scale(1.06);box-shadow:0 0 18px rgba(37,211,102,.3)}
.currency-wrap{position:relative}.currency{display:flex;align-items:center;gap:7px;cursor:pointer;color:#fff;font-weight:800}.currency-arrow{font-size:14px;color:#8b5cf6}.currency-menu{position:absolute;right:0;top:calc(100% + 10px);width:245px;background:linear-gradient(145deg,#070b12,#111827);border:1px solid #8b5cf6;border-radius:16px;padding:10px;z-index:9999;box-shadow:0 18px 45px #0008;display:none}.currency-menu.open{display:block}.currency-title{padding:8px 10px;color:#8b5cf6;font-weight:900;border-bottom:1px solid #24344d;margin-bottom:6px}.currency-option{width:100%;display:flex;align-items:center;gap:10px;background:transparent;border:0;color:#fff;padding:10px;border-radius:10px;cursor:pointer;text-align:left;font-size:15px}.currency-option:hover{background:#1d2a3d}.currency-option .flag{font-size:22px}.currency-option .code{font-weight:900}.currency-option .name{color:#9aa7b9;font-size:12px;margin-left:auto}.price-line{display:flex;flex-wrap:wrap;align-items:baseline;gap:7px}.foreign-price{color:#8fd3ff;font-size:12px;font-weight:800}.currency-note{color:#6f7d90;font-size:10px;margin-top:2px}@media(max-width:600px){.currency-menu{right:-45px;width:225px}.actions{gap:6px}.currency{padding:11px 10px;font-size:13px}}

/* stability fixes */
body{min-height:100vh;overflow-x:hidden}
main{width:100%}
.site-section{width:100%}
.card,.ps-group{min-width:0}
@media(max-width:600px){.header{padding:14px}.brand h1{font-size:17px}.brand p{font-size:12px}.actions{gap:6px}.currency{padding:10px 9px}.cart{padding:10px 11px}.buttons{flex-wrap:wrap;gap:10px}.btn{flex:1 1 100%;padding:15px 18px}.grid{grid-template-columns:1fr}h2{font-size:34px}.lead{font-size:16px}.tabs{overflow:auto}.tab{min-width:150px;padding:12px 8px;font-size:13px}.ps-row{gap:10px}.ps-actions{flex-wrap:wrap}}
</style>
<style id="extra-polish">
header,main{position:relative}
.card{transition:transform .22s ease,box-shadow .22s ease,border-color .22s ease}
.card:hover{transform:translateY(-5px);box-shadow:0 12px 35px rgba(0,0,0,.45),0 0 18px rgba(0,217,255,.10);border-color:rgba(0,217,255,.55)}
</style>


<style id="details-layout-style">
/* Two game cards per row */
.grid{grid-template-columns:repeat(2,minmax(0,1fr));gap:16px}
.info{padding:14px}
.game-details-btn{width:100%;margin-top:12px;padding:12px;border:1px solid #8b5cf6;border-radius:12px;background:#121a29;color:#8b5cf6;font-weight:900;font-size:15px;cursor:pointer}
.game-details-btn:hover{background:#8b5cf6;color:#05070d}
.card .ps-row,.card .buy{display:none!important}
.details-modal{position:fixed;inset:0;z-index:1000000;background:rgba(0,0,0,.78);display:none;align-items:center;justify-content:center;padding:18px}
.details-modal.show{display:flex}
.details-box{width:min(520px,100%);max-height:90vh;overflow:auto;background:#0b1220;border:1px solid #8b5cf6;border-radius:20px;padding:18px;box-shadow:0 20px 60px rgba(0,0,0,.55)}
.details-close{float:right;width:38px;height:38px;border:1px solid #24344d;border-radius:50%;background:#121a29;color:#fff;font-size:22px;cursor:pointer}
.details-cover{width:100%;aspect-ratio:2/3;object-fit:cover;border-radius:14px;display:block;background:#05070d;margin-bottom:16px}
.details-title{margin:0 45px 6px 0;font-size:24px}
.details-platform{color:#8d9bb0;margin:0 0 14px}
.details-description{color:#d7deea;line-height:1.6;margin:0 0 16px}
.details-prices{border-top:1px solid #24344d;padding-top:10px}
.details-price-row{display:flex;justify-content:space-between;gap:12px;padding:11px 0;border-bottom:1px solid #24344d}
.details-price-row b{color:#8b5cf6}
.details-buy{width:100%;margin-top:10px;padding:11px;border:0;border-radius:12px;background:#8b5cf6;color:#05070d;font-weight:900;cursor:pointer}
@media(max-width:600px){.grid{grid-template-columns:repeat(2,minmax(0,1fr)) !important;gap:10px !important}.info{padding:9px}.info h3{font-size:13px;line-height:1.2}.game-details-btn{font-size:11px;padding:9px 4px;margin-top:8px}.details-modal{padding:10px}.details-box{width:min(340px,92vw) !important;max-height:78vh !important;padding:12px !important;border-radius:16px !important}.details-cover{width:150px !important;height:190px !important;aspect-ratio:auto !important;object-fit:cover !important;margin:0 auto 10px !important;border-radius:10px !important}.details-title{font-size:18px !important;margin-right:38px}.details-platform{font-size:12px;margin-bottom:10px}.details-description{font-size:12px;line-height:1.45;margin-bottom:10px}.details-price-row{font-size:12px;padding:8px 0}.details-buy{font-size:12px;padding:9px;margin-top:7px}.details-close{width:32px;height:32px;font-size:19px}}
@media(min-width:601px){.grid{grid-template-columns:repeat(2,minmax(0,1fr)) !important}.details-box{width:min(380px,92vw) !important;max-height:82vh !important}.details-cover{width:170px !important;height:215px !important;aspect-ratio:auto !important;object-fit:cover !important;margin:0 auto 12px !important}}
</style>

<style id="final-layout-fix">
/* Final mobile two-column layout */
.grid { display:grid !important; grid-template-columns:repeat(2,minmax(0,1fr)) !important; gap:10px !important; }
@media (max-width:600px){
  main{padding:30px 12px !important;}
  .grid{grid-template-columns:repeat(2,minmax(0,1fr)) !important;gap:8px !important;}
  .card{border-radius:12px !important;}
  .cover{aspect-ratio:2/3 !important;}
  .info{padding:8px !important;}
  .info h3{font-size:12px !important;line-height:1.2 !important;}
  .game-details-btn{font-size:11px !important;padding:8px 3px !important;margin-top:6px !important;}
}
/* Smaller details popup */
.details-modal{padding:8px !important;}
.details-box{width:min(300px,88vw) !important;max-height:75vh !important;padding:10px !important;border-radius:14px !important;}
.details-cover{width:115px !important;height:145px !important;object-fit:cover !important;margin:0 auto 8px !important;}
.details-title{font-size:16px !important;}
.details-platform,.details-description,.details-price-row,.details-buy{font-size:11px !important;}
.details-description{line-height:1.35 !important;}
.details-price-row{padding:6px 0 !important;}
.details-buy{padding:7px !important;margin-top:5px !important;}
</style>

<style id="account-help-style">
.account-help{margin-top:12px;padding:10px 12px;border:1px solid #20314a;border-radius:12px;background:#080f1b}.account-help h4{margin:0 0 6px;color:#8b5cf6;font-size:13px}.account-help p{margin:5px 0;color:#c9d2df;font-size:11px;line-height:1.5}.account-help b{color:#fff}
</style>

<style id="equal-games-style">
#products.grid{display:grid !important;grid-template-columns:repeat(2,minmax(0,1fr)) !important;align-items:start !important;gap:12px !important}
#products.grid .card{display:flex !important;flex-direction:column !important;height:auto !important;min-width:0 !important}
#products.grid .cover{width:100% !important;aspect-ratio:2/3 !important;height:auto !important;flex:0 0 auto !important;overflow:hidden !important}
#products.grid .info{display:flex !important;flex-direction:column !important;flex:1 !important}
#products.grid .game-details-btn{margin-top:auto !important}
@media(max-width:600px){#products.grid{grid-template-columns:repeat(2,minmax(0,1fr)) !important;gap:8px !important}#products.grid .card{border-radius:12px !important}#products.grid .cover{aspect-ratio:2/3 !important}#products.grid .info{padding:8px !important}#products.grid .info h3{font-size:12px !important;min-height:30px !important}#products.grid .info p{font-size:10px !important;min-height:24px !important}}
</style>

<style id="store-feature-style">
#products.grid{background:transparent !important;}
.store-feature-card{background:linear-gradient(145deg,#111827,#070b12);border:1px solid #8b5cf6;border-radius:20px;overflow:hidden;min-width:0;display:flex;align-items:center;justify-content:center;text-align:center;padding:20px;min-height:100%;position:relative;}
.store-feature-card:before,.store-feature-card:after{content:"";position:absolute;border:1px solid #8b5cf6;border-radius:50%;opacity:.18;}
.store-feature-card:before{width:150px;height:150px;top:-75px;right:-55px;}
.store-feature-card:after{width:120px;height:120px;bottom:-60px;left:-45px;}
.store-feature-inner{position:relative;z-index:1;}
.store-feature-logo{font-size:25px;font-weight:1000;letter-spacing:2px;color:#8b5cf6;margin-bottom:8px;}
.store-feature-title{font-size:16px;font-weight:900;color:#fff;margin-bottom:10px;}
.store-feature-text{font-size:11px;line-height:1.7;color:#aeb9c9;margin:0 0 12px;}
.store-feature-points{display:grid;gap:7px;text-align:left;font-size:11px;color:#dbe3ed;}
.store-feature-points span{display:block;padding:7px 9px;border:1px solid #24344d;border-radius:9px;background:#0b1220;}
.store-feature-points b{color:#8b5cf6;}
@media(max-width:600px){.store-feature-card{border-radius:12px;padding:10px;}.store-feature-logo{font-size:17px;letter-spacing:1px}.store-feature-title{font-size:12px}.store-feature-text,.store-feature-points{font-size:9px}.store-feature-points{gap:5px}.store-feature-points span{padding:5px 6px}}
</style>

<style id="fix-yellow-and-gaps">
/* Prevent the whole games section from turning gold */
.site-section.active{background:transparent !important;color:inherit !important;}
/* Keep cards compact instead of stretching to the tallest card in the row */
#products.grid{align-items:stretch !important;}
#products.grid .card{align-self:stretch !important;height:100% !important;}
#products.grid .store-feature-card{align-self:start !important;height:100% !important;min-height:0 !important;}
@media(max-width:600px){
  #products.grid{align-items:stretch !important;}
  #products.grid .card{align-self:stretch !important;height:100% !important;}
  #products.grid .store-feature-card{align-self:stretch !important;height:auto !important;min-height:0 !important;}
}
</style>

<style id="plus-games-card-style">
/* PS Plus cards match the Games page cards */
#plusList.plus-games-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px;align-items:stretch}
#plusList.plus-games-grid .ps-group{margin:0;padding:0;background:#0b1220;border:1px solid #20314a;border-radius:20px;overflow:hidden;display:flex;flex-direction:column;min-width:0;height:100%}
#plusList.plus-games-grid .psplus-card-img{width:100%;height:auto;aspect-ratio:2/3;object-fit:cover;object-position:center;display:block;padding:0;border:0;background:#05070d}
#plusList.plus-games-grid .ps-group h3{padding:12px 12px 4px;margin:0;color:#c4b5fd;font-size:16px;line-height:1.25}
#plusList.plus-games-grid .ps-group .region{padding:0 12px 10px;margin:0;color:#8d9bb0;font-size:11px;line-height:1.35}
#plusList.plus-games-grid .ps-row{margin:0 12px;padding:9px 0;min-height:42px}
#plusList.plus-games-grid .ps-name{font-size:12px}.ps-type{font-size:10px}
#plusList.plu
