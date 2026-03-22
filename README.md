[SuperCash_Trial_1Hour_Updated.html](https://github.com/user-attachments/files/26165216/SuperCash_Trial_1Hour_Updated.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>💰 SuperCash Pro — نسخة مجانية ساعة</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Segoe UI',Tahoma,Arial,sans-serif;background:#f1f5f9;color:#1e293b;min-height:100vh}

/* ===== EXPIRED SCREEN ===== */
#expired-screen{position:fixed;inset:0;background:linear-gradient(135deg,#1a1f2e,#1e3a5f);display:none;align-items:center;justify-content:center;z-index:999;flex-direction:column;gap:0}
.exp-box{background:#fff;border-radius:20px;padding:36px 32px;width:400px;box-shadow:0 32px 80px rgba(0,0,0,.4);text-align:center}
.exp-icon{font-size:52px;margin-bottom:16px}
.exp-title{font-size:22px;font-weight:700;color:#dc2626;margin-bottom:8px}
.exp-sub{font-size:14px;color:#64748b;margin-bottom:24px;line-height:1.7}
.exp-field{display:flex;flex-direction:column;gap:6px;margin-bottom:14px;text-align:right}
.exp-label{font-size:12px;font-weight:500;color:#64748b}
.exp-input{padding:11px 14px;border:1.5px solid #e2e8f0;border-radius:8px;font-size:15px;font-family:inherit;color:#1e293b;letter-spacing:2px;direction:ltr;text-align:center}
.exp-input:focus{outline:none;border-color:#3b82f6}
.exp-btn{width:100%;padding:13px;background:#3b82f6;color:white;border:none;border-radius:10px;font-size:15px;font-weight:500;cursor:pointer;font-family:inherit;transition:background .15s}
.exp-btn:hover{background:#2563eb}
.exp-error{background:#fee2e2;color:#dc2626;padding:8px 12px;border-radius:7px;font-size:12px;margin-top:8px;display:none;text-align:center}
.exp-contact{margin-top:20px;padding:14px;background:#f8fafc;border-radius:10px;border:1px solid #e2e8f0}
.exp-contact-text{font-size:12px;color:#64748b;margin-bottom:6px}
.exp-contact-num{font-size:18px;font-weight:700;color:#3b82f6;direction:ltr}

/* ===== TRIAL BANNER ===== */
#trial-banner{background:linear-gradient(90deg,#f59e0b,#d97706);color:white;padding:7px 16px;font-size:12px;display:flex;align-items:center;justify-content:space-between;flex-shrink:0}
#trial-banner.danger{background:linear-gradient(90deg,#ef4444,#dc2626)}
#trial-banner.hidden{display:none}

/* ===== LAYOUT ===== */
.pos-wrapper{display:flex;height:calc(100vh - 0px);overflow:hidden}
.sidebar{width:210px;background:#1a1f2e;color:#e2e8f0;display:flex;flex-direction:column;flex-shrink:0}
.main-area{flex:1;display:flex;flex-direction:column;overflow:hidden}
.content{flex:1;overflow-y:auto}

.logo{padding:16px 14px;border-bottom:1px solid rgba(255,255,255,.08)}
.logo-text{font-size:17px;font-weight:700;color:#60a5fa}
.logo-sub{font-size:10px;color:#64748b;margin-top:2px}
.nav-section{padding:10px 0}
.nav-label{font-size:10px;color:#475569;padding:4px 14px;text-transform:uppercase;letter-spacing:.5px}
.nav-item{display:flex;align-items:center;gap:8px;padding:9px 14px;cursor:pointer;font-size:13px;color:#94a3b8;transition:all .15s;border-right:3px solid transparent}
.nav-item:hover{background:rgba(255,255,255,.05);color:#e2e8f0}
.nav-item.active{background:rgba(96,165,250,.1);color:#60a5fa;border-right-color:#60a5fa}
.nav-icon{font-size:14px;width:18px;text-align:center}
.support-box{margin:0 10px 14px;background:rgba(96,165,250,.08);border:1px solid rgba(96,165,250,.2);border-radius:10px;padding:10px 12px}
.support-label{font-size:10px;color:#64748b;margin-bottom:4px}
.support-number{font-size:13px;font-weight:600;color:#60a5fa;direction:ltr;text-align:center}
.support-hint{font-size:10px;color:#475569;text-align:center;margin-top:3px}

.topbar{background:#fff;border-bottom:1px solid #e2e8f0;padding:10px 16px;display:flex;align-items:center;justify-content:space-between;flex-shrink:0}
.topbar-title{font-size:15px;font-weight:500}
.topbar-actions{display:flex;gap:8px;align-items:center}
.user-chip{display:flex;align-items:center;gap:6px;background:#f1f5f9;border-radius:20px;padding:4px 10px;font-size:12px;border:1px solid #e2e8f0}
.avatar{width:22px;height:22px;border-radius:50%;background:#3b82f6;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:600;color:white}

.btn{padding:7px 14px;border-radius:7px;font-size:12px;cursor:pointer;border:1px solid #e2e8f0;background:#fff;color:#374151;transition:all .15s;font-family:inherit}
.btn:hover{background:#f8fafc}
.btn-primary{background:#3b82f6;color:white;border-color:#3b82f6}
.btn-primary:hover{background:#2563eb}
.btn-success{background:#22c55e;color:white;border-color:#22c55e}
.btn-success:hover{background:#16a34a}
.btn-danger{background:#ef4444;color:white;border-color:#ef4444}
.card{background:#fff;border:1px solid #e2e8f0;border-radius:10px;padding:14px}
.card-title{font-size:13px;font-weight:500;margin-bottom:12px;color:#374151}

/* POS */
.pos-screen{display:flex;gap:12px;padding:12px;height:100%}
.products-panel{flex:1;display:flex;flex-direction:column;min-width:0}
.search-bar{display:flex;gap:8px;margin-bottom:10px}
.search-bar input{flex:1;padding:8px 12px;border:1px solid #e2e8f0;border-radius:8px;background:#fff;font-size:13px;font-family:inherit;color:#1e293b}
.search-bar input:focus{outline:none;border-color:#3b82f6}
.categories{display:flex;gap:6px;margin-bottom:10px;flex-wrap:wrap}
.cat-btn{padding:5px 12px;border-radius:20px;font-size:11px;cursor:pointer;border:1px solid #e2e8f0;background:#fff;color:#64748b;transition:all .15s}
.cat-btn.active,.cat-btn:hover{background:#3b82f6;color:white;border-color:#3b82f6}
.products-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;overflow-y:auto;flex:1}
.product-card{background:#fff;border:1px solid #e2e8f0;border-radius:10px;padding:12px 8px;text-align:center;cursor:pointer;transition:all .15s}
.product-card:hover{border-color:#3b82f6;transform:translateY(-1px);box-shadow:0 2px 8px rgba(59,130,246,.15)}
.product-card:active{transform:scale(.97)}
.product-icon{font-size:28px;margin-bottom:6px}
.product-name{font-size:11px;font-weight:500;margin-bottom:4px;color:#374151}
.product-price{font-size:13px;color:#3b82f6;font-weight:600}
.product-stock{font-size:10px;color:#94a3b8;margin-top:2px}
.empty-big{display:flex;flex-direction:column;align-items:center;justify-content:center;height:100%;gap:12px;color:#94a3b8;text-align:center;padding:20px}
.add-big-btn{background:#3b82f6;color:white;border:none;border-radius:10px;padding:12px 24px;font-size:14px;cursor:pointer;font-family:inherit;margin-top:4px}
.add-big-btn:hover{background:#2563eb}

.cart-panel{width:290px;background:#fff;border-radius:12px;border:1px solid #e2e8f0;display:flex;flex-direction:column;flex-shrink:0}
.cart-header{padding:12px 14px;border-bottom:1px solid #e2e8f0;font-weight:500;font-size:14px;display:flex;justify-content:space-between;align-items:center}
.cart-items{flex:1;overflow-y:auto;padding:10px;min-height:100px}
.cart-item{display:flex;align-items:center;gap:8px;padding:8px 0;border-bottom:1px solid #f1f5f9}
.cart-item-name{flex:1;font-size:12px;color:#374151}
.cart-qty{display:flex;align-items:center;gap:4px}
.qty-btn{width:22px;height:22px;border-radius:50%;border:1px solid #e2e8f0;background:#f8fafc;cursor:pointer;font-size:14px;display:flex;align-items:center;justify-content:center;color:#374151}
.qty-num{font-size:12px;min-width:20px;text-align:center;font-weight:500}
.cart-item-price{font-size:12px;font-weight:500;min-width:70px;text-align:left;color:#374151}
.cart-footer{padding:12px 14px;border-top:1px solid #e2e8f0}
.cart-row{display:flex;justify-content:space-between;font-size:12px;color:#64748b;margin-bottom:4px}
.cart-row.total{font-size:16px;font-weight:600;color:#1e293b;margin-top:6px;padding-top:6px;border-top:1px solid #e2e8f0}
.pay-methods{display:flex;gap:6px;margin-bottom:10px}
.pay-btn{flex:1;padding:7px 4px;border-radius:7px;font-size:11px;cursor:pointer;border:1px solid #e2e8f0;background:#f8fafc;color:#64748b;transition:all .15s;text-align:center;font-family:inherit}
.pay-btn.active{background:#dbeafe;color:#1d4ed8;border-color:#93c5fd;font-weight:500}
.checkout-btn{width:100%;padding:12px;background:#3b82f6;color:white;border:none;border-radius:8px;font-size:14px;font-weight:500;cursor:pointer;font-family:inherit}
.checkout-btn:hover{background:#2563eb}
.empty-cart{text-align:center;padding:30px 10px;color:#94a3b8;font-size:13px}

/* Inventory */
.inventory-section{padding:16px}
.toolbar{display:flex;align-items:center;gap:10px;margin-bottom:14px;flex-wrap:wrap}
.toolbar input{flex:1;min-width:150px;padding:8px 12px;border:1px solid #e2e8f0;border-radius:8px;background:#fff;font-size:13px;font-family:inherit;color:#1e293b}
.toolbar input:focus{outline:none;border-color:#3b82f6}
.data-table{width:100%;border-collapse:collapse;font-size:12px}
.data-table th{text-align:right;padding:10px 12px;border-bottom:1px solid #e2e8f0;font-weight:500;font-size:11px;color:#64748b;background:#f8fafc}
.data-table td{padding:10px 12px;border-bottom:1px solid #f1f5f9;vertical-align:middle;color:#374151}
.data-table tr:hover td{background:#f8fafc}
.stock-badge{display:inline-block;padding:2px 8px;border-radius:10px;font-size:10px;font-weight:500}
.stock-ok{background:#dcfce7;color:#166534}
.stock-low{background:#fef3c7;color:#92400e}
.stock-out{background:#fee2e2;color:#991b1b}
.empty-td{text-align:center;padding:40px;color:#94a3b8;font-size:13px}

/* CRM */
.crm-section{padding:16px}
.crm-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.customer-card{background:#fff;border:1px solid #e2e8f0;border-radius:10px;padding:14px;cursor:pointer;transition:all .15s}
.customer-card:hover{border-color:#3b82f6}
.cstat{background:#f8fafc;border-radius:7px;padding:8px}
.cstat-label{font-size:10px;color:#64748b}
.cstat-val{font-size:13px;font-weight:500;margin-top:2px;color:#1e293b}
.loyalty-bar{height:4px;background:#e2e8f0;border-radius:2px;margin-top:8px}
.loyalty-fill{height:4px;background:#f59e0b;border-radius:2px}
.loyalty-label{font-size:10px;color:#64748b;margin-top:3px;display:flex;justify-content:space-between}

/* Dashboard */
.dashboard{padding:16px}
.stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-bottom:16px}
.stat-card{background:#fff;border:1px solid #e2e8f0;border-radius:10px;padding:14px}
.stat-label{font-size:11px;color:#64748b;margin-bottom:6px}
.stat-value{font-size:20px;font-weight:500;color:#1e293b}
.stat-sub{font-size:11px;color:#64748b;margin-top:4px}
.charts-row{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px}
.top-items{display:flex;flex-direction:column;gap:8px}
.top-item{display:flex;align-items:center;gap:10px}
.top-item-name{flex:1;font-size:12px;color:#374151}
.top-item-bar-wrap{width:80px;height:6px;background:#e2e8f0;border-radius:3px}
.top-item-bar{height:6px;background:#3b82f6;border-radius:3px}
.top-item-val{font-size:12px;font-weight:500;min-width:60px;text-align:left;color:#374151}

/* Reports */
.reports-section{padding:16px}
.report-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}

/* Users */
.users-section{padding:16px}
.users-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-bottom:16px}
.user-card{background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:16px;text-align:center}
.user-card-avatar{width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:20px;font-weight:600;color:white;margin:0 auto 10px}
.user-card-name{font-size:14px;font-weight:500;color:#1e293b;margin-bottom:4px}
.user-card-role{font-size:11px;padding:2px 10px;border-radius:10px;display:inline-block;margin-bottom:12px}
.role-admin{background:#dbeafe;color:#1d4ed8}
.role-cashier{background:#dcfce7;color:#166534}
.ustat{background:#f8fafc;border-radius:7px;padding:7px}
.ustat-label{font-size:10px;color:#64748b}
.ustat-val{font-size:13px;font-weight:500;margin-top:1px;color:#1e293b}
.user-card-actions{display:flex;gap:6px;margin-top:12px}
.user-card-actions button{flex:1;padding:6px;border-radius:6px;font-size:11px;cursor:pointer;border:1px solid #e2e8f0;background:#f8fafc;color:#374151;font-family:inherit}

/* Backup */
.backup-section{padding:16px}
.backup-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.backup-card{background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:20px}
.backup-icon{font-size:36px;margin-bottom:12px}
.backup-title{font-size:15px;font-weight:500;margin-bottom:6px;color:#1e293b}
.backup-desc{font-size:12px;color:#64748b;margin-bottom:16px;line-height:1.6}
.backup-history{display:flex;flex-direction:column;gap:8px}
.backup-item{display:flex;align-items:center;gap:10px;padding:10px;background:#f8fafc;border-radius:8px;border:1px solid #e2e8f0}
.backup-item-info{flex:1}
.backup-item-date{font-size:12px;font-weight:500;color:#1e293b}
.backup-item-size{font-size:11px;color:#64748b}
.backup-status{font-size:10px;padding:2px 8px;border-radius:8px;background:#dcfce7;color:#166534}

/* Branches */
.branches-section{padding:16px}
.branches-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.branch-card{background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:16px;position:relative;transition:all .15s}
.branch-card:hover{border-color:#3b82f6}
.branch-card.new-branch{border:2px dashed #cbd5e1;display:flex;flex-direction:column;align-items:center;justify-content:center;cursor:pointer;min-height:180px;gap:8px}
.branch-card.new-branch:hover{border-color:#3b82f6;background:#eff6ff}
.branch-status{position:absolute;top:12px;left:12px;padding:3px 8px;border-radius:10px;font-size:10px;font-weight:500}
.branch-active{background:#dcfce7;color:#166534}
.branch-pending{background:#fef3c7;color:#92400e}
.bstat{background:#f8fafc;border-radius:7px;padding:8px}
.bstat-label{font-size:10px;color:#64748b}
.bstat-val{font-size:13px;font-weight:500;margin-top:2px;color:#1e293b}
.branch-stats{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-top:10px}
.branch-actions{display:flex;gap:6px;margin-top:12px}
.branch-actions button{flex:1;padding:6px;border-radius:6px;font-size:11px;cursor:pointer;border:1px solid #e2e8f0;background:#f8fafc;color:#374151;font-family:inherit}
.steps-bar{display:flex;align-items:center;margin-bottom:20px}
.step{display:flex;align-items:center;gap:6px;font-size:12px;color:#94a3b8}
.step-num{width:24px;height:24px;border-radius:50%;border:1.5px solid #e2e8f0;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:500}
.step.active .step-num{background:#3b82f6;color:white;border-color:#3b82f6}
.step.done .step-num{background:#22c55e;color:white;border-color:#22c55e}
.step.active{color:#1e293b;font-weight:500}
.step-line{flex:1;height:1px;background:#e2e8f0;margin:0 8px}
.branch-form{background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:20px}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-bottom:18px}
.form-group{display:flex;flex-direction:column;gap:6px}
.form-group.full{grid-column:1/-1}
.form-label{font-size:12px;font-weight:500;color:#64748b}
.form-input{padding:9px 12px;border:1px solid #e2e8f0;border-radius:8px;background:#f8fafc;color:#1e293b;font-size:13px;font-family:inherit}
.form-input:focus{outline:none;border-color:#3b82f6;background:#fff}
.form-select{padding:9px 12px;border:1px solid #e2e8f0;border-radius:8px;background:#f8fafc;color:#1e293b;font-size:13px;font-family:inherit;cursor:pointer}
.form-section-title{font-size:12px;font-weight:500;color:#64748b;border-bottom:1px solid #e2e8f0;padding-bottom:8px;grid-column:1/-1}
.check-item{display:flex;align-items:center;gap:8px;font-size:13px;cursor:pointer;margin-bottom:8px;color:#374151}
.check-item input{accent-color:#3b82f6;width:15px;height:15px}
.form-actions{display:flex;gap:10px;justify-content:flex-end}

/* Modals */
.modal-overlay{position:fixed;inset:0;background:rgba(0,0,0,.45);display:flex;align-items:center;justify-content:center;z-index:200}
.modal{background:#fff;border-radius:12px;padding:20px;width:380px;border:1px solid #e2e8f0;max-height:90vh;overflow-y:auto;box-shadow:0 20px 60px rgba(0,0,0,.15)}
.modal-title{font-size:15px;font-weight:500;margin-bottom:16px;color:#1e293b}
.modal-row{display:flex;justify-content:space-between;padding:7px 0;font-size:13px;border-bottom:1px solid #f1f5f9;color:#374151}
.modal-actions{display:flex;gap:8px;margin-top:14px}
.modal-btn{flex:1;padding:9px;border-radius:8px;font-size:13px;cursor:pointer;border:1px solid #e2e8f0;background:#f8fafc;color:#374151;font-family:inherit}
.modal-btn.confirm{background:#22c55e;color:white;border-color:#22c55e}
.modal-btn.blue{background:#3b82f6;color:white;border-color:#3b82f6}
.modal-support{margin-top:12px;padding:9px 12px;background:#eff6ff;border-radius:8px;display:flex;align-items:center;gap:8px;border:1px solid #bfdbfe}
.modal-support-text{font-size:11px;color:#1e40af}
.icon-grid{display:grid;grid-template-columns:repeat(8,1fr);gap:5px;margin-top:6px}
.icon-opt{font-size:20px;text-align:center;padding:5px;border-radius:7px;cursor:pointer;border:1.5px solid transparent;transition:all .15s}
.icon-opt:hover,.icon-opt.selected{border-color:#3b82f6;background:#eff6ff}

.notification{position:fixed;top:14px;left:50%;transform:translateX(-50%);background:#1e293b;color:white;padding:9px 18px;border-radius:8px;font-size:13px;z-index:400;opacity:0;transition:opacity .3s;pointer-events:none;white-space:nowrap;box-shadow:0 4px 16px rgba(0,0,0,.2)}
.notification.show{opacity:1}
.pb-wrap{height:5px;background:#e2e8f0;border-radius:3px;width:70px;display:inline-block}
.pb-fill{height:5px;border-radius:3px}
@keyframes scan-line{0%{top:20%}50%{top:80%}100%{top:20%}}
</style>
</head>
<body>

<!-- ===== TRIAL BANNER ===== -->
<div id="trial-banner">
  <span>⏳ نسخة مجانية — متبقي <strong id="days-left">60 دقيقة</strong></span>
  <span style="font-size:11px;opacity:.85">للتفعيل الكامل اتصل: 07772234981</span>
</div>

<!-- ===== EXPIRED SCREEN ===== -->
<div id="expired-screen">
  <div class="exp-box">
    <div class="exp-icon">🔒</div>
    <div class="exp-title">انتهت مدة التجربة</div>
    <div class="exp-sub">
      انتهت فترة التجربة المجانية (ساعة واحدة)<br>
      أدخل كود التفعيل للاستمرار في استخدام النظام<br>
      <strong style="color:#374151">بياناتك محفوظة ولن تُحذف</strong>
    </div>
    <div class="exp-field">
      <label class="exp-label">كود التفعيل</label>
      <input class="exp-input" id="activation-code" placeholder="XXXX-XXXX-XXXX" maxlength="14" oninput="formatCode(this)" onkeydown="if(event.key==='Enter')activateCode()">
    </div>
    <button class="exp-btn" onclick="activateCode()">🔓 تفعيل النظام</button>
    <div class="exp-error" id="activation-error">❌ كود غير صحيح — تأكد من الكود أو تواصل معنا</div>
    <div class="exp-contact">
      <div class="exp-contact-text">للحصول على كود التفعيل تواصل معنا:</div>
      <div class="exp-contact-num">📞 07772234981</div>
    </div>
  </div>
</div>

<!-- ===== APP ===== -->
<div id="app" style="display:none">
<div class="pos-wrapper">
  <div class="sidebar">
    <div class="logo">
      <div class="logo-text">💰 SuperCash Pro</div>
      <div class="logo-sub" id="sb-sub">مجاني — ساعة واحدة</div>
    </div>
    <div class="nav-section">
      <div class="nav-label">العمليات</div>
      <div class="nav-item active" onclick="showPage('pos')"><span class="nav-icon">🛒</span> البيع السريع</div>
      <div class="nav-item" onclick="showPage('inventory')"><span class="nav-icon">📦</span> المخزون</div>
      <div class="nav-item" onclick="showPage('crm')"><span class="nav-icon">👥</span> العملاء</div>
    </div>
    <div class="nav-section">
      <div class="nav-label">الإدارة</div>
      <div class="nav-item" onclick="showPage('dashboard')"><span class="nav-icon">📊</span> لوحة التحكم</div>
      <div class="nav-item" onclick="showPage('reports')"><span class="nav-icon">📈</span> التقارير</div>
      <div class="nav-item" onclick="showPage('branches')"><span class="nav-icon">🏪</span> الفروع</div>
      <div class="nav-item" onclick="showPage('users')"><span class="nav-icon">🔐</span> الموظفون</div>
      <div class="nav-item" onclick="showPage('backup')"><span class="nav-icon">💾</span> النسخ الاحتياطي</div>
    </div>
    <div class="nav-section" style="margin-top:auto">
      <div class="nav-item" onclick="showPage('activate')" style="color:#f59e0b"><span class="nav-icon">🔑</span> تفعيل النظام</div>
      <div class="nav-item" onclick="openSupport()" style="color:#22c55e"><span class="nav-icon">🛠️</span> الدعم الفني</div>
    </div>
    <div class="support-box">
      <div class="support-label">📞 خدمة العملاء</div>
      <div class="support-number">07772234981</div>
      <div class="support-hint">متاح 24/7</div>
    </div>
  </div>

  <div class="main-area">
    <div class="topbar">
      <div class="topbar-title" id="page-title">البيع السريع</div>
      <div class="topbar-actions">
        <span id="current-date" style="font-size:12px;color:#64748b"></span>
        <div id="license-badge" style="background:#fef3c7;color:#92400e;border-radius:6px;padding:3px 8px;font-size:11px;cursor:pointer" onclick="showPage('activate')">
          ⏳ مجاني — <span id="days-left-top">60 دقيقة</span>
        </div>
        <div style="display:flex;align-items:center;gap:5px;background:#eff6ff;border:1px solid #bfdbfe;border-radius:20px;padding:4px 10px">
          <span style="font-size:11px">📞</span>
          <span style="font-size:12px;color:#1d4ed8;font-weight:600;direction:ltr">07772234981</span>
        </div>
        <div class="user-chip"><div class="avatar">م</div><span style="font-size:12px">مدير</span></div>
      </div>
    </div>

    <div class="content">

      <!-- POS -->
      <div id="page-pos" class="pos-screen">
        <div class="products-panel">
          <div class="search-bar">
            <input type="text" id="pos-search" placeholder="🔍 بحث بالاسم أو أدخل الباركود..." oninput="filterProducts(this.value)" onkeydown="if(event.key==='Enter')scanInPOS(this.value)">
            <button class="btn btn-primary" onclick="openAddProduct()">+ إضافة منتج</button>
            <button class="btn" onclick="startBarcodeScanner('pos')" style="background:#1e293b;color:white;border-color:#1e293b">📷 باركود</button>
          </div>
          <div class="categories" id="cat-bar"><div class="cat-btn active" onclick="filterCat('الكل',this)">الكل</div></div>
          <div class="products-grid" id="products-grid">
            <div style="grid-column:1/-1"><div class="empty-big"><div style="font-size:52px;opacity:.25">📦</div><div style="font-size:14px;color:#64748b">لا توجد منتجات بعد</div><div style="font-size:12px;color:#94a3b8">اضغط "+ إضافة منتج" للبدء</div><button class="add-big-btn" onclick="openAddProduct()">+ إضافة أول منتج</button></div></div>
          </div>
        </div>
        <div class="cart-panel">
          <div class="cart-header"><span>فاتورة جديدة</span><div style="display:flex;gap:6px"><button class="btn" style="font-size:11px;padding:4px 8px" onclick="holdInvoice()">⏸ تعليق</button><button class="btn" style="font-size:11px;padding:4px 8px" onclick="clearCart()">✕ مسح</button></div></div>
          <div class="cart-items" id="cart-items"><div class="empty-cart">لا توجد منتجات<br><span style="font-size:11px">اضغط على منتج للإضافة</span></div></div>
          <div class="cart-footer">
            <div style="margin-bottom:10px">
              <div class="cart-row"><span>المجموع</span><span id="subtotal">0 د.ع</span></div>
              <div class="cart-row"><span>خصم</span><span id="discount" style="color:#22c55e">0 د.ع</span></div>
              <div class="cart-row total"><span>الإجمالي</span><span id="total">0 د.ع</span></div>
            </div>
            <div style="margin-bottom:8px"><input type="text" id="coupon-input" placeholder="كوبون خصم..." style="width:100%;padding:6px 10px;border:1px solid #e2e8f0;border-radius:7px;background:#f8fafc;font-size:12px;font-family:inherit;color:#1e293b" oninput="applyCoupon(this.value)"></div>
            <div class="pay-methods">
              <div class="pay-btn active" onclick="setPayMethod(this,'نقدي')">💵 نقدي</div>
              <div class="pay-btn" onclick="setPayMethod(this,'بطاقة')">💳 بطاقة</div>
              <div class="pay-btn" onclick="setPayMethod(this,'آجل')">📋 آجل</div>
            </div>
            <!-- قائمة العملاء — تظهر عند اختيار آجل فقط -->
            <div id="deferred-customer-wrap" style="display:none;margin-bottom:10px">
              <div style="font-size:11px;color:#64748b;margin-bottom:5px">اختر العميل *</div>
              <select id="deferred-customer" class="form-select" style="width:100%;padding:8px 12px;font-size:13px">
                <option value="">— اختر عميلاً —</option>
              </select>
              <div style="font-size:10px;color:#94a3b8;margin-top:4px">
                لا يوجد العميل؟ <span style="color:#3b82f6;cursor:pointer" onclick="openAddCustomer()">+ أضفه الآن</span>
              </div>
            </div>
            <button class="checkout-btn" onclick="checkout()">✔ إتمام البيع</button>
          </div>
        </div>
      </div>

      <!-- INVENTORY -->
      <div id="page-inventory" class="inventory-section" style="display:none">
        <div class="toolbar">
          <input type="text" placeholder="🔍 بحث بالاسم أو الباركود..." oninput="filterInventory(this.value)">
          <button class="btn btn-primary" onclick="openAddProduct()">+ إضافة منتج</button>
          <button class="btn" onclick="startBarcodeScanner('inventory-search')" style="background:#1e293b;color:white;border-color:#1e293b">📷 مسح باركود</button>
          <button class="btn" onclick="showNotif('تقرير الجرد جاهز')">📄 تقرير جرد</button>
        </div>
        <div class="card" style="padding:0;overflow:hidden">
          <table class="data-table">
            <thead><tr><th>الصنف</th><th>الباركود</th><th>الفئة</th><th>الوحدة</th><th>الكمية</th><th>حد الطلب</th><th>السعر (د.ع)</th><th>الحالة</th><th>الإجراء</th></tr></thead>
            <tbody id="inventory-table"><tr><td colspan="9" class="empty-td">لا توجد منتجات</td></tr></tbody>
          </table>
        </div>
      </div>

      <!-- CRM -->
      <div id="page-crm" class="crm-section" style="display:none">
        <div class="toolbar" style="margin-bottom:14px">
          <input type="text" placeholder="🔍 بحث بالاسم أو الهاتف...">
          <button class="btn btn-primary" onclick="openAddCustomer()">+ عميل جديد</button>
        </div>
        <div class="crm-grid" id="crm-grid"><div style="grid-column:1/-1" class="empty-big"><div style="font-size:52px;opacity:.25">👥</div><div style="font-size:14px;color:#64748b">لا يوجد عملاء بعد</div><button class="add-big-btn" onclick="openAddCustomer()" style="margin-top:8px">+ إضافة أول عميل</button></div></div>
      </div>

      <!-- DASHBOARD -->
      <div id="page-dashboard" class="dashboard" style="display:none">
        <div class="stats-grid">
          <div class="stat-card"><div class="stat-label">مبيعات اليوم</div><div class="stat-value" id="dash-sales">0</div><div class="stat-sub">د.ع</div></div>
          <div class="stat-card"><div class="stat-label">عدد الفواتير</div><div class="stat-value" id="dash-inv">0</div><div class="stat-sub">فاتورة</div></div>
          <div class="stat-card"><div class="stat-label">عدد المنتجات</div><div class="stat-value" id="dash-prods">0</div><div class="stat-sub">صنف</div></div>
          <div class="stat-card"><div class="stat-label">عدد العملاء</div><div class="stat-value" id="dash-custs">0</div><div class="stat-sub">عميل</div></div>
        </div>
        <div class="charts-row">
          <div class="card"><div class="card-title">حالة المخزون</div><div id="stock-summary"></div></div>
          <div class="card"><div class="card-title">أعلى المنتجات مبيعاً</div><div class="top-items" id="top-items"><div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد مبيعات بعد</div></div></div>
        </div>
      </div>

      <!-- REPORTS -->
      <div id="page-reports" class="reports-section" style="display:none">
        <div class="report-grid">
          <div class="card"><div class="card-title">توزيع طرق الدفع</div><div id="payment-chart" style="display:flex;flex-direction:column;gap:10px;margin-top:10px"><div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد مبيعات بعد</div></div></div>
          <div class="card"><div class="card-title">المنتجات الراكدة</div><div class="top-items" id="slow-items"><div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد بيانات</div></div></div>
          <div class="card" style="grid-column:1/-1"><div class="card-title">تقارير جاهزة</div><div style="display:flex;gap:8px;flex-wrap:wrap;margin-top:8px"><button class="btn" onclick="showNotif('تم إنشاء التقرير')">📄 تقرير المبيعات</button><button class="btn" onclick="showNotif('تم تصدير Excel')">📊 تقرير المخزون</button><button class="btn" onclick="showNotif('تم إنشاء تقرير الأرباح')">💰 الأرباح</button><button class="btn" onclick="exportBackup()">💾 تصدير JSON</button></div></div>
        </div>
      </div>

      <!-- BRANCHES -->
      <div id="page-branches" class="branches-section" style="display:none">
        <div id="branches-list-view">
          <div class="toolbar" style="margin-bottom:16px"><span style="font-size:13px;color:#64748b">إجمالي الفروع: <strong id="branch-count">0</strong></span><button class="btn btn-success" onclick="showNewBranchForm()" style="margin-right:auto">🏪 + فتح فرع جديد</button></div>
          <div class="branches-grid" id="branches-grid"><div class="branch-card new-branch" onclick="showNewBranchForm()"><div style="font-size:36px">➕</div><div style="font-size:14px;font-weight:500;color:#3b82f6">فتح فرع جديد</div></div></div>
        </div>
        <div id="new-branch-view" style="display:none">
          <div class="toolbar" style="margin-bottom:16px"><button class="btn" onclick="hideBranchForm()">← رجوع</button></div>
          <div class="steps-bar"><div class="step active" id="step1-label"><div class="step-num">1</div><span>المعلومات</span></div><div class="step-line"></div><div class="step" id="step2-label"><div class="step-num">2</div><span>التجهيزات</span></div><div class="step-line"></div><div class="step" id="step3-label"><div class="step-num">3</div><span>التأكيد</span></div></div>
          <div id="form-step-1" class="branch-form">
            <div style="font-size:15px;font-weight:500;margin-bottom:18px">🏪 معلومات الفرع</div>
            <div class="form-grid">
              <div class="form-group"><label class="form-label">اسم الفرع *</label><input class="form-input" id="f-name" placeholder="مثال: فرع المنصور"></div>
              <div class="form-group"><label class="form-label">المدينة *</label><select class="form-select" id="f-city"><option>بغداد</option><option>البصرة</option><option>الموصل</option><option>أربيل</option><option>كركوك</option><option>النجف</option><option>كربلاء</option></select></div>
              <div class="form-group"><label class="form-label">المنطقة</label><input class="form-input" id="f-area" placeholder="الحي / الشارع"></div>
              <div class="form-group"><label class="form-label">مدير الفرع</label><input class="form-input" id="f-manager" placeholder="الاسم الكامل"></div>
            </div>
            <div class="form-actions"><button class="btn" onclick="hideBranchForm()">إلغاء</button><button class="btn btn-primary" onclick="goStep(2)">التالي ←</button></div>
          </div>
          <div id="form-step-2" class="branch-form" style="display:none">
            <div style="font-size:15px;font-weight:500;margin-bottom:18px">👥 التجهيزات</div>
            <div class="form-grid">
              <div class="form-section-title">الأجهزة</div>
              <div class="form-group"><label class="form-label">عدد الكاشيرين</label><input class="form-input" id="f-cashiers" type="number" min="1" value="1"></div>
              <div class="form-group"><label class="form-label">عدد نقاط POS</label><input class="form-input" id="f-pos" type="number" min="1" value="1"></div>
              <div class="form-section-title">الخدمات</div>
              <div class="form-group full"><label class="check-item"><input type="checkbox" checked> نقاط البيع السريع</label><label class="check-item"><input type="checkbox" checked> إدارة المخزون</label><label class="check-item"><input type="checkbox" checked> المزامنة والنسخ الاحتياطي</label><label class="check-item"><input type="checkbox"> نظام الولاء</label></div>
            </div>
            <div class="form-actions"><button class="btn" onclick="goStep(1)">← السابق</button><button class="btn btn-primary" onclick="goStep(3)">التالي ←</button></div>
          </div>
          <div id="form-step-3" class="branch-form" style="display:none">
            <div style="font-size:15px;font-weight:500;margin-bottom:18px">✅ مراجعة وتأكيد</div>
            <div id="review-content" style="margin-bottom:16px"></div>
            <div class="form-actions"><button class="btn" onclick="goStep(2)">← السابق</button><button class="btn btn-success" onclick="saveBranch()">🏪 حفظ وفتح الفرع</button></div>
          </div>
        </div>
      </div>

      <!-- USERS -->
      <div id="page-users" class="users-section" style="display:none">
        <div class="toolbar" style="margin-bottom:16px">
          <span style="font-size:13px;color:#64748b">إدارة الموظفين</span>
          <button class="btn btn-primary" onclick="openAddUser()" style="margin-right:auto">+ إضافة موظف</button>
        </div>
        <div class="users-grid" id="users-grid"></div>
      </div>

      <!-- BACKUP -->
      <div id="page-backup" class="backup-section" style="display:none">
        <div class="backup-grid">
          <div class="backup-card">
            <div class="backup-icon">💾</div>
            <div class="backup-title">الحفظ التلقائي</div>
            <div class="backup-desc">بياناتك تُحفظ تلقائياً في المتصفح. تبقى محفوظة حتى بعد الإغلاق وإعادة الفتح على نفس الجهاز.</div>
            <div style="display:flex;align-items:center;gap:10px;padding:10px;background:#f0fdf4;border-radius:8px;border:1px solid #bbf7d0;margin-bottom:12px"><span style="font-size:18px">✅</span><div><div style="font-size:12px;font-weight:500;color:#166534">الحفظ التلقائي مفعّل</div><div style="font-size:11px;color:#16a34a" id="last-save-time">آخر حفظ: الآن</div></div></div>
            <button class="btn btn-primary" onclick="manualSave()">💾 حفظ الآن</button>
          </div>
          <div class="backup-card">
            <div class="backup-icon">📤</div>
            <div class="backup-title">تصدير نسخة احتياطية</div>
            <div class="backup-desc">صدّر بياناتك كملف JSON لنقلها بين الأجهزة أو حفظها كنسخة احتياطية.</div>
            <div style="display:flex;gap:8px;flex-wrap:wrap"><button class="btn btn-primary" onclick="exportBackup()">📥 تصدير الآن</button><button class="btn" onclick="exportBackup('weekly')">📅 أسبوعي</button></div>
          </div>
          <div class="backup-card">
            <div class="backup-icon">📥</div>
            <div class="backup-title">استيراد بيانات</div>
            <div class="backup-desc">استورد ملف JSON من نسخة احتياطية سابقة لاستعادة البيانات على جهاز آخر.</div>
            <input type="file" id="import-file" accept=".json" onchange="importBackup(this)" style="display:none">
            <button class="btn btn-success" onclick="document.getElementById('import-file').click()">📂 اختر ملف النسخة</button>
          </div>
          <div class="backup-card">
            <div class="backup-icon">📋</div>
            <div class="backup-title">سجل النسخ</div>
            <div class="backup-desc">آخر النسخ الاحتياطية المصدّرة.</div>
            <div class="backup-history" id="backup-history"><div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد نسخ بعد</div></div>
          </div>
        </div>
      </div>

      <!-- ACTIVATE -->
      <div id="page-activate" style="display:none;padding:16px">
        <div style="max-width:480px">
          <div class="card">
            <div style="text-align:center;margin-bottom:20px">
              <div style="font-size:48px;margin-bottom:10px">🔑</div>
              <div style="font-size:18px;font-weight:600;color:#1e293b;margin-bottom:6px">تفعيل النظام</div>
              <div style="font-size:13px;color:#64748b;line-height:1.7">أدخل كود التفعيل الذي حصلت عليه<br>للاستمرار في استخدام النظام بشكل دائم</div>
            </div>
            <div style="display:flex;flex-direction:column;gap:12px">
              <input id="act-code" class="form-input" placeholder="XXXX-XXXX-XXXX" maxlength="14" oninput="formatCode(this)" onkeydown="if(event.key==='Enter')activateCode()" style="text-align:center;font-size:18px;letter-spacing:3px;direction:ltr;padding:14px">
              <button class="btn btn-primary" style="padding:12px;font-size:14px" onclick="activateCode()">🔓 تفعيل النظام</button>
              <div id="act-error" style="background:#fee2e2;color:#dc2626;padding:8px 12px;border-radius:7px;font-size:12px;display:none;text-align:center">❌ كود غير صحيح</div>
              <div id="act-success" style="background:#dcfce7;color:#166534;padding:10px 12px;border-radius:7px;font-size:13px;display:none;text-align:center">✅ تم التفعيل بنجاح! النظام مفعّل بشكل دائم</div>
            </div>
            <div style="margin-top:20px;padding:14px;background:#f8fafc;border-radius:10px;border:1px solid #e2e8f0;text-align:center">
              <div style="font-size:12px;color:#64748b;margin-bottom:6px">للحصول على كود التفعيل:</div>
              <div style="font-size:20px;font-weight:700;color:#3b82f6;direction:ltr">📞 07772234981</div>
              <div style="font-size:11px;color:#94a3b8;margin-top:4px">متاح 24/7</div>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
</div>
</div>

<!-- MODAL: منتج -->
<div class="modal-overlay" id="modal-product" style="display:none">
  <div class="modal">
    <div class="modal-title" id="modal-product-title">➕ إضافة منتج</div>
    <div style="display:flex;flex-direction:column;gap:10px">
      <div class="form-group"><label class="form-label">اسم المنتج *</label><input class="form-input" id="p-name" placeholder="اسم المنتج"></div>
      <div class="form-group"><label class="form-label">الفئة *</label><div style="display:flex;gap:6px"><input class="form-input" id="p-cat" placeholder="اكتب أو اختر" style="flex:1"><select class="form-select" id="p-cat-select" onchange="if(this.value)document.getElementById('p-cat').value=this.value" style="width:120px"><option value="">— موجودة —</option></select></div></div>
      <!-- حقل الباركود -->
      <div class="form-group">
        <label class="form-label">الباركود</label>
        <div style="display:flex;gap:6px">
          <input class="form-input" id="p-barcode" placeholder="أدخل يدوياً أو امسح" style="flex:1;direction:ltr" type="text">
          <button class="btn btn-primary" onclick="startBarcodeScanner('p-barcode')" style="padding:8px 12px;white-space:nowrap">📷 مسح</button>
        </div>
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
        <div class="form-group"><label class="form-label">السعر (د.ع) *</label><input class="form-input" id="p-price" type="number" min="0" placeholder="0"></div>
        <div class="form-group"><label class="form-label">الكمية *</label><input class="form-input" id="p-stock" type="number" min="0" placeholder="0"></div>
        <div class="form-group"><label class="form-label">حد الطلب</label><input class="form-input" id="p-min" type="number" min="0" placeholder="0"></div>
        <div class="form-group"><label class="form-label">الوحدة</label><select class="form-select" id="p-unit"><option>قطعة</option><option>كيلو</option><option>لتر</option><option>كرتون</option><option>علبة</option><option>وجبة</option><option>حبة</option><option>كيس</option></select></div>
      </div>
      <div class="form-group"><label class="form-label">الأيقونة</label><div class="icon-grid" id="icon-grid"></div></div>
    </div>
    <div class="modal-actions"><button class="modal-btn" onclick="closeProductModal()">إلغاء</button><button class="modal-btn blue" onclick="saveProduct()">💾 حفظ</button></div>
  </div>
</div>

<!-- MODAL: ماسح الباركود بالكاميرا -->
<div class="modal-overlay" id="modal-scanner" style="display:none">
  <div class="modal" style="width:360px">
    <div class="modal-title">📷 مسح الباركود</div>
    <div style="margin-bottom:12px">
      <div id="scanner-video-wrap" style="width:100%;border-radius:10px;overflow:hidden;background:#000;position:relative;min-height:220px;display:flex;align-items:center;justify-content:center">
        <video id="scanner-video" style="width:100%;max-height:220px;display:block" autoplay playsinline muted></video>
        <div id="scanner-line" style="position:absolute;left:10%;right:10%;height:2px;background:#3b82f6;top:50%;box-shadow:0 0 8px #3b82f6;animation:scan-line 2s linear infinite"></div>
        <div id="scanner-msg" style="position:absolute;bottom:8px;left:0;right:0;text-align:center;color:white;font-size:12px;background:rgba(0,0,0,.5);padding:4px">وجّه الكاميرا نحو الباركود</div>
      </div>
    </div>
    <!-- إدخال يدوي كبديل -->
    <div style="margin-bottom:10px">
      <div style="font-size:12px;color:#64748b;margin-bottom:6px;text-align:center">أو أدخل الباركود يدوياً</div>
      <div style="display:flex;gap:6px">
        <input class="form-input" id="manual-barcode" placeholder="اكتب الباركود هنا..." style="flex:1;direction:ltr" onkeydown="if(event.key==='Enter')confirmManualBarcode()">
        <button class="btn btn-primary" onclick="confirmManualBarcode()">✓ تأكيد</button>
      </div>
    </div>
    <div class="modal-actions"><button class="modal-btn" onclick="closeScanner()">إغلاق</button></div>
  </div>
</div>

<!-- MODAL: عميل -->
<div class="modal-overlay" id="modal-customer" style="display:none">
  <div class="modal">
    <div class="modal-title">👤 إضافة عميل</div>
    <div style="display:flex;flex-direction:column;gap:10px">
      <div class="form-group"><label class="form-label">الاسم *</label><input class="form-input" id="c-name" placeholder="اسم العميل"></div>
      <div class="form-group"><label class="form-label">الهاتف *</label><input class="form-input" id="c-phone" placeholder="07X XXXX XXXX"></div>
      <div class="form-group"><label class="form-label">ملاحظات</label><input class="form-input" id="c-note" placeholder="أي معلومة إضافية..."></div>
    </div>
    <div class="modal-actions"><button class="modal-btn" onclick="document.getElementById('modal-customer').style.display='none'">إلغاء</button><button class="modal-btn blue" onclick="saveCustomer()">💾 حفظ</button></div>
  </div>
</div>

<!-- MODAL: موظف -->
<div class="modal-overlay" id="modal-user" style="display:none">
  <div class="modal">
    <div class="modal-title">👤 إضافة موظف</div>
    <div style="display:flex;flex-direction:column;gap:10px">
      <div class="form-group"><label class="form-label">الاسم *</label><input class="form-input" id="u-name" placeholder="اسم الموظف"></div>
      <div class="form-group"><label class="form-label">رقم الهاتف *</label><input class="form-input" id="u-phone" placeholder="07X XXXX XXXX" dir="ltr"></div>
      <div class="form-group"><label class="form-label">الصلاحية</label><select class="form-select" id="u-role"><option value="cashier">كاشير — بيع فقط</option><option value="admin">مدير — صلاحيات كاملة</option></select></div>
    </div>
    <div class="modal-actions"><button class="modal-btn" onclick="document.getElementById('modal-user').style.display='none'">إلغاء</button><button class="modal-btn blue" onclick="saveUser()">💾 حفظ</button></div>
  </div>
</div>

<!-- MODAL: تأكيد البيع -->
<div class="modal-overlay" id="modal-sale" style="display:none">
  <div class="modal">
    <div class="modal-title">✅ تأكيد البيع</div>
    <div id="modal-sale-content"></div>
    <div class="modal-actions"><button class="modal-btn" onclick="document.getElementById('modal-sale').style.display='none'">إلغاء</button><button class="modal-btn confirm" onclick="confirmSale()">✔ تأكيد الدفع</button></div>
  </div>
</div>

<!-- MODAL: الدعم الفني -->
<div class="modal-overlay" id="modal-support" style="display:none">
  <div class="modal" style="width:420px">
    <div class="modal-title">🛠️ الدعم الفني</div>
    <div style="background:#f0fdf4;border:1px solid #bbf7d0;border-radius:8px;padding:12px;margin-bottom:14px;font-size:12px;color:#166534;line-height:1.8">
      ✅ تم تجميع معلومات جهازك تلقائياً — انسخها وأرسلها لفريق الدعم عبر واتساب
    </div>
    <textarea id="support-text" style="width:100%;height:200px;padding:10px;border:1px solid #e2e8f0;border-radius:8px;font-size:11px;font-family:monospace;background:#f8fafc;color:#374151;resize:none;direction:ltr" readonly></textarea>
    <div class="modal-actions" style="margin-top:12px">
      <button class="modal-btn" onclick="document.getElementById('modal-support').style.display='none'">إغلاق</button>
      <button class="modal-btn blue" onclick="copySupport()" id="copy-support-btn">📋 نسخ المعلومات</button>
      <button class="modal-btn confirm" onclick="sendWhatsapp()" style="background:#25d366;border-color:#25d366">📱 إرسال واتساب</button>
    </div>
  </div>
</div>

<div class="notification" id="notif"></div>

<script>
// ============================================================
//  ✏️ إعدادات — عدّلها أنت
// ============================================================
const SUPPORT_NUMBER  = '07772234981';
const TRIAL_DAYS      = 30;
const TRIAL_MS        = 60 * 60 * 1000;
const APP_KEY         = 'supercash_trial_1h';

// ✏️ أكواد التفعيل — الصيغة: 'XXXX-XXXX-XXXX' : عدد الأيام (0 = دائم)
const ACTIVATION_CODES = {

  // ===== دائم =====
  'PERM-GOLD-AA11' : 0,
  'PERM-GOLD-BB22' : 0,
  'PERM-GOLD-CC33' : 0,
  'PERM-GOLD-DD44' : 0,
  'PERM-GOLD-EE55' : 0,

  // ===== يوم واحد =====
  'DAY1-PLUS-F1G2' : 1,
  'DAY1-PLUS-H3J4' : 1,
  'DAY1-PLUS-K5L6' : 1,
  'DAY1-PLUS-M7N8' : 1,
  'DAY1-PLUS-P9Q0' : 1,
  'DAY1-PLUS-R2S3' : 1,
  'DAY1-PLUS-T4U5' : 1,
  'DAY1-PLUS-V6W7' : 1,
  'DAY1-PLUS-X8Y9' : 1,
  'DAY1-PLUS-Z0A1' : 1,
  'HJ98-MDK6-1001' : 1,
  'HJ98-MDK6-1002' : 1,
  'HJ98-MDK6-1003' : 1,
  'HJ98-MDK6-1004' : 1,
  'HJ98-MDK6-1005' : 1,
  'HJ98-MDK6-1006' : 1,
  'HJ98-MDK6-1007' : 1,
  'HJ98-MDK6-1008' : 1,
  'HJ98-MDK6-1009' : 1,
  'HJ98-MDK6-1010' : 1,

  // ===== شهر واحد =====
  'MNTH-PLUS-B2C3' : 30,
  'MNTH-PLUS-D4E5' : 30,
  'MNTH-PLUS-F6G7' : 30,
  'MNTH-PLUS-H8J9' : 30,
  'MNTH-PLUS-K0L1' : 30,
  'MNTH-PLUS-M2N3' : 30,
  'MNTH-PLUS-P4Q5' : 30,
  'MNTH-PLUS-R6S7' : 30,
  'MNTH-PLUS-T8U9' : 30,
  'MNTH-PLUS-V0W1' : 30,
  'MNTH-PLUS-X2Y3' : 30,
  'MNTH-PLUS-Z4A5' : 30,
  'MNTH-PLUS-B6C7' : 30,
  'MNTH-PLUS-D8E9' : 30,
  'MNTH-PLUS-F0G1' : 30,
  'MNTH-PLUS-H2J3' : 30,
  'MNTH-PLUS-K4L5' : 30,
  'MNTH-PLUS-M6N7' : 30,
  'MNTH-PLUS-P8Q9' : 30,
  'MNTH-PLUS-R0S1' : 30,

  // ===== 6 أشهر =====
  'HALF-YEAR-T2U3' : 180,
  'HALF-YEAR-V4W5' : 180,
  'HALF-YEAR-X6Y7' : 180,
  'HALF-YEAR-Z8A9' : 180,
  'HALF-YEAR-B0C1' : 180,

  // ===== سنة كاملة =====
  'YEAR-FULL-D2E3' : 365,
  'YEAR-FULL-F4G5' : 365,
  'YEAR-FULL-H6J7' : 365,
  'YEAR-FULL-K8L9' : 365,
  'YEAR-FULL-M0N1' : 365,
  'YEAR-FULL-P2Q3' : 365,
  'YEAR-FULL-R4S5' : 365,
  'YEAR-FULL-T6U7' : 365,
  'YEAR-FULL-V8W9' : 365,
  'YEAR-FULL-X0Y1' : 365,

  // ===== Power 30 DAY (30 يوم) =====
  'HJ98-MOK6-2F4A' : 30,
  'HJ98-MDK6-7W85' : 30,
  'HJ98-MDK6-84T3' : 30,
  'HJ98-MDK6-9U92' : 30,
  'HJ98-MDK6-3P93' : 30,
  'RTUB-OZAL-7OJ6' : 30,
  'RTUB-ANKI-8VXM' : 30,
  'RTUB-AQXO-9LSA' : 30,
  'HWIE-MQ40-8854' : 30,
  '8HW3-48N2-E4K6' : 30,
  'UQMT-4O1P-Y73E' : 30,
  '8MWX-IELA-8BN3' : 30,
  '8T4O-MV5Z-6S9M' : 30,
  'M8Q2-FWAJ-UDS6' : 30,
  'WU3Z-UN33-OM7M' : 30,
  'DEK8-J8QJ-HWN6' : 30,
  'QCP7-BR9E-WJCB' : 30,
  'WAX4-GQMO-4H75' : 30,
  'NKS0-FCHB-TALR' : 30,
  'GXYN-U7KZ-8TR5' : 30,
  'GQC9-CNM9-CACN' : 30,
  'T2VO-IMQP-WMLY' : 30,
  'FCPK-65D9-8KVA' : 30,
  'WQ9I-PZ4V-HAQX' : 30,
  'XMJD-RBQ7-Y3BK' : 30,
  'QKDS-O7CS-PQX8' : 30,
  'MA6B-FGJD-7B3A' : 30,
  'UQ3X-NYTS-BPOM' : 30,
  'B4NM-HEU3-JEQL' : 30,
  'T6WH-WI8P-QYNE' : 30,
  'WOM2-I1UW-BUAQ' : 30,
  'KDOG-WXOL-WNJC' : 30,

  // ===== Power 360 DAY (360 يوم) =====
  'HRKF-NFIS-5M39' : 360,
  'NURM-NRUF-84UT' : 360,
  'NRJ4-NFYS-VOW4' : 360,
  'QVUM-XWCY-754G' : 360,
  'UVGB-NU7M-VNUN' : 360,
  'UVBN-8NKM-5DCB' : 360,
  'FYJK-6SXC-TRAX' : 360,
  'UIEM-WM2Q-LP93' : 360,
  '73JW-MOWL-ETYQ' : 360,
  'FSPW-4ND9-BWY8' : 360,
  'GD82-2NSK-NWKQ' : 360,
  'VDBU-WDUW-TDN8' : 360,
};

const ICONS   = ['📦','🛒','🥤','💧','🍞','🌾','🍟','🧃','🥛','🍫','🧁','🍕','🍗','🥩','🥦','🍎','🍊','🧼','🧹','💊','📱','🎧','👕','👟','🪑','🔧','⚡','🎮','💄','🧴','🏠','📚','🎁','🌟','🍰'];
const COUPONS = {'SALE10':5000,'VIP20':10000,'DISC5':2500};
const COLORS  = ['#3b82f6','#8b5cf6','#f59e0b','#ec4899','#10b981','#ef4444','#06b6d4','#84cc16'];

// ============================================================
//  STATE
// ============================================================
let state = {
  products:[], customers:[], branches:[], staff:[],
  totalSales:0, totalInvoices:0,
  payStats:{'نقدي':0,'بطاقة':0,'آجل':0},
  salesByProduct:{}, backupHistory:[],
  usedCodes: [],
  license: { status:'trial', startDate: null, endDate: null, code: null, days: null }
};

let cart=[], payMethod='نقدي', discountAmt=0, currentCat='الكل', currentSearch='';
let editingProductId=null, selectedIcon='📦';

// ============================================================
//  STORAGE
// ============================================================
function saveState() {
  try {
    localStorage.setItem(APP_KEY, JSON.stringify(state));
    const t = new Date().toLocaleTimeString('ar-IQ');
    const el = document.getElementById('last-save-time');
    if(el) el.textContent = 'آخر حفظ: ' + t;
  } catch(e){}
}

function loadState() {
  try {
    const raw = localStorage.getItem(APP_KEY);
    if(raw) {
      const saved = JSON.parse(raw);
      Object.keys(state).forEach(k => { if(saved[k] !== undefined) state[k] = saved[k]; });
    }
  } catch(e){}
}

function manualSave() { saveState(); showNotif('✅ تم الحفظ بنجاح'); }
setInterval(() => saveState(), 60000);

// ============================================================
//  LICENSE / TRIAL
// ============================================================
function initLicense() {
  if (!state.license.startDate) {
    state.license.startDate = Date.now();
    state.license.status = 'trial';
    saveState();
  }

  const now = Date.now();
  const lic = state.license;

  // ===== مفعّل =====
  if (lic.status === 'active') {
    if (!lic.endDate) {
      // دائم — لا ينتهي أبداً
      showApp('active', 0, null);
      return;
    }
    // مؤقت — تحقق من تاريخ الانتهاء
    // تأكد أن endDate رقم وليس string
    const endDate = Number(lic.endDate);
    if (now >= endDate) {
      // انتهت صلاحية الكود — اعرض شاشة الانتهاء
      state.license.status = 'expired';
      saveState();
      showExpired();
    } else {
      showApp('active', lic.days || 0, endDate);
    }
    return;
  }

  // ===== منتهي الصلاحية (كود منتهي) =====
  if (lic.status === 'expired') {
    showExpired();
    return;
  }

  // ===== تجريبي =====
  const elapsed   = now - Number(lic.startDate);
  const remaining = TRIAL_MS - elapsed;
  if (remaining <= 0) {
    showExpired();
  } else {
    const minsLeft = Math.ceil(remaining / 60000);
    showApp('trial', minsLeft);
    setInterval(() => {
      const rem = TRIAL_MS - (Date.now() - Number(state.license.startDate));
      if (rem <= 0) { showExpired(); return; }
      const mins  = Math.ceil(rem / 60000);
      const label = mins >= 60 ? Math.ceil(mins/60)+' ساعة' : mins+' دقيقة';
      const el1   = document.getElementById('days-left');
      const el2   = document.getElementById('days-left-top');
      if(el1) el1.textContent = label;
      if(el2) el2.textContent = label;
    }, 30000);
  }
}

function showApp(status, daysOrTime, endDate) {
  document.getElementById('expired-screen').style.display = 'none';
  document.getElementById('app').style.display = 'block';

  const banner = document.getElementById('trial-banner');
  const badge  = document.getElementById('license-badge');
  const sbSub  = document.getElementById('sb-sub');

  if (status === 'active') {
    const days = daysOrTime !== undefined ? daysOrTime : (state.license.days || 0);
    const end  = endDate || state.license.endDate;

    if (days === 0 || !end) {
      // دائم
      banner.classList.add('hidden');
      badge.style.background = '#dcfce7';
      badge.style.color = '#166534';
      badge.innerHTML = '✅ مفعّل بشكل دائم';
      badge.onclick = null;
      sbSub.textContent = 'النسخة الكاملة — دائم';
    } else {
      // مؤقت — احسب الأيام المتبقية
      const now = Date.now();
      const remainMs = end - now;
      if (remainMs <= 0) { showExpired(); return; }
      const remainDays  = Math.ceil(remainMs / 86400000);
      const remainHours = Math.ceil(remainMs / 3600000);
      const label = remainDays >= 2  ? remainDays + ' يوم' :
                    remainHours >= 1 ? remainHours + ' ساعة' :
                    Math.ceil(remainMs / 60000) + ' دقيقة';

      banner.classList.remove('hidden');
      if (remainDays <= 5) banner.classList.add('danger');
      banner.querySelector('span').innerHTML =
        '✅ مفعّل — متبقي <strong id="days-left">' + label + '</strong>';
      badge.style.background = '#dcfce7';
      badge.style.color = '#166534';
      badge.innerHTML = '✅ مفعّل — ' + label;
      badge.onclick = () => showPage('activate');
      sbSub.textContent = 'مفعّل — ' + label;
      document.getElementById('days-left-top').textContent = label;

      // تحقق يومي من الانتهاء
      setInterval(() => {
        if (Date.now() >= end) showExpired();
      }, 3600000);
    }
  } else {
    // تجريبي
    banner.classList.remove('hidden');
    const minsLeft = daysOrTime || 60;
    const label = minsLeft >= 60 ? Math.ceil(minsLeft/60)+' ساعة' : minsLeft+' دقيقة';
    if (minsLeft <= 10) banner.classList.add('danger');
    banner.querySelector('span').innerHTML =
      '⏳ نسخة مجانية — متبقي <strong id="days-left">'+label+'</strong>';
    badge.style.background = '#fef3c7';
    badge.style.color = '#92400e';
    badge.innerHTML = '⏳ مجاني — <span id="days-left-top">'+label+'</span>';
    badge.onclick = () => showPage('activate');
    sbSub.textContent = 'مجاني — ساعة واحدة';
  }
}

function showExpired() {
  document.getElementById('app').style.display = 'none';
  document.getElementById('trial-banner').classList.add('hidden');
  const es = document.getElementById('expired-screen');
  es.style.display = 'flex';
}

function formatCode(input) {
  // أزل كل شيء غير حرف أو رقم
  let v = input.value.replace(/[^A-Za-z0-9]/g,'').toUpperCase();
  // أضف الشرطات تلقائياً
  if (v.length > 4)  v = v.slice(0,4) + '-' + v.slice(4);
  if (v.length > 9)  v = v.slice(0,9) + '-' + v.slice(9);
  if (v.length > 14) v = v.slice(0,14);
  input.value = v;
}

function activateCode() {
  const code1 = (document.getElementById('activation-code')?.value || '').trim().toUpperCase();
  const code2 = (document.getElementById('act-code')?.value || '').trim().toUpperCase();
  const code  = code1 || code2;

  const errEl1 = document.getElementById('activation-error');
  const errEl2 = document.getElementById('act-error');
  const sucEl  = document.getElementById('act-success');

  if (!code) { showErr(errEl1, errEl2, '⚠️ يرجى إدخال كود التفعيل'); return; }

  // ✅ تحقق إذا الكود استُخدم مسبقاً
  if (!state.usedCodes) state.usedCodes = [];
  if (state.usedCodes.includes(code)) {
    showErr(errEl1, errEl2, '⛔ هذا الكود تم استخدامه مسبقاً — تواصل معنا للحصول على كود جديد: ' + SUPPORT_NUMBER);
    return;
  }

  if (ACTIVATION_CODES.hasOwnProperty(code)) {
    const days    = ACTIVATION_CODES[code];
    const endDate = days > 0 ? Date.now() + days * 86400000 : null;

    // ✅ سجّل الكود كمستخدم
    state.usedCodes.push(code);

    state.license.status  = 'active';
    state.license.code    = code;
    state.license.endDate = endDate;
    state.license.days    = days;
    saveState();

    if(errEl1) errEl1.style.display = 'none';
    if(errEl2) errEl2.style.display = 'none';

    const durationText = days === 0   ? 'دائم' :
                         days === 1   ? 'يوم واحد' :
                         days === 30  ? 'شهر واحد' :
                         days === 180 ? '6 أشهر' :
                         days === 365 ? 'سنة كاملة' :
                         days + ' يوم';

    if(sucEl){
      sucEl.textContent = '✅ تم التفعيل! الصلاحية: ' + durationText;
      sucEl.style.display = 'block';
    }

    setTimeout(() => {
      showApp('active', days, endDate);
      showNotif('🎉 تم التفعيل — الصلاحية: ' + durationText);
    }, 1200);

  } else {
    showErr(errEl1, errEl2, '❌ كود غير صحيح — تواصل معنا: ' + SUPPORT_NUMBER);
  }
}

function showErr(el1, el2, msg) {
  if(el1){ el1.textContent=msg; el1.style.display='block'; setTimeout(()=>el1.style.display='none',4000); }
  if(el2){ el2.textContent=msg; el2.style.display='block'; setTimeout(()=>el2.style.display='none',4000); }
}

// ============================================================
//  NAV
// ============================================================
const PAGES=['pos','dashboard','inventory','crm','reports','branches','users','backup','activate'];
const TITLES={pos:'البيع السريع',dashboard:'لوحة التحكم',inventory:'إدارة المخزون',crm:'العملاء والولاء',reports:'التقارير',branches:'إدارة الفروع',users:'الموظفون',backup:'النسخ الاحتياطي',activate:'تفعيل النظام'};

function showPage(p) {
  PAGES.forEach(pg => document.getElementById('page-'+pg).style.display = 'none');
  document.querySelectorAll('.nav-item').forEach((n,i) => n.classList.toggle('active', i === PAGES.indexOf(p)));
  document.getElementById('page-'+p).style.display = p==='pos' ? 'flex' : 'block';
  document.getElementById('page-title').textContent = TITLES[p];
  if(p==='dashboard') updateDashboard();
  if(p==='reports')   updateReports();
  if(p==='backup')    renderBackupHistory();
}

// ============================================================
//  PRODUCTS
// ============================================================
function openAddProduct(id=null) {
  editingProductId=id; selectedIcon='📦';
  document.getElementById('modal-product-title').textContent = id ? '✏️ تعديل المنتج' : '➕ إضافة منتج';
  document.getElementById('icon-grid').innerHTML = ICONS.map(ic=>`<div class="icon-opt${ic===selectedIcon?' selected':''}" onclick="selectIcon('${ic}',this)">${ic}</div>`).join('');
  const cats=[...new Set(state.products.map(p=>p.cat))].filter(Boolean);
  document.getElementById('p-cat-select').innerHTML='<option value="">— موجودة —</option>'+cats.map(c=>`<option>${c}</option>`).join('');
  if(id){
    const p=state.products.find(x=>x.id===id);
    document.getElementById('p-name').value=p.name;
    document.getElementById('p-cat').value=p.cat;
    document.getElementById('p-price').value=p.price;
    document.getElementById('p-stock').value=p.stock;
    document.getElementById('p-min').value=p.min||0;
    document.getElementById('p-unit').value=p.unit;
    document.getElementById('p-barcode').value=p.barcode||'';
    selectedIcon=p.icon;
    document.querySelectorAll('.icon-opt').forEach(el=>el.classList.toggle('selected',el.textContent===selectedIcon));
  } else {
    ['p-name','p-cat','p-price','p-stock','p-min','p-barcode'].forEach(id=>document.getElementById(id).value='');
    document.getElementById('p-unit').value='قطعة';
  }
  document.getElementById('modal-product').style.display='flex';
}
function selectIcon(ic,el){selectedIcon=ic;document.querySelectorAll('.icon-opt').forEach(e=>e.classList.remove('selected'));el.classList.add('selected');}
function saveProduct(){
  const name=document.getElementById('p-name').value.trim(),cat=document.getElementById('p-cat').value.trim();
  const price=parseFloat(document.getElementById('p-price').value)||0,stock=parseInt(document.getElementById('p-stock').value)||0;
  const min=parseInt(document.getElementById('p-min').value)||0,unit=document.getElementById('p-unit').value;
  const barcode=document.getElementById('p-barcode').value.trim();
  if(!name||!cat||price<=0){showNotif('⚠️ يرجى تعبئة الاسم والفئة والسعر');return;}
  // تحقق من تكرار الباركود
  if(barcode){
    const dup=state.products.find(p=>p.barcode===barcode&&p.id!==editingProductId);
    if(dup){showNotif('⚠️ الباركود مستخدم مسبقاً في: '+dup.name);return;}
  }
  if(editingProductId!==null){
    const idx=state.products.findIndex(p=>p.id===editingProductId);
    state.products[idx]={...state.products[idx],name,cat,price,stock,min,unit,icon:selectedIcon,barcode};
    showNotif('✅ تم تعديل المنتج');
  } else {
    state.products.push({id:Date.now(),name,cat,price,stock,min,unit,icon:selectedIcon,barcode});
    showNotif('✅ تمت الإضافة: '+name);
  }
  closeProductModal();renderProducts();renderInventory();updateCatBar();saveState();
}
function closeProductModal(){document.getElementById('modal-product').style.display='none';editingProductId=null;}
function deleteProduct(id){if(!confirm('هل تريد حذف هذا المنتج؟'))return;state.products=state.products.filter(p=>p.id!==id);cart=cart.filter(c=>c.id!==id);renderProducts();renderInventory();renderCart();updateCatBar();saveState();showNotif('🗑 تم حذف المنتج');}
function updateCatBar(){const cats=['الكل',...new Set(state.products.map(p=>p.cat))];document.getElementById('cat-bar').innerHTML=cats.map(c=>`<div class="cat-btn${c===currentCat?' active':''}" onclick="filterCat('${c}',this)">${c}</div>`).join('');}
function renderProducts(){
  const grid=document.getElementById('products-grid');
  const f=state.products.filter(p=>(currentCat==='الكل'||p.cat===currentCat)&&(!currentSearch||p.name.includes(currentSearch)));
  if(!f.length){grid.innerHTML=`<div style="grid-column:1/-1"><div class="empty-big"><div style="font-size:52px;opacity:.25">${state.products.length?'🔍':'📦'}</div><div style="font-size:14px;color:#64748b">${state.products.length?'لا توجد نتائج':'لا توجد منتجات بعد'}</div>${!state.products.length?'<button class="add-big-btn" onclick="openAddProduct()">+ إضافة أول منتج</button>':''}</div></div>`;return;}
  grid.innerHTML=f.map(p=>`<div class="product-card" onclick="addToCart(${p.id})"><div class="product-icon">${p.icon}</div><div class="product-name">${p.name}</div><div class="product-price">${p.price.toLocaleString('ar-IQ')} د.ع</div><div class="product-stock">${p.stock<=0?'⛔ نافد':p.stock<(p.min||10)?'⚠️ '+p.stock+' فقط':'✓ '+p.stock}</div></div>`).join('');
}
function filterCat(cat,el){currentCat=cat;document.querySelectorAll('.cat-btn').forEach(b=>b.classList.remove('active'));el.classList.add('active');renderProducts();}
function filterProducts(v){currentSearch=v;renderProducts();}

function renderInventory(){
  const tbody=document.getElementById('inventory-table');
  if(!state.products.length){tbody.innerHTML='<tr><td colspan="9" class="empty-td">لا توجد منتجات</td></tr>';return;}
  tbody.innerHTML=state.products.map(p=>{
    const pct=p.min?Math.min(100,Math.round(p.stock/(p.min*2)*100)):(p.stock>0?60:0);
    const sc=p.stock===0?'stock-out':(p.min&&p.stock<p.min)?'stock-low':'stock-ok';
    const st=p.stock===0?'نافد':(p.min&&p.stock<p.min)?'منخفض':'جيد';
    const bc=p.stock===0?'#ef4444':(p.min&&p.stock<p.min)?'#f59e0b':'#22c55e';
    const barcodeCell=p.barcode
      ?`<span style="background:#f1f5f9;padding:2px 8px;border-radius:6px;font-size:11px;direction:ltr;display:inline-block">${p.barcode}</span>`
      :`<span style="color:#94a3b8;font-size:11px">—</span>`;
    return `<tr>
      <td style="font-weight:500">${p.name}</td>
      <td>${barcodeCell}</td>
      <td><span style="background:#f1f5f9;padding:2px 8px;border-radius:6px;font-size:11px">${p.cat}</span></td>
      <td>${p.unit}</td>
      <td><div style="display:flex;align-items:center;gap:6px"><span style="font-weight:500">${p.stock}</span><div class="pb-wrap"><div class="pb-fill" style="width:${pct}%;background:${bc}"></div></div></div></td>
      <td style="color:#64748b">${p.min||'—'}</td>
      <td>${p.price.toLocaleString('ar-IQ')}</td>
      <td><span class="stock-badge ${sc}">${st}</span></td>
      <td style="display:flex;gap:4px">
        <button class="btn" style="font-size:11px;padding:3px 8px" onclick="openAddProduct(${p.id})">✏️</button>
        <button class="btn btn-danger" style="font-size:11px;padding:3px 8px" onclick="deleteProduct(${p.id})">🗑</button>
      </td>
    </tr>`;
  }).join('');
}

// ============================================================
//  BARCODE SCANNER
// ============================================================
let scannerStream=null, scannerTarget=null, barcodeInterval=null;

function startBarcodeScanner(target){
  scannerTarget=target;
  document.getElementById('modal-scanner').style.display='flex';
  document.getElementById('manual-barcode').value='';
  if(navigator.mediaDevices&&navigator.mediaDevices.getUserMedia){
    navigator.mediaDevices.getUserMedia({video:{facingMode:'environment'}})
      .then(stream=>{
        scannerStream=stream;
        const video=document.getElementById('scanner-video');
        video.srcObject=stream; video.play();
        document.getElementById('scanner-msg').textContent='وجّه الكاميرا نحو الباركود';
        if('BarcodeDetector' in window){
          const detector=new BarcodeDetector({formats:['ean_13','ean_8','code_128','code_39','qr_code','upc_a','upc_e']});
          barcodeInterval=setInterval(async()=>{
            try{const codes=await detector.detect(video);if(codes.length>0){clearInterval(barcodeInterval);onBarcodeDetected(codes[0].rawValue);}}catch(e){}
          },500);
        } else {
          document.getElementById('scanner-msg').textContent='الكاميرا تعمل — أدخل الباركود يدوياً أدناه';
        }
      })
      .catch(()=>{ document.getElementById('scanner-msg').textContent='⚠️ لا يمكن الوصول للكاميرا — أدخل يدوياً'; });
  } else {
    document.getElementById('scanner-msg').textContent='الكاميرا غير مدعومة — أدخل يدوياً';
  }
  setTimeout(()=>document.getElementById('manual-barcode').focus(),300);
}

function onBarcodeDetected(code){
  closeScanner();
  if(scannerTarget==='pos') scanInPOS(code);
  else if(scannerTarget==='inventory-search'){ filterInventory(code); showNotif('🔍 باركود: '+code); }
  else { const el=document.getElementById(scannerTarget); if(el){el.value=code;showNotif('✅ تم مسح الباركود: '+code);} }
}

function scanInPOS(code){
  if(!code||!code.trim())return;
  const trimmed=code.trim();
  let product=state.products.find(p=>p.barcode===trimmed);
  if(!product) product=state.products.find(p=>p.name.includes(trimmed));
  if(product){ addToCart(product.id); const si=document.getElementById('pos-search'); if(si)si.value=''; }
  else showNotif('⚠️ لا يوجد منتج بهذا الباركود: '+trimmed);
}

function confirmManualBarcode(){
  const code=document.getElementById('manual-barcode').value.trim();
  if(!code){showNotif('⚠️ يرجى إدخال الباركود');return;}
  onBarcodeDetected(code);
}

function closeScanner(){
  document.getElementById('modal-scanner').style.display='none';
  if(barcodeInterval){clearInterval(barcodeInterval);barcodeInterval=null;}
  if(scannerStream){scannerStream.getTracks().forEach(t=>t.stop());scannerStream=null;}
  const video=document.getElementById('scanner-video');
  if(video)video.srcObject=null;
}

function filterInventory(v){
  document.querySelectorAll('#inventory-table tr').forEach(r=>{
    if(!r.cells[0])return;
    const name=r.cells[0].textContent, barcode=r.cells[1]?r.cells[1].textContent:'';
    r.style.display=(name.includes(v)||barcode.includes(v))?'':'none';
  });
}

// ============================================================
//  CART
// ============================================================
const IQD=n=>Number(n).toLocaleString('ar-IQ')+' د.ع';
function addToCart(id){const p=state.products.find(x=>x.id===id);if(!p||p.stock<=0){showNotif('⛔ هذا المنتج نافد');return;}const ex=cart.find(c=>c.id===id);if(ex)ex.qty++;else cart.push({...p,qty:1});renderCart();}
function changeQty(id,d){const idx=cart.findIndex(c=>c.id===id);if(idx===-1)return;cart[idx].qty+=d;if(cart[idx].qty<=0)cart.splice(idx,1);renderCart();}
function renderCart(){
  const el=document.getElementById('cart-items');
  if(!cart.length){el.innerHTML='<div class="empty-cart">لا توجد منتجات<br><span style="font-size:11px">اضغط على منتج للإضافة</span></div>';['subtotal','discount','total'].forEach(id=>document.getElementById(id).textContent='0 د.ع');return;}
  el.innerHTML=cart.map(c=>`<div class="cart-item"><span style="font-size:16px">${c.icon}</span><span class="cart-item-name">${c.name}</span><div class="cart-qty"><button class="qty-btn" onclick="changeQty(${c.id},-1)">-</button><span class="qty-num">${c.qty}</span><button class="qty-btn" onclick="changeQty(${c.id},1)">+</button></div><span class="cart-item-price">${(c.price*c.qty).toLocaleString('ar-IQ')} د.ع</span></div>`).join('');
  const sub=cart.reduce((s,c)=>s+c.price*c.qty,0),total=Math.max(0,sub-discountAmt);
  document.getElementById('subtotal').textContent=IQD(sub);document.getElementById('discount').textContent='-'+IQD(discountAmt);document.getElementById('total').textContent=IQD(total);
}
function clearCart(){cart=[];discountAmt=0;document.getElementById('coupon-input').value='';renderCart();}
function holdInvoice(){showNotif('✅ تم تعليق الفاتورة');clearCart();}
function applyCoupon(v){const k=v.toUpperCase();if(COUPONS[k]){discountAmt=COUPONS[k];showNotif('✅ خصم '+IQD(discountAmt));}else discountAmt=0;renderCart();}
let selectedDeferredCustomerId = null;

function setPayMethod(el,m){
  payMethod=m;
  document.querySelectorAll('.pay-btn').forEach(b=>b.classList.remove('active'));
  el.classList.add('active');
  const wrap=document.getElementById('deferred-customer-wrap');
  if(m==='آجل'){
    const sel=document.getElementById('deferred-customer');
    sel.innerHTML='<option value="">— اختر عميلاً —</option>'+
      state.customers.map(c=>`<option value="${c.id}">${c.name} — ${c.phone}</option>`).join('');
    wrap.style.display='block';
    selectedDeferredCustomerId=null;
  } else {
    wrap.style.display='none';
    document.getElementById('deferred-customer').value='';
    selectedDeferredCustomerId=null;
  }
}
function checkout(){
  if(!cart.length){showNotif('⚠️ لا توجد منتجات');return;}
  if(payMethod==='آجل'){
    const custId=document.getElementById('deferred-customer').value;
    if(!custId){showNotif('⚠️ يرجى اختيار عميل للبيع الآجل');document.getElementById('deferred-customer').focus();return;}
    selectedDeferredCustomerId=custId; // ✅ احفظه قبل فتح الـ modal
  } else {
    selectedDeferredCustomerId=null;
  }
  const sub=cart.reduce((s,c)=>s+c.price*c.qty,0),total=Math.max(0,sub-discountAmt);
  const custName=selectedDeferredCustomerId?state.customers.find(c=>String(c.id)===String(selectedDeferredCustomerId))?.name:'';
  const custRow=payMethod==='آجل'&&custName
    ?`<div class="modal-row"><span>العميل</span><span style="font-weight:500;color:#3b82f6">${custName}</span></div>`:'';
  document.getElementById('modal-sale-content').innerHTML=
    `${custRow}
    <div class="modal-row"><span>عدد الأصناف</span><span>${cart.length}</span></div>
    <div class="modal-row"><span>طريقة الدفع</span><span>${payMethod}</span></div>
    <div class="modal-row"><span>المجموع</span><span>${IQD(sub)}</span></div>
    <div class="modal-row"><span>الخصم</span><span style="color:#22c55e">- ${IQD(discountAmt)}</span></div>
    <div class="modal-row" style="font-weight:600;font-size:15px"><span>الإجمالي</span><span>${IQD(total)}</span></div>`;
  document.getElementById('modal-sale').style.display='flex';
}
function confirmSale(){
  const sub=cart.reduce((s,c)=>s+c.price*c.qty,0),total=Math.max(0,sub-discountAmt);
  state.totalSales+=total; state.totalInvoices++;
  state.payStats[payMethod]=(state.payStats[payMethod]||0)+total;

  // ✅ استخدم المتغير المحفوظ مسبقاً وليس الـ DOM
  if(payMethod==='آجل' && selectedDeferredCustomerId){
    const cust=state.customers.find(c=>String(c.id)===String(selectedDeferredCustomerId));
    if(cust){
      cust.total=(cust.total||0)+total;
      cust.visits=(cust.visits||0)+1;
      cust.points=Math.floor((cust.total||0)/10000);
      showNotif('✅ تم البيع الآجل — سُجّل في حساب: '+cust.name);
    }
  } else {
    showNotif('✅ تم إتمام البيع بنجاح');
  }

  cart.forEach(c=>{
    const p=state.products.find(x=>x.id===c.id);
    if(p) p.stock=Math.max(0,p.stock-c.qty);
    state.salesByProduct[c.id]=(state.salesByProduct[c.id]||0)+c.qty;
  });

  document.getElementById('modal-sale').style.display='none';
  // إعادة ضبط الآجل
  selectedDeferredCustomerId=null;
  document.getElementById('deferred-customer').value='';
  document.getElementById('deferred-customer-wrap').style.display='none';
  document.querySelectorAll('.pay-btn').forEach(b=>b.classList.remove('active'));
  document.querySelector('.pay-btn').classList.add('active');
  payMethod='نقدي';
  clearCart(); renderInventory(); renderProducts(); renderCRM(); saveState();
}

// ============================================================
//  CUSTOMERS
// ============================================================
function openAddCustomer(){['c-name','c-phone','c-note'].forEach(id=>document.getElementById(id).value='');document.getElementById('modal-customer').style.display='flex';}
function saveCustomer(){const name=document.getElementById('c-name').value.trim(),phone=document.getElementById('c-phone').value.trim();if(!name||!phone){showNotif('⚠️ يرجى تعبئة الاسم والهاتف');return;}state.customers.push({id:Date.now(),name,phone,note:document.getElementById('c-note').value,visits:0,total:0,points:0,color:COLORS[state.customers.length%COLORS.length]});document.getElementById('modal-customer').style.display='none';renderCRM();saveState();showNotif('✅ تم إضافة العميل: '+name);}
function renderCRM(){const grid=document.getElementById('crm-grid');if(!state.customers.length){grid.innerHTML='<div style="grid-column:1/-1" class="empty-big"><div style="font-size:52px;opacity:.25">👥</div><div style="font-size:14px;color:#64748b">لا يوجد عملاء بعد</div><button class="add-big-btn" onclick="openAddCustomer()" style="margin-top:8px">+ إضافة أول عميل</button></div>';return;}grid.innerHTML=state.customers.map(c=>{const loy=Math.min(100,c.points||0);return `<div class="customer-card"><div style="display:flex;align-items:center;gap:10px;margin-bottom:10px"><div style="width:36px;height:36px;border-radius:50%;background:${c.color};display:flex;align-items:center;justify-content:center;font-size:13px;font-weight:600;color:white;flex-shrink:0">${c.name.substring(0,2)}</div><div><div style="font-size:13px;font-weight:500;color:#1e293b">${c.name}</div><div style="font-size:11px;color:#64748b">${c.phone}</div></div></div><div style="display:grid;grid-template-columns:1fr 1fr;gap:8px"><div class="cstat"><div class="cstat-label">إجمالي الشراء</div><div class="cstat-val">${(c.total||0).toLocaleString('ar-IQ')} <span style="font-size:10px;color:#64748b">د.ع</span></div></div><div class="cstat"><div class="cstat-label">الزيارات</div><div class="cstat-val">${c.visits||0}</div></div></div><div class="loyalty-bar" style="margin-top:8px"><div class="loyalty-fill" style="width:${loy}%"></div></div><div class="loyalty-label"><span>نقاط: ${c.points||0}</span><span>${loy}%</span></div></div>`;}).join('');}

// ============================================================
//  USERS
// ============================================================
function openAddUser(){['u-name','u-phone'].forEach(id=>document.getElementById(id).value='');document.getElementById('modal-user').style.display='flex';}
function saveUser(){const name=document.getElementById('u-name').value.trim(),phone=document.getElementById('u-phone').value.trim(),role=document.getElementById('u-role').value;if(!name||!phone){showNotif('⚠️ يرجى تعبئة الاسم والهاتف');return;}state.staff.push({id:Date.now(),name,phone,role,color:COLORS[state.staff.length%COLORS.length],sales:0,invoices:0});document.getElementById('modal-user').style.display='none';renderUsersPage();saveState();showNotif('✅ تمت إضافة الموظف: '+name);}
function deleteStaff(id){if(!confirm('هل تريد حذف هذا الموظف؟'))return;state.staff=state.staff.filter(u=>u.id!==id);renderUsersPage();saveState();showNotif('🗑 تم حذف الموظف');}
function renderUsersPage(){const grid=document.getElementById('users-grid');if(!state.staff.length){grid.innerHTML='<div style="color:#94a3b8;font-size:13px;padding:20px 0;grid-column:1/-1;text-align:center">لا يوجد موظفون بعد — اضغط "+ إضافة موظف"</div>';return;}grid.innerHTML=state.staff.map(u=>`<div class="user-card"><div class="user-card-avatar" style="background:${u.color}">${u.name.substring(0,1)}</div><div class="user-card-name">${u.name}</div><span class="user-card-role ${u.role==='admin'?'role-admin':'role-cashier'}">${u.role==='admin'?'مدير':'كاشير'}</span><div style="display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-bottom:12px"><div class="ustat"><div class="ustat-label">مبيعاته</div><div class="ustat-val">${((u.sales||0)/1000000).toFixed(1)}م</div></div><div class="ustat"><div class="ustat-label">فواتيره</div><div class="ustat-val">${u.invoices||0}</div></div></div><div style="font-size:11px;color:#94a3b8;margin-bottom:10px;background:#f8fafc;padding:5px 8px;border-radius:6px;direction:ltr;text-align:center">${u.phone||'—'}</div><div class="user-card-actions"><button onclick="showNotif('تعديل ${u.name}')">✏️ تعديل</button><button onclick="deleteStaff(${u.id})">🗑 حذف</button></div></div>`).join('');}

// ============================================================
//  DASHBOARD & REPORTS
// ============================================================
function updateDashboard(){document.getElementById('dash-sales').textContent=state.totalSales.toLocaleString('ar-IQ');document.getElementById('dash-inv').textContent=state.totalInvoices;document.getElementById('dash-prods').textContent=state.products.length;document.getElementById('dash-custs').textContent=state.customers.length;const ok=state.products.filter(p=>p.stock>0&&(!p.min||p.stock>=p.min)).length,low=state.products.filter(p=>p.stock>0&&p.min&&p.stock<p.min).length,out=state.products.filter(p=>p.stock===0).length;document.getElementById('stock-summary').innerHTML=!state.products.length?'<div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد منتجات بعد</div>':[['جيد',ok,'#22c55e','#dcfce7'],['منخفض',low,'#d97706','#fef3c7'],['نافد',out,'#dc2626','#fee2e2']].map(([l,c,clr,bg])=>`<div style="display:flex;align-items:center;justify-content:space-between;padding:8px 12px;background:${bg};border-radius:8px;margin-bottom:6px"><span style="font-size:13px;color:${clr}">${l}</span><span style="font-weight:600;color:${clr}">${c} صنف</span></div>`).join('');const sorted=Object.entries(state.salesByProduct).sort((a,b)=>b[1]-a[1]).slice(0,5),mxQ=sorted[0]?sorted[0][1]:1;document.getElementById('top-items').innerHTML=sorted.length?sorted.map(([id,qty])=>{const p=state.products.find(x=>x.id==id);return p?`<div class="top-item"><span class="top-item-name">${p.icon} ${p.name}</span><div class="top-item-bar-wrap"><div class="top-item-bar" style="width:${Math.round(qty/mxQ*100)}%"></div></div><span class="top-item-val">${qty} ${p.unit}</span></div>`:''}).join(''):'<div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد مبيعات بعد</div>';}
function updateReports(){const tp=Object.values(state.payStats).reduce((s,v)=>s+v,0)||1,hasData=Object.values(state.payStats).some(v=>v>0);document.getElementById('payment-chart').innerHTML=hasData?[['نقدي','#60a5fa'],['بطاقة','#34d399'],['آجل','#fbbf24']].map(([label,color])=>{const pct=Math.round((state.payStats[label]||0)/tp*100);return `<div><div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px;color:#374151"><span>${label}</span><span style="font-weight:500">${pct}%</span></div><div style="height:8px;background:#e2e8f0;border-radius:4px"><div style="height:8px;border-radius:4px;background:${color};width:${pct}%"></div></div></div>`;}).join(''):'<div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد مبيعات بعد</div>';const slow=state.products.filter(p=>!state.salesByProduct[p.id]&&p.stock>0);document.getElementById('slow-items').innerHTML=slow.length?slow.slice(0,6).map(p=>`<div class="top-item"><span class="top-item-name">${p.icon} ${p.name}</span><span class="stock-badge stock-low">لم يُباع بعد</span></div>`).join(''):'<div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد بيانات</div>';}

// ============================================================
//  BRANCHES
// ============================================================
function renderBranches(){const sm={active:'branch-active',pending:'branch-pending'},sl={active:'نشط',pending:'قيد التجهيز'};document.getElementById('branches-grid').innerHTML=state.branches.map(b=>`<div class="branch-card"><span class="branch-status ${sm[b.status]||'branch-pending'}">${sl[b.status]||'قيد التجهيز'}</span><div style="margin-top:8px;font-size:32px;margin-bottom:8px">🏪</div><div style="font-size:14px;font-weight:600;margin-bottom:4px;color:#1e293b">${b.name}</div><div style="font-size:11px;color:#64748b;margin-bottom:12px">📍 ${b.city}${b.area?' — '+b.area:''}</div><div class="branch-stats"><div class="bstat"><div class="bstat-label">المدير</div><div class="bstat-val" style="font-size:12px">${b.manager||'—'}</div></div><div class="bstat"><div class="bstat-label">نقاط POS</div><div class="bstat-val">${b.pos||1}</div></div></div><div class="branch-actions"><button onclick="showNotif('${b.name}')">📊 تفاصيل</button><button onclick="showNotif('تعديل')">✏️ تعديل</button></div></div>`).join('')+`<div class="branch-card new-branch" onclick="showNewBranchForm()"><div style="font-size:36px">➕</div><div style="font-size:14px;font-weight:500;color:#3b82f6">فتح فرع جديد</div></div>`;document.getElementById('branch-count').textContent=state.branches.length;}
function showNewBranchForm(){document.getElementById('branches-list-view').style.display='none';document.getElementById('new-branch-view').style.display='block';goStep(1);}
function hideBranchForm(){document.getElementById('branches-list-view').style.display='block';document.getElementById('new-branch-view').style.display='none';}
function goStep(n){[1,2,3].forEach(i=>{document.getElementById('form-step-'+i).style.display=i===n?'block':'none';const lbl=document.getElementById('step'+i+'-label');lbl.className='step'+(i<n?' done':i===n?' active':'');});if(n===3){const vals=[['اسم الفرع',document.getElementById('f-name').value||'—'],['المدينة',document.getElementById('f-city').value],['المنطقة',document.getElementById('f-area').value||'—'],['المدير',document.getElementById('f-manager').value||'—']];document.getElementById('review-content').innerHTML=`<div style="display:grid;grid-template-columns:1fr 1fr;gap:8px">${vals.map(([l,v])=>`<div style="background:#f8fafc;border-radius:8px;padding:10px;border:1px solid #e2e8f0"><div style="font-size:10px;color:#64748b;margin-bottom:3px">${l}</div><div style="font-weight:500;color:#1e293b">${v}</div></div>`).join('')}</div>`;}}
function saveBranch(){const name=document.getElementById('f-name').value.trim()||'فرع جديد';state.branches.push({name,city:document.getElementById('f-city').value,area:document.getElementById('f-area').value,manager:document.getElementById('f-manager').value,pos:parseInt(document.getElementById('f-pos').value)||1,status:'pending'});hideBranchForm();renderBranches();saveState();showNotif('✅ تم إنشاء '+name);}

// ============================================================
//  BACKUP
// ============================================================
function exportBackup(type){const filename=(type==='weekly'?'SuperCash_اسبوعي_':'SuperCash_نسخة_')+new Date().toISOString().slice(0,10)+'.json';const data=JSON.stringify(state,null,2);const blob=new Blob([data],{type:'application/json'});const url=URL.createObjectURL(blob);const a=document.createElement('a');a.href=url;a.download=filename;a.click();URL.revokeObjectURL(url);state.backupHistory.unshift({date:new Date().toLocaleString('ar-IQ'),filename,size:Math.round(data.length/1024*10)/10+' KB',type:type||'يدوي'});if(state.backupHistory.length>8)state.backupHistory.pop();saveState();renderBackupHistory();showNotif('✅ تم تصدير: '+filename);}

function importBackup(input){
  const file=input.files[0]; if(!file)return;
  const reader=new FileReader();
  reader.onload=e=>{
    try{
      const d=JSON.parse(e.target.result);
      if(!d.products){showNotif('❌ ملف غير صالح');return;}

      // خيار الاستيراد
      const choice = confirm(
        '📥 طريقة الاستيراد:\n\n' +
        '✅ موافق = دمج ذكي (يضيف المنتجات الجديدة فقط، لا يكرر الباركود)\n' +
        '❌ إلغاء = استبدال كامل (يمسح البيانات الحالية ويستورد الجديدة)'
      );

      if(choice){
        // ===== دمج ذكي =====
        let addedCount=0, skippedCount=0;

        (d.products||[]).forEach(importedP=>{
          // تحقق من التكرار بالباركود أو بالاسم
          const dupBarcode = importedP.barcode && state.products.find(p=>p.barcode===importedP.barcode);
          const dupName    = state.products.find(p=>p.name===importedP.name&&p.cat===importedP.cat);
          if(dupBarcode||dupName){ skippedCount++; return; }
          // أضف بـ ID جديد لتجنب التعارض
          state.products.push({...importedP, id:Date.now()+Math.random()});
          addedCount++;
        });

        // دمج العملاء (بدون تكرار الهاتف)
        (d.customers||[]).forEach(c=>{
          if(!state.customers.find(x=>x.phone===c.phone))
            state.customers.push({...c,id:Date.now()+Math.random()});
        });

        // دمج الفروع (بدون تكرار الاسم)
        (d.branches||[]).forEach(b=>{
          if(!state.branches.find(x=>x.name===b.name))
            state.branches.push({...b,id:Date.now()+Math.random()});
        });

        saveState();
        renderProducts();renderInventory();renderCRM();updateCatBar();renderBranches();renderBackupHistory();
        showNotif(`✅ دمج مكتمل — أُضيف: ${addedCount} منتج، تجاهل: ${skippedCount} مكرر`);

      } else {
        // ===== استبدال كامل =====
        if(!confirm('⚠️ هذا سيمسح جميع بياناتك الحالية. هل أنت متأكد؟'))return;
        Object.keys(state).forEach(k=>{ if(d[k]!==undefined&&k!=='license')state[k]=d[k]; });
        saveState();
        renderProducts();renderInventory();renderCRM();updateCatBar();renderBranches();renderUsersPage();renderBackupHistory();
        showNotif('✅ تم الاستيراد الكامل من: '+file.name);
      }

    }catch(err){showNotif('❌ ملف غير صالح — تأكد من النسخة الاحتياطية');}
  };
  reader.readAsText(file);
  input.value='';
}
function renderBackupHistory(){const el=document.getElementById('backup-history');if(!state.backupHistory.length){el.innerHTML='<div style="color:#94a3b8;font-size:13px;text-align:center;padding:20px 0">لا توجد نسخ بعد</div>';return;}el.innerHTML=state.backupHistory.map(b=>`<div class="backup-item"><span style="font-size:18px">📁</span><div class="backup-item-info"><div class="backup-item-date">${b.filename}</div><div class="backup-item-size">${b.date} · ${b.size}</div></div><span class="backup-status">${b.type}</span></div>`).join('');}

// ============================================================
//  NOTIFICATIONS & DATE
// ============================================================
let notifTimeout;
function showNotif(msg){const el=document.getElementById('notif');el.textContent=msg;el.classList.add('show');clearTimeout(notifTimeout);notifTimeout=setTimeout(()=>el.classList.remove('show'),2800);}
document.getElementById('current-date').textContent=new Date().toLocaleDateString('ar-IQ',{weekday:'long',year:'numeric',month:'long',day:'numeric'});

// ============================================================
//  SUPPORT
// ============================================================
function openSupport() {
  const lic = state.license;
  const now = Date.now();

  // حساب المدة المتبقية
  let licStatus = '';
  if (lic.status === 'active' && !lic.endDate) {
    licStatus = 'مفعّل — دائم';
  } else if (lic.status === 'active' && lic.endDate) {
    const rem = Math.max(0, Math.ceil((Number(lic.endDate) - now) / 86400000));
    licStatus = `مفعّل — متبقي ${rem} يوم`;
  } else if (lic.status === 'trial') {
    const rem = Math.max(0, Math.ceil((state.license.startDate + 3600000 - now) / 60000));
    licStatus = `تجريبي — متبقي ${rem} دقيقة`;
  } else {
    licStatus = 'منتهي الصلاحية';
  }

  const info = [
    '====== معلومات الدعم الفني ======',
    `📅 التاريخ: ${new Date().toLocaleString('ar-IQ')}`,
    '',
    '--- الترخيص ---',
    `الحالة: ${licStatus}`,
    `الكود: ${lic.code || 'لا يوجد'}`,
    `تاريخ البداية: ${lic.startDate ? new Date(lic.startDate).toLocaleString('ar-IQ') : '—'}`,
    `تاريخ الانتهاء: ${lic.endDate ? new Date(Number(lic.endDate)).toLocaleString('ar-IQ') : 'دائم'}`,
    '',
    '--- البيانات ---',
    `عدد المنتجات: ${state.products.length}`,
    `عدد العملاء: ${state.customers.length}`,
    `عدد الفروع: ${state.branches.length}`,
    `إجمالي الفواتير: ${state.totalInvoices}`,
    `إجمالي المبيعات: ${state.totalSales.toLocaleString('ar-IQ')} د.ع`,
    '',
    '--- الجهاز ---',
    `المتصفح: ${navigator.userAgent.split(') ')[0].split('(')[1] || navigator.userAgent.slice(0,50)}`,
    `النظام: ${navigator.platform}`,
    `الإصدار: SuperCash Pro v4`,
    `APP_KEY: ${APP_KEY}`,
    '================================',
  ].join('\n');

  document.getElementById('support-text').value = info;
  document.getElementById('modal-support').style.display = 'flex';
}

function copySupport() {
  const text = document.getElementById('support-text').value;
  navigator.clipboard.writeText(text).then(() => {
    document.getElementById('copy-support-btn').textContent = '✅ تم النسخ!';
    setTimeout(() => document.getElementById('copy-support-btn').textContent = '📋 نسخ المعلومات', 2000);
    showNotif('✅ تم نسخ معلومات الدعم');
  }).catch(() => {
    document.getElementById('support-text').select();
    document.execCommand('copy');
    showNotif('✅ تم النسخ');
  });
}

function sendWhatsapp() {
  const text = document.getElementById('support-text').value;
  const encoded = encodeURIComponent(text);
  // رقم واتساب خدمة العملاء
  window.open(`https://wa.me/964${SUPPORT_NUMBER.replace(/^0/,'')}?text=${encoded}`, '_blank');
}

// ============================================================
//  INIT
// ============================================================
loadState();
renderProducts();renderInventory();renderCRM();updateCatBar();
renderBranches();renderUsersPage();renderBackupHistory();
initLicense(); // يفحص الترخيص ويعرض الشاشة المناسبة
showPage('pos');
</script>
</body>
</html>
