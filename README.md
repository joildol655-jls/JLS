Aplicativo JLS - LIMA SERRALHERIA
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="theme-color" content="#FF6B00">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="JLS">
<title>JLS – LIMA SERRALHERIA</title>
<style>
  :root {
    --bg: #0f1115;
    --surface: #181b22;
    --surface-2: #222732;
    --border: #2f3646;
    --text: #f3f4f6;
    --muted: #9ca3af;
    --accent: #FF6B00;
    --accent-soft: rgba(255, 107, 0, 0.16);
    --silver: #cbd5e1;
    --success: #16a34a;
    --danger: #dc2626;
    --warning: #eab308;
  }

  * {
    box-sizing: border-box;
    -webkit-tap-highlight-color: transparent;
  }

  body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    padding-bottom: 84px;
  }

  .hidden {
    display: none !important;
  }

  .topbar {
    position: sticky;
    top: 0;
    z-index: 30;
    background: rgba(15, 17, 21, 0.95);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid var(--border);
    padding: 12px 16px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
  }

  .brand-row {
    display: flex;
    align-items: center;
    gap: 10px;
    min-width: 0;
  }

  .brand-titles {
    min-width: 0;
  }

  .brand-name {
    font-size: 16px;
    font-weight: 800;
    letter-spacing: 0.4px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .brand-sub {
    font-size: 11px;
    color: var(--silver);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .pill-row {
    display: flex;
    align-items: center;
    gap: 6px;
    flex-shrink: 0;
  }

  .badge {
    font-size: 11px;
    font-weight: 700;
    padding: 4px 8px;
    border-radius: 999px;
    background: var(--accent-soft);
    color: var(--accent);
    border: 1px solid rgba(255, 107, 0, 0.35);
  }

  .btn-icon {
    background: var(--surface-2);
    color: var(--text);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 7px 10px;
    font-size: 12px;
    font-weight: 600;
    cursor: pointer;
  }

  .container {
    max-width: 820px;
    margin: 0 auto;
    padding: 16px;
  }

  .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 16px;
    margin-bottom: 14px;
  }

  .card-title {
    font-size: 15px;
    font-weight: 700;
    margin: 0 0 12px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 8px;
  }

  .muted {
    color: var(--muted);
    font-size: 13px;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 10px;
  }

  .grid-3 {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 10px;
  }

  @media (max-width: 600px) {
    .grid-2, .grid-3 {
      grid-template-columns: 1fr;
    }
  }

  .stat-box {
    background: var(--surface-2);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 12px;
  }

  .stat-label {
    font-size: 11px;
    color: var(--muted);
    text-transform: uppercase;
    letter-spacing: 0.4px;
  }

  .stat-value {
    font-size: 18px;
    font-weight: 800;
    margin-top: 4px;
    color: var(--text);
  }

  .stat-value.accent {
    color: var(--accent);
  }

  .stat-value.green {
    
