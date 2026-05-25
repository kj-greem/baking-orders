<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Baked Orders — Collaborative Tracker</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Mono:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --cream: #fdf6ec;
    --warm-white: #fffaf4;
    --brown: #3b2314;
    --caramel: #c4813a;
    --caramel-light: #e8a95c;
    --rose: #d4756b;
    --sage: #7a8c6e;
    --ink: #1e130a;
    --muted: #9a8070;
    --border: #e8d9c8;
    --shadow: rgba(59,35,20,0.1);
  }

  body {
    font-family: 'DM Mono', monospace;
    background: var(--cream);
    color: var(--ink);
    min-height: 100vh;
    background-image:
      radial-gradient(ellipse at 20% 10%, rgba(196,129,58,0.08) 0%, transparent 60%),
      radial-gradient(ellipse at 80% 90%, rgba(212,117,107,0.07) 0%, transparent 50%);
  }

  header {
    padding: 2.5rem 3rem 1.5rem;
    border-bottom: 1px solid var(--border);
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    gap: 1rem;
    flex-wrap: wrap;
    background: var(--warm-white);
  }

  .header-left h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(1.8rem, 4vw, 2.8rem);
    color: var(--brown);
    line-height: 1;
    letter-spacing: -0.02em;
  }

  .header-left h1 em {
    color: var(--caramel);
    font-style: italic;
  }

  .header-left p {
    margin-top: 0.4rem;
    font-size: 0.72rem;
    color: var(--muted);
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .month-nav {
    display: flex;
    align-items: center;
    gap: 0.75rem;
  }

  .month-nav button {
    width: 32px; height: 32px;
    border: 1px solid var(--border);
    background: var(--cream);
    border-radius: 50%;
    cursor: pointer;
    font-size: 1rem;
    color: var(--brown);
    display: flex; align-items: center; justify-content: center;
    transition: all 0.15s;
  }

  .month-nav button:hover { background: var(--caramel); color: white; border-color: var(--caramel); }

  #month-label {
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    color: var(--brown);
    min-width: 130px;
    text-align: center;
  }

  .stats-bar {
    display: flex;
    gap: 0;
    border-bottom: 1px solid var(--border);
    background: var(--warm-white);
    overflow-x: auto;
  }

  .stat {
    flex: 1;
    min-width: 120px;
    padding: 1rem 1.5rem;
    border-right: 1px solid var(--border);
  }

  .stat:last-child { border-right: none; }

  .stat-label {
    font-size: 0.62rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 0.3rem;
  }

  .stat-value {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
    color: var(--brown);
    font-weight: 700;
  }

  .stat-value.money { color: var(--sage); }
  .stat-value.pending { color: var(--rose); }

  main {
    display: grid;
    grid-template-columns: 1fr 340px;
    min-height: calc(100vh - 160px);
  }

  .orders-section {
    padding: 2rem 2.5rem;
    border-right: 1px solid var(--border);
  }

  .section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 1.5rem;
  }

  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    color: var(--brown);
  }

  .btn {
    font-family: 'DM Mono', monospace;
    font-size: 0.72rem;
    letter-spacing: 0.06em;
    padding: 0.5rem 1.1rem;
    border-radius: 2px;
    cursor: pointer;
    transition: all 0.15s;
    border: none;
  }

  .btn-primary {
    background: var(--brown);
    color: var(--cream);
  }

  .btn-primary:hover { background: var(--caramel); }

  .btn-ghost {
    background: transparent;
    border: 1px solid var(--border);
    color: var(--muted);
  }

  .btn-ghost:hover { border-color: var(--caramel); color: var(--caramel); }

  .table-wrap { overflow-x: auto; }

  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.78rem;
  }

  thead th {
    text-align: left;
    font-size: 0.62rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    padding: 0.5rem 0.75rem 0.75rem;
    border-bottom: 1px solid var(--border);
    white-space: nowrap;
  }

  tbody tr {
    border-bottom: 1px solid var(--border);
    transition: background 0.1s;
  }

  tbody tr:hover { background: rgba(196,129,58,0.04); }

  tbody td {
    padding: 0.85rem 0.75rem;
    vertical-align: middle;
    color: var(--ink);
  }

  .client-name {
    font-family: 'Playfair Display', serif;
    font-size: 0.9rem;
    color: var(--brown);
  }

  .badge {
    display: inline-block;
    padding: 0.2rem 0.55rem;
    border-radius: 20px;
    font-size: 0.62rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    font-weight: 500;
  }

  .badge-paid { background: rgba(122,140,110,0.15); color: var(--sage); }
  .badge-pending { background: rgba(212,117,107,0.15); color: var(--rose); }
  .badge-deposit { background: rgba(196,129,58,0.15); color: var(--caramel); }

  .amount { font-weight: 500; color: var(--sage); }

  .action-btns { display: flex; gap: 0.4rem; }

  .icon-btn {
    width: 26px; height: 26px;
    border: 1px solid var(--border);
    background: transparent;
    border-radius: 2px;
    cursor: pointer;
    font-size: 0.8rem;
    display: flex; align-items: center; justify-content: center;
    transition: all 0.12s;
    color: var(--muted);
  }

  .icon-btn:hover { background: var(--rose); color: white; border-color: var(--rose); }
  .icon-btn.edit:hover { background: var(--caramel); border-color: var(--caramel); }

  .empty-state {
    text-align: center;
    padding: 4rem 2rem;
    color: var(--muted);
  }

  .empty-state .emoji { font-size: 2.5rem; margin-bottom: 1rem; }

  .side-panel {
    padding: 2rem 1.75rem;
    background: var(--warm-white);
  }

  .form-title {
    font-family: 'Playfair Display', serif;
    font-size: 1rem;
    color: var(--brown);
    margin-bottom: 1.25rem;
    padding-bottom: 0.75rem;
    border-bottom: 1px solid var(--border);
  }

  .form-group { margin-bottom: 1rem; }

  label {
    display: block;
    font-size: 0.62rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 0.35rem;
  }

  input, select, textarea {
    width: 100%;
    font-family: 'DM Mono', monospace;
    font-size: 0.78rem;
    padding: 0.55rem 0.75rem;
    border: 1px solid var(--border);
    background: var(--cream);
    color: var(--ink);
    border-radius: 2px;
    outline: none;
    transition: border-color 0.15s;
  }

  input:focus, select:focus, textarea:focus {
    border-color: var(--caramel);
    background: var(--warm-white);
  }

  textarea { resize: vertical; min-height: 70px; }

  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 0.75rem; }

  .form-actions { display: flex; gap: 0.5rem; margin-top: 1.25rem; }
  .form-actions .btn { flex: 1; text-align: center; }

  .summary-section {
    margin-top: 2rem;
    padding-top: 1.5rem;
    border-top: 1px solid var(--border);
  }

  .summary-title {
    font-size: 0.62rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 1rem;
  }

  .summary-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5rem 0;
    border-bottom: 1px dashed var(--border);
    font-size: 0.75rem;
  }

  .summary-row:last-child { border-bottom: none; }
  .summary-row .label { color: var(--muted); }
  .summary-row .value { color: var(--brown); font-weight: 500; }
  .summary-row.total .value { color: var(--sage); font-family: 'Playfair Display', serif; font-size: 1rem; }

  .modal-overlay {
    display: none;
    position: fixed; inset: 0;
    background: rgba(30,19,10,0.5);
    z-index: 100;
    align-items: center;
    justify-content: center;
    backdrop-filter: blur(2px);
  }

  .modal-overlay.open { display: flex; }

  .modal {
    background: var(--warm-white);
    border: 1px solid var(--border);
    padding: 2rem;
    width: 90%;
    max-width: 480px;
    max-height: 90vh;
    overflow-y: auto;
    animation: slideUp 0.2s ease;
  }

  @keyframes slideUp {
    from { transform: translateY(20px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
  }

  .modal-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.5rem;
  }

  .modal-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.2rem;
    color: var(--brown);
  }

  .close-btn {
    background: none; border: none; cursor: pointer;
    font-size: 1.2rem; color: var(--muted);
    width: 28px; height: 28px;
    display: flex; align-items: center; justify-content: center;
    border-radius: 50%;
    transition: all 0.12s;
  }

  .close-btn:hover { background: var(--border); color: var(--brown); }

  .filters {
    display: flex;
    gap: 0.5rem;
    margin-bottom: 1.25rem;
    flex-wrap: wrap;
  }

  .filter-btn {
    font-family: 'DM Mono', monospace;
    font-size: 0.65rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 0.3rem 0.75rem;
    border: 1px solid var(--border);
    background: transparent;
    color: var(--muted);
    border-radius: 20px;
    cursor: pointer;
    transition: all 0.12s;
  }

  .filter-btn.active { background: var(--brown); color: var(--cream); border-color: var(--brown); }

  @media (max-width: 800px) {
    main { grid-template-columns: 1fr; }
    .side-panel { border-top: 1px solid var(--border); }
    header { padding: 1.5rem; }
    .orders-section { padding: 1.5rem; }
  }
</style>
</head>
<body>

<header>
  <div class="header-left">
    <h1>Baked <em>Orders</em></h1>
    <p>Collaborative monthly tracker</p>
  </div>
  <div class="month-nav">
    <button onclick="changeMonth(-1)">‹</button>
    <span id="month-label"></span>
    <button onclick="changeMonth(1)">›</button>
  </div>
</header>

<div class="stats-bar">
  <div class="stat">
    <div class="stat-label">Total Orders</div>
    <div class="stat-value" id="stat-total">—</div>
  </div>
  <div class="stat">
    <div class="stat-label">Revenue</div>
    <div class="stat-value money" id="stat-revenue">—</div>
  </div>
  <div class="stat">
    <div class="stat-label">Collected</div>
    <div class="stat-value money" id="stat-collected">—</div>
  </div>
  <div class="stat">
    <div class="stat-label">Outstanding</div>
    <div class="stat-value pending" id="stat-outstanding">—</div>
  </div>
</div>

<main>
  <section class="orders-section">
    <div class="section-header">
      <span class="section-title">Orders</span>
      <button class="btn btn-primary" onclick="openModal()">+ New Order</button>
    </div>

    <div class="filters">
      <button class="filter-btn active" onclick="setFilter('all', this)">All</button>
      <button class="filter-btn" onclick="setFilter('paid', this)">Paid</button>
      <button class="filter-btn" onclick="setFilter('deposit', this)">Deposit Only</button>
      <button class="filter-btn" onclick="setFilter('pending', this)">Unpaid</button>
    </div>

    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>Client</th>
            <th>Item</th>
            <th>Delivery</th>
            <th>Total</th>
            <th>Deposit</th>
            <th>Status</th>
            <th></th>
          </tr>
        </thead>
        <tbody id="orders-tbody"></tbody>
      </table>
      <div id="empty-state" class="empty-state" style="display:none">
        <div class="emoji">🧁</div>
        <p>No orders this month yet.</p>
      </div>
    </div>
  </section>

  <aside class="side-panel">
    <div class="form-title">Quick Add Order</div>

    <div class="form-group">
      <label>Client Name</label>
      <input type="text" id="f-client" placeholder="e.g. Sarah M.">
    </div>
    <div class="form-group">
      <label>Item / Description</label>
      <input type="text" id="f-item" placeholder="e.g. 6-inch layered cake">
    </div>
    <div class="form-row">
      <div class="form-group">
        <label>Delivery Date</label>
        <input type="date" id="f-date">
      </div>
      <div class="form-group">
        <label>Quantity</label>
        <input type="number" id="f-qty" value="1" min="1">
      </div>
    </div>
    <div class="form-row">
      <div class="form-group">
        <label>Total Price ($)</label>
        <input type="number" id="f-total" placeholder="0.00" step="0.01">
      </div>
      <div class="form-group">
        <label>Deposit Paid ($)</label>
        <input type="number" id="f-deposit" placeholder="0.00" step="0.01">
      </div>
    </div>
    <div class="form-group">
      <label>Payment Status</label>
      <select id="f-status">
        <option value="pending">Unpaid</option>
        <option value="deposit">Deposit Only</option>
        <option value="paid">Fully Paid</option>
      </select>
    </div>
    <div class="form-group">
      <label>Notes</label>
      <textarea id="f-notes" placeholder="Flavors, allergies, special requests..."></textarea>
    </div>
    <div class="form-actions">
      <button class="btn btn-primary" onclick="addOrder()">Add Order</button>
      <button class="btn btn-ghost" onclick="clearForm()">Clear</button>
    </div>

    <div class="summary-section">
      <div class="summary-title">Month Summary</div>
      <div class="summary-row">
        <span class="label">Orders</span>
        <span class="value" id="sum-orders">—</span>
      </div>
      <div class="summary-row">
        <span class="label">Paid in Full</span>
        <span class="value" id="sum-paid">—</span>
      </div>
      <div class="summary-row">
        <span class="label">Deposits Collected</span>
        <span class="value" id="sum-deposits">—</span>
      </div>
      <div class="summary-row">
        <span class="label">Remaining to Collect</span>
        <span class="value" id="sum-remaining">—</span>
      </div>
      <div class="summary-row total">
        <span class="label">Total Revenue</span>
        <span class="value" id="sum-total">—</span>
      </div>
    </div>
  </aside>
</main>

<div class="modal-overlay" id="modal">
  <div class="modal">
    <div class="modal-header">
      <span class="modal-title" id="modal-title">Edit Order</span>
      <button class="close-btn" onclick="closeModal()">✕</button>
    </div>
    <div class="form-group">
      <label>Client Name</label>
      <input type="text" id="m-client">
    </div>
    <div class="form-group">
      <label>Item / Description</label>
      <input type="text" id="m-item">
    </div>
    <div class="form-row">
      <div class="form-group">
        <label>Delivery Date</label>
        <input type="date" id="m-date">
      </div>
      <div class="form-group">
        <label>Quantity</label>
        <input type="number" id="m-qty" min="1">
      </div>
    </div>
    <div class="form-row">
      <div class="form-group">
        <label>Total Price ($)</label>
        <input type="number" id="m-total" step="0.01">
      </div>
      <div class="form-group">
        <label>Deposit Paid ($)</label>
        <input type="number" id="m-deposit" step="0.01">
      </div>
    </div>
    <div class="form-group">
      <label>Payment Status</label>
      <select id="m-status">
        <option value="pending">Unpaid</option>
        <option value="deposit">Deposit Only</option>
        <option value="paid">Fully Paid</option>
      </select>
    </div>
    <div class="form-group">
      <label>Notes</label>
      <textarea id="m-notes"></textarea>
    </div>
    <div class="form-actions">
      <button class="btn btn-primary" onclick="saveEdit()">Save Changes</button>
      <button class="btn btn-ghost" onclick="closeModal()">Cancel</button>
    </div>
  </div>
</div>

<script>
  const MONTHS = ['January','February','March','April','May','June','July','August','September','October','November','December'];
  const FIREBASE_DB = "https://baking-orders-default-rtdb.asia-southeast1.firebasedatabase.app";
  const FIREBASE_KEY = "AIzaSyCDTbjwS7O30LQiIh2SdRTsjCHi_NYzcOk";

  let currentDate = new Date();
  let currentMonth = currentDate.getMonth();
  let currentYear = currentDate.getFullYear();
  let activeFilter = 'all';
  let editingId = null;
  let allOrders = [];

  function dbPath() {
    return `orders/${currentYear}/${currentMonth}`;
  }

  function fmt(n) {
    return '$' + parseFloat(n || 0).toFixed(2);
  }

  function render() {
    document.getElementById('month-label').textContent = `${MONTHS[currentMonth]} ${currentYear}`;

    const filtered = activeFilter === 'all' ? allOrders : allOrders.filter(o => o.status === activeFilter);

    const totalRev = allOrders.reduce((s,o) => s + parseFloat(o.total||0), 0);
    const collected = allOrders.reduce((s,o) => {
      if (o.status === 'paid') return s + parseFloat(o.total||0);
      return s + parseFloat(o.deposit||0);
    }, 0);
    const outstanding = totalRev - collected;

    document.getElementById('stat-total').textContent = allOrders.length;
    document.getElementById('stat-revenue').textContent = fmt(totalRev);
    document.getElementById('stat-collected').textContent = fmt(collected);
    document.getElementById('stat-outstanding').textContent = fmt(outstanding);

    document.getElementById('sum-orders').textContent = allOrders.length;
    document.getElementById('sum-paid').textContent = allOrders.filter(o => o.status==='paid').length;
    document.getElementById('sum-deposits').textContent = fmt(allOrders.reduce((s,o) => s+parseFloat(o.deposit||0),0));
    document.getElementById('sum-remaining').textContent = fmt(outstanding);
    document.getElementById('sum-total').textContent = fmt(totalRev);

    const tbody = document.getElementById('orders-tbody');
    tbody.innerHTML = '';

    if (filtered.length === 0) {
      document.getElementById('empty-state').style.display = 'block';
    } else {
      document.getElementById('empty-state').style.display = 'none';
      filtered.forEach(o => {
        const tr = document.createElement('tr');
        const statusLabel = { paid: 'Paid', pending: 'Unpaid', deposit: 'Deposit' }[o.status];
        const statusClass = { paid: 'badge-paid', pending: 'badge-pending', deposit: 'badge-deposit' }[o.status];
        const delivDate = o.date ? new Date(o.date + 'T00:00:00').toLocaleDateString('en-US',{month:'short',day:'numeric'}) : '—';
        tr.innerHTML = `
          <td><div class="client-name">${o.client || '—'}</div>${o.notes ? `<div style="font-size:0.65rem;color:var(--muted);margin-top:2px">${o.notes.slice(0,40)}${o.notes.length>40?'…':''}</div>` : ''}</td>
          <td>${o.item || '—'}${o.qty > 1 ? ` <span style="color:var(--muted)">×${o.qty}</span>` : ''}</td>
          <td style="white-space:nowrap">${delivDate}</td>
          <td class="amount">${fmt(o.total)}</td>
          <td style="color:var(--muted)">${o.deposit > 0 ? fmt(o.deposit) : '—'}</td>
          <td><span class="badge ${statusClass}">${statusLabel}</span></td>
          <td>
            <div class="action-btns">
              <button class="icon-btn edit" title="Edit" onclick="openEditModal('${o.id}')">✎</button>
              <button class="icon-btn" title="Delete" onclick="deleteOrder('${o.id}')">✕</button>
            </div>
          </td>
        `;
        tbody.appendChild(tr);
      });
    }
  }

  async function loadOrders() {
    try {
      const path = dbPath();
      const url = `${FIREBASE_DB}/${path}.json?auth=${FIREBASE_KEY}`;
      const res = await fetch(url);
      const data = await res.json();
      if (data && typeof data === 'object' && data !== null) {
        allOrders = Object.keys(data).map(key => ({ id: key, ...data[key] }));
      } else {
        allOrders = [];
      }
      render();
    } catch (err) {
      console.error('Load error:', err);
    }
  }

  function changeMonth(dir) {
    currentMonth += dir;
    if (currentMonth > 11) { currentMonth = 0; currentYear++; }
    if (currentMonth < 0) { currentMonth = 11; currentYear--; }
    loadOrders();
  }

  function setFilter(f, btn) {
    activeFilter = f;
    document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    render();
  }

  function addOrder() {
    const client = document.getElementById('f-client').value.trim();
    const item = document.getElementById('f-item').value.trim();
    if (!client && !item) { alert('Please fill in at least a client name or item.'); return; }

    const newId = Date.now().toString();
    const order = {
      client,
      item,
      date: document.getElementById('f-date').value,
      qty: document.getElementById('f-qty').value || 1,
      total: document.getElementById('f-total').value || 0,
      deposit: document.getElementById('f-deposit').value || 0,
      status: document.getElementById('f-status').value,
      notes: document.getElementById('f-notes').value.trim(),
    };
    
    const url = `${FIREBASE_DB}/${dbPath()}/${newId}.json?auth=${FIREBASE_KEY}`;
    fetch(url, {
      method: 'PUT',
      body: JSON.stringify(order)
    }).then(() => {
      clearForm();
      loadOrders();
    }).catch(err => console.error('Add error:', err));
  }

  function clearForm() {
    ['f-client','f-item','f-date','f-total','f-deposit','f-notes'].forEach(id => document.getElementById(id).value = '');
    document.getElementById('f-qty').value = 1;
    document.getElementById('f-status').value = 'pending';
  }

  function deleteOrder(id) {
    if (!confirm('Delete this order?')) return;
    const url = `${FIREBASE_DB}/${dbPath()}/${id}.json?auth=${FIREBASE_KEY}`;
    fetch(url, { method: 'DELETE' })
      .then(() => loadOrders())
      .catch(err => console.error('Delete error:', err));
  }

  function openModal() {
    editingId = null;
    document.getElementById('modal-title').textContent = 'New Order';
    ['m-client','m-item','m-date','m-total','m-deposit','m-notes'].forEach(id => document.getElementById(id).value = '');
    document.getElementById('m-qty').value = 1;
    document.getElementById('m-status').value = 'pending';
    document.getElementById('modal').classList.add('open');
  }

  function openEditModal(id) {
    const o = allOrders.find(x => x.id === id);
    if (!o) return;
    editingId = id;
    document.getElementById('modal-title').textContent = 'Edit Order';
    document.getElementById('m-client').value = o.client || '';
    document.getElementById('m-item').value = o.item || '';
    document.getElementById('m-date').value = o.date || '';
    document.getElementById('m-qty').value = o.qty || 1;
    document.getElementById('m-total').value = o.total || '';
    document.getElementById('m-deposit').value = o.deposit || '';
    document.getElementById('m-status').value = o.status || 'pending';
    document.getElementById('m-notes').value = o.notes || '';
    document.getElementById('modal').classList.add('open');
  }

  function saveEdit() {
    const updated = {
      client: document.getElementById('m-client').value.trim(),
      item: document.getElementById('m-item').value.trim(),
      date: document.getElementById('m-date').value,
      qty: document.getElementById('m-qty').value,
      total: document.getElementById('m-total').value || 0,
      deposit: document.getElementById('m-deposit').value || 0,
      status: document.getElementById('m-status').value,
      notes: document.getElementById('m-notes').value.trim(),
    };
    
    const url = `${FIREBASE_DB}/${dbPath()}/${editingId}.json?auth=${FIREBASE_KEY}`;
    fetch(url, {
      method: 'PATCH',
      body: JSON.stringify(updated)
    }).then(() => {
      closeModal();
      loadOrders();
    }).catch(err => console.error('Update error:', err));
  }

  function closeModal() {
    document.getElementById('modal').classList.remove('open');
  }

  document.getElementById('modal').addEventListener('click', e => {
    if (e.target === document.getElementById('modal')) closeModal();
  });

  loadOrders();
  setInterval(loadOrders, 2000);
</script>

</body>
</html>
