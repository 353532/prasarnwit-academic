<!doctype html>
<html lang="th">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>ระบบค้นหาตารางสอน — معهد الثقافة الإسلامية 2026</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@400;500;600;700&family=Scheherazade+New:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f1f5f2;
      --surface: #ffffff;
      --surface-subtle: #f7faf8;
      --surface-tinted: #eff6f1;
      --border: #d5e0d7;
      --border-strong: #b8c9bc;
      --grid-border: #c0c0c0;
      --grid-border-dark: #808080;
      --ink: #132017;
      --ink-secondary: #3f5145;
      --muted: #647469;
      --brand: #1E662D;
      --brand-hover: #164f22;
      --brand-soft: #e6f4ea;
      --brand-border: #add8b7;
      --accent-gold: #E6BD72;
      --accent-gold-dark: #946817;
      --accent-gold-soft: #fdf7ea;
      --accent-green: #79C265;
      --danger: #F65244;
      --radius-sm: 10px;
      --radius: 14px;
      --radius-lg: 18px;
      --shadow-xs: 0 1px 2px rgba(16, 36, 22, 0.04);
      --shadow-sm: 0 2px 6px rgba(16, 36, 22, 0.05), 0 1px 2px rgba(16, 36, 22, 0.04);
      --shadow: 0 8px 24px rgba(16, 38, 22, 0.07), 0 2px 6px rgba(16, 38, 22, 0.04);
      --shadow-lg: 0 22px 50px rgba(12, 28, 17, 0.22), 0 4px 12px rgba(12, 28, 17, 0.08);
      --space-1: 4px;
      --space-2: 8px;
      --space-3: 12px;
      --space-4: 16px;
      --space-5: 20px;
      --space-6: 24px;
      --space-8: 32px;
      --font-ui: 'Sarabun', 'Scheherazade New', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      --font-ar: 'Scheherazade New', "Segoe UI", Tahoma, Arial, sans-serif;
    }

    * {
      box-sizing: border-box;
    }

    html {
      -webkit-text-size-adjust: 100%;
      overflow-x: clip;
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: var(--font-ui);
      color: var(--ink);
      background-color: var(--bg);
      background-image:
        radial-gradient(ellipse 90% 420px at 50% 0%, rgba(30, 102, 45, 0.065) 0%, rgba(30, 102, 45, 0) 75%);
      line-height: 1.55;
      font-size: 15px;
      -webkit-font-smoothing: antialiased;
      overflow-x: clip;
      min-height: 100vh;
    }

    /* Refined Scrollbars */
    .directory-list,
    .self-teacher-grid,
    .tt-scroll-wrap,
    .table-scroll,
    .modal-body {
      scrollbar-width: thin;
      scrollbar-color: #bdcfc1 transparent;
    }

    .directory-list::-webkit-scrollbar,
    .self-teacher-grid::-webkit-scrollbar,
    .tt-scroll-wrap::-webkit-scrollbar,
    .table-scroll::-webkit-scrollbar,
    .modal-body::-webkit-scrollbar {
      width: 7px;
      height: 7px;
    }

    .directory-list::-webkit-scrollbar-thumb,
    .self-teacher-grid::-webkit-scrollbar-thumb,
    .tt-scroll-wrap::-webkit-scrollbar-thumb,
    .table-scroll::-webkit-scrollbar-thumb,
    .modal-body::-webkit-scrollbar-thumb {
      background: #bdcfc1;
      border-radius: 999px;
    }

    .directory-list::-webkit-scrollbar-thumb:hover,
    .self-teacher-grid::-webkit-scrollbar-thumb:hover,
    .tt-scroll-wrap::-webkit-scrollbar-thumb:hover,
    .table-scroll::-webkit-scrollbar-thumb:hover {
      background: #96b09c;
    }

    @keyframes viewFadeIn {
      from {
        opacity: 0;
        transform: translateY(5px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes modalSlideUp {
      from {
        opacity: 0;
        transform: translateY(14px) scale(0.985);
      }
      to {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        transition-duration: 0.01ms !important;
      }
    }

    .ar-text {
      font-family: var(--font-ar);
      direction: rtl;
      unicode-bidi: isolate;
      line-height: 1.65;
      font-size: 1.13em;
    }

    /* Header */
    .app-header {
      background-color: #e6f5ea;
      background-image:
        url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='80' height='80' viewBox='0 0 80 80'%3E%3Cg fill='none' stroke='%231E662D' stroke-linejoin='round'%3E%3Cpath d='M40 0L48 16L64 16L64 32L80 40L64 48L64 64L48 64L40 80L32 64L16 64L16 48L0 40L16 32L16 16L32 16Z' stroke-opacity='0.14' stroke-width='1.2'/%3E%3Cpath d='M0 16L16 16L16 0M64 0L64 16L80 16M80 64L64 64L64 80M16 80L16 64L0 64M0 24L11 11L24 0M56 0L69 11L80 24M80 56L69 69L56 80M24 80L11 69L0 56' stroke-opacity='0.11' stroke-width='1'/%3E%3Cpath d='M40 19L61 40L40 61L19 40Z' fill='%23E6BD72' fill-opacity='0.14' stroke-opacity='0.18' stroke-width='1.15'/%3E%3Cpath d='M25.2 25.2H54.8V54.8H25.2Z' fill='%231E662D' fill-opacity='0.035' stroke-opacity='0.18' stroke-width='1.15'/%3E%3Ccircle cx='40' cy='40' r='5.5' stroke='%23C59638' stroke-opacity='0.26' stroke-width='1'/%3E%3C/g%3E%3C/svg%3E"),
        radial-gradient(circle at 18% 25%, rgba(255, 255, 255, 0.96) 0%, rgba(255, 255, 255, 0) 56%),
        linear-gradient(125deg, #ffffff 0%, #f1faf4 34%, #cdebd5 68%, #93d5a7 100%);
      background-size: 80px 80px, 100% 100%, 100% 100%;
      color: #103819;
      border-top: 4px solid var(--brand);
      border-bottom: 3px solid var(--accent-gold);
      box-shadow: 0 4px 18px rgba(20, 68, 31, 0.08);
      position: relative;
    }

    .header-logos-band {
      background: linear-gradient(90deg, rgba(255, 255, 255, 0.9) 0%, rgba(255, 255, 255, 0.65) 55%, rgba(255, 255, 255, 0.4) 100%);
      border-bottom: 1px solid rgba(30, 102, 45, 0.14);
      backdrop-filter: blur(4px);
    }

    .header-logos-inner {
      max-width: 1280px;
      margin: 0 auto;
      padding: clamp(10px, 2vw, 15px) clamp(12px, 3vw, 24px);
      display: flex;
      align-items: center;
      justify-content: center;
      gap: clamp(12px, 2.5vw, 24px) clamp(16px, 3vw, 32px);
      flex-wrap: wrap;
    }

    .header-logos-left {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: clamp(12px, 2.5vw, 22px);
      flex-wrap: wrap;
    }

    @media (min-width: 768px) {
      .header-logos-inner {
        justify-content: space-between;
      }
      .header-logos-left {
        justify-content: flex-start;
      }
    }

    .header-emblem-img {
      width: clamp(62px, 8.5vw, 82px);
      height: clamp(62px, 8.5vw, 82px);
      object-fit: contain;
      display: block;
      flex-shrink: 0;
      filter: drop-shadow(0 3px 6px rgba(18, 56, 26, 0.14));
    }

    .logos-divider {
      width: 1.5px;
      height: clamp(44px, 6vw, 60px);
      background: linear-gradient(180deg, transparent, #c79a3b, transparent);
      flex-shrink: 0;
    }

    .header-calligraphy-img {
      height: clamp(54px, 8vw, 76px);
      width: auto;
      max-width: min(100%, 224px);
      object-fit: contain;
      display: block;
      background: #ffffff;
      padding: 5px 12px;
      border-radius: 12px;
      border: 1px solid rgba(30, 102, 45, 0.12);
      box-shadow: 0 2px 8px rgba(20, 60, 30, 0.06);
    }

    .header-school-name-img {
      height: clamp(44px, 6.8vw, 68px);
      width: auto;
      max-width: min(92vw, 340px);
      object-fit: contain;
      display: block;
      filter: drop-shadow(0 1px 2px rgba(255, 255, 255, 0.9));
    }

    .header-inner {
      max-width: 1280px;
      margin: 0 auto;
      padding: clamp(14px, 2.8vw, 20px) clamp(12px, 3vw, 24px);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3) var(--space-4);
    }

    .brand-title-group {
      display: flex;
      flex-direction: column;
      gap: 5px;
      min-width: 0;
    }

    .school-badge {
      display: inline-flex;
      align-items: center;
      flex-wrap: wrap;
      gap: var(--space-2);
      font-size: 13px;
      font-weight: 600;
      color: #ffffff;
      background: linear-gradient(135deg, #185625 0%, #237433 100%);
      border: 1px solid rgba(255, 255, 255, 0.22);
      padding: 3.5px 12px;
      border-radius: 999px;
      width: fit-content;
      max-width: 100%;
      box-shadow: 0 2px 6px rgba(20, 60, 30, 0.18);
    }

    .app-title {
      margin: 0;
      font-size: clamp(20px, 2.6vw, 27px);
      font-weight: 700;
      letter-spacing: -0.015em;
      color: #0f3517;
      display: flex;
      flex-wrap: wrap;
      align-items: baseline;
      gap: 6px var(--space-3);
    }

    .app-title .ar-heading {
      font-family: var(--font-ar);
      font-size: clamp(19px, 2.5vw, 26px);
      font-weight: 700;
      color: var(--brand);
    }

    .header-meta {
      font-size: 13px;
      color: #1c3a23;
      background: rgba(255, 255, 255, 0.84);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(30, 102, 45, 0.2);
      box-shadow: 0 2px 8px rgba(20, 60, 30, 0.06);
      padding: 6px 14px;
      border-radius: 999px;
      display: flex;
      flex-wrap: wrap;
      gap: 4px var(--space-3);
      align-items: center;
    }

    /* Main Container */
    .main-container {
      max-width: 1280px;
      margin: 0 auto;
      padding: clamp(14px, 2.8vw, 24px) clamp(10px, 3vw, 24px) 40px;
      display: flex;
      flex-direction: column;
      gap: var(--space-5);
    }

    /* Mode Navigation & Filter Panel */
    .control-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow-sm);
      padding: clamp(12px, 2.5vw, 18px);
      display: flex;
      flex-direction: column;
      gap: var(--space-4);
    }

    .top-bar-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
    }

    .view-tabs {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      width: 100%;
      background: #ebf1ed;
      padding: 5px;
      border-radius: 12px;
      border: 1px solid #d5e0d8;
      gap: 5px;
    }

    .view-tabs .view-tab:first-child {
      grid-column: 1 / -1;
    }

    @media (min-width: 640px) {
      .view-tabs {
        display: inline-flex;
        flex-wrap: wrap;
        width: auto;
      }
      .view-tabs .view-tab:first-child {
        grid-column: auto;
      }
    }

    .view-tab {
      font: inherit;
      font-size: 14px;
      font-weight: 600;
      color: var(--ink-secondary);
      background: transparent;
      border: 1px solid transparent;
      padding: 9px 14px;
      min-height: 40px;
      border-radius: 9px;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 7px;
      text-align: center;
      transition: background 0.16s ease, color 0.16s ease, box-shadow 0.16s ease, transform 0.12s ease;
    }

    .view-tab svg {
      opacity: 0.78;
      flex-shrink: 0;
      transition: opacity 0.16s ease, transform 0.16s ease;
    }

    .view-tab:hover:not(.active) {
      color: var(--ink);
      background: rgba(255, 255, 255, 0.78);
    }

    .view-tab:hover svg {
      opacity: 1;
    }

    .view-tab:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 1px;
    }

    .view-tab.active {
      background: linear-gradient(135deg, #195926 0%, #227333 100%);
      color: #ffffff;
      border-color: rgba(255, 255, 255, 0.14);
      box-shadow: 0 3px 10px rgba(30, 102, 45, 0.28);
    }

    .view-tab.active svg {
      opacity: 1;
    }

    .search-status {
      font-size: 13.5px;
      color: var(--ink-secondary);
      background: var(--surface-subtle);
      border: 1px solid var(--border);
      padding: 6px 13px;
      border-radius: 999px;
      display: inline-flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 5px;
    }

    .search-status strong {
      color: var(--brand);
      font-weight: 700;
    }

    .filter-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: var(--space-3);
      padding-top: var(--space-1);
    }

    @media (min-width: 640px) {
      .filter-grid {
        grid-template-columns: repeat(2, 1fr);
      }
      .search-field-wrap {
        grid-column: span 2;
      }
    }

    @media (min-width: 1024px) {
      .filter-grid {
        grid-template-columns: 2fr 1.2fr 1fr 1.1fr 1fr 1fr;
      }
      .search-field-wrap {
        grid-column: span 1;
      }
    }

    .field {
      display: flex;
      flex-direction: column;
      gap: 6px;
      min-width: 0;
    }

    .field label {
      font-size: 12.5px;
      font-weight: 700;
      color: var(--ink-secondary);
      letter-spacing: 0.01em;
    }

    .input-wrap {
      position: relative;
      display: flex;
      align-items: center;
    }

    .input-icon {
      position: absolute;
      left: 12px;
      color: var(--muted);
      pointer-events: none;
      display: flex;
      align-items: center;
      transition: color 0.15s ease;
    }

    .input-wrap:focus-within .input-icon {
      color: var(--brand);
    }

    .text-input,
    .select-input {
      width: 100%;
      font: inherit;
      font-size: 14px;
      color: var(--ink);
      background-color: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-sm);
      padding: 8px 12px;
      min-height: 40px;
      box-shadow: var(--shadow-xs);
      transition: border-color 0.16s ease, box-shadow 0.16s ease, background-color 0.16s ease;
    }

    .select-input {
      appearance: none;
      -webkit-appearance: none;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 24 24' fill='none' stroke='%2347544c' stroke-width='2.2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpolyline points='6 9 12 15 18 9'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right 10px center;
      background-size: 15px 15px;
      padding-right: 34px;
      cursor: pointer;
    }

    #pageSizeSelect {
      padding-right: 30px !important;
    }

    .text-input:hover,
    .select-input:hover {
      border-color: var(--border-strong);
    }

    .text-input.has-icon {
      padding-left: 36px;
      padding-right: 32px;
    }

    .text-input:focus,
    .select-input:focus {
      outline: none;
      border-color: var(--brand);
      box-shadow: 0 0 0 3.5px rgba(30, 102, 45, 0.15);
    }

    .clear-input-btn {
      position: absolute;
      right: 7px;
      background: var(--bg);
      border: none;
      color: var(--muted);
      width: 24px;
      height: 24px;
      border-radius: 50%;
      cursor: pointer;
      display: none;
      align-items: center;
      justify-content: center;
      font-size: 15px;
      transition: background 0.14s ease, color 0.14s ease;
    }

    .clear-input-btn.visible {
      display: inline-flex;
    }

    .clear-input-btn:hover {
      background: #dce7df;
      color: var(--ink);
    }

    .active-filters-bar {
      display: none;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-2);
      padding-top: var(--space-3);
      border-top: 1px dashed var(--border);
    }

    .active-filters-bar.visible {
      display: flex;
    }

    .filter-chips {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
      align-items: center;
    }

    .filter-chip {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      font-size: 12.5px;
      font-weight: 600;
      background: var(--brand-soft);
      color: var(--brand);
      border: 1px solid var(--brand-border);
      padding: 4px 11px;
      border-radius: 999px;
      box-shadow: 0 1px 2px rgba(30, 102, 45, 0.06);
    }

    .filter-chip button {
      background: rgba(30, 102, 45, 0.12);
      border: none;
      color: var(--brand);
      width: 17px;
      height: 17px;
      border-radius: 50%;
      cursor: pointer;
      padding: 0;
      font-size: 13px;
      line-height: 1;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      transition: background 0.14s ease;
    }

    .filter-chip button:hover {
      background: rgba(30, 102, 45, 0.24);
    }

    .btn {
      font: inherit;
      font-size: 13.5px;
      font-weight: 600;
      padding: 8px 15px;
      border-radius: var(--radius-sm);
      border: 1px solid var(--border);
      background: linear-gradient(180deg, #ffffff 0%, #f8faf8 100%);
      color: var(--ink);
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      box-shadow: var(--shadow-xs);
      transition: background 0.15s ease, border-color 0.15s ease, box-shadow 0.15s ease, transform 0.12s ease;
    }

    .btn:hover:not(:disabled) {
      background: #ffffff;
      border-color: var(--border-strong);
      box-shadow: var(--shadow-sm);
      transform: translateY(-1px);
    }

    .btn:active:not(:disabled) {
      transform: translateY(0);
    }

    .btn:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 2px;
    }

    .btn:disabled {
      opacity: 0.42;
      cursor: not-allowed;
      box-shadow: none;
    }

    .btn-ghost-danger {
      color: #b42318;
      border-color: #fecdca;
      background: #fef3f2;
    }

    .btn-ghost-danger:hover:not(:disabled) {
      background: #fee4e2;
      border-color: #fda29b;
    }

    /* Split Layout for Teacher & Class Timetable Views */
    .workspace-split {
      display: grid;
      grid-template-columns: 1fr;
      gap: var(--space-4);
      align-items: start;
      animation: viewFadeIn 0.2s ease-out;
    }

    @media (min-width: 960px) {
      .workspace-split {
        grid-template-columns: 296px minmax(0, 1fr);
      }
    }

    .directory-panel {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow-sm);
      overflow: hidden;
      display: flex;
      flex-direction: column;
    }

    .directory-header {
      padding: var(--space-4);
      background: linear-gradient(180deg, #ffffff 0%, #f5f9f6 100%);
      border-bottom: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .directory-title-row {
      display: flex;
      align-items: center;
      justify-content: space-between;
      font-size: 14px;
      font-weight: 700;
      color: var(--ink);
    }

    .directory-list {
      max-height: 560px;
      overflow-y: auto;
      padding: 8px;
      display: flex;
      flex-direction: column;
      gap: 3px;
    }

    .dir-item {
      width: 100%;
      text-align: left;
      font: inherit;
      background: transparent;
      border: 1px solid transparent;
      border-radius: var(--radius-sm);
      padding: 9px 11px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-2);
      transition: background 0.14s ease, border-color 0.14s ease, transform 0.12s ease;
    }

    .dir-item:hover:not(.active) {
      background: var(--surface-subtle);
      border-color: #e4ece6;
    }

    .dir-item:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: -2px;
    }

    .dir-item.active {
      background: var(--brand-soft);
      border-color: var(--brand-border);
      box-shadow: inset 3px 0 0 var(--brand);
    }

    .dir-item-main {
      display: flex;
      align-items: center;
      gap: 9px;
      min-width: 0;
    }

    .dir-num {
      font-size: 11.5px;
      font-weight: 700;
      color: var(--ink-secondary);
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: 6px;
      padding: 1.5px 6.5px;
      flex-shrink: 0;
      font-variant-numeric: tabular-nums;
    }

    .dir-item.active .dir-num {
      background: var(--brand);
      color: #ffffff;
      border-color: var(--brand);
    }

    .dir-name {
      font-size: 15.5px;
      font-weight: 600;
      color: var(--ink);
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
    }

    .dir-meta {
      font-size: 12px;
      font-weight: 600;
      color: var(--muted);
      background: rgba(20, 45, 27, 0.04);
      padding: 2px 7px;
      border-radius: 999px;
      flex-shrink: 0;
      font-variant-numeric: tabular-nums;
    }

    /* Timetable Sheet Card */
    .timetable-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow);
      overflow: hidden;
      animation: viewFadeIn 0.2s ease-out;
    }

    .tt-card-top {
      padding: var(--space-4) var(--space-5);
      border-bottom: 1px solid var(--border);
      background: linear-gradient(180deg, #ffffff 0%, #f5f9f6 100%);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
    }

    .tt-identity {
      display: flex;
      flex-direction: column;
      gap: 3px;
    }

    .tt-institution-sub {
      font-size: 13.5px;
      color: var(--muted);
      font-weight: 600;
    }

    .tt-main-heading {
      margin: 0;
      font-size: 22px;
      font-weight: 700;
      color: var(--ink);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 10px;
    }

    .page-pill {
      font-family: var(--font-ui);
      font-size: 12.5px;
      font-weight: 700;
      background: var(--accent-gold-soft);
      color: #78520d;
      border: 1px solid var(--accent-gold);
      padding: 3px 11px;
      border-radius: 999px;
      box-shadow: 0 1px 2px rgba(180, 130, 40, 0.1);
    }

    .tt-nav-controls {
      display: flex;
      align-items: center;
      gap: var(--space-2);
    }

    .tt-scroll-wrap {
      overflow-x: auto;
      padding: var(--space-4) var(--space-5);
      background: #fcfdfc;
    }

    /* Authentic FET-inspired Timetable Grid with Modern Polish */
    .fet-grid {
      width: 100%;
      min-width: 680px;
      border-collapse: separate;
      border-spacing: 4px;
      background: #e9eeea;
      border: 1.5px solid #95a499;
      border-radius: 12px;
      padding: 4px;
      table-layout: fixed;
      box-shadow: inset 0 1px 3px rgba(15, 32, 20, 0.06);
    }

    .fet-grid th,
    .fet-grid td {
      border: 1px solid #cdd6cf;
      border-radius: 7px;
      text-align: center;
      vertical-align: middle;
    }

    .fet-grid thead th {
      background: linear-gradient(180deg, #ffffff 0%, #f4f8f5 100%);
      color: var(--ink);
      padding: 11px 6px;
      font-weight: 700;
      font-size: 13.5px;
      border-bottom: 2px solid #95a499;
    }

    .fet-grid thead th.corner-cell {
      width: 118px;
      background: #eef4f0;
      color: var(--ink-secondary);
      font-size: 12.5px;
    }

    .period-num-label {
      display: inline-block;
      font-size: 11.5px;
      font-weight: 700;
      color: var(--brand);
      background: var(--brand-soft);
      padding: 1px 8px;
      border-radius: 999px;
      margin-bottom: 3px;
    }

    .period-time-label {
      display: block;
      font-variant-numeric: tabular-nums;
      letter-spacing: -0.01em;
      color: var(--ink-secondary);
    }

    .fet-grid tbody th.day-header {
      background: linear-gradient(90deg, #f7faf8 0%, #ffffff 100%);
      padding: 10px 8px;
      width: 118px;
      border-right: 2px solid #b5c3b9;
    }

    .day-ar {
      display: block;
      font-family: var(--font-ar);
      font-size: 18px;
      font-weight: 700;
      color: var(--ink);
      line-height: 1.3;
    }

    .day-th {
      display: block;
      font-size: 12px;
      font-weight: 600;
      color: var(--muted);
      margin-top: 2px;
    }

    .tt-cell {
      height: 76px;
      padding: 6px 8px;
      background: #ffffff;
      position: relative;
      transition: transform 0.14s ease, box-shadow 0.14s ease, opacity 0.15s ease;
    }

    .tt-cell.free-slot {
      background: #ffffff;
      color: #a3afa7;
      font-size: 14px;
      letter-spacing: 2px;
    }

    .tt-cell.unavail-slot {
      background: repeating-linear-gradient(
        -45deg,
        #f2f5f3,
        #f2f5f3 6px,
        #eaeeea 6px,
        #eaeeea 12px
      );
      color: #758279;
      font-size: 13px;
      font-weight: 700;
    }

    .tt-cell.lesson-slot {
      cursor: pointer;
      border-color: rgba(0, 0, 0, 0.16);
      box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.28), 0 1px 2px rgba(0, 0, 0, 0.06);
    }

    .tt-cell.lesson-slot:hover {
      transform: translateY(-2px);
      box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.35), 0 7px 16px rgba(15, 28, 19, 0.18);
      z-index: 2;
    }

    .tt-cell.dimmed {
      opacity: 0.26;
      filter: grayscale(35%);
    }

    .tt-cell.matched-highlight {
      outline: 3px solid #17211b;
      outline-offset: -2px;
      box-shadow: 0 0 0 2.5px var(--accent-gold), 0 6px 14px rgba(0, 0, 0, 0.16);
      z-index: 3;
    }

    .cell-top-line {
      font-family: var(--font-ar);
      font-size: 16px;
      font-weight: 700;
      line-height: 1.25;
      margin-bottom: 2px;
    }

    .cell-bottom-line {
      font-family: var(--font-ar);
      font-size: 15.5px;
      font-weight: 600;
      line-height: 1.35;
    }

    .cell-span-tag {
      display: inline-block;
      margin-top: 3px;
      font-family: var(--font-ui);
      font-size: 10.5px;
      font-weight: 700;
      padding: 1.5px 7px;
      border-radius: 999px;
      background: rgba(0, 0, 0, 0.2);
      color: inherit;
    }

    .tt-footer {
      padding: var(--space-3) var(--space-5);
      border-top: 1px solid var(--border);
      background: var(--surface-subtle);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
      font-size: 12.5px;
      color: var(--muted);
    }

    .tt-legend {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: var(--space-4);
    }

    .legend-item {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      font-weight: 500;
      color: var(--ink-secondary);
    }

    .legend-box {
      width: 22px;
      height: 16px;
      border-radius: 4px;
      border: 1px solid var(--grid-border);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-size: 9.5px;
      font-weight: 700;
    }

    /* Data Explorer Table View */
    .table-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow-sm);
      overflow: hidden;
      animation: viewFadeIn 0.2s ease-out;
    }

    .table-scroll {
      overflow-x: auto;
    }

    .explorer-table {
      width: 100%;
      border-collapse: collapse;
      min-width: 780px;
    }

    .explorer-table thead th {
      background: linear-gradient(180deg, #f9fbf9 0%, #f0f5f1 100%);
      border-bottom: 1.5px solid var(--border);
      padding: 12px 15px;
      text-align: left;
      font-size: 13px;
      font-weight: 700;
      color: var(--ink-secondary);
      white-space: nowrap;
      user-select: none;
    }

    .explorer-table thead th.sortable {
      cursor: pointer;
      transition: background 0.14s ease, color 0.14s ease;
    }

    .explorer-table thead th.sortable:hover {
      background: #e6f0e8;
      color: var(--brand);
    }

    .explorer-table thead th.sorted {
      color: var(--brand);
      background: #eaf4ec;
    }

    .explorer-table thead th.num-col,
    .explorer-table tbody td.num-col {
      text-align: right;
      font-variant-numeric: tabular-nums;
    }

    .sort-ind {
      display: inline-block;
      margin-left: 4px;
      font-size: 11.5px;
      color: var(--muted);
    }

    .explorer-table thead th.sorted .sort-ind {
      color: var(--brand);
      font-weight: 800;
    }

    .explorer-table tbody tr {
      border-bottom: 1px solid #ebf0ec;
      cursor: pointer;
      transition: background 0.12s ease;
    }

    .explorer-table tbody tr:nth-child(even) {
      background: #fbfdfb;
    }

    .explorer-table tbody tr:hover {
      background: #edf7ef;
    }

    .explorer-table tbody td {
      padding: 12px 15px;
      vertical-align: middle;
      font-size: 14px;
    }

    .cls-badge {
      display: inline-flex;
      align-items: center;
      gap: 7px;
      font-family: var(--font-ar);
      font-weight: 700;
      font-size: 15px;
      padding: 2.5px 11px;
      border-radius: 8px;
      background: #ffffff;
      border: 1px solid var(--border);
      color: var(--ink);
      box-shadow: var(--shadow-xs);
    }

    .swatch-dot {
      width: 11px;
      height: 11px;
      border-radius: 50%;
      border: 1px solid rgba(0, 0, 0, 0.22);
      flex-shrink: 0;
    }

    .subj-cell-wrap {
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .period-pill {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      font-size: 13px;
      font-weight: 500;
      font-variant-numeric: tabular-nums;
      color: var(--ink-secondary);
      background: var(--surface-tinted);
      border: 1px solid #dfeae2;
      padding: 3px 10px;
      border-radius: 999px;
    }

    .pagination-bar {
      padding: var(--space-3) var(--space-5);
      background: var(--surface-subtle);
      border-top: 1px solid var(--border);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
      font-size: 13.5px;
      color: var(--ink-secondary);
    }

    .page-controls {
      display: flex;
      align-items: center;
      gap: var(--space-2);
    }

    /* Empty State */
    .empty-state {
      padding: 52px 24px;
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: var(--space-3);
    }

    .empty-icon {
      width: 54px;
      height: 54px;
      border-radius: 50%;
      background: var(--brand-soft);
      border: 1px solid var(--brand-border);
      color: var(--brand);
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 12px rgba(30, 102, 45, 0.1);
    }

    .empty-state h3 {
      margin: 0;
      font-size: 17.5px;
      color: var(--ink);
    }

    .empty-state p {
      margin: 0;
      font-size: 14px;
      color: var(--muted);
      max-width: 420px;
    }

    /* Modal for Quick Timetable Inspection from Table Row */
    .modal-backdrop {
      position: fixed;
      inset: 0;
      background: rgba(12, 24, 16, 0.58);
      backdrop-filter: blur(4px);
      display: none;
      align-items: center;
      justify-content: center;
      padding: var(--space-4);
      z-index: 100;
    }

    .modal-backdrop.open {
      display: flex;
    }

    .modal-dialog {
      background: var(--surface);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow-lg);
      width: 100%;
      max-width: 1000px;
      max-height: 90vh;
      display: flex;
      flex-direction: column;
      overflow: hidden;
      border: 1px solid var(--border);
      animation: modalSlideUp 0.2s ease-out;
    }

    .modal-body {
      overflow-y: auto;
    }

    /* Substitute / Free Teacher Finder View */
    .sub-controls-bar {
      padding: var(--space-4) var(--space-5);
      background: linear-gradient(180deg, #ffffff 0%, #f5f9f6 100%);
      border-bottom: 1px solid var(--border);
      display: flex;
      flex-direction: column;
      gap: var(--space-3);
    }

    .sub-picker-group {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: var(--space-2);
    }

    .sub-picker-label {
      font-size: 13px;
      font-weight: 700;
      color: var(--ink-secondary);
      min-width: 96px;
    }

    .pill-btn-row {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
    }

    .slot-pill-btn {
      font: inherit;
      font-size: 13px;
      font-weight: 600;
      padding: 6.5px 13px;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: var(--surface);
      color: var(--ink-secondary);
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 5px;
      box-shadow: var(--shadow-xs);
      transition: background 0.14s ease, border-color 0.14s ease, color 0.14s ease, transform 0.12s ease, box-shadow 0.14s ease;
    }

    .slot-pill-btn:hover:not(.active) {
      border-color: var(--brand);
      background: var(--brand-soft);
      color: var(--brand);
      transform: translateY(-1px);
    }

    .slot-pill-btn:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 1px;
    }

    .slot-pill-btn.active {
      background: linear-gradient(135deg, #195926 0%, #237433 100%);
      border-color: var(--brand);
      color: #ffffff;
      box-shadow: 0 3px 8px rgba(30, 102, 45, 0.25);
    }

    .sub-context-note {
      font-size: 13.5px;
      color: #593d08;
      background: var(--accent-gold-soft);
      border: 1px solid var(--accent-gold);
      border-radius: var(--radius-sm);
      padding: 9px 14px;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 8px;
    }

    .day-mini-track {
      display: inline-grid;
      grid-template-columns: repeat(5, 36px);
      gap: 4px;
      vertical-align: middle;
    }

    .mini-slot {
      height: 25px;
      border-radius: 5px;
      font-size: 11px;
      font-weight: 700;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      border: 1px solid var(--border);
      font-variant-numeric: tabular-nums;
    }

    .mini-slot.is-target-free {
      background: var(--brand-soft);
      border-color: var(--brand);
      color: var(--brand);
      box-shadow: 0 0 0 1px var(--brand);
    }

    .mini-slot.is-free {
      background: #ffffff;
      color: var(--muted);
    }

    .mini-slot.is-busy {
      background: #edf2ee;
      color: var(--ink);
      border-color: #c2cfc5;
    }

    .mini-slot.is-unavail {
      background: #f3f5f4;
      color: #96a29a;
      border-style: dashed;
    }

    .subj-tag-list {
      display: flex;
      flex-wrap: wrap;
      gap: 5px;
    }

    .subj-mini-tag {
      font-family: var(--font-ar);
      font-size: 14px;
      font-weight: 600;
      background: var(--surface-subtle);
      border: 1px solid var(--border);
      color: var(--ink);
      padding: 1.5px 9px;
      border-radius: 7px;
    }

    .subj-mini-tag.matched {
      background: var(--brand-soft);
      border-color: var(--brand-border);
      color: var(--brand);
    }

    /* Self-Service Teacher Lookup View */
    .self-lookup-wrap {
      display: flex;
      flex-direction: column;
      gap: var(--space-4);
      animation: viewFadeIn 0.2s ease-out;
    }

    .self-hero-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-top: 3.5px solid var(--brand);
      border-radius: var(--radius-lg);
      box-shadow: var(--shadow);
      padding: var(--space-6);
      display: flex;
      flex-direction: column;
      gap: var(--space-4);
    }

    .self-hero-head {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
      padding-bottom: var(--space-3);
      border-bottom: 1px solid #ebf0ec;
    }

    .self-hero-head h2 {
      margin: 0;
      font-size: 21px;
      font-weight: 700;
      color: #103819;
      letter-spacing: -0.01em;
    }

    .self-hero-head p {
      margin: 4px 0 0;
      font-size: 14px;
      color: var(--muted);
    }

    .self-search-row {
      display: grid;
      grid-template-columns: 1fr;
      gap: var(--space-4);
    }

    @media (min-width: 768px) {
      .self-search-row {
        grid-template-columns: 1.45fr 1fr;
      }
    }

    .self-input-lg {
      min-height: 48px;
      font-size: 15.5px;
      border-width: 1.5px;
      border-radius: 11px;
      background-color: #fcfdfc;
    }

    .self-input-lg:focus {
      background-color: #ffffff;
    }

    .self-teacher-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(228px, 1fr));
      gap: 10px;
      max-height: 356px;
      overflow-y: auto;
      padding: 6px 4px;
    }

    .self-teacher-btn {
      font: inherit;
      text-align: left;
      background: linear-gradient(180deg, #ffffff 0%, #f9fbf9 100%);
      border: 1px solid #dbe4dd;
      border-radius: 12px;
      padding: 11px 13px;
      cursor: pointer;
      display: flex;
      flex-direction: column;
      align-items: stretch;
      gap: 4px;
      box-shadow: var(--shadow-xs);
      transition: background 0.15s ease, border-color 0.15s ease, transform 0.14s ease, box-shadow 0.15s ease;
    }

    .self-teacher-btn-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 8px;
      width: 100%;
    }

    .self-teacher-sub {
      font-size: 13.5px;
      color: var(--muted);
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      padding-left: 36px;
    }

    .self-teacher-btn:hover:not(.active) {
      background: #f2f9f4;
      border-color: #9ecba9;
      transform: translateY(-2px);
      box-shadow: 0 6px 14px rgba(24, 78, 35, 0.09);
    }

    .self-teacher-btn:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 1px;
    }

    .self-teacher-btn.active {
      background: linear-gradient(135deg, #195926 0%, #237433 100%);
      border-color: var(--brand);
      color: #ffffff;
      box-shadow: 0 6px 16px rgba(30, 102, 45, 0.26);
    }

    .self-teacher-btn.active .dir-name,
    .self-teacher-btn.active .dir-meta,
    .self-teacher-btn.active .self-teacher-sub {
      color: #ffffff;
    }

    .self-teacher-btn.active .dir-meta {
      background: rgba(255, 255, 255, 0.18);
    }

    .self-teacher-btn.active .dir-num {
      background: rgba(255, 255, 255, 0.22);
      color: #ffffff;
      border-color: transparent;
    }

    .quick-letter-wrap {
      display: flex;
      flex-direction: column;
      gap: 8px;
      background: var(--surface-subtle);
      border: 1px solid #e3ebe5;
      border-radius: 12px;
      padding: 11px 14px;
    }

    .quick-letter-label {
      font-size: 12.5px;
      font-weight: 700;
      color: var(--ink-secondary);
    }

    .quick-letter-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      align-items: center;
    }

    .letter-pill {
      font: inherit;
      min-width: 38px;
      height: 36px;
      padding: 0 11px;
      border-radius: 9px;
      border: 1px solid var(--border);
      background: #ffffff;
      color: var(--ink);
      font-weight: 700;
      font-size: 14px;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 1px 2px rgba(16, 38, 22, 0.04);
      transition: background 0.14s ease, border-color 0.14s ease, color 0.14s ease, transform 0.12s ease, box-shadow 0.14s ease;
    }

    .letter-pill.ar-letter {
      font-family: var(--font-ar);
      font-size: 19px;
      line-height: 1;
    }

    .letter-pill:hover:not(.active) {
      border-color: var(--brand);
      background: var(--brand-soft);
      color: var(--brand);
      transform: translateY(-1px);
    }

    .letter-pill:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 1px;
    }

    .letter-pill.active {
      background: linear-gradient(135deg, #195926 0%, #237433 100%);
      border-color: var(--brand);
      color: #ffffff;
      box-shadow: 0 3px 8px rgba(30, 102, 45, 0.25);
    }

    .self-selected-banner {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
      padding: 12px 16px;
      border-radius: 12px;
      background: linear-gradient(90deg, #eaf5ed 0%, #f4faf6 100%);
      border: 1px solid var(--brand-border);
      font-size: 14.5px;
      color: var(--ink);
    }

    .self-day-filter-bar {
      padding: var(--space-3) var(--space-5);
      background: #ffffff;
      border-bottom: 1px solid var(--border);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: var(--space-2);
    }

    .daily-cards-wrap {
      padding: var(--space-4) var(--space-5);
      display: flex;
      flex-direction: column;
      gap: 10px;
      background: #fbfdfb;
    }

    .daily-slot-row {
      display: grid;
      grid-template-columns: 150px minmax(0, 1fr);
      gap: var(--space-3);
      align-items: center;
      padding: 12px 16px;
      border-radius: 12px;
      border: 1px solid var(--border);
      border-left: 4px solid var(--brand-border);
      background: var(--surface);
      box-shadow: var(--shadow-xs);
    }

    @media (max-width: 520px) {
      .daily-slot-row {
        grid-template-columns: 1fr;
        gap: 8px;
      }
    }

    .daily-slot-time {
      display: flex;
      flex-direction: column;
      gap: 3px;
      align-items: flex-start;
    }

    .daily-slot-badge {
      padding: 11px 16px;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-3);
      border: 1px solid rgba(0, 0, 0, 0.15);
      cursor: pointer;
      box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.25), 0 2px 5px rgba(0, 0, 0, 0.06);
      transition: transform 0.14s ease, box-shadow 0.14s ease;
    }

    .daily-slot-badge:hover {
      transform: translateY(-2px);
      box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.35), 0 6px 14px rgba(0, 0, 0, 0.14);
    }

    /* Cross-Device Responsive Enhancements (Phones, Tablets, Desktops) */
    .workspace-split > *,
    .timetable-card,
    .table-card,
    .self-hero-card {
      min-width: 0;
    }

    .tt-scroll-wrap,
    .table-scroll {
      -webkit-overflow-scrolling: touch;
      overscroll-behavior-x: contain;
    }

    @media (max-width: 959px) {
      .directory-list {
        max-height: 220px;
      }
    }

    @media (max-width: 767px) {
      .text-input,
      .select-input {
        font-size: 16px;
        min-height: 44px;
      }

      .btn {
        min-height: 40px;
      }

      .slot-pill-btn {
        min-height: 38px;
        padding: 7px 13px;
      }

      .letter-pill {
        min-width: 40px;
        height: 40px;
      }

      .self-hero-card {
        padding: var(--space-4);
      }

      .tt-card-top {
        padding: var(--space-3) var(--space-4);
      }

      .tt-main-heading {
        font-size: 19px;
      }

      .tt-scroll-wrap {
        padding: var(--space-3);
      }

      .tt-footer,
      .self-day-filter-bar,
      .daily-cards-wrap {
        padding-left: var(--space-4);
        padding-right: var(--space-4);
      }

      .fet-grid {
        min-width: 560px;
      }

      .fet-grid thead th.corner-cell,
      .fet-grid tbody th.day-header {
        width: 92px;
        padding: 8px 4px;
      }

      .tt-cell {
        height: 68px;
        padding: 5px 6px;
      }
    }

    @media (max-width: 639px) {
      .search-status {
        width: 100%;
        justify-content: center;
      }

      .tt-nav-controls {
        width: 100%;
      }

      .tt-nav-controls .btn {
        flex: 1 1 auto;
        justify-content: center;
      }

      .pagination-bar {
        flex-direction: column;
        align-items: stretch;
        text-align: center;
      }

      .page-controls {
        justify-content: center;
        flex-wrap: wrap;
      }

      .self-teacher-grid {
        grid-template-columns: 1fr;
        max-height: 290px;
      }

      .quick-letter-row,
      .self-day-filter-bar .pill-btn-row,
      .sub-picker-group .pill-btn-row {
        flex-wrap: nowrap;
        overflow-x: auto;
        -webkit-overflow-scrolling: touch;
        max-width: 100%;
        padding-bottom: 4px;
      }

      .quick-letter-row > *,
      .self-day-filter-bar .pill-btn-row > *,
      .sub-picker-group .pill-btn-row > * {
        flex-shrink: 0;
      }

      .sub-picker-group {
        flex-direction: column;
        align-items: flex-start;
      }

      .modal-backdrop {
        align-items: flex-end;
        padding: 0;
      }

      .modal-dialog {
        max-width: 100%;
        max-height: 92vh;
        max-height: 92dvh;
        border-radius: var(--radius-lg) var(--radius-lg) 0 0;
        border-bottom: none;
      }
    }

    /* Multi-Language (Thai / Arabic / Jawi) & Gradient Themes */
    :root,
    html[data-theme="emerald"] {
      --brand: #1E662D;
      --brand-hover: #154d21;
      --brand-soft: #e6f4ea;
      --brand-border: #add8b7;
      --brand-grad: linear-gradient(135deg, #165322 0%, #1E662D 52%, #2c8a40 100%);
      --header-grad: linear-gradient(125deg, #ffffff 0%, #f0faf3 34%, #cbead4 68%, #8bd1a0 100%);
      --page-grad: linear-gradient(160deg, #e8f5ec 0%, #f4f8f5 42%, #eef5f0 100%);
      --card-grad: linear-gradient(180deg, #ffffff 0%, #fafdfb 100%);
      --title-ink: #0f3517;
    }

    html[data-theme="sapphire"] {
      --bg: #eef3fb;
      --surface-subtle: #f5f8fd;
      --surface-tinted: #eaf1fb;
      --border: #cfdceb;
      --border-strong: #b0c4de;
      --brand: #1d4ed8;
      --brand-hover: #1e40af;
      --brand-soft: #e6effe;
      --brand-border: #b3ccfb;
      --brand-grad: linear-gradient(135deg, #1e3a8a 0%, #1d4ed8 55%, #3b82f6 100%);
      --header-grad: linear-gradient(125deg, #ffffff 0%, #eff5ff 34%, #cfe1fd 68%, #98befa 100%);
      --page-grad: linear-gradient(160deg, #e4eefc 0%, #f3f7fc 42%, #edf3fb 100%);
      --card-grad: linear-gradient(180deg, #ffffff 0%, #f9fbff 100%);
      --title-ink: #12295d;
    }

    html[data-theme="teal"] {
      --bg: #edf6f5;
      --surface-subtle: #f4faf9;
      --surface-tinted: #e7f5f3;
      --border: #cce0de;
      --border-strong: #adcac7;
      --brand: #0f766e;
      --brand-hover: #115e59;
      --brand-soft: #e2f6f4;
      --brand-border: #a3ded8;
      --brand-grad: linear-gradient(135deg, #115e59 0%, #0f766e 52%, #14b8a6 100%);
      --header-grad: linear-gradient(125deg, #ffffff 0%, #edfaf8 34%, #c4ece7 68%, #84d8ce 100%);
      --page-grad: linear-gradient(160deg, #e2f5f2 0%, #f2f9f8 42%, #ebf5f4 100%);
      --card-grad: linear-gradient(180deg, #ffffff 0%, #f9fdfd 100%);
      --title-ink: #0c3b37;
    }

    html[data-theme="amber"] {
      --bg: #faf5ec;
      --surface-subtle: #fdfaf4;
      --surface-tinted: #f8f0e2;
      --border: #e6dac4;
      --border-strong: #d4c2a2;
      --brand: #9a5812;
      --brand-hover: #7c440b;
      --brand-soft: #fef3de;
      --brand-border: #f3d299;
      --brand-grad: linear-gradient(135deg, #7c430a 0%, #a35e14 54%, #ca8a2e 100%);
      --header-grad: linear-gradient(125deg, #ffffff 0%, #fefaf0 34%, #f7e4bc 68%, #ecc983 100%);
      --page-grad: linear-gradient(160deg, #f9efdc 0%, #fcf9f2 42%, #f7f1e6 100%);
      --card-grad: linear-gradient(180deg, #ffffff 0%, #fffdf9 100%);
      --title-ink: #472806;
    }

    body {
      background-image: var(--page-grad);
      background-attachment: fixed;
    }

    .app-header {
      background-image:
        url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='80' height='80' viewBox='0 0 80 80'%3E%3Cg fill='none' stroke='%231E662D' stroke-linejoin='round'%3E%3Cpath d='M40 0L48 16L64 16L64 32L80 40L64 48L64 64L48 64L40 80L32 64L16 64L16 48L0 40L16 32L16 16L32 16Z' stroke-opacity='0.12' stroke-width='1.2'/%3E%3Cpath d='M0 16L16 16L16 0M64 0L64 16L80 16M80 64L64 64L64 80M16 80L16 64L0 64M0 24L11 11L24 0M56 0L69 11L80 24M80 56L69 69L56 80M24 80L11 69L0 56' stroke-opacity='0.09' stroke-width='1'/%3E%3Cpath d='M40 19L61 40L40 61L19 40Z' fill='%23E6BD72' fill-opacity='0.14' stroke-opacity='0.16' stroke-width='1.15'/%3E%3Cpath d='M25.2 25.2H54.8V54.8H25.2Z' fill='%231E662D' fill-opacity='0.03' stroke-opacity='0.16' stroke-width='1.15'/%3E%3Ccircle cx='40' cy='40' r='5.5' stroke='%23C59638' stroke-opacity='0.24' stroke-width='1'/%3E%3C/g%3E%3C/svg%3E"),
        radial-gradient(circle at 18% 25%, rgba(255, 255, 255, 0.94) 0%, rgba(255, 255, 255, 0) 56%),
        var(--header-grad);
    }

    .app-title,
    .self-hero-head h2 {
      color: var(--title-ink);
    }

    .control-card,
    .self-hero-card,
    .timetable-card,
    .table-card,
    .directory-panel {
      background: var(--card-grad);
    }

    .school-badge,
    .view-tab.active,
    .slot-pill-btn.active,
    .letter-pill.active,
    .self-teacher-btn.active,
    .lang-btn.active {
      background: var(--brand-grad);
    }

    .header-right-stack {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      gap: 8px;
    }

    .header-prefs-bar {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: flex-end;
      gap: 8px;
    }

    @media (max-width: 767px) {
      .header-right-stack {
        width: 100%;
        align-items: stretch;
      }
      .header-prefs-bar {
        justify-content: space-between;
      }
    }

    .lang-switcher,
    .theme-switcher {
      display: inline-flex;
      align-items: center;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(20, 45, 28, 0.16);
      border-radius: 999px;
      padding: 3px;
      gap: 3px;
      box-shadow: 0 2px 8px rgba(16, 38, 22, 0.07);
      direction: ltr;
    }

    .theme-switcher {
      padding: 4px 8px;
      gap: 6px;
    }

    .theme-label {
      font-size: 12px;
      font-weight: 700;
      color: var(--ink-secondary);
      padding: 0 4px;
      white-space: nowrap;
    }

    html[dir="rtl"] .theme-label {
      font-family: var(--font-ar);
      font-size: 14.5px;
    }

    .theme-swatch-btn {
      width: 24px;
      height: 24px;
      border-radius: 50%;
      border: 2px solid #ffffff;
      box-shadow: 0 0 0 1px rgba(0, 0, 0, 0.18);
      cursor: pointer;
      padding: 0;
      transition: transform 0.15s ease, box-shadow 0.15s ease;
    }

    .theme-swatch-btn:hover {
      transform: scale(1.12);
    }

    .theme-swatch-btn:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 2px;
    }

    .theme-swatch-btn.active {
      transform: scale(1.14);
      box-shadow: 0 0 0 2.5px var(--brand);
    }

    .theme-swatch-emerald {
      background: linear-gradient(135deg, #1E662D 0%, #93d5a7 65%, #E6BD72 100%);
    }

    .theme-swatch-sapphire {
      background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 65%, #dbeafe 100%);
    }

    .theme-swatch-teal {
      background: linear-gradient(135deg, #115e59 0%, #14b8a6 65%, #ccfbf1 100%);
    }

    .theme-swatch-amber {
      background: linear-gradient(135deg, #7c430a 0%, #d99b38 65%, #fef3c7 100%);
    }

    .lang-btn {
      font: inherit;
      font-size: 13px;
      font-weight: 700;
      color: var(--ink-secondary);
      background: transparent;
      border: none;
      border-radius: 999px;
      padding: 5px 12px;
      min-height: 32px;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      line-height: 1.2;
      transition: background 0.15s ease, color 0.15s ease, box-shadow 0.15s ease;
    }

    .lang-btn.ar-lang-font {
      font-family: var(--font-ar);
      font-size: 16px;
      padding: 4px 13px;
    }

    .lang-btn:hover:not(.active) {
      background: var(--brand-soft);
      color: var(--brand);
    }

    .lang-btn:focus-visible {
      outline: 2px solid var(--brand);
      outline-offset: 1px;
    }

    .lang-btn.active {
      color: #ffffff;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.18);
    }

    .ltr-token {
      direction: ltr;
      unicode-bidi: isolate;
      display: inline-block;
    }

    html[dir="rtl"] body {
      font-family: var(--font-ar);
      font-size: 17px;
    }

    html[dir="rtl"] .field label,
    html[dir="rtl"] .quick-letter-label,
    html[dir="rtl"] .sub-picker-label,
    html[dir="rtl"] .directory-title-row {
      font-size: 15px;
    }

    html[dir="rtl"] .view-tab,
    html[dir="rtl"] .btn,
    html[dir="rtl"] .slot-pill-btn {
      font-size: 15.5px;
    }

    html[dir="rtl"] .text-input,
    html[dir="rtl"] .select-input {
      font-size: 16px;
    }

    html[dir="rtl"] .input-icon {
      left: auto;
      right: 12px;
    }

    html[dir="rtl"] .clear-input-btn {
      right: auto;
      left: 7px;
    }

    html[dir="rtl"] .text-input.has-icon {
      padding-left: 32px;
      padding-right: 36px;
    }

    html[dir="rtl"] .select-input {
      background-position: left 10px center;
      padding-right: 12px;
      padding-left: 34px;
    }

    html[dir="rtl"] #pageSizeSelect {
      padding-right: 10px !important;
      padding-left: 30px !important;
    }

    html[dir="rtl"] .dir-item,
    html[dir="rtl"] .self-teacher-btn,
    html[dir="rtl"] .explorer-table thead th,
    html[dir="rtl"] .explorer-table tbody td {
      text-align: right;
    }

    html[dir="rtl"] .explorer-table thead th.num-col,
    html[dir="rtl"] .explorer-table tbody td.num-col {
      text-align: left;
    }

    html[dir="rtl"] .sort-ind {
      margin-left: 0;
      margin-right: 4px;
    }

    html[dir="rtl"] .dir-item.active {
      box-shadow: inset -3px 0 0 var(--brand);
    }

    html[dir="rtl"] .self-teacher-sub {
      padding-left: 0;
      padding-right: 36px;
    }

    html[dir="rtl"] .daily-slot-row {
      border-left: 1px solid var(--border);
      border-right: 4px solid var(--brand-border);
    }

    html[dir="rtl"] .fet-grid tbody th.day-header {
      border-right: 1px solid #cdd6cf;
      border-left: 2px solid #b5c3b9;
    }

    /* Academic Affairs Timetable Editor */
    .view-tabs.six-tabs .view-tab:first-child { grid-column: auto; }
    .btn-primary { background: var(--brand-grad); color: #ffffff; border-color: var(--brand); box-shadow: 0 2px 6px rgba(20, 60, 30, 0.2); }
    .btn-primary:hover:not(:disabled) { background: var(--brand-grad); filter: brightness(1.06); color: #ffffff; }
    .manage-top-bar { padding: var(--space-4) var(--space-5); border-bottom: 1px solid var(--border); background: linear-gradient(180deg, #ffffff 0%, var(--surface-subtle) 100%); display: flex; flex-wrap: wrap; align-items: flex-end; justify-content: space-between; gap: var(--space-3); }
    .manage-teacher-picker { display: flex; flex-wrap: wrap; align-items: flex-end; gap: var(--space-2); flex: 1 1 320px; }
    .manage-teacher-picker .field { flex: 1 1 230px; max-width: 360px; }
    .manage-actions-group { display: flex; flex-wrap: wrap; align-items: center; gap: var(--space-2); }
    .manage-hint-bar { padding: 10px var(--space-5); background: var(--brand-soft); border-bottom: 1px solid var(--brand-border); font-size: 13.5px; color: var(--ink); display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: var(--space-2); }
    .custom-modified-pill { display: inline-flex; align-items: center; gap: 6px; font-size: 12px; font-weight: 700; padding: 3px 10px; border-radius: 999px; background: var(--accent-gold-soft); color: #78520d; border: 1px solid var(--accent-gold); }
    .inline-confirm-box { display: inline-flex; flex-wrap: wrap; align-items: center; gap: 6px; background: #fef3f2; border: 1px solid #fecdca; padding: 4px 10px; border-radius: 8px; font-size: 13px; color: #b42318; font-weight: 600; }
    .tt-cell.editable-cell { cursor: pointer; }
    .tt-cell.editable-cell.free-slot:hover, .tt-cell.editable-cell.unavail-slot:hover { border-color: var(--brand); background: var(--brand-soft); color: var(--brand); box-shadow: inset 0 0 0 1.5px var(--brand); }
    .editor-modal-dialog { max-width: 560px; }
    .editor-modal-header { padding: var(--space-4) var(--space-5); border-bottom: 1px solid var(--border); background: linear-gradient(180deg, #ffffff 0%, var(--surface-subtle) 100%); display: flex; align-items: center; justify-content: space-between; gap: var(--space-3); }
    .editor-modal-header h3 { margin: 0; font-size: 18px; font-weight: 700; color: var(--title-ink); }
    .editor-modal-body { padding: var(--space-5); overflow-y: auto; display: flex; flex-direction: column; gap: var(--space-4); }
    .slot-type-tabs { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 6px; background: var(--bg); padding: 4px; border-radius: 10px; border: 1px solid var(--border); }
    .slot-type-btn { font: inherit; font-size: 13.5px; font-weight: 700; padding: 8px 10px; border-radius: 7px; border: none; background: transparent; color: var(--ink-secondary); cursor: pointer; transition: background 0.15s ease, color 0.15s ease; }
    .slot-type-btn.active { background: var(--brand-grad); color: #ffffff; box-shadow: 0 2px 6px rgba(0,0,0,0.15); }
    .editor-form-grid { display: grid; grid-template-columns: 1fr 1fr; gap: var(--space-3); }
    .editor-form-grid .span-full { grid-column: 1 / -1; }
    @media (max-width: 520px) { .editor-form-grid, .slot-type-tabs { grid-template-columns: 1fr; } }
    .color-picker-wrap { display: flex; flex-wrap: wrap; align-items: center; gap: 8px; }
    .color-input-native { width: 42px; height: 36px; padding: 2px; border: 1px solid var(--border); border-radius: 8px; background: #ffffff; cursor: pointer; }
    .preset-color-dot { width: 26px; height: 26px; border-radius: 50%; border: 2px solid #ffffff; box-shadow: 0 0 0 1px rgba(0,0,0,0.22); cursor: pointer; padding: 0; }
    .preset-color-dot.active { box-shadow: 0 0 0 2.5px var(--ink); transform: scale(1.12); }
    .form-alert { padding: 10px 14px; border-radius: var(--radius-sm); font-size: 13.5px; font-weight: 600; background: #fef3f2; border: 1px solid #fecdca; color: #b42318; }
    .editor-modal-footer { padding: var(--space-3) var(--space-5); border-top: 1px solid var(--border); background: var(--surface-subtle); display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: var(--space-2); }
    .editor-footer-right { display: flex; flex-wrap: wrap; align-items: center; gap: var(--space-2); margin-inline-start: auto; }

    .hidden {
      display: none !important;
    }
  </style>
</head>
<body>
  <header class="app-header">
    <div class="header-logos-band">
      <div class="header-logos-inner">
        <div class="header-logos-left">
          <img src="data:image/png;base64,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" alt="ตราโรงเรียนประสานวิทยามูลนิธิ معهد الثقافة الإسلامية" class="header-emblem-img">
        <span class="logos-divider" aria-hidden="true"></span>
        <img src="data:image/jpeg;base64,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" alt="شؤون التعليم معهد الثقافة الإسلامية" class="header-calligraphy-img">
        </div>
        <img src="data:image/png;base64,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" alt="معهد الثقافة الإسلامية" class="header-school-name-img">
      </div>
    </div>
    <div class="header-inner">
      <div class="brand-title-group">
        <span class="school-badge">
          <span class="ar-text">معهد الثقافة الإسلامية</span>
          <span id="badgeYearText">• ปีการศึกษา 2026</span>
        </span>
        <h1 class="app-title">
          <span id="appTitleMainText">ระบบค้นหาตารางสอน</span>
          <span class="ar-heading" dir="rtl">جدول فغاجين معهد الثقافة الإسلامية 2026</span>
        </h1>
      </div>
      <div class="header-right-stack">
        <div class="header-prefs-bar">
          <div class="lang-switcher" id="langSwitcher" role="group" aria-label="Language / اللغة / بهاس">
            <button type="button" class="lang-btn active" data-set-lang="th" aria-pressed="true">ไทย</button>
            <button type="button" class="lang-btn ar-lang-font" data-set-lang="ar" aria-pressed="false">العربية</button>
            <button type="button" class="lang-btn ar-lang-font" data-set-lang="jawi" aria-pressed="false">جاوي</button>
          </div>
          <div class="theme-switcher" id="themeSwitcher" role="group" aria-label="Gradient Theme">
            <span class="theme-label" id="themeLabelText">ธีมสี</span>
            <button type="button" class="theme-swatch-btn theme-swatch-emerald active" data-set-theme="emerald" title="เขียวมรกต–ทอง" aria-label="เขียวมรกต–ทอง" aria-pressed="true"></button>
            <button type="button" class="theme-swatch-btn theme-swatch-sapphire" data-set-theme="sapphire" title="น้ำเงินคราม–ฟ้า" aria-label="น้ำเงินคราม–ฟ้า" aria-pressed="false"></button>
            <button type="button" class="theme-swatch-btn theme-swatch-teal" data-set-theme="teal" title="เขียวหยก–มิ้นต์" aria-label="เขียวหยก–มิ้นต์" aria-pressed="false"></button>
            <button type="button" class="theme-swatch-btn theme-swatch-amber" data-set-theme="amber" title="ทองอำพัน–ครีม" aria-label="ทองอำพัน–ครีม" aria-pressed="false"></button>
          </div>
        </div>
        <div class="header-meta" id="headerMetaBox">
          <span>ข้อมูลจากไฟล์: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span>
          <span>• ครูผู้สอน 73 ท่าน • 51 ห้องเรียน • 40 รายวิชา</span>
        </div>
      </div>
    </div>
  </header>

  <main class="main-container">
    <!-- Unified Search & Filter Controls -->
    <section class="control-card" aria-label="ตัวกรองและการค้นหาตารางสอน">
      <div class="top-bar-row">
        <div class="view-tabs six-tabs" role="tablist" aria-label="รูปแบบการแสดงผล">
          <button type="button" class="view-tab active" data-view="self" role="tab" aria-selected="true">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
            <span>สำหรับครูค้นหาเอง</span>
          </button>
          <button type="button" class="view-tab" data-view="explorer" role="tab" aria-selected="false">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
            <span>ค้นหารายการสอน</span>
          </button>
          <button type="button" class="view-tab" data-view="teacher" role="tab" aria-selected="false">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><rect x="3" y="4" width="18" height="16" rx="2"></rect><line x1="3" y1="10" x2="21" y2="10"></line><line x1="9" y1="10" x2="9" y2="20"></line></svg>
            <span>ตารางสอนรายครู</span>
          </button>
          <button type="button" class="view-tab" data-view="class" role="tab" aria-selected="false">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path><polyline points="9 22 9 12 15 12 15 22"></polyline></svg>
            <span>ตารางเรียนรายห้อง</span>
          </button>
          <button type="button" class="view-tab" data-view="free" role="tab" aria-selected="false">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="8.5" cy="7" r="4"></circle><polyline points="17 11 19 13 23 9"></polyline></svg>
            <span>ค้นหาครูว่างสอนแทน</span>
          </button>
          <button type="button" class="view-tab" data-view="manage" role="tab" aria-selected="false">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>
            <span>จัดการตารางสอน</span>
          </button>
        </div>

        <div class="search-status" id="liveResultSummary" aria-live="polite"></div>
      </div>

      <div class="filter-grid hidden" id="adminFilterGrid">
        <div class="field search-field-wrap">
          <label for="searchInput">คำค้นหา (ชื่อครู / ห้อง / วิชา / วัน / เลขหน้า)</label>
          <div class="input-wrap">
            <span class="input-icon">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
            </span>
            <input type="text" id="searchInput" class="text-input has-icon" placeholder="เช่น أحمد, الفقه, بهاس ملايو, 8/1, ت6, เสาร์..." autocomplete="off">
            <button type="button" id="clearSearchBtn" class="clear-input-btn" title="ล้างคำค้นหา" aria-label="ล้างคำค้นหา">×</button>
          </div>
        </div>

        <div class="field">
          <label for="teacherFilter">ครูผู้สอน</label>
          <select id="teacherFilter" class="select-input">
            <option value="">ทั้งหมด (73 ท่าน)</option>
          </select>
        </div>

        <div class="field">
          <label for="classFilter">ห้องเรียน</label>
          <select id="classFilter" class="select-input">
            <option value="">ทั้งหมด (51 ห้อง)</option>
          </select>
        </div>

        <div class="field">
          <label for="subjectFilter">รายวิชา</label>
          <select id="subjectFilter" class="select-input">
            <option value="">ทั้งหมด (40 วิชา)</option>
          </select>
        </div>

        <div class="field">
          <label for="dayFilter">วัน</label>
          <select id="dayFilter" class="select-input">
            <option value="">ทุกวัน</option>
          </select>
        </div>

        <div class="field">
          <label for="periodFilter">คาบเรียน / เวลา</label>
          <select id="periodFilter" class="select-input">
            <option value="">ทุกคาบเวลา</option>
          </select>
        </div>
      </div>

      <div class="active-filters-bar" id="activeFiltersBar">
        <div class="filter-chips" id="filterChipsContainer"></div>
        <button type="button" class="btn btn-ghost-danger" id="resetAllBtn">ล้างตัวกรองทั้งหมด</button>
      </div>
    </section>

    <!-- VIEW 0: Self-Service Teacher Lookup -->
    <section id="selfView" class="self-lookup-wrap" aria-label="สำหรับครูค้นหาตารางสอนด้วยตนเอง">
      <div class="self-hero-card">
        <div class="self-hero-head">
          <div>
            <h2>ค้นหาตารางสอนของคุณ</h2>
            <p>พิมพ์ชื่อครูผู้สอน เลขหน้า (1–73) หรือเลือกชื่อจากรายการเพื่อดูตารางสอนรายสัปดาห์ทันที</p>
          </div>
          <button type="button" class="btn hidden" id="selfClearTeacherBtn">ค้นหาชื่ออื่น</button>
        </div>

        <div class="self-search-row">
          <div class="field">
            <label for="selfSearchInput">พิมพ์ชื่อครู / ห้องที่สอน / วิชา / เลขหน้า</label>
            <div class="input-wrap">
              <span class="input-icon">
                <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
              </span>
              <input type="text" id="selfSearchInput" class="text-input has-icon self-input-lg" placeholder="พิมพ์ชื่อครู, ห้องเรียน (เช่น 8/1, ت6), วิชา หรือเลขหน้า (1–73)..." autocomplete="off">
              <button type="button" id="selfClearInputBtn" class="clear-input-btn" title="ล้างข้อความ" aria-label="ล้างข้อความ">×</button>
            </div>
          </div>

          <div class="field">
            <label for="selfTeacherSelect">หรือเลือกจากรายชื่อครูทั้งหมด (73 ท่าน)</label>
            <select id="selfTeacherSelect" class="select-input self-input-lg">
              <option value="">-- เลือกชื่อครูผู้สอน --</option>
            </select>
          </div>
        </div>

        <div class="quick-letter-wrap" id="selfLetterWrap">
          <span class="quick-letter-label">แตะเลือกตามอักษรตัวแรกของชื่อครู (ไม่ต้องพิมพ์ภาษาอาหรับ/ยาวี):</span>
          <div class="quick-letter-row" id="selfLetterRow" role="group" aria-label="กรองตามอักษรตัวแรกของชื่อครู"></div>
        </div>

        <div id="selfSelectedBanner" class="self-selected-banner hidden"></div>

        <div id="selfMatchSection">
          <div class="self-teacher-grid" id="selfTeacherGrid" role="listbox" aria-label="รายชื่อครูที่ตรงกับการค้นหา"></div>
          <div id="selfNoMatch" class="empty-state hidden" style="padding: 24px 16px;">
            <h3>ไม่พบชื่อครูที่ตรงกับคำค้นหา</h3>
            <p>ลองพิมพ์เฉพาะบางส่วนของชื่อ หรือเลือกจากช่องรายชื่อครูด้านบน</p>
          </div>
        </div>
      </div>

      <div id="selfTimetableResult" class="timetable-card hidden"></div>
    </section>

    <!-- VIEW 1: All Lessons Search Explorer -->
    <section id="explorerView" class="table-card hidden" aria-label="ผลการค้นหารายการสอน">
      <div class="table-scroll">
        <table class="explorer-table" id="lessonsTable">
          <thead>
            <tr>
              <th class="sortable num-col" data-sort="page" style="width: 78px;">หน้า <span class="sort-ind">↑</span></th>
              <th class="sortable" data-sort="teacher">ครูผู้สอน <span class="sort-ind">↕</span></th>
              <th class="sortable" data-sort="dayIdx">วัน <span class="sort-ind">↕</span></th>
              <th class="sortable" data-sort="pStart">คาบ / เวลา <span class="sort-ind">↕</span></th>
              <th class="sortable" data-sort="cls">ห้องเรียน <span class="sort-ind">↕</span></th>
              <th class="sortable" data-sort="subj">รายวิชา <span class="sort-ind">↕</span></th>
              <th class="sortable num-col" data-sort="span" style="width: 105px;">จำนวนคาบ <span class="sort-ind">↕</span></th>
            </tr>
          </thead>
          <tbody id="explorerTableBody"></tbody>
        </table>
      </div>

      <div id="explorerEmptyState" class="empty-state hidden">
        <div class="empty-icon">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
        </div>
        <h3>ไม่พบตารางสอนที่ตรงกับเงื่อนไข</h3>
        <p>ลองเปลี่ยนคำค้นหา หรือล้างตัวกรองเพื่อดูรายการสอนทั้งหมดในระบบ</p>
        <button type="button" class="btn" id="emptyResetBtn">ล้างตัวกรองทั้งหมด</button>
      </div>

      <div class="pagination-bar" id="paginationBar">
        <div id="paginationInfo"></div>
        <div class="page-controls">
          <label for="pageSizeSelect" style="font-size:13px;">แสดง:</label>
          <select id="pageSizeSelect" class="select-input" style="width:auto; min-height:32px; padding:4px 8px; font-size:13px;">
            <option value="25">25 รายการ</option>
            <option value="50">50 รายการ</option>
            <option value="100">100 รายการ</option>
          </select>
          <button type="button" class="btn" id="prevPageBtn">ก่อนหน้า</button>
          <span id="pageIndicator" style="padding: 0 6px; font-weight: 600;"></span>
          <button type="button" class="btn" id="nextPageBtn">ถัดไป</button>
        </div>
      </div>
    </section>

    <!-- VIEW 2: Teacher Timetable Grid -->
    <section id="teacherView" class="workspace-split hidden" aria-label="ตารางสอนรายครู">
      <aside class="directory-panel">
        <div class="directory-header">
          <div class="directory-title-row">
            <span>รายชื่อครูผู้สอน</span>
            <span id="teacherDirCount" style="color:var(--brand);"></span>
          </div>
          <input type="text" id="teacherQuickSearch" class="text-input" placeholder="กรองรายชื่อครู..." style="min-height:34px; font-size:13.5px; padding:6px 10px;">
        </div>
        <div class="directory-list" id="teacherDirList" role="listbox" aria-label="เลือกครูผู้สอน"></div>
      </aside>

      <div class="timetable-card" id="teacherTimetableContainer"></div>
    </section>

    <!-- VIEW 3: Class Timetable Grid -->
    <section id="classView" class="workspace-split hidden" aria-label="ตารางเรียนรายห้อง">
      <aside class="directory-panel">
        <div class="directory-header">
          <div class="directory-title-row">
            <span>รายชื่อห้องเรียน</span>
            <span id="classDirCount" style="color:var(--brand);"></span>
          </div>
          <input type="text" id="classQuickSearch" class="text-input" placeholder="ค้นหาห้อง เช่น 8/1, ت6, C1..." style="min-height:34px; font-size:13.5px; padding:6px 10px;">
        </div>
        <div class="directory-list" id="classDirList" role="listbox" aria-label="เลือกห้องเรียน"></div>
      </aside>

      <div class="timetable-card" id="classTimetableContainer"></div>
    </section>

    <!-- VIEW 4: Free / Substitute Teacher Finder -->
    <section id="freeView" class="table-card hidden" aria-label="ค้นหาครูว่างสอนแทน">
      <div class="sub-controls-bar">
        <div class="sub-picker-group">
          <span class="sub-picker-label">เลือกวัน:</span>
          <div class="pill-btn-row" id="subDayPills" role="group" aria-label="เลือกวันที่ต้องการหาครูสอนแทน"></div>
        </div>
        <div class="sub-picker-group">
          <span class="sub-picker-label">เลือกคาบเวลา:</span>
          <div class="pill-btn-row" id="subPeriodPills" role="group" aria-label="เลือกคาบเวลาที่ต้องการหาครูสอนแทน"></div>
        </div>
        <div id="subClassContext" class="sub-context-note hidden"></div>
      </div>

      <div class="table-scroll">
        <table class="explorer-table" id="freeTeachersTable">
          <thead>
            <tr>
              <th class="sortable num-col" data-sub-sort="id" style="width: 78px;">หน้า <span class="sort-ind">↕</span></th>
              <th class="sortable" data-sub-sort="name">ครูที่ว่างพร้อมสอนแทน (---) <span class="sort-ind">↕</span></th>
              <th>รายวิชาที่สอนประจำ</th>
              <th>ตารางรายคาบในวันนั้น (คาบ 1–5)</th>
              <th class="sortable num-col" data-sub-sort="dayBusy" style="width: 120px;">สอนวันนี้ <span class="sort-ind">↑</span></th>
              <th class="sortable num-col" data-sub-sort="periods" style="width: 125px;">รวมทั้งสัปดาห์ <span class="sort-ind">↕</span></th>
            </tr>
          </thead>
          <tbody id="freeTableBody"></tbody>
        </table>
      </div>

      <div id="freeEmptyState" class="empty-state hidden">
        <div class="empty-icon">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
        </div>
        <h3>ไม่พบครูว่างที่ตรงกับเงื่อนไขในคาบเวลานี้</h3>
        <p>ลองเลือกคาบเวลาอื่น หรือล้างตัวกรองรายวิชา/คำค้นหาเพื่อดูรายชื่อครูว่างทั้งหมดในคาบนี้</p>
        <button type="button" class="btn" id="freeEmptyResetBtn">ล้างตัวกรองเพิ่มเติม</button>
      </div>

      <div class="tt-footer">
        <span>หมายเหตุ: แสดงเฉพาะครูที่มีสถานะคาบว่างจริง (<strong>---</strong>) ในวันและคาบที่เลือก โดยตัดครูที่ติดสอนและครูที่งดสอน/ไม่ว่าง (<strong>-x-</strong>) ออกโดยอัตโนมัติ • คลิกที่แถวเพื่อดูตารางสอนเต็ม</span>
      </div>
    </section>

    <!-- VIEW 5: Academic Affairs Timetable Editor -->
    <section id="manageView" class="timetable-card hidden" aria-label="จัดการตารางสอน">
      <div class="manage-top-bar">
        <div class="manage-teacher-picker">
          <div class="field">
            <label for="manageTeacherSelect" id="lblManageTeacher">เลือกครูผู้สอนเพื่อแก้ไขตาราง</label>
            <select id="manageTeacherSelect" class="select-input"></select>
          </div>
          <button type="button" class="btn" id="editTeacherNameBtn">แก้ไขชื่อครู</button>
          <button type="button" class="btn" id="addNewTeacherBtn">+ เพิ่มครูใหม่</button>
        </div>
        <div class="manage-actions-group">
          <span id="customModifiedBadge" class="custom-modified-pill hidden">มีการแก้ไขเพิ่มเติม</span>
          <button type="button" class="btn btn-primary" id="openAddSlotBtn">+ เพิ่ม / แก้ไขคาบสอน</button>
          <button type="button" class="btn btn-ghost-danger hidden" id="resetDefaultDataBtn">คืนค่าต้นฉบับ</button>
          <span id="resetConfirmBox" class="inline-confirm-box hidden">
            <span id="resetConfirmLabel">ยืนยันคืนค่าต้นฉบับ?</span>
            <button type="button" class="btn btn-ghost-danger" id="confirmResetYesBtn" style="padding:4px 10px; font-size:12.5px;">ยืนยัน</button>
            <button type="button" class="btn" id="confirmResetNoBtn" style="padding:4px 10px; font-size:12.5px;">ยกเลิก</button>
          </span>
        </div>
      </div>
      <div class="manage-hint-bar">
        <span id="manageHintText">คลิกที่ช่องใดก็ได้ในตารางด้านล่าง (คาบสอน, คาบว่าง ---, หรือคาบงดสอน -x-) เพื่อเพิ่ม แก้ไข หรือลบคาบสอนได้ทันที</span>
      </div>
      <div id="manageGridContainer"></div>
    </section>
  </main>

  <datalist id="classDatalist"></datalist>
  <datalist id="subjectDatalist"></datalist>

  <!-- Teacher Detail Modal (opened when clicking a row in Explorer) -->
  <div class="modal-backdrop" id="teacherModal" role="dialog" aria-modal="true" aria-labelledby="modalTeacherHeading">
    <div class="modal-dialog">
      <div class="modal-body" id="modalContentArea"></div>
    </div>
  </div>

  <!-- Slot Add/Edit Modal -->
  <div class="modal-backdrop" id="slotEditorModal" role="dialog" aria-modal="true" aria-labelledby="slotModalTitle">
    <div class="modal-dialog editor-modal-dialog">
      <div class="editor-modal-header">
        <h3 id="slotModalTitle">เพิ่ม / แก้ไขคาบสอน</h3>
        <button type="button" class="btn" id="closeSlotModalTopBtn" style="padding:4px 10px;">×</button>
      </div>
      <form id="slotEditorForm" novalidate>
        <div class="editor-modal-body">
          <div class="slot-type-tabs" role="tablist" id="slotTypeTabs">
            <button type="button" class="slot-type-btn active" data-slot-type="lesson" id="tabTypeLesson">คาบสอนปกติ</button>
            <button type="button" class="slot-type-btn" data-slot-type="free" id="tabTypeFree">คาบว่าง (---)</button>
            <button type="button" class="slot-type-btn" data-slot-type="unavail" id="tabTypeUnavail">งดสอน (-x-)</button>
          </div>
          <div class="editor-form-grid">
            <div class="field span-full">
              <label for="slotTeacherSelect" id="lblSlotTeacher">ครูผู้สอน</label>
              <select id="slotTeacherSelect" class="select-input"></select>
            </div>
            <div class="field">
              <label for="slotDaySelect" id="lblSlotDay">วัน</label>
              <select id="slotDaySelect" class="select-input"></select>
            </div>
            <div class="field">
              <label for="slotPeriodSelect" id="lblSlotPeriod">คาบเริ่มต้น</label>
              <select id="slotPeriodSelect" class="select-input"></select>
            </div>
            <div id="lessonSpecificFields" class="span-full editor-form-grid">
              <div class="field">
                <label for="slotClassInput" id="lblSlotClass">ห้องเรียน</label>
                <input type="text" id="slotClassInput" class="text-input" list="classDatalist" placeholder="เช่น 8/1, ت6, C1..." autocomplete="off">
              </div>
              <div class="field">
                <label for="slotSpanSelect" id="lblSlotSpan">จำนวนคาบต่อเนื่อง</label>
                <select id="slotSpanSelect" class="select-input">
                  <option value="1" id="optSpan1">1 คาบ (ปกติ)</option>
                  <option value="2" id="optSpan2">2 คาบต่อเนื่อง</option>
                </select>
              </div>
              <div class="field span-full">
                <label for="slotSubjectInput" id="lblSlotSubject">รายวิชา</label>
                <input type="text" id="slotSubjectInput" class="text-input" list="subjectDatalist" placeholder="เช่น الفقه, بهاس ملايو..." autocomplete="off">
              </div>
              <div class="field span-full">
                <label for="slotColorInput" id="lblSlotColor">สีพื้นหลังช่องตาราง</label>
                <div class="color-picker-wrap">
                  <input type="color" id="slotColorInput" class="color-input-native" value="#E6BD72">
                  <div class="pill-btn-row" id="presetColorSwatches"></div>
                </div>
              </div>
            </div>
          </div>
          <div id="slotFormAlert" class="form-alert hidden"></div>
        </div>
        <div class="editor-modal-footer">
          <button type="button" class="btn btn-ghost-danger hidden" id="deleteLessonBtn">ลบคาบสอนนี้</button>
          <div class="editor-footer-right">
            <button type="button" class="btn" id="cancelSlotModalBtn">ยกเลิก</button>
            <button type="submit" class="btn btn-primary" id="saveSlotBtn">บันทึกการเปลี่ยนแปลง</button>
          </div>
        </div>
      </form>
    </div>
  </div>

  <!-- Teacher Add/Rename Modal -->
  <div class="modal-backdrop" id="teacherProfileModal" role="dialog" aria-modal="true" aria-labelledby="teacherProfileModalTitle">
    <div class="modal-dialog editor-modal-dialog" style="max-width:460px;">
      <div class="editor-modal-header">
        <h3 id="teacherProfileModalTitle">ข้อมูลครูผู้สอน</h3>
        <button type="button" class="btn" id="closeTeacherProfileTopBtn" style="padding:4px 10px;">×</button>
      </div>
      <form id="teacherProfileForm" novalidate>
        <div class="editor-modal-body">
          <div class="field">
            <label for="teacherProfileNameInput" id="lblTeacherProfileName">ชื่อครูผู้สอน (อาหรับ / ยาวี / ไทย)</label>
            <input type="text" id="teacherProfileNameInput" class="text-input" placeholder="เช่น أحمد رمزي حاج تيه..." autocomplete="off">
          </div>
          <div id="teacherProfileAlert" class="form-alert hidden"></div>
        </div>
        <div class="editor-modal-footer">
          <div class="editor-footer-right">
            <button type="button" class="btn" id="cancelTeacherProfileBtn">ยกเลิก</button>
            <button type="submit" class="btn btn-primary" id="saveTeacherProfileBtn">บันทึก</button>
          </div>
        </div>
      </form>
    </div>
  </div>

  <script id="app-data" type="application/json">{"meta": {"school": "معهد الثقافة الإسلامية", "title": "جدول فغاجين معهد الثقافة الإسلامية 2026", "generated": "Timetable generated with FET 7.8.5 on 5/9/26 2:20 PM", "days": ["السبت", "الأحد", "الإثنين", "الثلاثاء", "الأربعاء", "الخميس"], "periods": ["08:00 - 08.45", "08.45 - 09.30", "09.30 - 10.15", "10.15 - 11.00", "11.00 - 11.45"]}, "teachers": [{"id": 1, "name": "أحمد رمزي حاج تيه", "periods": 7, "free": 23, "unavail": 0, "unavailGrid": [[], [], [], [], [], []]}, {"id": 2, "name": "حاج عبد الكريم ياموسنا", "periods": 15, "free": 5, "unavail": 10, "unavailGrid": [[0], [0], [0, 1, 2, 3, 4], [0], [0], [0]]}, {"id": 3, "name": "حاج محمد يوسف كاويڠ", "periods": 16, "free": 4, "unavail": 10, "unavailGrid": [[3], [1], [0], [2], [4], [0, 1, 2, 3, 4]]}, {"id": 4, "name": "عمران وي يوسف", "periods": 16, "free": 3, "unavail": 11, "unavailGrid": [[0, 1, 2, 3, 4], [3], [0], [2, 4], [0], [1]]}, {"id": 5, "name": "محمد شكري چالئ", "periods": 16, "free": 1, "unavail": 13, "unavailGrid": [[0], [2], [0, 1, 2, 3, 4], [2, 4], [0, 3, 4], [0]]}, {"id": 6, "name": "عبد الـبر سـامو", "periods": 18, "free": 3, "unavail": 9, "unavailGrid": [[0, 1, 2, 3, 4], [4], [], [4], [], [2, 3]]}, {"id": 7, "name": "إسماعيل نئ سنيك", "periods": 19, "free": 1, "unavail": 10, "unavailGrid": [[2], [0, 1, 2, 3, 4], [], [0, 4], [4], [0]]}, {"id": 8, "name": "نورية چئ هأ", "periods": 18, "free": 6, "unavail": 6, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [4], []]}, {"id": 9, "name": "ذكية داليڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 10, "name": "شريفة لاديڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 11, "name": "ريسـاني قـالي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 12, "name": "نور أنيس مألي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 13, "name": "غزالي مأسي", "periods": 18, "free": 2, "unavail": 10, "unavailGrid": [[0], [0, 1, 2, 3, 4], [0], [0], [0], [0]]}, {"id": 14, "name": "عـائشة صيديق", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 15, "name": "زكريـا چئ تيه", "periods": 17, "free": 3, "unavail": 10, "unavailGrid": [[], [0, 1, 2, 3, 4], [4], [3, 4], [0], [1]]}, {"id": 16, "name": "سورايدا مأدية", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 17, "name": "مريم سئ كاسق", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 18, "name": "رقية چئ لوڠ", "periods": 20, "free": 4, "unavail": 6, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [4], []]}, {"id": 19, "name": "يحيى فوتيه", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 20, "name": "أمير المؤمنين يري", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 21, "name": "حسن كانوڠميڠ", "periods": 19, "free": 5, "unavail": 6, "unavailGrid": [[], [], [], [4], [], [0, 1, 2, 3, 4]]}, {"id": 22, "name": "هارون راديڠ", "periods": 20, "free": 3, "unavail": 7, "unavailGrid": [[0], [0, 1, 2, 3, 4], [], [4], [], []]}, {"id": 23, "name": "جميلة فوسو", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 24, "name": "نئ صه چيئناروڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 25, "name": "مريم سي مأسي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 26, "name": "عبدالحكيم فأوه", "periods": 18, "free": 5, "unavail": 7, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [4], [4], []]}, {"id": 27, "name": "سواني موليڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 28, "name": "رمزية چئ تيه", "periods": 19, "free": 6, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 29, "name": "وي رقية وي حاج", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 30, "name": "حسين مـامأ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 31, "name": "عبد الله براهيڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 32, "name": "فرحـانـا علي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 33, "name": "محمد راضي كيتـؤ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 34, "name": "نورحياتي وي هأمأ", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 35, "name": "ذوالكفلي أبواء", "periods": 17, "free": 5, "unavail": 8, "unavailGrid": [[4], [], [4], [], [4], [0, 1, 2, 3, 4]]}, {"id": 36, "name": "زكريـا فأچوتيه", "periods": 18, "free": 7, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 37, "name": "بـلـيـــا يــؤ", "periods": 19, "free": 4, "unavail": 7, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [4], [4], []]}, {"id": 38, "name": "محمد رافي كونـا", "periods": 16, "free": 5, "unavail": 9, "unavailGrid": [[], [1], [0], [2], [4], [0, 1, 2, 3, 4]]}, {"id": 39, "name": "إسماعيل چئ هي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 40, "name": "إرحم دوميدي", "periods": 20, "free": 4, "unavail": 6, "unavailGrid": [[], [], [], [4], [], [0, 1, 2, 3, 4]]}, {"id": 41, "name": "وان جميلة عـاكئ", "periods": 19, "free": 5, "unavail": 6, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [4], []]}, {"id": 42, "name": "جـارودين ميره", "periods": 19, "free": 5, "unavail": 6, "unavailGrid": [[], [], [], [4], [], [0, 1, 2, 3, 4]]}, {"id": 43, "name": "مـارية أوي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 44, "name": "عثمـان وي سالئ", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 45, "name": "أمينة كاهوڠ", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 46, "name": "ثويبة وي هأيي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 47, "name": "برهـان ويئـچـا", "periods": 17, "free": 5, "unavail": 8, "unavailGrid": [[2], [4], [0, 1, 2, 3, 4], [4], [], []]}, {"id": 48, "name": "إسمـاعيل عـاكئ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 49, "name": "حمدي يونو", "periods": 16, "free": 9, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 50, "name": "بدرية سأتيـا", "periods": 20, "free": 2, "unavail": 8, "unavailGrid": [[0], [], [0, 1, 2, 3, 4], [0], [0], []]}, {"id": 51, "name": "سلـمى تـاكيه", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 52, "name": "حبيبة يونو", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 53, "name": "خديجة تبيڠمس", "periods": 20, "free": 3, "unavail": 7, "unavailGrid": [[], [0, 1, 2, 3, 4], [0], [], [], [0]]}, {"id": 54, "name": "رشيدة كالو", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 55, "name": "حليمة يونو", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 56, "name": "عاديلة حاج باكا", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [], []]}, {"id": 57, "name": "عبد الله سي مأسي", "periods": 20, "free": 4, "unavail": 6, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [4], [], []]}, {"id": 58, "name": "حاج محمد چئ هي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 59, "name": "نئ قوب مأيوسف", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 60, "name": "سليمـان مألي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}, {"id": 61, "name": "سليمـان مأيي", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 62, "name": "حمزة يئ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 63, "name": "عدنـان كرؤفي", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 64, "name": "إسماعيل وان محمود", "periods": 18, "free": 6, "unavail": 6, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [4], [], []]}, {"id": 65, "name": "عزة درامت", "periods": 20, "free": 4, "unavail": 6, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [4], []]}, {"id": 66, "name": "إسماعيل تؤهيڠ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 67, "name": "نصري كامأ", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 68, "name": "أمينة مأسه", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 69, "name": "فـاطمة فوڠ", "periods": 17, "free": 7, "unavail": 6, "unavailGrid": [[], [0, 1, 2, 3, 4], [], [], [4], []]}, {"id": 70, "name": "فـاطيمـا واسـا", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[0, 1, 2, 3, 4], [], [], [], [], []]}, {"id": 71, "name": "ڬورو 001", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 72, "name": "ڬورو 002", "periods": 20, "free": 5, "unavail": 5, "unavailGrid": [[], [], [0, 1, 2, 3, 4], [], [], []]}, {"id": 73, "name": "ڬورو 003", "periods": 21, "free": 4, "unavail": 5, "unavailGrid": [[], [], [], [], [], [0, 1, 2, 3, 4]]}], "lessons": [[1, 0, 1, 1, "8/1", "علم النفس", "#E18D04", 0], [1, 0, 3, 1, "9/2", "التربية", "#DE30BB", 1], [1, 0, 4, 1, "9/1", "طرق التدريس", "#F123D8", 1], [1, 2, 1, 1, "9/1", "التربية", "#D2A94D", 0], [1, 2, 2, 1, "8/2", "علم النفس", "#ED14F2", 1], [1, 5, 1, 1, "9/2", "طرق التدريس", "#FDBA2E", 0], [1, 5, 3, 1, "8/3", "علم النفس", "#6B5809", 1], [2, 0, 1, 1, "2/5", "الفقه", "#E6BD72", 0], [2, 0, 3, 1, "2/4", "الفقه", "#60F189", 0], [2, 0, 4, 1, "2/3", "الفقه", "#FF8E9E", 0], [2, 1, 2, 1, "2/4", "الفقه", "#60F189", 0], [2, 1, 3, 1, "2/2", "الفقه", "#79C265", 0], [2, 1, 4, 1, "3/1", "الفقه", "#F65244", 0], [2, 3, 1, 1, "3/1", "الفقه", "#F65244", 0], [2, 3, 3, 1, "2/4", "الفقه", "#60F189", 0], [2, 3, 4, 1, "2/2", "الفقه", "#79C265", 0], [2, 4, 3, 1, "2/5", "الفقه", "#E6BD72", 0], [2, 4, 4, 1, "2/3", "الفقه", "#FF8E9E", 0], [2, 5, 1, 1, "2/5", "الفقه", "#E6BD72", 0], [2, 5, 2, 1, "2/2", "الفقه", "#79C265", 0], [2, 5, 3, 1, "3/1", "الفقه", "#F65244", 0], [2, 5, 4, 1, "2/3", "الفقه", "#FF8E9E", 0], [3, 0, 0, 1, "5/4", "التوحيد", "#847F82", 0], [3, 0, 1, 1, "7/2", "النحو", "#BB97CD", 0], [3, 0, 2, 1, "9/2", "المنطق", "#D42FD3", 1], [3, 0, 4, 1, "5/2", "النحو", "#3BC898", 0], [3, 1, 0, 1, "5/4", "التوحيد", "#847F82", 0], [3, 1, 2, 1, "8/1", "المنطق", "#5BBFF2", 0], [3, 1, 3, 1, "6/2", "النحو", "#389E1A", 1], [3, 1, 4, 1, "5/2", "النحو", "#3BC898", 0], [3, 2, 1, 1, "10/1", "الإدارة", "#651E1F", 1], [3, 2, 2, 1, "6/2", "النحو", "#389E1A", 1], [3, 2, 3, 1, "8/2", "المنطق", "#572604", 1], [3, 2, 4, 1, "10/1", "المنطق", "#868064", 1], [3, 3, 0, 1, "9/1", "المنطق", "#D8B625", 0], [3, 3, 1, 1, "8/3", "المنطق", "#D16AFF", 0], [3, 3, 4, 1, "9/1", "النشاط", "#E4FD23", 0], [3, 4, 0, 1, "7/2", "النحو", "#BB97CD", 0], [4, 1, 0, 1, "6/2", "الورشة", "#B9F8D2", 0], [4, 1, 1, 1, "6/1", "الفقه", "#F3A9C2", 0], [4, 1, 2, 1, "8/2", "الفقه", "#723569", 1], [4, 1, 4, 1, "7/2", "الورشة", "#3AF105", 0], [4, 2, 1, 2, "2/1", "الفقه", "#755B93", 1], [4, 2, 4, 1, "5/2", "الورشة", "#BAAE50", 0], [4, 3, 0, 1, "8/3", "الفقه", "#F47992", 0], [4, 3, 1, 1, "C2", "الورشة", "#AA239D", 1], [4, 3, 3, 1, "8/1", "الفقه", "#7EAC9F", 0], [4, 4, 1, 1, "8/3", "الفقه", "#F47992", 0], [4, 4, 2, 1, "2/1", "الفقه", "#755B93", 1], [4, 4, 4, 1, "9/2", "الورشة", "#B7F458", 0], [4, 5, 2, 1, "8/2", "الفقه", "#723569", 1], [4, 5, 3, 1, "6/1", "الفقه", "#F3A9C2", 0], [4, 5, 4, 1, "8/1", "الفقه", "#7EAC9F", 0], [5, 0, 1, 1, "6/2", "الصرف", "#235D94", 1], [5, 0, 2, 1, "5/2", "الصرف", "#200B16", 1], [5, 0, 3, 1, "ت6", "الحديث", "#7B3D0C", 1], [5, 0, 4, 1, "9/2", "قاعة البحث", "#7AE4EA", 0], [5, 1, 1, 1, "7/2", "الصرف", "#A05443", 1], [5, 1, 3, 1, "ت6", "الحديث", "#7B3D0C", 1], [5, 1, 4, 1, "8/1", "النشاط", "#67F4F4", 0], [5, 3, 0, 1, "2/1", "المطالعة والإملاء", "#51613A", 1], [5, 3, 1, 1, "10/1", "القرءان", "#9A83E4", 0], [5, 3, 3, 1, "7/4", "أصول التفسير", "#CF95E4", 0], [5, 4, 1, 1, "7/2", "الصرف", "#A05443", 1], [5, 4, 2, 1, "6/2", "الصرف", "#235D94", 1], [5, 5, 1, 1, "5/2", "الصرف", "#200B16", 1], [5, 5, 2, 1, "2/1", "المطالعة والإملاء", "#51613A", 1], [5, 5, 3, 1, "10/1", "القرءان", "#9A83E4", 0], [5, 5, 4, 1, "9/1", "قاعة البحث", "#767D1C", 1], [6, 1, 0, 2, "8/3", "القرءان", "#125081", 1], [6, 1, 2, 1, "2/1", "الحديث", "#663DFB", 1], [6, 1, 3, 1, "C1", "الفقه", "#ECCE54", 0], [6, 2, 0, 1, "2/1", "الحديث", "#663DFB", 1], [6, 2, 2, 1, "10/1", "الفقه", "#8C9697", 0], [6, 2, 3, 1, "9/2", "الفقه", "#F13CBE", 0], [6, 3, 0, 2, "C1", "الفقه", "#ECCE54", 0], [6, 3, 2, 1, "6/2", "التحويد", "#F11658", 1], [6, 4, 0, 1, "9/1", "الفقه", "#FDA548", 0], [6, 4, 1, 1, "7/4", "المطالعة والإملاء", "#4130A6", 1], [6, 4, 2, 1, "8/3", "القرءان", "#125081", 1], [6, 4, 3, 1, "9/2", "الفقه", "#F13CBE", 0], [6, 4, 4, 1, "8/2", "الورشة", "#34FD8F", 0], [6, 5, 0, 1, "5/2", "التحويد", "#F240DA", 0], [6, 5, 1, 1, "9/1", "الفقه", "#FDA548", 0], [6, 5, 4, 1, "7/4", "المطالعة والإملاء", "#4130A6", 1], [7, 0, 0, 1, "C2", "التوحيد", "#EC04EF", 1], [7, 0, 1, 1, "C1", "التوحيد", "#E09D19", 0], [7, 0, 3, 1, "7/2", "التوحيد", "#1D133B", 1], [7, 0, 4, 1, "8/2", "النشاط", "#6B6D02", 1], [7, 2, 0, 2, "3/7", "القرءان", "#0948BB", 1], [7, 2, 2, 1, "C2", "التوحيد", "#EC04EF", 1], [7, 2, 3, 1, "6/2", "التوحيد", "#9E1AEC", 1], [7, 2, 4, 1, "C1", "النشاط", "#674953", 1], [7, 3, 2, 1, "2/1", "التوحيد", "#14714B", 1], [7, 3, 3, 1, "7/2", "التوحيد", "#1D133B", 1], [7, 4, 0, 2, "3/7", "القرءان", "#0948BB", 1], [7, 4, 2, 1, "C4", "النشاط", "#72E349", 0], [7, 4, 3, 1, "5/2", "التوحيد", "#9D4C6E", 1], [7, 5, 1, 1, "6/2", "التوحيد", "#9E1AEC", 1], [7, 5, 2, 1, "C1", "التوحيد", "#E09D19", 0], [7, 5, 3, 1, "5/2", "التوحيد", "#9D4C6E", 1], [7, 5, 4, 1, "2/1", "التوحيد", "#14714B", 1], [8, 1, 0, 2, "C4", "القرءان", "#2F74FE", 1], [8, 1, 2, 1, "9/1", "التفسير", "#E5E0E3", 0], [8, 1, 3, 1, "8/1", "التفسير", "#66E934", 0], [8, 1, 4, 1, "8/3", "التفسير", "#EC3C39", 1], [8, 2, 0, 1, "9/2", "التفسير", "#E97915", 0], [8, 2, 1, 1, "8/2", "التفسير", "#6A70C2", 1], [8, 2, 3, 1, "9/1", "أصول التفسير", "#573AA3", 1], [8, 2, 4, 1, "9/1", "التفسير", "#E5E0E3", 0], [8, 3, 0, 1, "10/1", "أصول التفسير", "#07BFEE", 0], [8, 3, 3, 1, "8/2", "التفسير", "#6A70C2", 1], [8, 3, 4, 1, "8/1", "التفسير", "#66E934", 0], [8, 4, 0, 1, "10/1", "التفسير", "#ADF227", 0], [8, 4, 1, 1, "9/2", "التفسير", "#E97915", 0], [8, 5, 0, 2, "C4", "القرءان", "#2F74FE", 1], [8, 5, 3, 1, "9/2", "أصول التفسير", "#5BA355", 0], [8, 5, 4, 1, "8/3", "التفسير", "#EC3C39", 1], [9, 0, 0, 1, "ت5", "التفسير", "#7C8739", 1], [9, 0, 2, 1, "2/1", "التفسير", "#6D1E38", 1], [9, 0, 3, 1, "7/1", "أصول التفسير", "#DA3FFE", 0], [9, 0, 4, 1, "ت4", "التفسير", "#FACBC2", 0], [9, 2, 0, 2, "6/2", "القرءان", "#191927", 1], [9, 2, 2, 1, "5/2", "التفسير", "#E4231D", 1], [9, 2, 3, 1, "7/2", "التفسير", "#647C48", 1], [9, 2, 4, 1, "6/2", "التفسير", "#E7759F", 0], [9, 3, 0, 1, "6/2", "التفسير", "#E7759F", 0], [9, 3, 1, 1, "2/1", "التفسير", "#6D1E38", 1], [9, 3, 4, 1, "8/3", "أصول التفسير", "#5EE679", 0], [9, 4, 0, 2, "6/2", "القرءان", "#191927", 1], [9, 4, 4, 1, "7/2", "التفسير", "#647C48", 1], [9, 5, 0, 1, "8/2", "أصول التفسير", "#D8AA82", 0], [9, 5, 1, 1, "8/1", "أصول التفسير", "#D43374", 1], [9, 5, 2, 1, "7/2", "أصول التفسير", "#D6A608", 0], [9, 5, 3, 1, "7/3", "أصول التفسير", "#50EAF3", 0], [9, 5, 4, 1, "5/2", "التفسير", "#E4231D", 1], [10, 0, 0, 1, "4/6", "التحويد", "#E2AFEC", 0], [10, 0, 2, 1, "4/1", "التحويد", "#7DD0FB", 0], [10, 0, 3, 1, "4/3", "التحويد", "#F705F6", 1], [10, 0, 4, 1, "3/1", "التحويد", "#F87428", 0], [10, 1, 0, 1, "4/5", "التحويد", "#EE361A", 1], [10, 1, 1, 1, "4/7", "التحويد", "#64E317", 0], [10, 1, 2, 1, "4/4", "التحويد", "#687AE1", 0], [10, 1, 3, 1, "4/1", "التحويد", "#7DD0FB", 0], [10, 1, 4, 1, "4/3", "التحويد", "#F705F6", 1], [10, 2, 0, 2, "4/5", "القرءان", "#063965", 1], [10, 2, 2, 1, "4/2", "التحويد", "#71490D", 1], [10, 2, 3, 1, "4/7", "التحويد", "#64E317", 0], [10, 2, 4, 1, "3/1", "التحويد", "#F87428", 0], [10, 3, 1, 1, "4/5", "التحويد", "#EE361A", 1], [10, 3, 3, 1, "4/2", "التحويد", "#71490D", 1], [10, 4, 0, 2, "4/5", "القرءان", "#063965", 1], [10, 4, 2, 1, "4/6", "التحويد", "#E2AFEC", 0], [10, 4, 4, 1, "4/4", "التحويد", "#687AE1", 0], [11, 0, 0, 1, "5/7", "التفسير", "#F18907", 0], [11, 0, 1, 1, "5/3", "التفسير", "#626FE6", 1], [11, 0, 2, 1, "5/5", "التفسير", "#7B5C0A", 1], [11, 0, 3, 1, "5/1", "التفسير", "#E8BAEB", 0], [11, 0, 4, 1, "5/6", "التفسير", "#77C5FC", 0], [11, 2, 0, 2, "3/6", "القرءان", "#8F0440", 1], [11, 2, 2, 1, "AEP1", "التفسير", "#8DB43B", 0], [11, 2, 3, 1, "5/4", "التفسير", "#FD10F1", 1], [11, 2, 4, 1, "5/6", "التفسير", "#77C5FC", 0], [11, 3, 1, 1, "3/4", "التحويد", "#EDDE32", 0], [11, 3, 4, 1, "5/3", "التفسير", "#626FE6", 1], [11, 4, 1, 1, "5/4", "التفسير", "#FD10F1", 1], [11, 4, 2, 1, "5/7", "التفسير", "#F18907", 0], [11, 4, 3, 1, "5/5", "التفسير", "#7B5C0A", 1], [11, 5, 0, 2, "3/6", "القرءان", "#8F0440", 1], [11, 5, 2, 1, "AEP1", "التفسير", "#8DB43B", 0], [11, 5, 3, 1, "3/4", "التحويد", "#EDDE32", 0], [11, 5, 4, 1, "5/1", "التفسير", "#E8BAEB", 0], [12, 0, 1, 1, "7/3", "التفسير", "#E230B3", 1], [12, 0, 2, 1, "6/4", "التفسير", "#FE4673", 0], [12, 1, 1, 1, "C1", "التفسير", "#06DB70", 0], [12, 1, 2, 1, "6/1", "التفسير", "#EBEC69", 0], [12, 1, 3, 1, "C2", "التفسير", "#0A4286", 1], [12, 1, 4, 1, "6/3", "التفسير", "#613964", 1], [12, 2, 0, 2, "3/5", "القرءان", "#839DB6", 0], [12, 2, 2, 1, "7/1", "التفسير", "#68E5BE", 0], [12, 2, 3, 1, "6/3", "التفسير", "#613964", 1], [12, 2, 4, 1, "7/4", "التفسير", "#7D4FA4", 1], [12, 3, 0, 1, "7/1", "التفسير", "#68E5BE", 0], [12, 3, 1, 1, "6/4", "التفسير", "#FE4673", 0], [12, 3, 2, 1, "7/4", "التفسير", "#7D4FA4", 1], [12, 3, 3, 1, "7/3", "التفسير", "#E230B3", 1], [12, 3, 4, 1, "C2", "التفسير", "#0A4286", 1], [12, 4, 0, 2, "3/5", "القرءان", "#839DB6", 0], [12, 4, 3, 1, "6/1", "التفسير", "#EBEC69", 0], [12, 4, 4, 1, "C1", "التفسير", "#06DB70", 0], [13, 0, 1, 1, "3/5", "التفسير", "#7DF10E", 0], [13, 0, 2, 1, "2/3", "التفسير", "#E7CB35", 0], [13, 0, 3, 1, "3/4", "التفسير", "#FBBDF5", 0], [13, 0, 4, 1, "2/2", "التفسير", "#6187CE", 0], [13, 2, 1, 1, "3/1", "التفسير", "#EE17EF", 1], [13, 2, 2, 1, "3/3", "التفسير", "#64C2E2", 0], [13, 2, 3, 1, "3/2", "التفسير", "#E28E19", 0], [13, 2, 4, 1, "3/6", "التفسير", "#7168F8", 1], [13, 3, 1, 1, "2/4", "التفسير", "#78B422", 0], [13, 3, 2, 1, "3/3", "التفسير", "#64C2E2", 0], [13, 3, 4, 1, "2/3", "التفسير", "#E7CB35", 0], [13, 4, 2, 1, "3/6", "التفسير", "#7168F8", 1], [13, 4, 3, 1, "3/1", "التفسير", "#EE17EF", 1], [13, 4, 4, 1, "3/4", "التفسير", "#FBBDF5", 0], [13, 5, 1, 1, "3/2", "التفسير", "#E28E19", 0], [13, 5, 2, 1, "2/4", "التفسير", "#78B422", 0], [13, 5, 3, 1, "3/5", "التفسير", "#7DF10E", 0], [13, 5, 4, 1, "2/2", "التفسير", "#6187CE", 0], [14, 0, 0, 1, "4/2", "التفسير", "#672ACA", 1], [14, 0, 1, 1, "4/6", "التفسير", "#F4CC2B", 0], [14, 0, 4, 1, "4/4", "التفسير", "#7E1926", 1], [14, 1, 0, 1, "4/7", "التفسير", "#7280D0", 0], [14, 1, 1, 1, "3/7", "التفسير", "#F72403", 1], [14, 1, 2, 1, "4/3", "التفسير", "#E16631", 0], [14, 1, 3, 1, "ت2", "التفسير", "#E3F82E", 0], [14, 1, 4, 1, "ت3", "التفسير", "#65B4D5", 0], [14, 3, 0, 1, "4/1", "التفسير", "#6BB33C", 0], [14, 3, 3, 1, "4/7", "التفسير", "#7280D0", 0], [14, 3, 4, 1, "4/5", "التفسير", "#F855DD", 0], [14, 4, 1, 1, "4/6", "التفسير", "#F4CC2B", 0], [14, 4, 2, 1, "4/2", "التفسير", "#672ACA", 1], [14, 4, 3, 1, "4/4", "التفسير", "#7E1926", 1], [14, 4, 4, 1, "ت1", "التفسير", "#EF61D8", 0], [14, 5, 0, 1, "4/1", "التفسير", "#6BB33C", 0], [14, 5, 1, 1, "4/5", "التفسير", "#F855DD", 0], [14, 5, 2, 1, "3/7", "التفسير", "#F72403", 1], [14, 5, 3, 1, "ت6", "التفسير", "#701ECF", 1], [14, 5, 4, 1, "4/3", "التفسير", "#E16631", 0], [15, 0, 0, 1, "9/2", "الحديث", "#E25AD6", 0], [15, 0, 1, 1, "8/2", "الحديث", "#615301", 1], [15, 0, 3, 1, "8/3", "الحديث", "#E71FFA", 1], [15, 0, 4, 1, "8/3", "مصطلح الحديث", "#362FA6", 1], [15, 2, 0, 1, "8/3", "الحديث", "#E71FFA", 1], [15, 2, 1, 1, "9/2", "مصطلح الحديث", "#336A8A", 1], [15, 2, 2, 1, "9/1", "مصطلح الحديث", "#3FF37C", 0], [15, 2, 3, 1, "10/1", "مصطلح الحديث", "#7A93EC", 0], [15, 3, 0, 1, "8/2", "مصطلح الحديث", "#B0635D", 1], [15, 3, 1, 1, "9/2", "الحديث", "#E25AD6", 0], [15, 4, 1, 1, "9/1", "الحديث", "#EEC320", 0], [15, 4, 2, 1, "8/2", "الحديث", "#615301", 1], [15, 4, 3, 1, "8/1", "الحديث", "#6DCAF7", 0], [15, 4, 4, 1, "10/1", "الحديث", "#2329E8", 1], [15, 5, 0, 1, "8/1", "الحديث", "#6DCAF7", 0], [15, 5, 2, 1, "8/1", "مصطلح الحديث", "#BCFAAB", 0], [15, 5, 3, 1, "9/1", "الحديث", "#EEC320", 0], [16, 0, 0, 1, "5/1", "الحديث", "#E39928", 0], [16, 0, 1, 1, "ت5", "الحديث", "#77A4FA", 0], [16, 0, 2, 1, "7/2", "الحديث", "#6F5F8B", 1], [16, 0, 3, 1, "C1", "الحديث", "#F88B9A", 0], [16, 0, 4, 1, "C2", "الحديث", "#F4126C", 1], [16, 2, 0, 2, "7/2", "القرءان", "#9A10F0", 1], [16, 2, 2, 1, "7/2", "الحديث", "#6F5F8B", 1], [16, 2, 4, 1, "ت4", "الحديث", "#F1E801", 0], [16, 3, 3, 1, "ت4", "الحديث", "#F1E801", 0], [16, 3, 4, 1, "5/2", "الحديث", "#EF00DE", 1], [16, 4, 0, 1, "C1", "الحديث", "#F88B9A", 0], [16, 4, 1, 1, "5/2", "الحديث", "#EF00DE", 1], [16, 4, 3, 1, "C2", "الحديث", "#F4126C", 1], [16, 4, 4, 1, "6/2", "الحديث", "#EC565C", 0], [16, 5, 0, 2, "7/2", "القرءان", "#9A10F0", 1], [16, 5, 2, 1, "5/1", "الحديث", "#E39928", 0], [16, 5, 3, 1, "6/2", "الحديث", "#EC565C", 0], [16, 5, 4, 1, "ت5", "الحديث", "#77A4FA", 0], [17, 0, 0, 1, "4/3", "الحديث", "#EA45F2", 0], [17, 0, 1, 1, "5/2", "كماهيران بهاس", "#C9A9F7", 0], [17, 0, 2, 1, "AEP1", "الحديث", "#036FF4", 1], [17, 0, 3, 1, "2/5", "الحديث", "#F5DB1A", 0], [17, 0, 4, 1, "4/6", "الحديث", "#FFEFE8", 0], [17, 2, 0, 2, "4/6", "القرءان", "#0AA093", 1], [17, 2, 2, 1, "4/3", "الحديث", "#EA45F2", 0], [17, 2, 3, 1, "2/4", "الحديث", "#7397E1", 0], [17, 2, 4, 1, "4/6", "الحديث", "#FFEFE8", 0], [17, 3, 1, 1, "4/7", "الحديث", "#79A313", 0], [17, 3, 3, 1, "4/1", "الحديث", "#6090FF", 0], [17, 3, 4, 1, "2/5", "الحديث", "#F5DB1A", 0], [17, 4, 2, 1, "5/2", "كماهيران بهاس", "#C9A9F7", 0], [17, 4, 4, 1, "4/7", "الحديث", "#79A313", 0], [17, 5, 0, 2, "4/6", "القرءان", "#0AA093", 1], [17, 5, 2, 1, "4/1", "الحديث", "#6090FF", 0], [17, 5, 3, 1, "AEP1", "الحديث", "#036FF4", 1], [17, 5, 4, 1, "2/4", "الحديث", "#7397E1", 0], [18, 0, 0, 1, "5/3", "الحديث", "#694C25", 1], [18, 0, 1, 1, "5/6", "الحديث", "#7CE63F", 0], [18, 0, 2, 1, "5/4", "الحديث", "#F63332", 1], [18, 0, 3, 1, "6/3", "الحديث", "#6A1AA7", 1], [18, 1, 0, 1, "4/6", "سني توليسن", "#A220AC", 1], [18, 1, 1, 1, "6/2", "النصوص", "#CED6B7", 0], [18, 1, 2, 1, "6/4", "الحديث", "#F565B0", 0], [18, 1, 3, 1, "4/7", "سني توليسن", "#246C57", 1], [18, 1, 4, 1, "5/7", "الحديث", "#FAAAC4", 0], [18, 3, 0, 1, "5/3", "الحديث", "#694C25", 1], [18, 3, 1, 1, "5/6", "الحديث", "#7CE63F", 0], [18, 3, 3, 1, "5/7", "الحديث", "#FAAAC4", 0], [18, 3, 4, 1, "7/2", "النصوص", "#4DDF60", 0], [18, 4, 0, 1, "5/4", "الحديث", "#F63332", 1], [18, 4, 2, 1, "5/5", "الحديث", "#707FC9", 0], [18, 4, 3, 1, "4/1", "سني توليسن", "#3D5FBB", 1], [18, 5, 0, 1, "6/3", "الحديث", "#6A1AA7", 1], [18, 5, 1, 1, "4/2", "سني توليسن", "#31C64D", 0], [18, 5, 2, 1, "5/5", "الحديث", "#707FC9", 0], [18, 5, 4, 1, "6/4", "الحديث", "#F565B0", 0], [19, 1, 2, 1, "2/2", "الحديث", "#6AA40D", 0], [19, 1, 3, 1, "3/2", "الحديث", "#E9ADDA", 0], [19, 1, 4, 1, "2/3", "الحديث", "#ECE8F6", 0], [19, 2, 0, 1, "2/2", "الحديث", "#6AA40D", 0], [19, 2, 1, 1, "4/2", "الحديث", "#6C0909", 1], [19, 2, 2, 1, "3/7", "الحديث", "#FC07C0", 1], [19, 2, 3, 1, "3/1", "الحديث", "#E5342C", 1], [19, 2, 4, 1, "3/3", "الحديث", "#6FE121", 0], [19, 3, 0, 1, "3/4", "الحديث", "#F09E36", 0], [19, 3, 2, 1, "4/2", "الحديث", "#6C0909", 1], [19, 3, 3, 1, "3/6", "الحديث", "#7A4B3B", 1], [19, 3, 4, 1, "3/3", "الحديث", "#6FE121", 0], [19, 4, 2, 1, "3/7", "الحديث", "#FC07C0", 1], [19, 4, 3, 1, "3/5", "الحديث", "#76D2CD", 0], [19, 4, 4, 1, "3/2", "الحديث", "#E9ADDA", 0], [19, 5, 0, 1, "3/1", "الحديث", "#E5342C", 1], [19, 5, 1, 1, "2/3", "الحديث", "#ECE8F6", 0], [19, 5, 2, 1, "3/5", "الحديث", "#76D2CD", 0], [19, 5, 3, 1, "3/6", "الحديث", "#7A4B3B", 1], [19, 5, 4, 1, "3/4", "الحديث", "#F09E36", 0], [20, 0, 0, 1, "4/5", "الحديث", "#F3761E", 0], [20, 0, 1, 1, "ت3", "الحديث", "#6E9716", 1], [20, 0, 2, 1, "ت1", "الحديث", "#E4421B", 1], [20, 0, 4, 1, "6/1", "الحديث", "#E0CFAA", 0], [20, 1, 0, 2, "5/7", "القرءان", "#0FE5BF", 0], [20, 1, 2, 1, "7/4", "الحديث", "#766C67", 1], [20, 1, 3, 1, "7/1", "الحديث", "#63C67D", 0], [20, 1, 4, 1, "ت2", "الحديث", "#E8DBED", 0], [20, 2, 0, 1, "7/1", "الحديث", "#63C67D", 0], [20, 2, 2, 1, "6/1", "الحديث", "#E0CFAA", 0], [20, 2, 3, 1, "ت3", "الحديث", "#6E9716", 1], [20, 2, 4, 1, "7/3", "الحديث", "#E91370", 1], [20, 3, 2, 1, "7/3", "الحديث", "#E91370", 1], [20, 3, 3, 1, "ت2", "الحديث", "#E8DBED", 0], [20, 3, 4, 1, "7/4", "الحديث", "#766C67", 1], [20, 4, 0, 2, "5/7", "القرءان", "#0FE5BF", 0], [20, 4, 2, 1, "4/5", "الحديث", "#F3761E", 0], [20, 4, 3, 1, "ت1", "الحديث", "#E4421B", 1], [21, 0, 0, 1, "7/4", "التوحيد", "#0420D7", 1], [21, 0, 1, 1, "ت6", "التوحيد", "#0971BC", 1], [21, 0, 2, 1, "ت4", "التوحيد", "#83A4B1", 0], [21, 0, 3, 1, "7/3", "التوحيد", "#9B5FC0", 1], [21, 0, 4, 1, "7/1", "التوحيد", "#118ACD", 1], [21, 1, 0, 2, "8/2", "القرءان", "#941C7A", 1], [21, 1, 3, 1, "ت5", "التوحيد", "#05E84A", 0], [21, 1, 4, 1, "7/4", "التوحيد", "#0420D7", 1], [21, 2, 0, 1, "8/2", "العروض", "#F6AC70", 0], [21, 2, 1, 1, "7/1", "التوحيد", "#118ACD", 1], [21, 2, 2, 1, "8/1", "العروض", "#FA3586", 1], [21, 2, 4, 1, "ت5", "التوحيد", "#05E84A", 0], [21, 3, 2, 1, "8/3", "العروض", "#70E08B", 0], [21, 3, 3, 1, "ت6", "التوحيد", "#0971BC", 1], [21, 4, 0, 1, "8/2", "القرءان", "#941C7A", 1], [21, 4, 1, 1, "10/1", "التوحيد", "#357057", 1], [21, 4, 2, 1, "7/3", "التوحيد", "#9B5FC0", 1], [21, 4, 4, 1, "ت4", "التوحيد", "#83A4B1", 0], [22, 0, 1, 1, "ت1", "التوحيد", "#960EAB", 1], [22, 0, 2, 1, "ت3", "التوحيد", "#1CDBA6", 0], [22, 0, 3, 1, "5/3", "التوحيد", "#1B0095", 1], [22, 0, 4, 1, "ت2", "التوحيد", "#9A975D", 0], [22, 2, 0, 1, "4/2", "التوحيد", "#1E45B9", 1], [22, 2, 1, 1, "4/3", "التوحيد", "#980942", 1], [22, 2, 2, 1, "4/7", "التوحيد", "#0BEFA3", 0], [22, 2, 3, 1, "ت1", "التوحيد", "#960EAB", 1], [22, 2, 4, 1, "4/5", "التوحيد", "#813AAE", 1], [22, 3, 1, 1, "5/3", "التوحيد", "#1B0095", 1], [22, 3, 2, 1, "4/6", "التوحيد", "#8DA358", 0], [22, 3, 3, 1, "ت3", "التوحيد", "#1CDBA6", 0], [22, 4, 0, 1, "4/6", "التوحيد", "#8DA358", 0], [22, 4, 1, 1, "4/4", "التوحيد", "#077655", 1], [22, 4, 3, 1, "ت2", "التوحيد", "#9A975D", 0], [22, 5, 0, 1, "4/7", "التوحيد", "#0BEFA3", 0], [22, 5, 1, 1, "4/4", "التوحيد", "#077655", 1], [22, 5, 2, 1, "4/2", "التوحيد", "#1E45B9", 1], [22, 5, 3, 1, "4/3", "التوحيد", "#980942", 1], [22, 5, 4, 1, "4/5", "التوحيد", "#813AAE", 1], [23, 1, 0, 2, "4/4", "القرءان", "#80759E", 1], [23, 1, 2, 1, "5/5", "التوحيد", "#023379", 1], [23, 1, 3, 1, "5/6", "التوحيد", "#0EAA8F", 1], [23, 1, 4, 1, "5/1", "التوحيد", "#91D598", 0], [23, 2, 0, 1, "6/4", "التوحيد", "#872900", 1], [23, 2, 2, 1, "6/3", "التوحيد", "#185617", 1], [23, 2, 3, 1, "4/1", "التوحيد", "#12DC4F", 0], [23, 2, 4, 1, "5/7", "التوحيد", "#88E674", 0], [23, 3, 0, 2, "4/4", "القرءان", "#80759E", 1], [23, 3, 2, 1, "6/1", "التوحيد", "#92831A", 1], [23, 3, 3, 1, "5/5", "التوحيد", "#023379", 1], [23, 3, 4, 1, "6/3", "التوحيد", "#185617", 1], [23, 4, 2, 1, "5/6", "التوحيد", "#0EAA8F", 1], [23, 4, 4, 1, "6/4", "التوحيد", "#872900", 1], [23, 5, 0, 1, "5/1", "التوحيد", "#91D598", 0], [23, 5, 1, 1, "6/1", "التوحيد", "#92831A", 1], [23, 5, 3, 1, "4/1", "التوحيد", "#12DC4F", 0], [23, 5, 4, 1, "5/7", "التوحيد", "#88E674", 0], [24, 0, 0, 1, "2/3", "التوحيد", "#9EA446", 0], [24, 0, 1, 1, "3/1", "التوحيد", "#97789C", 0], [24, 0, 2, 1, "3/2", "التوحيد", "#9BE16A", 0], [24, 0, 3, 1, "2/2", "التوحيد", "#18E8BD", 0], [24, 0, 4, 1, "2/4", "التوحيد", "#01DB51", 0], [24, 1, 0, 2, "2/4", "القرءان", "#86D89A", 0], [24, 1, 2, 1, "2/5", "التوحيد", "#8797AA", 0], [24, 1, 3, 1, "3/7", "بهاس ملايو", "#80FEA7", 0], [24, 1, 4, 1, "3/2", "التوحيد", "#9BE16A", 0], [24, 3, 1, 1, "2/3", "التوحيد", "#9EA446", 0], [24, 3, 3, 1, "3/7", "بهاس ملايو", "#80FEA7", 0], [24, 3, 4, 1, "3/6", "بهاس ملايو", "#06B25C", 1], [24, 4, 1, 1, "2/4", "التوحيد", "#01DB51", 0], [24, 4, 2, 1, "2/5", "التوحيد", "#8797AA", 0], [24, 5, 0, 2, "2/4", "القرءان", "#86D89A", 0], [24, 5, 2, 1, "3/6", "بهاس ملايو", "#06B25C", 1], [24, 5, 3, 1, "2/2", "التوحيد", "#18E8BD", 0], [24, 5, 4, 1, "3/1", "التوحيد", "#97789C", 0], [25, 0, 0, 1, "3/4", "التوحيد", "#82D286", 0], [25, 0, 1, 1, "3/6", "التوحيد", "#08078B", 1], [25, 0, 2, 1, "2/4", "جاوي", "#1E662D", 1], [25, 0, 4, 1, "3/5", "التوحيد", "#049E7D", 1], [25, 1, 0, 2, "2/5", "القرءان", "#009461", 1], [25, 1, 2, 1, "3/6", "التوحيد", "#08078B", 1], [25, 1, 3, 1, "2/4", "جاوي", "#1E662D", 1], [25, 1, 4, 1, "3/4", "التوحيد", "#82D286", 0], [25, 3, 0, 1, "2/5", "بهاس ملايو", "#89227D", 1], [25, 3, 2, 1, "3/7", "التوحيد", "#8E4B70", 1], [25, 3, 3, 1, "3/3", "التوحيد", "#1DAD91", 1], [25, 4, 0, 2, "2/5", "القرءان", "#009461", 1], [25, 4, 2, 1, "2/4", "جاوي", "#1E662D", 1], [25, 4, 4, 1, "2/5", "بهاس ملايو", "#89227D", 1], [25, 5, 0, 1, "3/7", "التوحيد", "#8E4B70", 1], [25, 5, 1, 1, "3/3", "التوحيد", "#1DAD91", 1], [25, 5, 3, 1, "2/5", "بهاس ملايو", "#89227D", 1], [25, 5, 4, 1, "3/5", "التوحيد", "#049E7D", 1], [26, 0, 0, 1, "7/2", "الفقه", "#7C39E3", 1], [26, 0, 1, 1, "6/4", "الفرائض", "#59E803", 0], [26, 0, 2, 1, "6/2", "الفرائض", "#40DBEF", 0], [26, 0, 3, 1, "5/7", "الفرائض", "#562777", 1], [26, 2, 0, 2, "7/4", "القرءان", "#83231C", 1], [26, 2, 3, 1, "6/4", "الفرائض", "#59E803", 0], [26, 2, 4, 1, "6/3", "الفرائض", "#C69714", 0], [26, 3, 0, 1, "5/7", "الفرائض", "#562777", 1], [26, 3, 1, 1, "7/2", "الفقه", "#7C39E3", 1], [26, 3, 2, 1, "5/2", "الفرائض", "#438D6D", 1], [26, 3, 3, 1, "6/1", "الفرائض", "#4C4219", 1], [26, 4, 0, 1, "5/2", "الفرائض", "#438D6D", 1], [26, 4, 3, 1, "6/2", "الفرائض", "#40DBEF", 0], [26, 5, 0, 2, "7/4", "القرءان", "#83231C", 1], [26, 5, 2, 1, "6/1", "الفرائض", "#4C4219", 1], [26, 5, 4, 1, "6/3", "الفرائض", "#C69714", 0], [27, 0, 0, 1, "7/3", "الفرائض", "#459EC3", 0], [27, 0, 1, 1, "7/1", "الفرائض", "#CF4BCE", 0], [27, 0, 2, 1, "6/3", "الفقه", "#797CCF", 0], [27, 0, 3, 1, "7/4", "الفرائض", "#DAE1D4", 0], [27, 0, 4, 1, "6/2", "الفقه", "#FF3034", 1], [27, 1, 0, 2, "C2", "الفقه", "#E057A2", 0], [27, 1, 2, 1, "7/2", "الفرائض", "#C3D238", 0], [27, 1, 4, 1, "6/2", "الفقه", "#FF3034", 1], [27, 2, 0, 1, "C4", "الفقه المعاصر", "#4B85E5", 1], [27, 2, 1, 1, "6/4", "الفقه", "#E603D8", 1], [27, 2, 3, 1, "5/2", "الفقه", "#FC66B6", 0], [27, 2, 4, 1, "7/1", "الفرائض", "#CF4BCE", 0], [27, 3, 1, 1, "5/1", "الفقه", "#F0FF40", 0], [27, 3, 2, 1, "6/3", "الفقه", "#797CCF", 0], [27, 3, 3, 1, "5/2", "الفقه", "#FC66B6", 0], [27, 3, 4, 1, "6/4", "الفقه", "#E603D8", 1], [27, 4, 0, 1, "C4", "الفقه المعاصر", "#4B85E5", 1], [27, 4, 3, 1, "5/1", "الفقه", "#F0FF40", 0], [27, 4, 4, 1, "C2", "الفقه", "#E057A2", 0], [28, 1, 0, 1, "5/1", "الفرائض", "#4F149B", 1], [28, 1, 1, 2, "C5", "القرءان", "#A93805", 1], [28, 1, 4, 1, "5/6", "الفرائض", "#D06B8C", 0], [28, 2, 0, 1, "5/3", "الفرائض", "#C5C196", 0], [28, 2, 1, 1, "C4", "الفرائض", "#6A2135", 1], [28, 2, 2, 1, "C5", "الفرائض", "#EC6DCE", 0], [28, 2, 3, 1, "AEP1", "الفرائض", "#832D61", 1], [28, 2, 4, 1, "5/5", "الفرائض", "#DCF27A", 0], [28, 3, 1, 1, "C5", "الفرائض", "#EC6DCE", 0], [28, 3, 2, 1, "C4", "الفرائض", "#6A2135", 1], [28, 3, 3, 1, "5/1", "الفرائض", "#4F149B", 1], [28, 3, 4, 1, "5/4", "الفرائض", "#5ABE81", 0], [28, 4, 1, 2, "C5", "القرءان", "#A93805", 1], [28, 4, 4, 1, "5/5", "الفرائض", "#DCF27A", 0], [28, 5, 0, 1, "5/3", "الفرائض", "#C5C196", 0], [28, 5, 2, 1, "5/4", "الفرائض", "#5ABE81", 0], [28, 5, 3, 1, "5/6", "الفرائض", "#D06B8C", 0], [29, 0, 0, 1, "3/5", "الفقه", "#65B4A5", 0], [29, 0, 1, 2, "4/7", "القرءان", "#8CEC68", 0], [29, 0, 3, 2, "3/7", "الفقه", "#EF61A8", 0], [29, 2, 0, 1, "C5", "النشاط", "#F4AFB2", 0], [29, 2, 1, 1, "5/2", "الأخلاق", "#3BEAAD", 0], [29, 2, 2, 2, "3/6", "الفقه", "#692D53", 1], [29, 2, 4, 1, "7/2", "الأخلاق", "#BBB5F8", 0], [29, 3, 1, 2, "3/5", "الفقه", "#65B4A5", 0], [29, 3, 4, 1, "6/2", "الأخلاق", "#38BC2F", 0], [29, 4, 1, 1, "3/6", "الفقه", "#692D53", 1], [29, 4, 4, 1, "5/2", "الأخلاق", "#3BEAAD", 0], [29, 5, 0, 1, "6/2", "الأخلاق", "#38BC2F", 0], [29, 5, 1, 1, "3/7", "الفقه", "#EF61A8", 0], [29, 5, 2, 2, "4/7", "القرءان", "#8CEC68", 0], [29, 5, 4, 1, "7/2", "الأخلاق", "#BBB5F8", 0], [30, 0, 0, 1, "9/1", "أصول الفقه", "#A8931C", 0], [30, 0, 1, 1, "7/4", "الفقه", "#650A0F", 1], [30, 0, 2, 1, "8/3", "أصول الفقه", "#A14FC6", 1], [30, 0, 3, 1, "ت5", "الفقه", "#64C292", 0], [30, 0, 4, 1, "7/3", "الفقه", "#FA7518", 0], [30, 1, 0, 2, "5/3", "القرءان", "#9C035E", 1], [30, 1, 2, 1, "7/1", "الفقه", "#70A015", 0], [30, 1, 3, 1, "9/2", "أصول الفقه", "#A40AEA", 1], [30, 1, 4, 1, "ت5", "الفقه", "#64C292", 0], [30, 3, 2, 1, "7/1", "الفقه", "#70A015", 0], [30, 4, 0, 2, "5/3", "القرءان", "#9C035E", 1], [30, 4, 2, 1, "8/1", "أصول الفقه", "#2B9ACB", 1], [30, 4, 3, 1, "7/4", "الفقه", "#650A0F", 1], [30, 4, 4, 1, "ت6", "الفقه", "#685B64", 1], [30, 5, 0, 1, "7/3", "الفقه", "#FA7518", 0], [30, 5, 2, 1, "10/1", "أصول الفقه", "#7385D6", 0], [30, 5, 3, 1, "8/2", "أصول الفقه", "#27033D", 1], [30, 5, 4, 1, "ت6", "الفقه", "#685B64", 1], [31, 0, 0, 1, "ت1", "الفقه", "#F72473", 1], [31, 0, 1, 1, "ت4", "الفقه", "#E28E69", 0], [31, 0, 2, 1, "5/6", "الفقه", "#6F8057", 1], [31, 0, 3, 1, "ت2", "الفقه", "#FBBD85", 0], [31, 0, 4, 1, "ت3", "الفقه", "#7DF17E", 0], [31, 2, 0, 2, "5/5", "القرءان", "#8530B2", 1], [31, 2, 2, 1, "5/3", "الفقه", "#7A2A4D", 1], [31, 2, 3, 1, "ت4", "الفقه", "#E28E69", 0], [31, 2, 4, 1, "5/4", "الفقه", "#E5555A", 0], [31, 3, 0, 1, "5/4", "الفقه", "#E5555A", 0], [31, 3, 1, 1, "5/7", "الفقه", "#E9CCAC", 0], [31, 3, 3, 1, "5/3", "الفقه", "#7A2A4D", 1], [31, 3, 4, 1, "ت2", "الفقه", "#FBBD85", 0], [31, 4, 3, 1, "ت3", "الفقه", "#7DF17E", 0], [31, 4, 4, 1, "5/6", "الفقه", "#6F8057", 1], [31, 5, 0, 2, "5/5", "القرءان", "#8530B2", 1], [31, 5, 2, 1, "5/7", "الفقه", "#E9CCAC", 0], [31, 5, 3, 1, "ت1", "الفقه", "#F72473", 1], [32, 0, 0, 1, "4/1", "الفقه", "#73F697", 0], [32, 0, 1, 1, "4/5", "الفقه", "#E01076", 1], [32, 0, 2, 1, "4/6", "الفقه", "#EC8980", 0], [32, 0, 3, 1, "4/4", "الفقه", "#665C8D", 1], [32, 0, 4, 1, "4/7", "الفقه", "#6AC57B", 0], [32, 1, 0, 1, "4/1", "الفقه", "#73F697", 0], [32, 1, 1, 1, "4/5", "الفقه", "#E01076", 1], [32, 1, 2, 1, "4/2", "الفقه", "#7F6F61", 1], [32, 1, 3, 1, "4/3", "الفقه", "#F9239A", 1], [32, 1, 4, 1, "4/6", "الفقه", "#EC8980", 0], [32, 2, 0, 1, "4/3", "الفقه", "#F9239A", 1], [32, 2, 1, 1, "4/7", "الفقه", "#6AC57B", 0], [32, 2, 2, 1, "4/6", "الفقه", "#EC8980", 0], [32, 2, 3, 1, "4/2", "الفقه", "#7F6F61", 1], [32, 2, 4, 1, "4/4", "الفقه", "#665C8D", 1], [32, 3, 3, 1, "4/5", "الفقه", "#E01076", 1], [32, 3, 4, 1, "4/3", "الفقه", "#F9239A", 1], [32, 4, 0, 1, "4/4", "الفقه", "#665C8D", 1], [32, 4, 1, 1, "4/7", "الفقه", "#6AC57B", 0], [32, 4, 4, 1, "4/2", "الفقه", "#7F6F61", 1], [33, 0, 0, 1, "2/1", "النحو والصرف", "#30BAC1", 0], [33, 0, 2, 1, "3/3", "الفقه", "#7C8749", 1], [33, 0, 3, 1, "9/1", "النحو والصرف", "#B8441A", 1], [33, 1, 0, 1, "7/2", "أصول الفقه", "#290FB7", 1], [33, 1, 1, 1, "7/4", "أصول الفقه", "#303C5B", 1], [33, 1, 2, 1, "9/2", "النحو والصرف", "#B4DDEC", 0], [33, 1, 3, 1, "7/3", "أصول الفقه", "#AF434C", 1], [33, 1, 4, 1, "4/5", "النحو", "#27BE58", 0], [33, 3, 0, 1, "C5", "الفقه المعاصر", "#CDC91E", 0], [33, 3, 2, 1, "4/5", "النحو", "#27BE58", 0], [33, 3, 3, 1, "2/1", "النحو والصرف", "#30BAC1", 0], [33, 3, 4, 1, "7/1", "أصول الفقه", "#259641", 1], [33, 4, 0, 1, "9/2", "النحو والصرف", "#B4DDEC", 0], [33, 4, 2, 1, "3/3", "الفقه", "#7C8749", 1], [33, 4, 3, 1, "10/1", "النحو والصرف", "#61CD5F", 0], [33, 4, 4, 1, "2/1", "النحو والصرف", "#30BAC1", 0], [33, 5, 0, 1, "9/1", "النحو والصرف", "#B8441A", 1], [33, 5, 1, 1, "10/1", "النحو والصرف", "#61CD5F", 0], [33, 5, 2, 1, "C5", "الفقه المعاصر", "#CDC91E", 0], [33, 5, 4, 1, "3/3", "الفقه", "#7C8749", 1], [34, 0, 0, 1, "3/1", "النحو والصرف", "#B3B316", 0], [34, 0, 1, 1, "3/2", "الفقه", "#FACBB2", 0], [34, 0, 2, 1, "5/7", "المطالعة والإملاء", "#CDF605", 0], [34, 0, 3, 1, "4/6", "النحو", "#2B27AE", 1], [34, 0, 4, 1, "5/3", "المحادثة", "#F5DC4E", 0], [34, 1, 0, 1, "3/4", "الفقه", "#E3F85E", 0], [34, 1, 1, 1, "5/4", "المطالعة والإملاء", "#C16FF3", 0], [34, 1, 3, 1, "4/4", "المطالعة والإملاء", "#426624", 1], [34, 3, 0, 1, "3/2", "الفقه", "#FACBB2", 0], [34, 3, 1, 1, "4/6", "النحو", "#2B27AE", 1], [34, 3, 2, 1, "5/7", "المطالعة والإملاء", "#CDF605", 0], [34, 3, 3, 1, "3/1", "النحو والصرف", "#B3B316", 0], [34, 3, 4, 1, "5/5", "الفقه", "#6319A1", 1], [34, 4, 0, 1, "5/5", "الفقه", "#6319A1", 1], [34, 4, 2, 1, "3/1", "النحو والصرف", "#B3B316", 0], [34, 4, 3, 1, "3/4", "الفقه", "#E3F85E", 0], [34, 5, 0, 1, "4/4", "المطالعة والإملاء", "#426624", 1], [34, 5, 1, 1, "3/4", "الفقه", "#E3F85E", 0], [34, 5, 2, 1, "5/3", "المحادثة", "#F5DC4E", 0], [34, 5, 3, 1, "5/4", "المطالعة والإملاء", "#C16FF3", 0], [34, 5, 4, 1, "3/2", "الفقه", "#FACBB2", 0], [35, 0, 0, 1, "6/2", "التاريخ الإسلامي", "#CDD8FF", 0], [35, 0, 1, 1, "2/1", "التاريخ الإسلامي", "#47B358", 0], [35, 0, 2, 1, "8/1", "التاريخ الإسلامي", "#4C4454", 1], [35, 0, 3, 1, "5/2", "التاريخ الإسلامي", "#CE8E7D", 0], [35, 1, 0, 2, "5/6", "القرءان", "#89A944", 0], [35, 1, 3, 1, "8/3", "التاريخ الإسلامي", "#C69159", 0], [35, 1, 4, 1, "2/1", "التاريخ الإسلامي", "#47B358", 0], [35, 2, 2, 1, "8/3", "التاريخ الإسلامي", "#C69159", 0], [35, 3, 0, 1, "7/2", "التاريخ الإسلامي", "#4ED128", 0], [35, 3, 1, 1, "6/2", "التاريخ الإسلامي", "#CDD8FF", 0], [35, 3, 2, 1, "8/1", "التاريخ الإسلامي", "#4C4454", 1], [35, 3, 3, 1, "10/1", "التاريخ الإسلامي", "#2717FA", 1], [35, 3, 4, 1, "9/2", "النشاط", "#E864D5", 0], [35, 4, 0, 2, "5/6", "القرءان", "#89A944", 0], [35, 4, 2, 1, "7/2", "التاريخ الإسلامي", "#4ED128", 0], [36, 0, 0, 1, "8/3", "التاريخ التشريعي", "#F43395", 1], [36, 0, 1, 1, "4/4", "التاريخ الإسلامي", "#54B446", 0], [36, 0, 2, 1, "9/1", "التاريخ التشريعي", "#FDEF4F", 0], [36, 0, 3, 1, "4/5", "التاريخ الإسلامي", "#D2F8BD", 0], [36, 1, 0, 1, "8/1", "التاريخ التشريعي", "#7EE698", 0], [36, 1, 1, 1, "4/1", "التاريخ الإسلامي", "#411E5C", 1], [36, 1, 2, 1, "4/5", "التاريخ الإسلامي", "#D2F8BD", 0], [36, 1, 3, 1, "8/2", "التاريخ التشريعي", "#727F6E", 1], [36, 1, 4, 1, "4/2", "التاريخ الإسلامي", "#4D87AA", 1], [36, 2, 0, 1, "10/1", "التاريخ التشريعي", "#C69197", 0], [36, 2, 3, 1, "4/6", "التاريخ الإسلامي", "#DE614B", 0], [36, 2, 4, 1, "4/1", "التاريخ الإسلامي", "#411E5C", 1], [36, 3, 1, 1, "4/3", "التاريخ الإسلامي", "#CBCB51", 0], [36, 3, 2, 1, "4/4", "التاريخ الإسلامي", "#54B446", 0], [36, 3, 3, 1, "9/2", "التاريخ التشريعي", "#F176B9", 0], [36, 3, 4, 1, "4/6", "التاريخ الإسلامي", "#DE614B", 0], [36, 4, 1, 1, "4/2", "التاريخ الإسلامي", "#4D87AA", 1], [36, 4, 4, 1, "4/3", "التاريخ الإسلامي", "#CBCB51", 0], [37, 0, 0, 1, "4/7", "التاريخ الإسلامي", "#582DB0", 1], [37, 0, 1, 1, "AEP1", "التاريخ الإسلامي", "#0751E6", 1], [37, 0, 2, 1, "ت5", "التاريخ الإسلامي", "#562A59", 1], [37, 0, 4, 1, "7/4", "التاريخ الإسلامي", "#57E2C4", 0], [37, 2, 0, 1, "7/3", "التاريخ الإسلامي", "#C89DD3", 0], [37, 2, 1, 1, "6/3", "التاريخ الإسلامي", "#4B9404", 1], [37, 2, 2, 1, "7/4", "التاريخ الإسلامي", "#57E2C4", 0], [37, 2, 4, 1, "8/3", "النشاط", "#ED21F9", 1], [37, 3, 0, 1, "6/4", "التاريخ الإسلامي", "#D4EB13", 0], [37, 3, 1, 1, "7/3", "التاريخ الإسلامي", "#C89DD3", 0], [37, 3, 3, 1, "AEP1", "التاريخ الإسلامي", "#0751E6", 1], [37, 4, 0, 1, "4/7", "التاريخ الإسلامي", "#582DB0", 1], [37, 4, 1, 1, "7/1", "التاريخ الإسلامي", "#4248DE", 1], [37, 4, 2, 1, "6/1", "التاريخ الإسلامي", "#C14109", 1], [37, 4, 3, 1, "6/3", "التاريخ الإسلامي", "#4B9404", 1], [37, 5, 0, 1, "6/1", "التاريخ الإسلامي", "#C14109", 1], [37, 5, 1, 1, "6/4", "التاريخ الإسلامي", "#D4EB13", 0], [37, 5, 3, 1, "ت4", "التاريخ الإسلامي", "#D066A2", 0], [37, 5, 4, 1, "7/1", "التاريخ الإسلامي", "#4248DE", 1], [38, 0, 0, 1, "5/6", "التاريخ الإسلامي", "#5D689C", 1], [38, 0, 1, 1, "5/4", "التاريخ الإسلامي", "#D7BD91", 0], [38, 0, 2, 1, "8/2", "التاريخ الإسلامي", "#40DDA2", 0], [38, 0, 3, 1, "5/5", "التاريخ الإسلامي", "#51F16A", 0], [38, 0, 4, 1, "5/7", "التاريخ الإسلامي", "#DB2467", 1], [38, 1, 2, 1, "5/4", "التاريخ الإسلامي", "#D7BD91", 0], [38, 1, 3, 1, "5/1", "التاريخ الإسلامي", "#C2178B", 1], [38, 1, 4, 1, "9/1", "التاريخ الإسلامي", "#CF4D83", 1], [38, 2, 2, 1, "5/1", "التاريخ الإسلامي", "#C2178B", 1], [38, 2, 3, 1, "5/3", "التاريخ الإسلامي", "#48C286", 0], [38, 2, 4, 1, "9/2", "التاريخ الإسلامي", "#C3D475", 0], [38, 3, 0, 1, "5/6", "التاريخ الإسلامي", "#5D689C", 1], [38, 3, 1, 1, "5/5", "التاريخ الإسلامي", "#51F16A", 0], [38, 3, 4, 1, "8/2", "التاريخ الإسلامي", "#40DDA2", 0], [38, 4, 2, 1, "5/3", "التاريخ الإسلامي", "#48C286", 0], [38, 4, 3, 1, "5/7", "التاريخ الإسلامي", "#DB2467", 1], [39, 1, 0, 2, "3/1", "القرءان", "#107B57", 1], [39, 1, 2, 1, "C1", "التاريخ الإسلامي", "#363842", 1], [39, 1, 3, 1, "2/5", "التاريخ الإسلامي", "#D455B9", 0], [39, 2, 0, 1, "2/3", "التاريخ الإسلامي", "#CD6655", 0], [39, 2, 1, 1, "3/2", "التاريخ الإسلامي", "#C82379", 1], [39, 2, 2, 1, "2/4", "التاريخ الإسلامي", "#521942", 1], [39, 2, 3, 1, "2/5", "التاريخ الإسلامي", "#D455B9", 0], [39, 3, 0, 1, "2/2", "التاريخ الإسلامي", "#4B2AAE", 1], [39, 3, 1, 1, "3/3", "التاريخ الإسلامي", "#4E6F82", 1], [39, 3, 2, 1, "3/2", "التاريخ الإسلامي", "#C82379", 1], [39, 3, 3, 1, "C2", "التاريخ الإسلامي", "#3AA1B4", 0], [39, 4, 0, 2, "3/1", "القرءان", "#107B57", 1], [39, 4, 4, 1, "2/4", "التاريخ الإسلامي", "#521942", 1], [39, 5, 0, 1, "3/3", "التاريخ الإسلامي", "#4E6F82", 1], [39, 5, 1, 1, "2/2", "التاريخ الإسلامي", "#4B2AAE", 1], [39, 5, 2, 1, "2/3", "التاريخ الإسلامي", "#CD6655", 0], [39, 5, 3, 1, "C2", "التاريخ الإسلامي", "#3AA1B4", 0], [39, 5, 4, 1, "C1", "التاريخ الإسلامي", "#363842", 1], [40, 0, 0, 1, "ت3", "التاريخ الإسلامي", "#4F19B5", 1], [40, 0, 1, 1, "ت2", "التاريخ الإسلامي", "#C9554E", 1], [40, 0, 2, 1, "3/6", "التاريخ الإسلامي", "#5BC598", 0], [40, 0, 3, 1, "3/1", "التاريخ الإسلامي", "#C4BA8F", 0], [40, 0, 4, 1, "ت6", "التاريخ الإسلامي", "#5AB3AF", 0], [40, 1, 0, 2, "2/3", "القرءان", "#19A78D", 1], [40, 1, 2, 1, "3/5", "التاريخ الإسلامي", "#575C6E", 1], [40, 1, 3, 1, "3/6", "التاريخ الإسلامي", "#5BC598", 0], [40, 1, 4, 1, "3/7", "التاريخ الإسلامي", "#DD8963", 0], [40, 2, 0, 1, "3/1", "التاريخ الإسلامي", "#C4BA8F", 0], [40, 2, 3, 1, "3/5", "التاريخ الإسلامي", "#575C6E", 1], [40, 2, 4, 1, "4/3", "النحو", "#3E8DB4", 1], [40, 3, 1, 1, "3/7", "التاريخ الإسلامي", "#DD8963", 0], [40, 3, 2, 1, "3/4", "التاريخ الإسلامي", "#D11095", 1], [40, 3, 3, 1, "ت1", "التاريخ الإسلامي", "#C5CCB8", 0], [40, 4, 0, 2, "2/3", "القرءان", "#19A78D", 1], [40, 4, 2, 1, "3/4", "التاريخ الإسلامي", "#D11095", 1], [40, 4, 3, 1, "4/3", "النحو", "#3E8DB4", 1], [41, 0, 0, 1, "3/7", "التحويد", "#E147C4", 0], [41, 0, 1, 1, "5/5", "الأخلاق", "#A495BA", 0], [41, 0, 2, 1, "4/4", "سني توليسن", "#28F5A1", 0], [41, 0, 3, 1, "5/6", "الأخلاق", "#A80C4C", 1], [41, 0, 4, 1, "5/4", "الأخلاق", "#22D941", 0], [41, 1, 0, 2, "6/4", "القرءان", "#002ACB", 1], [41, 1, 2, 1, "5/6", "الأخلاق", "#A80C4C", 1], [41, 1, 4, 1, "5/3", "الأخلاق", "#BDA656", 0], [41, 3, 0, 1, "4/3", "سني توليسن", "#B78AB6", 0], [41, 3, 2, 1, "5/4", "الأخلاق", "#22D941", 0], [41, 3, 4, 1, "5/7", "الأخلاق", "#2E40B7", 1], [41, 4, 0, 2, "6/4", "القرءان", "#002ACB", 1], [41, 4, 3, 1, "5/3", "الأخلاق", "#BDA656", 0], [41, 5, 0, 1, "5/7", "الأخلاق", "#2E40B7", 1], [41, 5, 2, 1, "4/5", "سني توليسن", "#AEB95A", 0], [41, 5, 3, 1, "3/7", "التحويد", "#E147C4", 0], [41, 5, 4, 1, "5/5", "الأخلاق", "#A495BA", 0], [42, 0, 0, 1, "C1", "الأخلاق", "#1E6076", 1], [42, 0, 1, 1, "5/1", "الأخلاق", "#37735B", 1], [42, 0, 2, 1, "4/5", "الصرف", "#3C7DD6", 1], [42, 0, 3, 1, "ت4", "الأخلاق", "#250272", 1], [42, 0, 4, 1, "2/1", "الأخلاق", "#B2D788", 0], [42, 1, 0, 2, "4/3", "القرءان", "#1F0A89", 1], [42, 1, 2, 1, "5/1", "الأخلاق", "#37735B", 1], [42, 1, 3, 1, "2/1", "الأخلاق", "#B2D788", 0], [42, 1, 4, 1, "4/4", "الصرف", "#BA312D", 1], [42, 2, 1, 1, "4/4", "الصرف", "#BA312D", 1], [42, 2, 2, 1, "4/5", "الصرف", "#3C7DD6", 1], [42, 2, 3, 1, "C2", "الأخلاق", "#12F980", 0], [42, 2, 4, 1, "ت6", "الأخلاق", "#AFD77F", 0], [42, 3, 0, 1, "C2", "الأخلاق", "#12F980", 0], [42, 4, 0, 2, "4/3", "القرءان", "#1F0A89", 1], [42, 4, 3, 1, "C1", "الأخلاق", "#1E6076", 1], [42, 4, 4, 1, "ت5", "الأخلاق", "#A34E89", 1], [43, 0, 0, 1, "2/2", "الأخلاق", "#BE4E7E", 1], [43, 0, 1, 1, "2/4", "الأخلاق", "#A77D92", 0], [43, 0, 2, 1, "2/5", "الأخلاق", "#213169", 1], [43, 0, 3, 1, "3/6", "الأخلاق", "#AEA148", 0], [43, 1, 0, 1, "3/7", "الأخلاق", "#28EDB3", 0], [43, 1, 3, 1, "3/5", "الأخلاق", "#A238BE", 1], [43, 2, 0, 2, "3/4", "القرءان", "#05D14D", 0], [43, 2, 2, 1, "3/5", "الأخلاق", "#A238BE", 1], [43, 2, 3, 1, "4/4", "الأخلاق", "#A1D096", 0], [43, 2, 4, 1, "2/4", "الأخلاق", "#A77D92", 0], [43, 3, 0, 1, "4/7", "الأخلاق", "#AD4960", 1], [43, 3, 1, 1, "2/2", "الأخلاق", "#BE4E7E", 1], [43, 3, 2, 1, "2/5", "الأخلاق", "#213169", 1], [43, 3, 4, 1, "4/4", "الأخلاق", "#A1D096", 0], [43, 4, 0, 2, "3/4", "القرءان", "#05D14D", 0], [43, 4, 2, 1, "4/7", "الأخلاق", "#AD4960", 1], [43, 4, 3, 1, "3/7", "الأخلاق", "#28EDB3", 0], [43, 4, 4, 1, "3/6", "الأخلاق", "#AEA148", 0], [44, 0, 0, 1, "3/3", "التحويد", "#72A125", 0], [44, 0, 1, 1, "4/3", "الأخلاق", "#3EAF81", 0], [44, 0, 2, 1, "ت2", "الأخلاق", "#3C319E", 1], [44, 0, 3, 1, "2/3", "الأخلاق", "#380285", 1], [44, 0, 4, 1, "4/2", "الأخلاق", "#B8E37A", 0], [44, 1, 0, 2, "2/2", "القرءان", "#9FEB76", 0], [44, 1, 2, 1, "3/3", "التحويد", "#72A125", 0], [44, 1, 3, 1, "3/1", "الأخلاق", "#31DE5F", 0], [44, 1, 4, 1, "ت1", "الأخلاق", "#30A868", 1], [44, 3, 0, 1, "3/3", "الأخلاق", "#BB0B52", 1], [44, 3, 2, 1, "2/3", "الأخلاق", "#380285", 1], [44, 3, 3, 1, "4/3", "الأخلاق", "#3EAF81", 0], [44, 3, 4, 1, "3/2", "الأخلاق", "#3D47A9", 1], [44, 4, 0, 2, "2/2", "القرءان", "#9FEB76", 0], [44, 4, 3, 1, "3/3", "الأخلاق", "#BB0B52", 1], [44, 4, 4, 1, "ت3", "الأخلاق", "#BA7D65", 0], [44, 5, 1, 1, "3/1", "الأخلاق", "#31DE5F", 0], [44, 5, 3, 1, "3/2", "الأخلاق", "#3D47A9", 1], [44, 5, 4, 1, "4/2", "الأخلاق", "#B8E37A", 0], [45, 0, 0, 1, "AEP1", "الأخلاق", "#9550EA", 1], [45, 0, 2, 1, "7/3", "الأخلاق", "#3DF903", 0], [45, 0, 3, 1, "6/1", "الأخلاق", "#3425D9", 1], [45, 0, 4, 1, "2/5", "المحادثة", "#694B71", 1], [45, 2, 0, 2, "5/1", "القرءان", "#16D653", 0], [45, 2, 2, 1, "6/4", "الأخلاق", "#218FC3", 1], [45, 2, 3, 1, "7/4", "الأخلاق", "#A28614", 0], [45, 2, 4, 1, "2/5", "المحادثة", "#694B71", 1], [45, 3, 1, 1, "7/4", "الأخلاق", "#A28614", 0], [45, 3, 3, 1, "7/1", "الأخلاق", "#B72C0E", 1], [45, 3, 4, 1, "2/1", "المحادثة", "#FAAD90", 0], [45, 4, 0, 2, "5/1", "القرءان", "#16D653", 0], [45, 4, 2, 1, "6/3", "الأخلاق", "#BEF0D4", 0], [45, 4, 3, 1, "7/3", "الأخلاق", "#3DF903", 0], [45, 5, 0, 1, "2/1", "المحادثة", "#FAAD90", 0], [45, 5, 1, 1, "6/3", "الأخلاق", "#BEF0D4", 0], [45, 5, 2, 1, "7/1", "الأخلاق", "#B72C0E", 1], [45, 5, 3, 1, "6/4", "الأخلاق", "#218FC3", 1], [45, 5, 4, 1, "6/1", "الأخلاق", "#3425D9", 1], [46, 0, 0, 1, "2/5", "التفسير", "#FEF8D9", 0], [46, 0, 1, 1, "3/4", "الأخلاق", "#247445", 1], [46, 0, 2, 1, "3/7", "المحادثة", "#6097AB", 0], [46, 0, 3, 1, "4/7", "المطالعة والإملاء", "#4EFFD2", 0], [46, 0, 4, 1, "4/1", "الأخلاق", "#B47A8C", 0], [46, 2, 0, 1, "4/7", "المطالعة والإملاء", "#4EFFD2", 0], [46, 2, 1, 1, "2/2", "المطالعة والإملاء", "#5DF8CC", 0], [46, 2, 2, 1, "4/4", "الحديث", "#753AE5", 1], [46, 2, 3, 1, "3/4", "الأخلاق", "#247445", 1], [46, 2, 4, 1, "3/7", "المحادثة", "#6097AB", 0], [46, 3, 0, 1, "4/5", "الأخلاق", "#279C6D", 1], [46, 3, 1, 1, "3/6", "المحادثة", "#E6DB50", 0], [46, 3, 3, 1, "4/6", "الأخلاق", "#2B059B", 1], [46, 4, 2, 1, "4/1", "الأخلاق", "#B47A8C", 0], [46, 4, 3, 1, "2/2", "المطالعة والإملاء", "#5DF8CC", 0], [46, 4, 4, 1, "4/6", "الأخلاق", "#2B059B", 1], [46, 5, 0, 1, "2/5", "التفسير", "#FEF8D9", 0], [46, 5, 2, 1, "4/4", "الحديث", "#753AE5", 1], [46, 5, 3, 1, "4/5", "الأخلاق", "#279C6D", 1], [46, 5, 4, 1, "3/6", "المحادثة", "#E6DB50", 0], [47, 0, 0, 1, "5/2", "المحادثة", "#7390B5", 0], [47, 0, 3, 1, "6/2", "المحادثة", "#70C637", 0], [47, 0, 4, 1, "7/2", "المحادثة", "#F3CFE0", 0], [47, 1, 0, 2, "7/3", "القرءان", "#1C5C0B", 1], [47, 1, 2, 1, "5/2", "المحادثة", "#7390B5", 0], [47, 1, 3, 1, "7/2", "المحادثة", "#F3CFE0", 0], [47, 3, 2, 1, "9/1", "البلاغة", "#415778", 1], [47, 3, 3, 1, "6/2", "المحادثة", "#70C637", 0], [47, 4, 0, 2, "7/3", "القرءان", "#1C5C0B", 1], [47, 4, 2, 1, "10/1", "البلاغة", "#B6198B", 1], [47, 4, 3, 1, "7/2", "المحادثة", "#F3CFE0", 0], [47, 4, 4, 1, "8/3", "الورشة", "#B2B174", 0], [47, 5, 0, 1, "9/2", "البلاغة", "#4DCE8E", 0], [47, 5, 2, 1, "5/2", "المحادثة", "#7390B5", 0], [47, 5, 4, 1, "6/2", "المحادثة", "#70C637", 0], [48, 0, 0, 1, "3/2", "المطالعة والإملاء", "#DEF11B", 0], [48, 0, 1, 1, "9/1", "الأدب والنصوص", "#E6F609", 0], [48, 0, 2, 1, "4/2", "المطالعة والإملاء", "#5B55C8", 1], [48, 0, 3, 1, "8/1", "الأدب والنصوص", "#65FFDE", 0], [48, 0, 4, 1, "3/3", "المطالعة والإملاء", "#58BDE0", 0], [48, 1, 0, 2, "6/3", "القرءان", "#9F55DC", 1], [48, 1, 2, 1, "3/1", "المطالعة والإملاء", "#D268ED", 0], [48, 1, 3, 1, "4/2", "المطالعة والإملاء", "#5B55C8", 1], [48, 1, 4, 1, "8/2", "الأدب والنصوص", "#696628", 1], [48, 3, 0, 1, "9/2", "الأدب والنصوص", "#EA6FFF", 0], [48, 3, 2, 1, "4/3", "المطالعة والإملاء", "#DD1933", 1], [48, 3, 3, 1, "8/3", "الأدب والنصوص", "#EF2AD3", 1], [48, 3, 4, 1, "10/1", "الأدب والنصوص", "#B781D1", 0], [48, 4, 0, 2, "6/3", "القرءان", "#9F55DC", 1], [48, 5, 0, 1, "3/2", "المطالعة والإملاء", "#DEF11B", 0], [48, 5, 1, 1, "4/3", "المطالعة والإملاء", "#DD1933", 1], [48, 5, 2, 1, "3/1", "المطالعة والإملاء", "#D268ED", 0], [48, 5, 3, 1, "3/3", "المطالعة والإملاء", "#58BDE0", 0], [49, 1, 1, 1, "8/1", "التوحيد", "#1F8647", 1], [49, 1, 4, 1, "ت4", "المحادثة", "#6D786A", 1], [49, 2, 0, 1, "9/1", "التوحيد", "#9C8F90", 0], [49, 2, 2, 1, "9/2", "التوحيد", "#901666", 1], [49, 2, 3, 1, "8/3", "التوحيد", "#95534A", 1], [49, 2, 4, 1, "AEP1", "الورشة", "#64A6B5", 0], [49, 3, 0, 1, "8/1", "التوحيد", "#1F8647", 1], [49, 3, 3, 1, "ت5", "المحادثة", "#EB3491", 1], [49, 3, 4, 1, "ت4", "المحادثة", "#6D786A", 1], [49, 4, 1, 1, "8/2", "التوحيد", "#131FB1", 1], [49, 4, 2, 1, "9/1", "التوحيد", "#9C8F90", 0], [49, 4, 4, 1, "9/1", "الورشة", "#BB6DAE", 0], [49, 5, 0, 1, "8/3", "التوحيد", "#95534A", 1], [49, 5, 1, 1, "8/2", "التوحيد", "#131FB1", 1], [49, 5, 3, 1, "ت5", "المحادثة", "#EB3491", 1], [49, 5, 4, 1, "9/2", "التوحيد", "#901666", 1], [50, 0, 1, 1, "9/2", "المحادثة", "#7ECABD", 0], [50, 0, 2, 1, "5/1", "المحادثة", "#7F0943", 1], [50, 0, 3, 1, "4/1", "المحادثة", "#FC0094", 1], [50, 0, 4, 1, "AEP1", "الفقه", "#ACD08B", 0], [50, 1, 0, 2, "7/1", "القرءان", "#968906", 1], [50, 1, 2, 1, "AEP1", "المحادثة", "#576A01", 1], [50, 1, 3, 1, "5/4", "المحادثة", "#6AA359", 0], [50, 1, 4, 1, "AEP1", "الفقه", "#ACD08B", 0], [50, 3, 1, 1, "4/1", "المحادثة", "#FC0094", 1], [50, 3, 2, 1, "10/1", "المحادثة", "#772C1D", 1], [50, 3, 3, 1, "5/4", "المحادثة", "#6AA359", 0], [50, 3, 4, 1, "4/1", "الإملاء", "#F21BD2", 1], [50, 4, 3, 1, "7/1", "القرءان", "#968906", 1], [50, 4, 4, 1, "7/1", "الورشة", "#3668F3", 1], [50, 5, 0, 1, "AEP1", "المحادثة", "#576A01", 1], [50, 5, 1, 1, "7/1", "القراءة", "#BABAD5", 0], [50, 5, 2, 1, "9/2", "المحادثة", "#7ECABD", 0], [50, 5, 3, 1, "5/1", "المحادثة", "#7F0943", 1], [50, 5, 4, 1, "10/1", "المحادثة", "#772C1D", 1], [51, 1, 1, 1, "AEP1", "القرءان", "#BAC5F8", 0], [51, 1, 2, 1, "7/3", "المحادثة", "#75831B", 1], [51, 1, 3, 1, "7/4", "المحادثة", "#EAFC0C", 0], [51, 1, 4, 1, "C1", "المحادثة", "#738955", 1], [51, 2, 0, 1, "5/7", "المحادثة", "#663AAF", 1], [51, 2, 1, 1, "7/3", "المحادثة", "#75831B", 1], [51, 2, 2, 1, "5/6", "المحادثة", "#E07654", 0], [51, 2, 3, 1, "C1", "المحادثة", "#738955", 1], [51, 2, 4, 1, "2/2", "المحادثة", "#F63466", 1], [51, 3, 0, 2, "AEP1", "القرءان", "#BAC5F8", 0], [51, 3, 2, 1, "5/5", "المحادثة", "#ECEFA2", 0], [51, 4, 0, 1, "7/4", "المحادثة", "#EAFC0C", 0], [51, 4, 1, 1, "5/5", "المحادثة", "#ECEFA2", 0], [51, 4, 2, 1, "C2", "المحادثة", "#7F10A3", 1], [51, 4, 3, 1, "5/6", "المحادثة", "#E07654", 0], [51, 4, 4, 1, "6/1", "الورشة", "#B56124", 1], [51, 5, 0, 1, "2/2", "المحادثة", "#F63466", 1], [51, 5, 1, 1, "AEP1", "التحويد", "#320E5E", 1], [51, 5, 3, 1, "5/7", "المحادثة", "#663AAF", 1], [51, 5, 4, 1, "C2", "المحادثة", "#7F10A3", 1], [52, 0, 0, 1, "8/1", "المحادثة", "#F15A9C", 0], [52, 0, 1, 1, "8/3", "المحادثة", "#7B8F91", 0], [52, 0, 2, 1, "7/1", "المحادثة", "#FF5616", 0], [52, 0, 4, 1, "6/3", "المحادثة", "#F68ACC", 0], [52, 1, 0, 1, "AEP1", "الإملاء", "#F49ED4", 0], [52, 1, 2, 1, "8/3", "المحادثة", "#7B8F91", 0], [52, 1, 4, 1, "4/1", "القراءة", "#B9EC57", 0], [52, 2, 0, 2, "8/1", "القرءان", "#98858C", 0], [52, 2, 2, 1, "4/1", "القراءة", "#B9EC57", 0], [52, 2, 3, 1, "5/1", "القراءة", "#3AE580", 0], [52, 2, 4, 1, "6/1", "القراءة", "#39B302", 1], [52, 3, 0, 1, "6/3", "المحادثة", "#F68ACC", 0], [52, 3, 1, 1, "8/2", "المحادثة", "#FDC36A", 0], [52, 3, 2, 1, "5/1", "القراءة", "#3AE580", 0], [52, 3, 4, 1, "6/1", "القراءة", "#39B302", 1], [52, 4, 0, 1, "8/1", "المحادثة", "#F15A9C", 0], [52, 4, 1, 1, "8/1", "القرءان", "#98858C", 0], [52, 4, 2, 1, "7/1", "المحادثة", "#FF5616", 0], [52, 4, 3, 1, "8/2", "المحادثة", "#FDC36A", 0], [52, 4, 4, 1, "8/1", "الورشة", "#386479", 1], [53, 0, 0, 2, "6/1", "القرءان", "#1580D1", 1], [53, 0, 2, 1, "C1", "المطالعة والإملاء", "#6E53FC", 1], [53, 0, 3, 1, "C2", "المطالعة والإملاء", "#62CA0A", 0], [53, 0, 4, 1, "5/5", "المطالعة والإملاء", "#472308", 1], [53, 2, 1, 1, "5/6", "المطالعة والإملاء", "#4BBAFE", 0], [53, 2, 2, 1, "5/5", "المطالعة والإملاء", "#472308", 1], [53, 2, 3, 1, "4/5", "المحادثة", "#6FE675", 0], [53, 2, 4, 1, "4/7", "المحادثة", "#E53378", 1], [53, 3, 0, 2, "6/1", "القرءان", "#1580D1", 1], [53, 3, 3, 1, "4/4", "المحادثة", "#E9AA8E", 0], [53, 3, 4, 1, "C1", "المطالعة والإملاء", "#6E53FC", 1], [53, 4, 2, 1, "4/4", "المحادثة", "#E9AA8E", 0], [53, 4, 3, 1, "4/6", "المحادثة", "#637F83", 1], [53, 4, 4, 1, "4/5", "المحادثة", "#6FE675", 0], [53, 5, 1, 1, "C2", "المطالعة والإملاء", "#62CA0A", 0], [53, 5, 2, 1, "5/6", "المطالعة والإملاء", "#4BBAFE", 0], [53, 5, 3, 1, "4/6", "المحادثة", "#637F83", 1], [53, 5, 4, 1, "4/7", "المحادثة", "#E53378", 1], [54, 0, 0, 1, "2/4", "المطالعة والإملاء", "#44CB20", 0], [54, 0, 1, 1, "3/7", "المطالعة والإملاء", "#CB5B01", 1], [54, 0, 2, 1, "3/4", "المطالعة والإملاء", "#C7C2F7", 0], [54, 0, 3, 1, "3/5", "المطالعة والإملاء", "#418E0C", 1], [54, 0, 4, 1, "3/6", "المطالعة والإملاء", "#4D17FA", 1], [54, 1, 0, 1, "3/6", "المطالعة والإملاء", "#4D17FA", 1], [54, 1, 1, 1, "3/4", "المطالعة والإملاء", "#C7C2F7", 0], [54, 1, 3, 1, "4/5", "المطالعة والإملاء", "#C42ADF", 1], [54, 1, 4, 1, "2/4", "المطالعة والإملاء", "#44CB20", 0], [54, 2, 0, 2, "4/1", "القرءان", "#95DF84", 0], [54, 2, 2, 1, "2/5", "المطالعة والإملاء", "#C287DB", 0], [54, 2, 3, 1, "3/7", "المطالعة والإملاء", "#CB5B01", 1], [54, 2, 4, 1, "2/3", "المطالعة والإملاء", "#DBB437", 0], [54, 3, 3, 1, "2/5", "المطالعة والإملاء", "#C287DB", 0], [54, 4, 0, 2, "4/1", "القرءان", "#95DF84", 0], [54, 4, 2, 1, "2/3", "المطالعة والإملاء", "#DBB437", 0], [54, 4, 3, 1, "4/5", "المطالعة والإملاء", "#C42ADF", 1], [54, 4, 4, 1, "3/5", "المطالعة والإملاء", "#418E0C", 1], [55, 1, 0, 2, "9/1", "القرءان", "#1B8C5B", 1], [55, 1, 2, 1, "C4", "الإملاء", "#7D4502", 1], [55, 1, 3, 1, "9/1", "المحادثة", "#72534B", 1], [55, 1, 4, 1, "6/1", "مهارات لغوية", "#6D0670", 1], [55, 2, 0, 1, "6/1", "المحادثة", "#7C5FC1", 1], [55, 2, 1, 1, "C5", "الإملاء", "#FB09F9", 1], [55, 2, 2, 1, "7/3", "القراءة", "#306FD8", 1], [55, 2, 3, 1, "7/1", "مهارات لغوية", "#EE0FA7", 1], [55, 3, 0, 1, "C4", "الإملاء", "#7D4502", 1], [55, 3, 1, 1, "9/1", "المحادثة", "#72534B", 1], [55, 3, 2, 1, "AEP1", "المطالعة", "#4C3739", 1], [55, 3, 4, 1, "AEP1", "مهارات لغوية", "#4DD973", 0], [55, 4, 0, 1, "6/1", "المحادثة", "#7C5FC1", 1], [55, 4, 3, 1, "9/1", "القرءان", "#1B8C5B", 1], [55, 4, 4, 1, "5/1", "الورشة", "#B637A6", 1], [55, 5, 0, 1, "C5", "الإملاء", "#FB09F9", 1], [55, 5, 1, 1, "5/1", "مهارات لغوية", "#6E50F2", 1], [55, 5, 2, 1, "7/3", "القراءة", "#306FD8", 1], [55, 5, 4, 1, "AEP1", "المطالعة", "#4C3739", 1], [56, 0, 0, 1, "ت6", "المحادثة", "#E7AD67", 0], [56, 0, 1, 1, "6/3", "المطالعة والإملاء", "#5D4666", 1], [56, 0, 3, 1, "ت1", "المحادثة", "#78D270", 0], [56, 0, 4, 1, "6/4", "المطالعة والإملاء", "#C23971", 1], [56, 2, 0, 2, "C1", "القرءان", "#3ADEE4", 0], [56, 2, 2, 1, "C4", "القراءة", "#983D6A", 1], [56, 2, 3, 1, "ت6", "المحادثة", "#E7AD67", 0], [56, 2, 4, 1, "ت1", "المحادثة", "#78D270", 0], [56, 3, 2, 1, "C5", "القراءة", "#1E7191", 1], [56, 3, 4, 1, "ت3", "المحادثة", "#F2077D", 1], [56, 4, 0, 1, "C5", "القراءة", "#1E7191", 1], [56, 4, 1, 1, "C4", "القراءة", "#983D6A", 1], [56, 4, 3, 1, "6/4", "المطالعة والإملاء", "#C23971", 1], [56, 4, 4, 1, "ت2", "المحادثة", "#744B86", 1], [56, 5, 0, 2, "C1", "القرءان", "#3ADEE4", 0], [56, 5, 2, 1, "6/3", "المطالعة والإملاء", "#5D4666", 1], [56, 5, 3, 1, "ت3", "المحادثة", "#F2077D", 1], [56, 5, 4, 1, "ت2", "المحادثة", "#744B86", 1], [57, 0, 0, 1, "8/2", "النحو والصرف", "#37D43B", 0], [57, 0, 2, 1, "6/1", "الصرف", "#2FC462", 0], [57, 0, 3, 1, "AEP1", "الصرف", "#1CBDAC", 0], [57, 0, 4, 1, "5/1", "الصرف", "#2C92E0", 1], [57, 2, 0, 2, "5/4", "القرءان", "#037C49", 1], [57, 2, 3, 1, "6/1", "الصرف", "#2FC462", 0], [57, 2, 4, 1, "8/1", "النحو والصرف", "#3B4DCD", 1], [57, 3, 0, 1, "5/1", "الصرف", "#2C92E0", 1], [57, 3, 1, 1, "7/1", "الصرف", "#ACCDB5", 0], [57, 3, 2, 1, "8/2", "النحو والصرف", "#37D43B", 0], [57, 4, 0, 1, "7/1", "الصرف", "#ACCDB5", 0], [57, 4, 1, 1, "AEP1", "الصرف", "#1CBDAC", 0], [57, 4, 3, 1, "8/3", "النحو والصرف", "#B198C0", 0], [57, 4, 4, 1, "4/1", "الصرف", "#AF9B37", 0], [57, 5, 0, 2, "5/4", "القرءان", "#037C49", 1], [57, 5, 2, 1, "8/3", "النحو والصرف", "#B198C0", 0], [57, 5, 3, 1, "8/1", "النحو والصرف", "#3B4DCD", 1], [57, 5, 4, 1, "4/1", "الصرف", "#AF9B37", 0], [58, 1, 0, 1, "5/5", "الصرف", "#BF7401", 1], [58, 1, 1, 1, "4/6", "الصرف", "#30E420", 0], [58, 1, 2, 1, "5/7", "الصرف", "#35A10C", 1], [58, 1, 3, 1, "6/3", "الصرف", "#A5116F", 1], [58, 1, 4, 1, "5/4", "الصرف", "#3938FA", 1], [58, 2, 1, 1, "5/3", "الصرف", "#A647ED", 1], [58, 2, 2, 1, "5/7", "الصرف", "#35A10C", 1], [58, 2, 3, 1, "4/3", "الصرف", "#254E3A", 1], [58, 2, 4, 1, "6/4", "الصرف", "#3A6E78", 1], [58, 3, 0, 1, "4/6", "الصرف", "#30E420", 0], [58, 3, 2, 1, "5/6", "الصرف", "#B3EDF7", 0], [58, 3, 3, 1, "6/3", "الصرف", "#A5116F", 1], [58, 3, 4, 1, "4/7", "الصرف", "#B6A8DB", 0], [58, 4, 2, 1, "6/4", "الصرف", "#3A6E78", 1], [58, 4, 3, 1, "4/7", "الصرف", "#B6A8DB", 0], [58, 4, 4, 1, "5/4", "الصرف", "#3938FA", 1], [58, 5, 0, 1, "5/6", "الصرف", "#B3EDF7", 0], [58, 5, 1, 1, "5/3", "الصرف", "#A647ED", 1], [58, 5, 2, 1, "4/3", "الصرف", "#254E3A", 1], [58, 5, 3, 1, "5/5", "الصرف", "#BF7401", 1], [59, 0, 0, 1, "ت2", "النحو والصرف", "#BE5CD7", 0], [59, 0, 1, 1, "5/7", "النحو", "#2E6282", 1], [59, 0, 2, 1, "ت6", "النحو والصرف", "#2DBA36", 0], [59, 0, 3, 1, "ت3", "النحو والصرف", "#38102C", 1], [59, 0, 4, 1, "ت1", "النحو والصرف", "#B2C521", 0], [59, 1, 1, 1, "5/5", "النحو", "#A4B78F", 0], [59, 1, 2, 1, "4/7", "النحو", "#AD6B55", 1], [59, 1, 3, 1, "ت3", "النحو والصرف", "#38102C", 1], [59, 1, 4, 1, "ت6", "النحو والصرف", "#2DBA36", 0], [59, 2, 0, 1, "5/6", "النحو", "#A82E79", 1], [59, 2, 1, 1, "5/7", "النحو", "#2E6282", 1], [59, 2, 2, 1, "5/4", "النحو", "#22FB74", 0], [59, 2, 3, 1, "ت2", "النحو والصرف", "#BE5CD7", 0], [59, 2, 4, 1, "5/3", "النحو", "#BD8463", 0], [59, 3, 0, 1, "5/5", "النحو", "#A4B78F", 0], [59, 3, 2, 1, "4/7", "النحو", "#AD6B55", 1], [59, 3, 3, 1, "5/6", "النحو", "#A82E79", 1], [59, 3, 4, 1, "ت1", "النحو والصرف", "#B2C521", 0], [59, 4, 3, 1, "5/4", "النحو", "#22FB74", 0], [59, 4, 4, 1, "5/3", "النحو", "#BD8463", 0], [60, 0, 0, 1, "ت4", "النحو والصرف", "#A76F3B", 1], [60, 0, 1, 1, "4/2", "الصرف", "#A302C1", 1], [60, 0, 2, 1, "2/2", "النحو والصرف", "#3C2337", 1], [60, 0, 3, 1, "8/2", "البلاغة", "#CEC759", 0], [60, 0, 4, 1, "8/1", "البلاغة", "#C25EAF", 0], [60, 1, 0, 2, "3/2", "القرءان", "#1CE2A1", 0], [60, 1, 3, 1, "ت4", "النحو والصرف", "#A76F3B", 1], [60, 1, 4, 1, "7/3", "الصرف", "#2618B8", 1], [60, 2, 1, 1, "8/3", "البلاغة", "#488BA2", 1], [60, 2, 2, 1, "2/2", "النحو والصرف", "#3C2337", 1], [60, 2, 3, 1, "7/3", "الصرف", "#2618B8", 1], [60, 2, 4, 1, "4/2", "الصرف", "#A302C1", 1], [60, 3, 0, 1, "7/4", "الصرف", "#B967AF", 0], [60, 3, 4, 1, "ت5", "النحو والصرف", "#2123C0", 1], [60, 4, 0, 2, "3/2", "القرءان", "#1CE2A1", 0], [60, 4, 2, 1, "2/2", "النحو والصرف", "#3C2337", 1], [60, 4, 3, 1, "ت5", "النحو والصرف", "#2123C0", 1], [60, 4, 4, 1, "7/4", "الصرف", "#B967AF", 0], [61, 0, 0, 1, "6/3", "النحو", "#BED2E1", 0], [61, 0, 1, 2, "C2", "النحو والصرف", "#632D9D", 1], [61, 0, 3, 1, "6/4", "النحو", "#21ADF6", 0], [61, 0, 4, 1, "C1", "النحو والصرف", "#6FB46B", 0], [61, 1, 0, 2, "3/3", "القرءان", "#9AAE5A", 0], [61, 1, 2, 1, "6/3", "النحو", "#BED2E1", 0], [61, 1, 3, 1, "AEP1", "التوحيد", "#15364B", 1], [61, 3, 2, 2, "C1", "النحو والصرف", "#6FB46B", 0], [61, 4, 0, 2, "3/3", "القرءان", "#9AAE5A", 0], [61, 4, 2, 1, "7/4", "النحو", "#A2A421", 0], [61, 4, 3, 1, "AEP1", "التوحيد", "#15364B", 1], [61, 4, 4, 1, "7/3", "النحو", "#3DDB36", 0], [61, 5, 0, 1, "6/4", "النحو", "#21ADF6", 0], [61, 5, 2, 1, "C2", "النحو والصرف", "#632D9D", 1], [61, 5, 3, 1, "7/4", "النحو", "#A2A421", 0], [61, 5, 4, 1, "7/3", "النحو", "#3DDB36", 0], [62, 1, 0, 1, "6/1", "النحو", "#3407EC", 1], [62, 1, 1, 1, "5/1", "النحو", "#37516E", 1], [62, 1, 3, 1, "3/3", "النحو والصرف", "#39661B", 1], [62, 1, 4, 1, "7/1", "النحو", "#B70E3B", 1], [62, 2, 0, 1, "4/4", "النحو", "#A1F2A3", 0], [62, 2, 1, 1, "AEP1", "النحو", "#B765EA", 0], [62, 2, 3, 1, "3/3", "النحو والصرف", "#39661B", 1], [62, 2, 4, 1, "3/2", "النحو والصرف", "#BF2AE0", 1], [62, 3, 2, 1, "4/1", "النحو", "#B458B9", 1], [62, 3, 3, 1, "3/2", "النحو والصرف", "#BF2AE0", 1], [62, 3, 4, 1, "4/2", "النحو", "#B8C14F", 0], [62, 4, 0, 1, "AEP1", "النحو", "#B765EA", 0], [62, 4, 1, 1, "6/1", "النحو", "#3407EC", 1], [62, 4, 2, 1, "5/1", "النحو", "#37516E", 1], [62, 4, 4, 1, "3/3", "النحو والصرف", "#39661B", 1], [62, 5, 0, 1, "4/2", "النحو", "#B8C14F", 0], [62, 5, 1, 1, "4/1", "النحو", "#B458B9", 1], [62, 5, 2, 1, "3/2", "النحو والصرف", "#BF2AE0", 1], [62, 5, 3, 1, "7/1", "النحو", "#B70E3B", 1], [62, 5, 4, 1, "4/4", "النحو", "#A1F2A3", 0], [63, 1, 0, 1, "3/5", "النحو والصرف", "#2055F7", 1], [63, 1, 1, 1, "3/6", "النحو والصرف", "#2CCC01", 0], [63, 1, 2, 1, "3/7", "النحو والصرف", "#AA80FA", 0], [63, 1, 3, 1, "2/3", "النحو والصرف", "#BA6FCC", 0], [63, 1, 4, 1, "2/5", "النحو والصرف", "#A35C20", 1], [63, 2, 0, 1, "2/4", "النحو والصرف", "#2510DB", 1], [63, 2, 1, 1, "2/5", "النحو والصرف", "#A35C20", 1], [63, 2, 3, 1, "2/3", "النحو والصرف", "#BA6FCC", 0], [63, 2, 4, 1, "3/4", "النحو والصرف", "#A6190C", 1], [63, 3, 0, 1, "3/7", "النحو والصرف", "#AA80FA", 0], [63, 3, 2, 1, "3/6", "النحو والصرف", "#2CCC01", 0], [63, 3, 3, 1, "3/4", "النحو والصرف", "#A6190C", 1], [63, 3, 4, 1, "2/4", "النحو والصرف", "#2510DB", 1], [63, 4, 0, 1, "3/6", "النحو والصرف", "#2CCC01", 0], [63, 4, 2, 1, "3/5", "النحو والصرف", "#2055F7", 1], [63, 4, 3, 1, "2/3", "النحو والصرف", "#BA6FCC", 0], [63, 4, 4, 1, "3/7", "النحو والصرف", "#AA80FA", 0], [63, 5, 1, 1, "3/5", "النحو والصرف", "#2055F7", 1], [63, 5, 2, 1, "3/4", "النحو والصرف", "#A6190C", 1], [63, 5, 3, 1, "2/4", "النحو والصرف", "#2510DB", 1], [63, 5, 4, 1, "2/5", "النحو والصرف", "#A35C20", 1], [64, 1, 0, 2, "9/2", "القرءان", "#1715AD", 1], [64, 1, 3, 1, "6/1", "بهاس ملايو", "#9C36CD", 1], [64, 1, 4, 1, "9/2", "سسترا", "#A0F1D6", 0], [64, 2, 0, 1, "6/3", "بهاس ملايو", "#16E3C0", 0], [64, 2, 1, 1, "6/1", "بهاس ملايو", "#9C36CD", 1], [64, 2, 3, 1, "8/1", "سسترا", "#2F61F7", 1], [64, 2, 4, 1, "8/2", "سسترا", "#23F801", 0], [64, 3, 1, 1, "8/1", "سسترا", "#2F61F7", 1], [64, 3, 2, 1, "9/2", "سسترا", "#A0F1D6", 0], [64, 3, 3, 1, "9/1", "سسترا", "#AC6820", 1], [64, 4, 0, 1, "8/3", "سسترا", "#A5B4FA", 0], [64, 4, 2, 1, "9/2", "القرءان", "#1715AD", 1], [64, 5, 0, 1, "10/1", "سسترا", "#1B5F37", 1], [64, 5, 1, 1, "8/3", "سسترا", "#A5B4FA", 0], [64, 5, 2, 1, "9/1", "سسترا", "#AC6820", 1], [64, 5, 3, 1, "6/3", "بهاس ملايو", "#16E3C0", 0], [64, 5, 4, 1, "8/2", "سسترا", "#23F801", 0], [65, 1, 0, 2, "5/2", "القرءان", "#1A4FA5", 1], [65, 1, 2, 1, "6/2", "بهاس ملايو", "#90AF3B", 0], [65, 1, 3, 1, "5/2", "بهاس ملايو", "#93F9B9", 0], [65, 1, 4, 1, "C2", "بهاس ملايو", "#8A061B", 1], [65, 2, 0, 1, "5/2", "بهاس ملايو", "#93F9B9", 0], [65, 2, 2, 1, "C1", "بهاس ملايو", "#869FED", 0], [65, 2, 3, 1, "5/6", "بهاس ملايو", "#001F58", 1], [65, 2, 4, 1, "5/1", "بهاس ملايو", "#9F604F", 1], [65, 3, 0, 2, "5/2", "القرءان", "#1A4FA5", 1], [65, 3, 2, 1, "7/2", "بهاس ملايو", "#13A6EC", 0], [65, 3, 4, 1, "5/1", "بهاس ملايو", "#9F604F", 1], [65, 4, 1, 1, "C1", "بهاس ملايو", "#869FED", 0], [65, 4, 2, 1, "5/4", "بهاس ملايو", "#8ACA55", 0], [65, 5, 0, 1, "C2", "بهاس ملايو", "#8A061B", 1], [65, 5, 1, 1, "5/6", "بهاس ملايو", "#001F58", 1], [65, 5, 2, 1, "6/2", "بهاس ملايو", "#90AF3B", 0], [65, 5, 3, 1, "7/2", "بهاس ملايو", "#13A6EC", 0], [65, 5, 4, 1, "5/4", "بهاس ملايو", "#8ACA55", 0], [66, 0, 0, 1, "4/4", "بهاس ملايو", "#09C382", 0], [66, 0, 1, 1, "4/1", "بهاس ملايو", "#1C6998", 1], [66, 0, 2, 1, "4/3", "بهاس ملايو", "#96BC95", 0], [66, 0, 3, 1, "4/2", "بهاس ملايو", "#10F06E", 0], [66, 0, 4, 1, "4/5", "بهاس ملايو", "#8F8F79", 0], [66, 1, 0, 2, "4/2", "القرءان", "#994672", 1], [66, 1, 2, 1, "4/1", "بهاس ملايو", "#1C6998", 1], [66, 1, 3, 1, "4/6", "بهاس ملايو", "#83168F", 1], [66, 1, 4, 1, "4/7", "بهاس ملايو", "#055A74", 1], [66, 3, 0, 2, "4/2", "القرءان", "#994672", 1], [66, 3, 2, 1, "5/3", "بهاس ملايو", "#15B542", 1], [66, 4, 2, 1, "4/3", "بهاس ملايو", "#96BC95", 0], [66, 4, 3, 1, "4/2", "بهاس ملايو", "#10F06E", 0], [66, 5, 0, 1, "4/5", "بهاس ملايو", "#8F8F79", 0], [66, 5, 1, 1, "4/7", "بهاس ملايو", "#055A74", 1], [66, 5, 2, 1, "4/6", "بهاس ملايو", "#83168F", 1], [66, 5, 3, 1, "4/4", "بهاس ملايو", "#09C382", 0], [66, 5, 4, 1, "5/3", "بهاس ملايو", "#15B542", 1], [67, 1, 0, 2, "2/1", "القرءان", "#937280", 1], [67, 1, 2, 1, "3/2", "جاوي", "#845C16", 1], [67, 1, 3, 1, "ت1", "بهاس ملايو", "#98BB7C", 0], [67, 1, 4, 1, "3/3", "جاوي", "#0210ED", 1], [67, 2, 0, 1, "3/3", "جاوي", "#0210ED", 1], [67, 2, 1, 1, "2/3", "جاوي", "#81193A", 1], [67, 2, 2, 1, "3/1", "جاوي", "#88C5E0", 0], [67, 2, 3, 1, "2/2", "جاوي", "#0755C1", 1], [67, 2, 4, 1, "ت2", "بهاس ملايو", "#94228A", 1], [67, 3, 0, 1, "2/3", "جاوي", "#81193A", 1], [67, 3, 2, 1, "2/2", "جاوي", "#0755C1", 1], [67, 3, 4, 1, "3/1", "جاوي", "#88C5E0", 0], [67, 4, 0, 2, "2/1", "القرءان", "#937280", 1], [67, 4, 2, 1, "3/2", "جاوي", "#845C16", 1], [67, 4, 4, 1, "2/2", "جاوي", "#0755C1", 1], [67, 5, 0, 1, "2/3", "جاوي", "#81193A", 1], [67, 5, 3, 1, "ت2", "بهاس ملايو", "#94228A", 1], [67, 5, 4, 1, "ت1", "بهاس ملايو", "#98BB7C", 0], [68, 1, 0, 1, "C1", "جاوي", "#6C8384", 1], [68, 1, 2, 1, "C2", "جاوي", "#601A72", 1], [68, 1, 3, 1, "3/4", "جاوي", "#9D6FFA", 0], [68, 1, 4, 1, "3/6", "جاوي", "#17BAF7", 0], [68, 2, 0, 1, "2/5", "جاوي", "#982AD6", 1], [68, 2, 2, 1, "3/4", "جاوي", "#9D6FFA", 0], [68, 2, 3, 1, "2/1", "جاوي", "#0BCC37", 0], [68, 2, 4, 1, "C2", "جاوي", "#601A72", 1], [68, 3, 0, 1, "3/6", "جاوي", "#17BAF7", 0], [68, 3, 1, 1, "2/5", "جاوي", "#982AD6", 1], [68, 3, 2, 1, "C2", "جاوي", "#601A72", 1], [68, 3, 3, 1, "3/5", "جاوي", "#1B2301", 1], [68, 3, 4, 1, "3/7", "جاوي", "#91F60C", 0], [68, 4, 2, 1, "C1", "جاوي", "#6C8384", 1], [68, 4, 3, 1, "2/1", "جاوي", "#0BCC37", 0], [68, 5, 0, 1, "3/5", "جاوي", "#1B2301", 1], [68, 5, 1, 1, "2/1", "جاوي", "#0BCC37", 0], [68, 5, 2, 1, "2/5", "جاوي", "#982AD6", 1], [68, 5, 3, 1, "C1", "جاوي", "#6C8384", 1], [68, 5, 4, 1, "3/7", "جاوي", "#91F60C", 0], [69, 0, 0, 1, "7/1", "بهاس ملايو", "#1F3F1A", 1], [69, 0, 2, 1, "7/4", "بهاس ملايو", "#0A9500", 1], [69, 0, 3, 1, "2/1", "بهاس ملايو", "#1AC49C", 0], [69, 0, 4, 1, "ت5", "بهاس ملايو", "#0B5D9D", 1], [69, 2, 0, 2, "C2", "القرءان", "#364712", 1], [69, 2, 3, 1, "ت5", "بهاس ملايو", "#0B5D9D", 1], [69, 2, 4, 1, "2/1", "بهاس ملايو", "#1AC49C", 0], [69, 3, 4, 1, "7/3", "بهاس ملايو", "#95EA17", 0], [69, 4, 0, 2, "C2", "القرءان", "#364712", 1], [69, 4, 3, 1, "ت4", "بهاس ملايو", "#8D1166", 1], [69, 5, 0, 1, "7/1", "بهاس ملايو", "#1F3F1A", 1], [69, 5, 1, 1, "7/3", "بهاس ملايو", "#95EA17", 0], [69, 5, 2, 1, "7/4", "بهاس ملايو", "#0A9500", 1], [69, 5, 3, 1, "2/1", "بهاس ملايو", "#1AC49C", 0], [69, 5, 4, 1, "ت4", "بهاس ملايو", "#8D1166", 1], [70, 1, 0, 1, "C5", "جاوي", "#FF6565", 0], [70, 1, 2, 1, "2/3", "بهاس ملايو", "#901191", 1], [70, 1, 3, 1, "6/4", "بهاس ملايو", "#899CD7", 0], [70, 1, 4, 1, "5/5", "بهاس ملايو", "#0C86AE", 1], [70, 2, 0, 1, "AEP1", "جاوي", "#53FAEC", 0], [70, 2, 1, 1, "2/4", "بهاس ملايو", "#0F6E86", 1], [70, 2, 2, 1, "2/3", "بهاس ملايو", "#901191", 1], [70, 2, 3, 1, "5/5", "بهاس ملايو", "#0C86AE", 1], [70, 2, 4, 1, "ت3", "بهاس ملايو", "#126E71", 1], [70, 3, 0, 1, "2/4", "بهاس ملايو", "#0F6E86", 1], [70, 3, 1, 1, "C4", "جاوي", "#79299E", 1], [70, 3, 2, 1, "6/4", "بهاس ملايو", "#899CD7", 0], [70, 3, 4, 1, "ت6", "بهاس ملايو", "#07C46B", 0], [70, 4, 0, 1, "2/4", "بهاس ملايو", "#0F6E86", 1], [70, 4, 2, 1, "AEP1", "بهاس ملايو", "#18539E", 1], [70, 4, 3, 1, "ت6", "بهاس ملايو", "#07C46B", 0], [70, 4, 4, 1, "AEP1", "جاوي", "#53FAEC", 0], [70, 5, 1, 1, "C5", "جاوي", "#FF6565", 0], [70, 5, 2, 1, "C4", "جاوي", "#79299E", 1], [70, 5, 3, 1, "2/3", "بهاس ملايو", "#901191", 1], [70, 5, 4, 1, "ت3", "بهاس ملايو", "#126E71", 1], [71, 0, 0, 1, "5/5", "النصوص", "#52FF22", 0], [71, 0, 1, 1, "2/3", "المحادثة", "#70789D", 1], [71, 0, 2, 1, "3/1", "المحادثة", "#79A447", 0], [71, 0, 3, 1, "5/4", "النصوص", "#D4B3D9", 0], [71, 0, 4, 1, "3/4", "المحادثة", "#6C0E5D", 1], [71, 1, 2, 1, "5/3", "النصوص", "#4BCCCE", 0], [71, 1, 3, 1, "5/5", "النصوص", "#52FF22", 0], [71, 1, 4, 1, "6/4", "المحادثة", "#69F5DB", 0], [71, 3, 0, 1, "3/1", "المحادثة", "#79A447", 0], [71, 3, 1, 1, "5/4", "النصوص", "#D4B3D9", 0], [71, 3, 2, 1, "2/4", "المحادثة", "#EF078A", 1], [71, 3, 3, 1, "2/3", "المحادثة", "#70789D", 1], [71, 3, 4, 1, "5/6", "النصوص", "#5E66D4", 1], [71, 4, 3, 1, "2/4", "المحادثة", "#EF078A", 1], [71, 4, 4, 1, "5/7", "النصوص", "#D82A2F", 1], [71, 5, 0, 1, "3/4", "المحادثة", "#6C0E5D", 1], [71, 5, 1, 1, "5/7", "النصوص", "#D82A2F", 1], [71, 5, 2, 1, "6/4", "المحادثة", "#69F5DB", 0], [71, 5, 3, 1, "5/3", "النصوص", "#4BCCCE", 0], [71, 5, 4, 1, "5/6", "النصوص", "#5E66D4", 1], [72, 0, 0, 1, "6/4", "النصوص", "#D7E55B", 0], [72, 0, 1, 1, "3/3", "المحادثة", "#F3714A", 0], [72, 0, 2, 1, "5/3", "القراءة", "#B0308D", 1], [72, 0, 3, 1, "3/2", "المحادثة", "#753DB1", 1], [72, 0, 4, 1, "4/3", "المحادثة", "#76D599", 0], [72, 1, 0, 1, "7/4", "النصوص", "#54EC8C", 0], [72, 1, 2, 1, "4/6", "المطالعة والإملاء", "#C8B329", 0], [72, 1, 3, 1, "5/3", "القراءة", "#B0308D", 1], [72, 1, 4, 1, "3/5", "المحادثة", "#EA42A6", 0], [72, 3, 0, 1, "7/3", "النصوص", "#CB939B", 0], [72, 3, 1, 1, "6/3", "النصوص", "#489A4C", 1], [72, 3, 3, 1, "6/4", "النصوص", "#D7E55B", 0], [72, 3, 4, 1, "3/5", "المحادثة", "#EA42A6", 0], [72, 4, 0, 1, "4/2", "المحادثة", "#F09962", 0], [72, 4, 3, 1, "3/2", "المحادثة", "#753DB1", 1], [72, 4, 4, 1, "6/3", "النصوص", "#489A4C", 1], [72, 5, 0, 1, "4/3", "المحادثة", "#76D599", 0], [72, 5, 2, 1, "3/3", "المحادثة", "#F3714A", 0], [72, 5, 3, 1, "4/2", "المحادثة", "#F09962", 0], [72, 5, 4, 1, "4/6", "المطالعة والإملاء", "#C8B329", 0], [73, 0, 0, 1, "3/6", "التحويد", "#670B3F", 1], [73, 0, 1, 1, "2/2", "بهاس ملايو", "#165D6A", 1], [73, 0, 2, 1, "3/5", "بهاس ملايو", "#0A2BAA", 1], [73, 0, 3, 1, "3/3", "بهاس ملايو", "#131846", 1], [73, 0, 4, 1, "3/2", "التحويد", "#F4EDDE", 0], [73, 1, 1, 1, "3/5", "التحويد", "#6B92C9", 0], [73, 1, 2, 1, "3/4", "بهاس ملايو", "#8C6751", 1], [73, 1, 3, 1, "5/7", "بهاس ملايو", "#8653A3", 1], [73, 1, 4, 1, "2/2", "بهاس ملايو", "#165D6A", 1], [73, 2, 0, 1, "3/2", "التحويد", "#F4EDDE", 0], [73, 2, 1, 1, "3/3", "بهاس ملايو", "#131846", 1], [73, 2, 2, 1, "3/2", "بهاس ملايو", "#9554BD", 1], [73, 2, 3, 1, "5/7", "بهاس ملايو", "#8653A3", 1], [73, 2, 4, 1, "3/5", "بهاس ملايو", "#0A2BAA", 1], [73, 3, 0, 1, "3/5", "التحويد", "#6B92C9", 0], [73, 3, 1, 1, "3/2", "بهاس ملايو", "#9554BD", 1], [73, 3, 2, 1, "3/1", "بهاس ملايو", "#99CD4B", 0], [73, 3, 3, 1, "2/2", "بهاس ملايو", "#165D6A", 1], [73, 3, 4, 1, "3/4", "بهاس ملايو", "#8C6751", 1], [73, 4, 3, 1, "3/6", "التحويد", "#670B3F", 1], [73, 4, 4, 1, "3/1", "بهاس ملايو", "#99CD4B", 0]]}</script>
  <script>
    (function () {
      const rawData = JSON.parse(document.getElementById('app-data').textContent || '{}');
      const META = rawData.meta || { days: [], periods: [], generated: '' };
      const DEFAULT_TEACHERS_JSON = JSON.stringify(Array.isArray(rawData.teachers) ? rawData.teachers : []);
      const DEFAULT_LESSONS_JSON = JSON.stringify(Array.isArray(rawData.lessons) ? rawData.lessons : []);

      let TEACHERS = JSON.parse(DEFAULT_TEACHERS_JSON);
      let RAW_LESSONS = JSON.parse(DEFAULT_LESSONS_JSON);
      let hasCustomEdits = false;

      try {
        const savedCustom = localStorage.getItem('thaqafah_tt_custom_v1');
        if (savedCustom) {
          const parsedCustom = JSON.parse(savedCustom);
          if (Array.isArray(parsedCustom.teachers) && Array.isArray(parsedCustom.lessons)) {
            TEACHERS = parsedCustom.teachers;
            RAW_LESSONS = parsedCustom.lessons;
            hasCustomEdits = true;
          }
        }
      } catch (e) {}

      const THAI_DAYS = ['เสาร์', 'อาทิตย์', 'จันทร์', 'อังคาร', 'พุธ', 'พฤหัสบดี'];
      const JAWI_DAYS = ['سبت', 'أحد', 'اثنين', 'ثلاث', 'أربعاء', 'خميس'];

      const I18N = {
        th: {
          docTitle: 'ระบบค้นหาตารางสอน — معهد الثقافة الإسلامية 2026',
          badgeYear: '• ปีการศึกษา 2026',
          appTitleMain: 'ระบบค้นหาตารางสอน',
          themeLabel: 'ธีมสี',
          themeNames: {
            emerald: 'เขียวมรกต–ทอง',
            sapphire: 'น้ำเงินคราม–ฟ้า',
            teal: 'เขียวหยก–มิ้นต์',
            amber: 'ทองอำพัน–ครีม'
          },
          headerMetaHtml: '<span>ข้อมูลจากไฟล์: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• ครูผู้สอน 73 ท่าน • 51 ห้องเรียน • 40 รายวิชา</span>',
          tabs: {
            self: 'สำหรับครูค้นหาเอง',
            explorer: 'ค้นหารายการสอน',
            teacher: 'ตารางสอนรายครู',
            class: 'ตารางเรียนรายห้อง',
            free: 'ค้นหาครูว่างสอนแทน'
          },
          lblSearch: 'คำค้นหา (ชื่อครู / ห้อง / วิชา / วัน / เลขหน้า)',
          phSearch: 'เช่น أحمد, الفقه, بهاس ملايو, 8/1, ت6, เสาร์...',
          lblTeacher: 'ครูผู้สอน',
          allTeachers: 'ทั้งหมด (73 ท่าน)',
          lblClass: 'ห้องเรียน',
          allClasses: 'ทั้งหมด (51 ห้อง)',
          lblSubject: 'รายวิชา',
          allSubjects: 'ทั้งหมด (40 วิชา)',
          lblDay: 'วัน',
          allDays: 'ทุกวัน',
          lblPeriod: 'คาบเรียน / เวลา',
          allPeriods: 'ทุกคาบเวลา',
          btnResetAll: 'ล้างตัวกรองทั้งหมด',
          btnResetExtra: 'ล้างตัวกรองเพิ่มเติม',
          chipQuery: 'คำค้นหา',
          chipTeacher: 'ครู',
          chipClass: 'ห้อง',
          chipSubj: 'วิชา',
          chipDay: 'วัน',
          chipPeriod: 'คาบ',
          selfHeading: 'ค้นหาตารางสอนของคุณ',
          selfSub: 'พิมพ์ชื่อครูผู้สอน เลขหน้า (1–73) หรือเลือกชื่อจากรายการเพื่อดูตารางสอนรายสัปดาห์ทันที',
          btnSelfOther: 'ค้นหาชื่ออื่น',
          btnChangeTeacher: 'เปลี่ยนชื่อครู',
          lblSelfSearch: 'พิมพ์ชื่อครู / ห้องที่สอน / วิชา / เลขหน้า',
          phSelfSearch: 'พิมพ์ชื่อครู, ห้องเรียน (เช่น 8/1, ت6), วิชา หรือเลขหน้า (1–73)...',
          lblSelfSelect: 'หรือเลือกจากรายชื่อครูทั้งหมด (73 ท่าน)',
          optSelfPrompt: '-- เลือกชื่อครูผู้สอน --',
          lblQuickLetter: 'แตะเลือกตามอักษรตัวแรกของชื่อครู (ไม่ต้องพิมพ์ภาษาอาหรับ/ยาวี):',
          allLetters: 'ทั้งหมด',
          selfEmptyTitle: 'ไม่พบชื่อครูที่ตรงกับคำค้นหา',
          selfEmptySub: 'ลองพิมพ์เฉพาะบางส่วนของชื่อ หรือเลือกจากช่องรายชื่อครูด้านบน',
          lblPickViewDay: 'เลือกดูวัน:',
          wholeWeek: 'ทั้งสัปดาห์',
          btnExpandList: 'แสดงรายชื่อครูทั้งหมด / เลือกท่านอื่น',
          selfFooterDaily: 'แตะปุ่ม "ทั้งสัปดาห์" ด้านบนเพื่อดูตารางรวมทั้ง 6 วัน • แตะที่กล่องวิชาเพื่อดูตารางเรียนของห้องนั้น',
          colPage: 'หน้า',
          colTeacher: 'ครูผู้สอน',
          colDay: 'วัน',
          colPeriod: 'คาบ / เวลา',
          colClass: 'ห้องเรียน',
          colSubj: 'รายวิชา',
          colSpan: 'จำนวนคาบ',
          expEmptyTitle: 'ไม่พบตารางสอนที่ตรงกับเงื่อนไข',
          expEmptySub: 'ลองเปลี่ยนคำค้นหา หรือล้างตัวกรองเพื่อดูรายการสอนทั้งหมดในระบบ',
          lblShowRows: 'แสดง:',
          unitItems: 'รายการ',
          btnPrev: 'ก่อนหน้า',
          btnNext: 'ถัดไป',
          dirTeachersTitle: 'รายชื่อครูผู้สอน',
          phTeacherQuick: 'กรองรายชื่อครู...',
          teacherEmptyDir: 'ไม่พบรายชื่อครูที่ตรงกัน',
          teacherEmptyTitle: 'ไม่พบตารางสอนครูที่ตรงกับตัวกรอง',
          teacherEmptySub: 'ลองล้างตัวกรองหรือคำค้นหาเพื่อดูตารางสอนครูทั้งหมด 73 ท่าน',
          dirClassesTitle: 'รายชื่อห้องเรียน',
          phClassQuick: 'ค้นหาห้อง เช่น 8/1, ت6, C1...',
          classEmptyDir: 'ไม่พบห้องเรียนที่ตรงกัน',
          classEmptyTitle: 'ไม่พบตารางเรียนรายห้องที่ตรงกับตัวกรอง',
          classEmptySub: 'ลองล้างตัวกรองหรือคำค้นหาเพื่อดูตารางเรียนทั้งหมด 51 ห้อง',
          classSheetSub: 'ตารางเรียนรวมรายห้อง (ประมวลผลจากตารางครูทั้ง 73 ท่าน)',
          classHeadingPrefix: 'ห้องเรียน',
          btnPrevTeacher: '← ก่อนหน้า',
          btnNextTeacher: 'ถัดไป →',
          btnPrevClass: '← ห้องก่อนหน้า',
          btnNextClass: 'ห้องถัดไป →',
          btnOpenTeacherTab: 'เปิดในหน้าตารางสอนรายครู',
          btnCloseModal: 'ปิดหน้าต่าง',
          cornerDayTime: 'วัน / เวลา',
          periodOrdinal: (n) => `คาบที่ ${n}`,
          periodShort: (n) => `คาบ ${n}`,
          periodSpanShort: (s, e) => `คาบ ${s}–${e}`,
          periodSpanOrdinal: (s, e) => `คาบที่ ${s}–${e}`,
          unitPeriods: 'คาบ',
          unitPeriodsWeek: 'คาบ/สัปดาห์',
          unitPersons: 'ท่าน',
          unitRooms: 'ห้อง',
          spanContTag: (n) => `${n} คาบต่อเนื่อง`,
          freeSlotLabel: 'คาบว่าง',
          unavailSlotLabel: 'งดสอน / ไม่ว่าง',
          noLessonSlot: 'ไม่มีคาบเรียน',
          hintClickCellToClass: 'คลิกช่องวิชาเพื่อดูตารางเรียนของห้องนั้น',
          hintClassFooter: 'แสดงชื่อวิชาและครูผู้สอนประจำคาบ • คลิกช่องวิชาเพื่อเปิดดูตารางสอนของครูท่านนั้น',
          lblPickSubDay: 'เลือกวัน:',
          lblPickSubPeriod: 'เลือกคาบเวลา:',
          colFreeTeacher: 'ครูที่ว่างพร้อมสอนแทน (---)',
          colRegSubjects: 'รายวิชาที่สอนประจำ',
          colDayTrack: 'ตารางรายคาบในวันนั้น (คาบ 1–5)',
          colDayBusy: 'สอนวันนี้',
          colWeekTotal: 'รวมทั้งสัปดาห์',
          miniFreeWord: 'ว่าง',
          freeEmptyTitle: 'ไม่พบครูว่างที่ตรงกับเงื่อนไขในคาบเวลานี้',
          freeEmptySub: 'ลองเลือกคาบเวลาอื่น หรือล้างตัวกรองรายวิชา/คำค้นหาเพื่อดูรายชื่อครูว่างทั้งหมดในคาบนี้',
          freeFooterHtml: 'หมายเหตุ: แสดงเฉพาะครูที่มีสถานะคาบว่างจริง (<strong>---</strong>) ในวันและคาบที่เลือก โดยตัดครูที่ติดสอนและครูที่งดสอน/ไม่ว่าง (<strong>-x-</strong>) ออกโดยอัตโนมัติ • คลิกที่แถวเพื่อดูตารางสอนเต็ม'
        },
        ar: {
          docTitle: 'نظام البحث في الجدول الدراسي — معهد الثقافة الإسلامية 2026',
          badgeYear: '• العام الدراسي 2026',
          appTitleMain: 'نظام البحث في الجدول الدراسي',
          themeLabel: 'السمة',
          themeNames: {
            emerald: 'زمردي وذهبي',
            sapphire: 'أزرق ياقوتي',
            teal: 'فيروزي هادئ',
            amber: 'كهرماني دافئ'
          },
          headerMetaHtml: '<span>المصدر: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• 73 معلماً • 51 فصلاً • 40 مادة دراسية</span>',
          tabs: {
            self: 'بحث المعلم الذاتي',
            explorer: 'استكشاف الحصص',
            teacher: 'جدول المعلمين',
            class: 'جدول الفصول',
            free: 'معلمون متاحون للبديل'
          },
          lblSearch: 'كلمة البحث (اسم المعلم / الفصل / المادة / اليوم / الصفحة)',
          phSearch: 'مثال: أحمد، الفقه، بهاس ملايو، 8/1، ت6، السبت...',
          lblTeacher: 'المعلم',
          allTeachers: 'الكل (73 معلماً)',
          lblClass: 'الفصل الدراسي',
          allClasses: 'الكل (51 فصلاً)',
          lblSubject: 'المادة الدراسية',
          allSubjects: 'الكل (40 مادة)',
          lblDay: 'اليوم',
          allDays: 'جميع الأيام',
          lblPeriod: 'الحصة / الوقت',
          allPeriods: 'جميع الحصص',
          btnResetAll: 'مسح جميع الفلاتر',
          btnResetExtra: 'مسح الفلاتر الإضافية',
          chipQuery: 'بحث',
          chipTeacher: 'المعلم',
          chipClass: 'الفصل',
          chipSubj: 'المادة',
          chipDay: 'اليوم',
          chipPeriod: 'الحصة',
          selfHeading: 'ابحث عن جدولك الدراسي',
          selfSub: 'اكتب اسم المعلم أو رقم الصفحة (1–73) أو اختر اسمك من القائمة لعرض جدولك الأسبوعي فوراً',
          btnSelfOther: 'بحث عن معلم آخر',
          btnChangeTeacher: 'تغيير المعلم',
          lblSelfSearch: 'اكتب اسم المعلم / الفصل / المادة / رقم الصفحة',
          phSelfSearch: 'اكتب اسم المعلم، الفصل (مثل 8/1، ت6)، المادة أو رقم الصفحة (1–73)...',
          lblSelfSelect: 'أو اختر من قائمة جميع المعلمين (73 معلماً)',
          optSelfPrompt: '-- اختر اسم المعلم --',
          lblQuickLetter: 'اختر حسب الحرف الأول من اسم المعلم:',
          allLetters: 'الكل',
          selfEmptyTitle: 'لم يتم العثور على معلم مطابق للبحث',
          selfEmptySub: 'جرّب كتابة جزء من الاسم أو اختر من قائمة المعلمين أعلاه',
          lblPickViewDay: 'عرض اليوم:',
          wholeWeek: 'الأسبوع كاملاً',
          btnExpandList: 'عرض قائمة جميع المعلمين / اختيار معلم آخر',
          selfFooterDaily: 'اضغط على "الأسبوع كاملاً" أعلاه لعرض جدول الأيام الستة • اضغط على البطاقة لعرض جدول الفصل',
          colPage: 'صفحة',
          colTeacher: 'المعلم',
          colDay: 'اليوم',
          colPeriod: 'الحصة / الوقت',
          colClass: 'الفصل',
          colSubj: 'المادة الدراسية',
          colSpan: 'عدد الحصص',
          expEmptyTitle: 'لا توجد حصص مطابقة لشروط البحث',
          expEmptySub: 'جرّب تغيير كلمة البحث أو مسح الفلاتر لعرض جميع الحصص الدراسية',
          lblShowRows: 'عرض:',
          unitItems: 'سجلاً',
          btnPrev: 'السابق',
          btnNext: 'التالي',
          dirTeachersTitle: 'قائمة المعلمين',
          phTeacherQuick: 'تصفية أسماء المعلمين...',
          teacherEmptyDir: 'لا يوجد معلمون مطابقون',
          teacherEmptyTitle: 'لا يوجد جدول معلم مطابق للفلاتر',
          teacherEmptySub: 'جرّب مسح الفلاتر أو كلمة البحث لعرض جميع المعلمين (73 معلماً)',
          dirClassesTitle: 'قائمة الفصول الدراسية',
          phClassQuick: 'ابحث عن فصل مثل 8/1، ت6، C1...',
          classEmptyDir: 'لا توجد فصول مطابقة',
          classEmptyTitle: 'لا يوجد جدول فصل مطابق للفلاتر',
          classEmptySub: 'جرّب مسح الفلاتر أو كلمة البحث لعرض جميع الفصول (51 فصلاً)',
          classSheetSub: 'الجدول الأسبوعي المجمّع للفصل (مستخلص من جداول 73 معلماً)',
          classHeadingPrefix: 'الفصل',
          btnPrevTeacher: '→ السابق',
          btnNextTeacher: 'التالي ←',
          btnPrevClass: '→ الفصل السابق',
          btnNextClass: 'الفصل التالي ←',
          btnOpenTeacherTab: 'فتح في صفحة جدول المعلمين',
          btnCloseModal: 'إغلاق النافذة',
          cornerDayTime: 'اليوم / الوقت',
          periodOrdinal: (n) => `الحصة ${n}`,
          periodShort: (n) => `حصة ${n}`,
          periodSpanShort: (s, e) => `حصة ${s}–${e}`,
          periodSpanOrdinal: (s, e) => `الحصة ${s}–${e}`,
          unitPeriods: 'حصص',
          unitPeriodsWeek: 'حصة/أسبوع',
          unitPersons: 'معلماً',
          unitRooms: 'فصلاً',
          spanContTag: (n) => `حصتان متتاليتان (${n})`,
          freeSlotLabel: 'حصة شاغرة',
          unavailSlotLabel: 'غير متاح',
          noLessonSlot: 'لا توجد حصة',
          hintClickCellToClass: 'اضغط على خلية المادة لعرض جدول ذلك الفصل',
          hintClassFooter: 'يعرض اسم المادة ومعلمها في كل حصة • اضغط على الخلية لعرض جدول المعلم',
          lblPickSubDay: 'اختر اليوم:',
          lblPickSubPeriod: 'اختر الحصة:',
          colFreeTeacher: 'المعلمون المتاحون للبديل (---)',
          colRegSubjects: 'المواد التي يدرّسها',
          colDayTrack: 'جدول حصص هذا اليوم (1–5)',
          colDayBusy: 'حصص اليوم',
          colWeekTotal: 'مجموع الأسبوع',
          miniFreeWord: 'متاح',
          freeEmptyTitle: 'لا يوجد معلم متاح مطابق للشروط في هذه الحصة',
          freeEmptySub: 'جرّب اختيار حصة أخرى أو مسح فلتر المادة لعرض جميع المعلمين المتاحين',
          freeFooterHtml: 'ملاحظة: يظهر فقط المعلمون المتاحون فعلياً (<strong>---</strong>) في اليوم والحصة المحددين، مع استبعاد المنشغلين بحصة أخرى أو غير المتاحين (<strong>-x-</strong>) تلقائياً • اضغط على الصف لعرض الجدول الكامل'
        },
        jawi: {
          docTitle: 'سيستم چارين جدول فڠاجين — معهد الثقافة الإسلامية 2026',
          badgeYear: '• تاهون فڠاجين 2026',
          appTitleMain: 'سيستم چارين جدول فڠاجين',
          themeLabel: 'تيما ورنا',
          themeNames: {
            emerald: 'هيجاو زمرد & امس',
            sapphire: 'بيرو نيلم & لاڠيت',
            teal: 'هيجاو فيروز & فودينا',
            amber: 'امس عمبر & كريم'
          },
          headerMetaHtml: '<span>سومبر فايل: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• 73 ڬورو فڠاجر • 51 كلس • 40 مات فلاجرن</span>',
          tabs: {
            self: 'چارين سنديري ڬورو',
            explorer: 'چاري سناراي فڠاجرن',
            teacher: 'جدول مڠاجر ڬورو',
            class: 'جدول فلاجرن كلس',
            free: 'چاري ڬورو كوسوڠ (ڬنتي)'
          },
          lblSearch: 'كات چارين (نام ڬورو / كلس / مات فلاجرن / هاري / موك سورت)',
          phSearch: 'چونتوه: أحمد، الفقه، بهاس ملايو، 8/1، ت6، سبت...',
          lblTeacher: 'ڬورو فڠاجر',
          allTeachers: 'سموا (73 ڬورو)',
          lblClass: 'كلس',
          allClasses: 'سموا (51 كلس)',
          lblSubject: 'مات فلاجرن',
          allSubjects: 'سموا (40 مات فلاجرن)',
          lblDay: 'هاري',
          allDays: 'سموا هاري',
          lblPeriod: 'وقتو فڠاجرن',
          allPeriods: 'سموا وقتو',
          btnResetAll: 'فادم سموا تافيسن',
          btnResetExtra: 'فادم تافيسن تمبهن',
          chipQuery: 'چارين',
          chipTeacher: 'ڬورو',
          chipClass: 'كلس',
          chipSubj: 'مات فلاجرن',
          chipDay: 'هاري',
          chipPeriod: 'وقتو',
          selfHeading: 'چاري جدول مڠاجر اندا',
          selfSub: 'تايف نام ڬورو، نومبور موك سورت (1–73) اتاو فيليه نام دري سناراي اونتوق مليهت جدول ميڠڬوان سڬرا',
          btnSelfOther: 'چاري نام لاين',
          btnChangeTeacher: 'توكر نام ڬورو',
          lblSelfSearch: 'تايف نام ڬورو / كلس / مات فلاجرن / موك سورت',
          phSelfSearch: 'تايف نام ڬورو، كلس (چونتوه 8/1، ت6)، مات فلاجرن اتاو موك سورت (1–73)...',
          lblSelfSelect: 'اتاو فيليه درفد سناراي سموا ڬورو (73 اورڠ)',
          optSelfPrompt: '-- فيليه نام ڬورو فڠاجر --',
          lblQuickLetter: 'سنتوه فيليه مڠيكوت حروف اول نام ڬورو:',
          allLetters: 'سموا',
          selfEmptyTitle: 'تيدق دجومفأي نام ڬورو يڠ سفادن',
          selfEmptySub: 'چوبا تايف سبهاڬين نام اتاو فيليه درفد سناراي ڬورو د أتس',
          lblPickViewDay: 'فيليه هاري:',
          wholeWeek: 'سفنجڠ ميڠڬو',
          btnExpandList: 'تنجوق سموا سناراي ڬورو / فيليه ڬورو لاين',
          selfFooterDaily: 'سنتوه بوتڠ "سفنجڠ ميڠڬو" د أتس اونتوق مليهت جدول فنوه 6 هاري • سنتوه كوتق مات فلاجرن اونتوق مليهت جدول كلس ايت',
          colPage: 'موك سورت',
          colTeacher: 'ڬورو فڠاجر',
          colDay: 'هاري',
          colPeriod: 'وقتو / ماس',
          colClass: 'كلس',
          colSubj: 'مات فلاجرن',
          colSpan: 'بيلڠن وقتو',
          expEmptyTitle: 'تياد جدول مڠاجر يڠ سفادن دڠن شرط',
          expEmptySub: 'چوبا اوبه كات چارين اتاو فادم تافيسن اونتوق مليهت سموا سناراي فڠاجرن',
          lblShowRows: 'فافر:',
          unitItems: 'سيناراي',
          btnPrev: 'سبلومڽ',
          btnNext: 'ستروسڽ',
          dirTeachersTitle: 'سناراي نام ڬورو',
          phTeacherQuick: 'تافيس نام ڬورو...',
          teacherEmptyDir: 'تياد نام ڬورو يڠ سفادن',
          teacherEmptyTitle: 'تياد جدول ڬورو يڠ سفادن دڠن تافيسن',
          teacherEmptySub: 'چوبا فادم تافيسن اتاو كات چارين اونتوق مليهت سموا 73 ڬورو',
          dirClassesTitle: 'سناراي كلس',
          phClassQuick: 'چاري كلس سفرتي 8/1، ت6، C1...',
          classEmptyDir: 'تياد كلس يڠ سفادن',
          classEmptyTitle: 'تياد جدول كلس يڠ سفادن دڠن تافيسن',
          classEmptySub: 'چوبا فادم تافيسن اتاو كات چارين اونتوق مليهت سموا 51 كلس',
          classSheetSub: 'جدول فلاجرن تركومفول مڠيكوت كلس (دفروسيس درفد جدول 73 ڬورو)',
          classHeadingPrefix: 'كلس',
          btnPrevTeacher: '→ سبلومڽ',
          btnNextTeacher: 'ستروسڽ ←',
          btnPrevClass: '→ كلس سبلومڽ',
          btnNextClass: 'كلس ستروسڽ ←',
          btnOpenTeacherTab: 'بوك د هلامن جدول ڬورو',
          btnCloseModal: 'توتوف تيڠكف',
          cornerDayTime: 'هاري / وقتو',
          periodOrdinal: (n) => `وقتو ك-${n}`,
          periodShort: (n) => `وقتو ${n}`,
          periodSpanShort: (s, e) => `وقتو ${s}–${e}`,
          periodSpanOrdinal: (s, e) => `وقتو ك-${s}–${e}`,
          unitPeriods: 'وقتو',
          unitPeriodsWeek: 'وقتو/ميڠڬو',
          unitPersons: 'اورڠ',
          unitRooms: 'كلس',
          spanContTag: (n) => `${n} وقتو برتوروت`,
          freeSlotLabel: 'وقتو كوسوڠ',
          unavailSlotLabel: 'تيدق لاڤڠ / عذور',
          noLessonSlot: 'تياد وقتو بليجر',
          hintClickCellToClass: 'كليك فد كوتق مات فلاجرن اونتوق مليهت جدول كلس ترسبوت',
          hintClassFooter: 'ممفافركن مات فلاجرن دان ڬورو فڠاجر • كليك كوتق مات فلاجرن اونتوق مليهت جدول ڬورو ترسبوت',
          lblPickSubDay: 'فيليه هاري:',
          lblPickSubPeriod: 'فيليه وقتو:',
          colFreeTeacher: 'ڬورو يڠ كوسوڠ سديا مڠڬنتي (---)',
          colRegSubjects: 'مات فلاجرن تتف',
          colDayTrack: 'جدول وقتو فد هاري ترسبوت (1–5)',
          colDayBusy: 'مڠاجر هاري اين',
          colWeekTotal: 'جومله سميڠڬو',
          miniFreeWord: 'كوسوڠ',
          freeEmptyTitle: 'تياد ڬورو كوسوڠ يڠ سفادن فد وقتو اين',
          freeEmptySub: 'چوبا فيليه وقتو لاين اتاو فادم تافيسن مات فلاجرن اونتوق مليهت سموا ڬورو كوسوڠ',
          freeFooterHtml: 'چاتتن: هاڽ ممفافركن ڬورو يڠ بنر٢ ميمفوڽأي وقتو كوسوڠ (<strong>---</strong>) فد هاري دان وقتو يڠ دفيليه، سرتا مڠچواليكن ڬورو يڠ سدڠ مڠاجر اتاو تيدق لاڤڠ (<strong>-x-</strong>) سچارا اوتوماتيك • كليك فد باريس اونتوق مليهت جدول فنوه'
        }
      };

      // Forgiving Arabic/Jawi/Thai text normalization for search
      function normalizeText(str) {
        if (!str) return '';
        return String(str)
          .toLowerCase()
          .replace(/[\u0640\u064B-\u065F\u0670]/g, '')
          .replace(/[أإآٱ]/g, 'ا')
          .replace(/ؤ/g, 'و')
          .replace(/[ئى]/g, 'ي')
          .replace(/ة/g, 'ه')
          .replace(/چ/g, 'ج')
          .replace(/ڠ/g, 'غ')
          .replace(/[ڬݢ]/g, 'ك')
          .replace(/ڤ/g, 'ف')
          .replace(/ڽ/g, 'ن')
          .replace(/\s+/g, ' ')
          .trim();
      }

      I18N.th.tabs.manage = 'จัดการตารางสอน';
      I18N.ar.tabs.manage = 'إدارة الجدول';
      I18N.jawi.tabs.manage = 'أوروس جدول';

      Object.assign(I18N.th, {
        lblManageTeacher: 'เลือกครูผู้สอนเพื่อแก้ไขตาราง',
        btnEditTeacherName: 'แก้ไขชื่อครู',
        btnAddTeacher: '+ เพิ่มครูใหม่',
        badgeModified: 'มีการแก้ไขเพิ่มเติม',
        btnOpenAddSlot: '+ เพิ่ม / แก้ไขคาบสอน',
        btnResetDefault: 'คืนค่าต้นฉบับ',
        lblConfirmReset: 'ยืนยันคืนค่าต้นฉบับ?',
        btnConfirmYes: 'ยืนยัน',
        btnCancel: 'ยกเลิก',
        manageHint: 'คลิกที่ช่องใดก็ได้ในตารางด้านล่าง (คาบสอน, คาบว่าง ---, หรือคาบงดสอน -x-) เพื่อเพิ่ม แก้ไข หรือลบคาบสอนได้ทันที',
        slotModalTitle: 'เพิ่ม / แก้ไขคาบสอน',
        tabTypeLesson: 'คาบสอนปกติ',
        tabTypeFree: 'คาบว่าง (---)',
        tabTypeUnavail: 'งดสอน (-x-)',
        lblSlotStartPeriod: 'คาบเริ่มต้น',
        lblSlotSpan: 'จำนวนคาบต่อเนื่อง',
        optSpan1: '1 คาบ (ปกติ)',
        optSpan2: '2 คาบต่อเนื่อง',
        lblSlotColor: 'สีพื้นหลังช่องตาราง',
        btnDeleteLesson: 'ลบคาบสอนนี้',
        btnSaveChanges: 'บันทึกการเปลี่ยนแปลง',
        teacherAddTitle: 'เพิ่มครูผู้สอนใหม่',
        teacherEditTitle: 'แก้ไขชื่อครูผู้สอน',
        lblTeacherProfileName: 'ชื่อครูผู้สอน (อาหรับ / ยาวี / ไทย)',
        errReqClassSubj: 'กรุณากรอกชื่อห้องเรียนและรายวิชาให้ครบถ้วน',
        errReqTeacherName: 'กรุณากรอกชื่อครูผู้สอน',
        errSpanOverflow: 'คาบที่ 5 ไม่สามารถตั้งเป็น 2 คาบต่อเนื่องได้',
        errClassConflict: (cls, subj, tName) => `ซ้ำซ้อน: ห้อง ${cls} มีคาบเรียนวิชา ${subj} (ครู ${tName}) ในเวลานี้อยู่แล้ว`,
        manageStatusText: (tName, p) => `โหมดฝ่ายวิชาการ • กำลังแก้ไขตารางของ ${tName} (${p} คาบ/สัปดาห์)`
      });

      Object.assign(I18N.ar, {
        lblManageTeacher: 'اختر المعلم لتعديل جدوله',
        btnEditTeacherName: 'تعديل اسم المعلم',
        btnAddTeacher: '+ إضافة معلم جديد',
        badgeModified: 'تعديلات مخصصة محفوظة',
        btnOpenAddSlot: '+ إضافة / تعديل حصة',
        btnResetDefault: 'استعادة الأصل',
        lblConfirmReset: 'تأكيد استعادة الجدول الأصلي؟',
        btnConfirmYes: 'تأكيد',
        btnCancel: 'إلغاء',
        manageHint: 'اضغط على أي خلية في الجدول أدناه (حصة دراسية، شاغرة ---، أو غير متاح -x-) للإضافة أو التعديل أو الحذف فوراً',
        slotModalTitle: 'إضافة / تعديل حصة دراسية',
        tabTypeLesson: 'حصة دراسية',
        tabTypeFree: 'حصة شاغرة (---)',
        tabTypeUnavail: 'غير متاح (-x-)',
        lblSlotStartPeriod: 'الحصة الأولى',
        lblSlotSpan: 'عدد الحصص المتتالية',
        optSpan1: 'حصة واحدة (1)',
        optSpan2: 'حصتان متتاليتان (2)',
        lblSlotColor: 'لون خلفية الخلية',
        btnDeleteLesson: 'حذف هذه الحصة',
        btnSaveChanges: 'حفظ التغييرات',
        teacherAddTitle: 'إضافة معلم جديد',
        teacherEditTitle: 'تعديل اسم المعلم',
        lblTeacherProfileName: 'اسم المعلم',
        errReqClassSubj: 'يرجى إدخال اسم الفصل والمادة الدراسية',
        errReqTeacherName: 'يرجى إدخال اسم المعلم',
        errSpanOverflow: 'لا يمكن جعل الحصة الخامسة حصتين متتاليتين',
        errClassConflict: (cls, subj, tName) => `تعارض: الفصل ${cls} لديه حصة (${subj} - ${tName}) في نفس الوقت`,
        manageStatusText: (tName, p) => `وضع الشؤون التعليمية • تعديل جدول ${tName} (${p} حصة/أسبوع)`
      });

      Object.assign(I18N.jawi, {
        lblManageTeacher: 'فيليه ڬورو اونتوق اوبه جدول',
        btnEditTeacherName: 'اوبه نام ڬورو',
        btnAddTeacher: '+ تمبه ڬورو بارو',
        badgeModified: 'أد فينداأن ترسيمفن',
        btnOpenAddSlot: '+ تمبه / اوبه وقتو',
        btnResetDefault: 'كمبالي كفد اصل',
        lblConfirmReset: 'صحكن كمبالي كفد جدول اصل؟',
        btnConfirmYes: 'صحكن',
        btnCancel: 'بطل',
        manageHint: 'كليك فد مان٢ كوتق د باوه (وقتو مڠاجر، وقتو كوسوڠ ---، اتاو عذور -x-) اونتوق منمبه، مڠوبه اتاو ممادم سڬرا',
        slotModalTitle: 'تمبه / اوبه وقتو فڠاجرن',
        tabTypeLesson: 'وقتو مڠاجر',
        tabTypeFree: 'وقتو كوسوڠ (---)',
        tabTypeUnavail: 'تيدق لاڤڠ (-x-)',
        lblSlotStartPeriod: 'وقتو اول',
        lblSlotSpan: 'بيلڠن وقتو برتوروت',
        optSpan1: '1 وقتو (بياسا)',
        optSpan2: '2 وقتو برتوروت',
        lblSlotColor: 'ورنا لاتربلاكڠ كوتق',
        btnDeleteLesson: 'فادم وقتو اين',
        btnSaveChanges: 'سيمفن فروبهن',
        teacherAddTitle: 'تمبه ڬورو فڠاجر بارو',
        teacherEditTitle: 'اوبه نام ڬورو فڠاجر',
        lblTeacherProfileName: 'نام ڬورو فڠاجر',
        errReqClassSubj: 'سيلا ايسي كلس دان مات فلاجرن دڠن لڠكف',
        errReqTeacherName: 'سيلا ايسي نام ڬورو فڠاجر',
        errSpanOverflow: 'وقتو ك-5 تيدق بوليه دجاديكن 2 وقتو برتوروت',
        errClassConflict: (cls, subj, tName) => `برتينديه: كلس ${cls} سوده أد وقتو (${subj} - ${tName}) فد ماس اين`,
        manageStatusText: (tName, p) => `مود فنتدبيرن • مڠوبه جدول ${tName} (${p} وقتو/ميڠڬو)`
      });

      function compareClasses(a, b) {
        const parseCls = (c) => {
          if (c.startsWith('ت')) return { group: 1, major: parseInt(c.slice(1), 10) || 0, minor: 0, raw: c };
          const slashMatch = c.match(/^(\d+)\/(\d+)$/);
          if (slashMatch) return { group: 2, major: parseInt(slashMatch[1], 10), minor: parseInt(slashMatch[2], 10), raw: c };
          if (c.startsWith('AEP')) return { group: 3, major: parseInt(c.slice(3), 10) || 0, minor: 0, raw: c };
          if (c.startsWith('C')) return { group: 4, major: parseInt(c.slice(1), 10) || 0, minor: 0, raw: c };
          return { group: 5, major: 0, minor: 0, raw: c };
        };
        const pa = parseCls(a);
        const pb = parseCls(b);
        if (pa.group !== pb.group) return pa.group - pb.group;
        if (pa.major !== pb.major) return pa.major - pb.major;
        if (pa.minor !== pb.minor) return pa.minor - pb.minor;
        return pa.raw.localeCompare(pb.raw, 'ar');
      }

      function getInitialGroupLetter(name) {
        const ch = (name || '').trim().charAt(0);
        if (!ch) return '';
        if (/[أإآٱ]/.test(ch)) return 'ا';
        return ch;
      }

      const teacherById = new Map();
      const classMap = new Map();
      let LESSONS = [];
      let CLASSES = [];
      let SUBJECTS = [];
      let INITIAL_LETTERS = [];

      function rebuildDataIndexes() {
        teacherById.clear();
        classMap.clear();

        TEACHERS.forEach(t => {
          if (!Array.isArray(t.unavailGrid) || t.unavailGrid.length < 6) {
            t.unavailGrid = [[], [], [], [], [], []];
          }
          t.normName = normalizeText(t.name);
          t.lessons = [];
          teacherById.set(t.id, t);
        });

        LESSONS = RAW_LESSONS.map((row, idx) => {
          const [page, dayIdx, pStart, span, cls, subj, bg, isWhiteFg] = row;
          const teacherObj = teacherById.get(page);
          const teacherName = teacherObj ? teacherObj.name : '';
          const dayAr = META.days[dayIdx] || '';
          const dayTh = THAI_DAYS[dayIdx] || '';
          const dayJawi = JAWI_DAYS[dayIdx] || '';
          const pEnd = pStart + span - 1;
          const startTime = (META.periods[pStart] || '').split('-')[0].trim();
          const endTime = (META.periods[pEnd] || '').split('-')[1]?.trim() || '';
          const timeRange = span > 1 ? `${startTime} - ${endTime}` : (META.periods[pStart] || '');
          const timeLabel = span > 1
            ? `คาบ ${pStart + 1}–${pEnd + 1} (${startTime} - ${endTime})`
            : `คาบ ${pStart + 1} (${META.periods[pStart] || ''})`;

          const item = {
            id: idx,
            rawIdx: idx,
            page,
            teacher: teacherName,
            dayIdx,
            dayAr,
            dayTh,
            dayJawi,
            pStart,
            pEnd,
            span,
            timeRange,
            timeLabel,
            cls,
            subj,
            bg,
            fg: isWhiteFg ? '#FFFFFF' : '#000000',
            searchBlob: normalizeText(`${page} #${page} หน้า${page} صفحة${page} ${teacherName} ${cls} ${subj} ${dayAr} ${dayJawi} วัน${dayTh} ${timeLabel}`)
          };
          if (teacherObj) teacherObj.lessons.push(item);
          return item;
        });

        const subjectSet = new Set();
        LESSONS.forEach(l => {
          subjectSet.add(l.subj);
          if (!classMap.has(l.cls)) {
            classMap.set(l.cls, { name: l.cls, normName: normalizeText(l.cls), periods: 0, lessons: [] });
          }
          const cObj = classMap.get(l.cls);
          cObj.periods += l.span;
          cObj.lessons.push(l);
        });

        CLASSES = Array.from(classMap.values()).sort((a, b) => compareClasses(a.name, b.name));
        SUBJECTS = Array.from(subjectSet).sort((a, b) => a.localeCompare(b, 'ar'));

        const initialLetterSet = new Set();
        TEACHERS.forEach(t => {
          // Recalculate exact periods, unavail, and free out of 30 slots
          const occupied = Array.from({ length: 6 }, () => [false, false, false, false, false]);
          let pSum = 0;
          t.lessons.forEach(l => {
            pSum += l.span;
            for (let p = l.pStart; p <= l.pEnd; p++) {
              if (l.dayIdx >= 0 && l.dayIdx < 6 && p >= 0 && p < 5) occupied[l.dayIdx][p] = true;
            }
          });
          let uCount = 0;
          for (let d = 0; d < 6; d++) {
            t.unavailGrid[d] = (t.unavailGrid[d] || []).filter(p => p >= 0 && p < 5 && !occupied[d][p]);
            uCount += t.unavailGrid[d].length;
          }
          t.periods = pSum;
          t.unavail = uCount;
          t.free = Math.max(0, 30 - pSum - uCount);

          const sSet = new Set(t.lessons.map(l => l.subj));
          const cSet = new Set(t.lessons.map(l => l.cls));
          t.subjects = Array.from(sSet).sort((a, b) => a.localeCompare(b, 'ar'));
          t.classes = Array.from(cSet).sort(compareClasses);
          t.firstLetter = getInitialGroupLetter(t.name);
          if (t.firstLetter) initialLetterSet.add(t.firstLetter);
          t.searchBlob = normalizeText(`${t.id} #${t.id} หน้า${t.id} ${t.name} ${t.subjects.join(' ')} ${t.classes.join(' ')}`);
        });

        INITIAL_LETTERS = Array.from(initialLetterSet).sort((a, b) => a.localeCompare(b, 'ar'));
      }

      rebuildDataIndexes();

      let savedLang = 'th';
      let savedTheme = 'emerald';
      try {
        const sl = localStorage.getItem('thaqafah_tt_lang');
        if (sl && I18N[sl]) savedLang = sl;
        const st = localStorage.getItem('thaqafah_tt_theme');
        if (st && ['emerald', 'sapphire', 'teal', 'amber'].includes(st)) savedTheme = st;
      } catch (e) {}

      // App State
      const state = {
        lang: savedLang,
        theme: savedTheme,
        view: 'self', // 'self' | 'explorer' | 'teacher' | 'class' | 'free'
        selfQuery: '',
        selfLetter: '',
        selfPickedTeacherId: null,
        selfShowList: true,
        selfDayFilter: 'all',
        query: '',
        teacherId: '',
        cls: '',
        subj: '',
        dayIdx: '',
        periodIdx: '',
        sortKey: 'page',
        sortDir: 'asc',
        page: 1,
        pageSize: 25,
        selectedTeacherId: TEACHERS[0] ? TEACHERS[0].id : 1,
        selectedClass: CLASSES[0] ? CLASSES[0].name : '',
        teacherQuickFilter: '',
        classQuickFilter: '',
        subDayIdx: 0,
        subPeriodIdx: 0,
        subSortKey: 'dayBusy',
        subSortDir: 'asc',
        modalTeacherId: null
      };

      function T() {
        return I18N[state.lang] || I18N.th;
      }

      // DOM Elements
      const langSwitcher = document.getElementById('langSwitcher');
      const themeSwitcher = document.getElementById('themeSwitcher');
      const badgeYearText = document.getElementById('badgeYearText');
      const appTitleMainText = document.getElementById('appTitleMainText');
      const themeLabelText = document.getElementById('themeLabelText');
      const headerMetaBox = document.getElementById('headerMetaBox');

      const adminFilterGrid = document.getElementById('adminFilterGrid');
      const selfView = document.getElementById('selfView');
      const selfSearchInput = document.getElementById('selfSearchInput');
      const selfClearInputBtn = document.getElementById('selfClearInputBtn');
      const selfTeacherSelect = document.getElementById('selfTeacherSelect');
      const selfClearTeacherBtn = document.getElementById('selfClearTeacherBtn');
      const selfLetterWrap = document.getElementById('selfLetterWrap');
      const selfLetterRow = document.getElementById('selfLetterRow');
      const selfSelectedBanner = document.getElementById('selfSelectedBanner');
      const selfMatchSection = document.getElementById('selfMatchSection');
      const selfTeacherGrid = document.getElementById('selfTeacherGrid');
      const selfNoMatch = document.getElementById('selfNoMatch');
      const selfTimetableResult = document.getElementById('selfTimetableResult');

      const searchInput = document.getElementById('searchInput');
      const clearSearchBtn = document.getElementById('clearSearchBtn');
      const teacherFilter = document.getElementById('teacherFilter');
      const classFilter = document.getElementById('classFilter');
      const subjectFilter = document.getElementById('subjectFilter');
      const dayFilter = document.getElementById('dayFilter');
      const periodFilter = document.getElementById('periodFilter');
      const activeFiltersBar = document.getElementById('activeFiltersBar');
      const filterChipsContainer = document.getElementById('filterChipsContainer');
      const resetAllBtn = document.getElementById('resetAllBtn');
      const emptyResetBtn = document.getElementById('emptyResetBtn');
      const liveResultSummary = document.getElementById('liveResultSummary');

      const explorerView = document.getElementById('explorerView');
      const teacherView = document.getElementById('teacherView');
      const classView = document.getElementById('classView');
      const freeView = document.getElementById('freeView');

      const subDayPills = document.getElementById('subDayPills');
      const subPeriodPills = document.getElementById('subPeriodPills');
      const subClassContext = document.getElementById('subClassContext');
      const freeTeachersTable = document.getElementById('freeTeachersTable');
      const freeTableBody = document.getElementById('freeTableBody');
      const freeEmptyState = document.getElementById('freeEmptyState');
      const freeEmptyResetBtn = document.getElementById('freeEmptyResetBtn');

      const explorerTableBody = document.getElementById('explorerTableBody');
      const explorerEmptyState = document.getElementById('explorerEmptyState');
      const paginationBar = document.getElementById('paginationBar');
      const paginationInfo = document.getElementById('paginationInfo');
      const pageSizeSelect = document.getElementById('pageSizeSelect');
      const prevPageBtn = document.getElementById('prevPageBtn');
      const nextPageBtn = document.getElementById('nextPageBtn');
      const pageIndicator = document.getElementById('pageIndicator');

      const teacherQuickSearch = document.getElementById('teacherQuickSearch');
      const teacherDirCount = document.getElementById('teacherDirCount');
      const teacherDirList = document.getElementById('teacherDirList');
      const teacherTimetableContainer = document.getElementById('teacherTimetableContainer');

      const classQuickSearch = document.getElementById('classQuickSearch');
      const classDirCount = document.getElementById('classDirCount');
      const classDirList = document.getElementById('classDirList');
      const classTimetableContainer = document.getElementById('classTimetableContainer');

      const teacherModal = document.getElementById('teacherModal');
      const modalContentArea = document.getElementById('modalContentArea');

      function escapeHtml(str) {
        return String(str)
          .replace(/&/g, '&amp;')
          .replace(/</g, '&lt;')
          .replace(/>/g, '&gt;')
          .replace(/"/g, '&quot;');
      }

      function getDayPlainText(dIdx) {
        const dAr = META.days[dIdx] || '';
        if (state.lang === 'ar') return dAr;
        if (state.lang === 'jawi') return JAWI_DAYS[dIdx] || dAr;
        return `${dAr} (${THAI_DAYS[dIdx] || ''})`;
      }

      function getDayPillHtml(dIdx) {
        const dAr = META.days[dIdx] || '';
        if (state.lang === 'ar') return `<span class="ar-text">${escapeHtml(dAr)}</span>`;
        if (state.lang === 'jawi') return `<span class="ar-text">${escapeHtml(JAWI_DAYS[dIdx] || dAr)}</span>`;
        return `<span class="ar-text">${escapeHtml(dAr)}</span><span>(${escapeHtml(THAI_DAYS[dIdx] || '')})</span>`;
      }

      function getLessonPeriodHtml(item) {
        const tr = T();
        const pPart = item.span > 1
          ? tr.periodSpanShort(item.pStart + 1, item.pEnd + 1)
          : tr.periodShort(item.pStart + 1);
        return `<span>${escapeHtml(pPart)}</span> <span class="ltr-token">(${escapeHtml(item.timeRange)})</span>`;
      }

      function setSortHeaderLabel(th, label) {
        if (!th) return;
        const ind = th.querySelector('.sort-ind');
        const indText = ind ? ind.textContent : '↕';
        th.innerHTML = `${escapeHtml(label)} <span class="sort-ind">${escapeHtml(indText)}</span>`;
      }

      function applyTheme(themeName) {
        state.theme = themeName;
        document.documentElement.setAttribute('data-theme', themeName);
        if (themeSwitcher) {
          themeSwitcher.querySelectorAll('[data-set-theme]').forEach(btn => {
            const active = btn.getAttribute('data-set-theme') === themeName;
            btn.classList.toggle('active', active);
            btn.setAttribute('aria-pressed', active ? 'true' : 'false');
          });
        }
        try {
          localStorage.setItem('thaqafah_tt_theme', themeName);
        } catch (e) {}
      }

      function syncDynamicDropdownOptions() {
        const tr = T();
        if (teacherFilter.options[0]) teacherFilter.options[0].textContent = tr.allTeachers;
        if (classFilter.options[0]) classFilter.options[0].textContent = tr.allClasses;
        if (subjectFilter.options[0]) subjectFilter.options[0].textContent = tr.allSubjects;
        if (dayFilter.options[0]) dayFilter.options[0].textContent = tr.allDays;
        if (periodFilter.options[0]) periodFilter.options[0].textContent = tr.allPeriods;
        if (selfTeacherSelect.options[0]) selfTeacherSelect.options[0].textContent = tr.optSelfPrompt;

        for (let i = 0; i < META.days.length; i++) {
          if (dayFilter.options[i + 1]) {
            dayFilter.options[i + 1].textContent = getDayPlainText(i);
          }
        }
        for (let i = 0; i < META.periods.length; i++) {
          if (periodFilter.options[i + 1]) {
            periodFilter.options[i + 1].textContent = `${tr.periodShort(i + 1)}: ${META.periods[i]}`;
          }
        }
        Array.from(pageSizeSelect.options).forEach(opt => {
          opt.textContent = `${opt.value} ${tr.unitItems}`;
        });
      }

      function applyStaticTranslations() {
        const tr = T();
        const isRtl = state.lang !== 'th';
        document.documentElement.lang = state.lang === 'ar' ? 'ar' : (state.lang === 'jawi' ? 'ms-Arab' : 'th');
        document.documentElement.dir = isRtl ? 'rtl' : 'ltr';
        document.title = tr.docTitle;

        if (langSwitcher) {
          langSwitcher.querySelectorAll('[data-set-lang]').forEach(btn => {
            const active = btn.getAttribute('data-set-lang') === state.lang;
            btn.classList.toggle('active', active);
            btn.setAttribute('aria-pressed', active ? 'true' : 'false');
          });
        }

        if (badgeYearText) badgeYearText.textContent = tr.badgeYear;
        if (appTitleMainText) appTitleMainText.textContent = tr.appTitleMain;
        if (themeLabelText) themeLabelText.textContent = tr.themeLabel;
        if (headerMetaBox) headerMetaBox.innerHTML = tr.headerMetaHtml;

        if (themeSwitcher) {
          themeSwitcher.querySelectorAll('[data-set-theme]').forEach(btn => {
            const key = btn.getAttribute('data-set-theme');
            const tName = tr.themeNames[key] || key;
            btn.title = tName;
            btn.setAttribute('aria-label', tName);
          });
        }

        document.querySelectorAll('.view-tab').forEach(btn => {
          const v = btn.getAttribute('data-view');
          const sp = btn.querySelector('span');
          if (sp && tr.tabs[v]) sp.textContent = tr.tabs[v];
        });

        const setLabelFor = (id, txt) => {
          const lbl = document.querySelector(`label[for="${id}"]`);
          if (lbl) lbl.textContent = txt;
        };

        setLabelFor('searchInput', tr.lblSearch);
        searchInput.placeholder = tr.phSearch;
        setLabelFor('teacherFilter', tr.lblTeacher);
        setLabelFor('classFilter', tr.lblClass);
        setLabelFor('subjectFilter', tr.lblSubject);
        setLabelFor('dayFilter', tr.lblDay);
        setLabelFor('periodFilter', tr.lblPeriod);
        resetAllBtn.textContent = tr.btnResetAll;
        emptyResetBtn.textContent = tr.btnResetAll;
        freeEmptyResetBtn.textContent = tr.btnResetExtra;

        // Self-service view static texts
        const selfH2 = selfView.querySelector('.self-hero-head h2');
        const selfP = selfView.querySelector('.self-hero-head p');
        if (selfH2) selfH2.textContent = tr.selfHeading;
        if (selfP) selfP.textContent = tr.selfSub;
        selfClearTeacherBtn.textContent = tr.btnSelfOther;
        setLabelFor('selfSearchInput', tr.lblSelfSearch);
        selfSearchInput.placeholder = tr.phSelfSearch;
        setLabelFor('selfTeacherSelect', tr.lblSelfSelect);
        const qlLabel = selfLetterWrap.querySelector('.quick-letter-label');
        if (qlLabel) qlLabel.textContent = tr.lblQuickLetter;
        const selfEmpH3 = selfNoMatch.querySelector('h3');
        const selfEmpP = selfNoMatch.querySelector('p');
        if (selfEmpH3) selfEmpH3.textContent = tr.selfEmptyTitle;
        if (selfEmpP) selfEmpP.textContent = tr.selfEmptySub;

        // Explorer table headers & empty state & pagination
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="page"]'), tr.colPage);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="teacher"]'), tr.colTeacher);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="dayIdx"]'), tr.colDay);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="pStart"]'), tr.colPeriod);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="cls"]'), tr.colClass);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="subj"]'), tr.colSubj);
        setSortHeaderLabel(document.querySelector('#lessonsTable th[data-sort="span"]'), tr.colSpan);

        const expEmpH3 = explorerEmptyState.querySelector('h3');
        const expEmpP = explorerEmptyState.querySelector('p');
        if (expEmpH3) expEmpH3.textContent = tr.expEmptyTitle;
        if (expEmpP) expEmpP.textContent = tr.expEmptySub;

        setLabelFor('pageSizeSelect', tr.lblShowRows);
        prevPageBtn.textContent = tr.btnPrev;
        nextPageBtn.textContent = tr.btnNext;

        // Teacher & Class directories
        const tDirTitle = teacherView.querySelector('.directory-title-row > span:first-child');
        if (tDirTitle) tDirTitle.textContent = tr.dirTeachersTitle;
        teacherQuickSearch.placeholder = tr.phTeacherQuick;

        const cDirTitle = classView.querySelector('.directory-title-row > span:first-child');
        if (cDirTitle) cDirTitle.textContent = tr.dirClassesTitle;
        classQuickSearch.placeholder = tr.phClassQuick;

        // Free / Substitute view static texts
        const subLabels = freeView.querySelectorAll('.sub-controls-bar .sub-picker-label');
        if (subLabels[0]) subLabels[0].textContent = tr.lblPickSubDay;
        if (subLabels[1]) subLabels[1].textContent = tr.lblPickSubPeriod;

        const freeThs = freeTeachersTable.querySelectorAll('thead th');
        setSortHeaderLabel(freeThs[0], tr.colPage);
        setSortHeaderLabel(freeThs[1], tr.colFreeTeacher);
        if (freeThs[2]) freeThs[2].textContent = tr.colRegSubjects;
        if (freeThs[3]) freeThs[3].textContent = tr.colDayTrack;
        setSortHeaderLabel(freeThs[4], tr.colDayBusy);
        setSortHeaderLabel(freeThs[5], tr.colWeekTotal);

        const freeEmpH3 = freeEmptyState.querySelector('h3');
        const freeEmpP = freeEmptyState.querySelector('p');
        if (freeEmpH3) freeEmpH3.textContent = tr.freeEmptyTitle;
        if (freeEmpP) freeEmpP.textContent = tr.freeEmptySub;

        const freeFooterSpan = freeView.querySelector('.tt-footer > span');
        if (freeFooterSpan) freeFooterSpan.innerHTML = tr.freeFooterHtml;

        syncDynamicDropdownOptions();
      }

      function setLanguage(lang) {
        if (!I18N[lang]) return;
        state.lang = lang;
        try {
          localStorage.setItem('thaqafah_tt_lang', lang);
        } catch (e) {}
        applyStaticTranslations();
        renderAll();
        if (state.modalTeacherId !== null && teacherModal.classList.contains('open')) {
          openTeacherModal(state.modalTeacherId);
        }
      }

      // Populate Select Filters
      function initDropdowns() {
        TEACHERS.forEach(t => {
          const labelText = `${String(t.id).padStart(2, '0')}. ${t.name}`;
          const opt = document.createElement('option');
          opt.value = String(t.id);
          opt.textContent = labelText;
          teacherFilter.appendChild(opt);

          const selfOpt = document.createElement('option');
          selfOpt.value = String(t.id);
          selfOpt.textContent = labelText;
          selfTeacherSelect.appendChild(selfOpt);
        });

        CLASSES.forEach(c => {
          const opt = document.createElement('option');
          opt.value = c.name;
          opt.textContent = c.name;
          classFilter.appendChild(opt);
        });

        SUBJECTS.forEach(s => {
          const opt = document.createElement('option');
          opt.value = s;
          opt.textContent = s;
          subjectFilter.appendChild(opt);
        });

        META.days.forEach((d, idx) => {
          const opt = document.createElement('option');
          opt.value = String(idx);
          opt.textContent = `${d} (${THAI_DAYS[idx]})`;
          dayFilter.appendChild(opt);
        });

        META.periods.forEach((p, idx) => {
          const opt = document.createElement('option');
          opt.value = String(idx);
          opt.textContent = `คาบ ${idx + 1}: ${p}`;
          periodFilter.appendChild(opt);
        });
      }

      // Check if a lesson matches active toolbar filters
      function lessonMatches(l) {
        if (state.teacherId !== '' && l.page !== Number(state.teacherId)) return false;
        if (state.cls !== '' && l.cls !== state.cls) return false;
        if (state.subj !== '' && l.subj !== state.subj) return false;
        if (state.dayIdx !== '' && l.dayIdx !== Number(state.dayIdx)) return false;
        if (state.periodIdx !== '') {
          const p = Number(state.periodIdx);
          if (p < l.pStart || p > l.pEnd) return false;
        }
        if (state.query.trim() !== '') {
          const tokens = normalizeText(state.query).split(' ').filter(Boolean);
          for (const tk of tokens) {
            if (!l.searchBlob.includes(tk)) return false;
          }
        }
        return true;
      }

      function hasAnyFilter() {
        return Boolean(
          state.query.trim() ||
          state.teacherId !== '' ||
          state.cls !== '' ||
          state.subj !== '' ||
          state.dayIdx !== '' ||
          state.periodIdx !== ''
        );
      }

      function getFilteredLessons() {
        const matched = LESSONS.filter(lessonMatches);
        const dir = state.sortDir === 'asc' ? 1 : -1;
        matched.sort((a, b) => {
          let cmp = 0;
          switch (state.sortKey) {
            case 'page':
              cmp = a.page - b.page || a.dayIdx - b.dayIdx || a.pStart - b.pStart;
              break;
            case 'teacher':
              cmp = a.teacher.localeCompare(b.teacher, 'ar') || a.dayIdx - b.dayIdx || a.pStart - b.pStart;
              break;
            case 'dayIdx':
              cmp = a.dayIdx - b.dayIdx || a.pStart - b.pStart || a.page - b.page;
              break;
            case 'pStart':
              cmp = a.pStart - b.pStart || a.dayIdx - b.dayIdx || a.page - b.page;
              break;
            case 'cls':
              cmp = compareClasses(a.cls, b.cls) || a.dayIdx - b.dayIdx || a.pStart - b.pStart;
              break;
            case 'subj':
              cmp = a.subj.localeCompare(b.subj, 'ar') || compareClasses(a.cls, b.cls);
              break;
            case 'span':
              cmp = a.span - b.span || a.page - b.page;
              break;
            default:
              cmp = a.id - b.id;
          }
          return cmp * dir;
        });
        return matched;
      }

      function renderFilterChips() {
        const tr = T();
        clearSearchBtn.classList.toggle('visible', state.query.length > 0);
        if (state.view === 'self' || !hasAnyFilter()) {
          activeFiltersBar.classList.remove('visible');
          filterChipsContainer.innerHTML = '';
          return;
        }
        activeFiltersBar.classList.add('visible');
        const chips = [];
        if (state.query.trim()) {
          chips.push({ key: 'query', label: `${tr.chipQuery}: "${state.query.trim()}"` });
        }
        if (state.teacherId !== '') {
          const t = teacherById.get(Number(state.teacherId));
          chips.push({ key: 'teacherId', label: `${tr.chipTeacher}: ${t ? t.name : state.teacherId}` });
        }
        if (state.cls !== '') {
          chips.push({ key: 'cls', label: `${tr.chipClass}: ${state.cls}` });
        }
        if (state.subj !== '') {
          chips.push({ key: 'subj', label: `${tr.chipSubj}: ${state.subj}` });
        }
        if (state.dayIdx !== '') {
          const di = Number(state.dayIdx);
          chips.push({ key: 'dayIdx', label: `${tr.chipDay}: ${getDayPlainText(di)}` });
        }
        if (state.periodIdx !== '') {
          const pi = Number(state.periodIdx);
          chips.push({ key: 'periodIdx', label: `${tr.periodShort(pi + 1)}: ${META.periods[pi]}` });
        }

        filterChipsContainer.innerHTML = chips.map(ch => `
          <span class="filter-chip">
            <span>${escapeHtml(ch.label)}</span>
            <button type="button" data-clear-key="${ch.key}" aria-label="×">×</button>
          </span>
        `).join('');
      }

      // Render Explorer Table
      function renderExplorer(filtered) {
        const tr = T();
        const totalPeriods = filtered.reduce((acc, item) => acc + item.span, 0);
        if (state.lang === 'ar') {
          liveResultSummary.innerHTML = `النتائج: <strong>${filtered.length.toLocaleString()}</strong> حصة مجدولة (إجمالي <strong>${totalPeriods.toLocaleString()}</strong> ${escapeHtml(tr.unitPeriods)})`;
        } else if (state.lang === 'jawi') {
          liveResultSummary.innerHTML = `دجومفأي <strong>${filtered.length.toLocaleString()}</strong> سناراي فڠاجرن (جومله <strong>${totalPeriods.toLocaleString()}</strong> ${escapeHtml(tr.unitPeriods)})`;
        } else {
          liveResultSummary.innerHTML = `พบ <strong>${filtered.length.toLocaleString()}</strong> รายการสอน (รวม <strong>${totalPeriods.toLocaleString()}</strong> คาบ)`;
        }

        document.querySelectorAll('#lessonsTable thead th.sortable').forEach(th => {
          const key = th.getAttribute('data-sort');
          const ind = th.querySelector('.sort-ind');
          if (key === state.sortKey) {
            th.classList.add('sorted');
            if (ind) ind.textContent = state.sortDir === 'asc' ? '↑' : '↓';
          } else {
            th.classList.remove('sorted');
            if (ind) ind.textContent = '↕';
          }
        });

        if (filtered.length === 0) {
          explorerTableBody.innerHTML = '';
          document.getElementById('lessonsTable').classList.add('hidden');
          paginationBar.classList.add('hidden');
          explorerEmptyState.classList.remove('hidden');
          return;
        }

        document.getElementById('lessonsTable').classList.remove('hidden');
        paginationBar.classList.remove('hidden');
        explorerEmptyState.classList.add('hidden');

        const totalPages = Math.max(1, Math.ceil(filtered.length / state.pageSize));
        if (state.page > totalPages) state.page = totalPages;
        const startIdx = (state.page - 1) * state.pageSize;
        const slice = filtered.slice(startIdx, startIdx + state.pageSize);

        explorerTableBody.innerHTML = slice.map(item => {
          const dayCellHtml = state.lang === 'ar'
            ? `<span class="ar-text" style="font-weight:700;">${escapeHtml(item.dayAr)}</span>`
            : state.lang === 'jawi'
            ? `<span class="ar-text" style="font-weight:700;">${escapeHtml(item.dayJawi)}</span>`
            : `<span class="ar-text" style="font-weight:700;">${escapeHtml(item.dayAr)}</span><span style="color:var(--muted); font-size:12.5px; margin-left:4px;">(${escapeHtml(item.dayTh)})</span>`;

          return `
            <tr data-open-teacher="${item.page}">
              <td class="num-col"><span class="dir-num ltr-token">#${String(item.page).padStart(2, '0')}</span></td>
              <td><strong class="ar-text" style="font-size:15.5px;">${escapeHtml(item.teacher)}</strong></td>
              <td>${dayCellHtml}</td>
              <td><span class="period-pill">${getLessonPeriodHtml(item)}</span></td>
              <td>
                <span class="cls-badge">
                  <span class="swatch-dot" style="background:${escapeHtml(item.bg)};"></span>
                  <span class="ltr-token">${escapeHtml(item.cls)}</span>
                </span>
              </td>
              <td>
                <span class="subj-cell-wrap">
                  <span class="ar-text" style="font-size:15.5px; font-weight:600;">${escapeHtml(item.subj)}</span>
                </span>
              </td>
              <td class="num-col">${item.span} ${escapeHtml(tr.unitPeriods)}</td>
            </tr>
          `;
        }).join('');

        const endNum = Math.min(startIdx + state.pageSize, filtered.length);
        if (state.lang === 'ar') {
          paginationInfo.textContent = `عرض ${startIdx + 1}–${endNum} من أصل ${filtered.length.toLocaleString()}`;
          pageIndicator.textContent = `${tr.colPage} ${state.page} / ${totalPages}`;
        } else if (state.lang === 'jawi') {
          paginationInfo.textContent = `ممفافركن ${startIdx + 1}–${endNum} درفد ${filtered.length.toLocaleString()} سناراي`;
          pageIndicator.textContent = `${tr.colPage} ${state.page} / ${totalPages}`;
        } else {
          paginationInfo.textContent = `แสดง ${startIdx + 1}–${endNum} จาก ${filtered.length.toLocaleString()} รายการ`;
          pageIndicator.textContent = `หน้า ${state.page} / ${totalPages}`;
        }
        prevPageBtn.disabled = state.page <= 1;
        nextPageBtn.disabled = state.page >= totalPages;
      }

      function buildDayHeaderCellHtml(dayAr, dIdx) {
        if (state.lang === 'ar') {
          return `<span class="day-ar">${escapeHtml(dayAr)}</span>`;
        }
        if (state.lang === 'jawi') {
          return `<span class="day-ar">${escapeHtml(JAWI_DAYS[dIdx] || dayAr)}</span>`;
        }
        return `<span class="day-ar">${escapeHtml(dayAr)}</span><span class="day-th">${escapeHtml(THAI_DAYS[dIdx])}</span>`;
      }

      // Build Weekly Timetable Grid HTML for a Teacher
      function buildTeacherTimetableHtml(teacher, options = {}) {
        const tr = T();
        if (!teacher) {
          return `<div class="empty-state"><h3>${escapeHtml(tr.teacherEmptyDir)}</h3></div>`;
        }
        const isModal = Boolean(options.isModal);
        const isSelf = Boolean(options.isSelf);
        const filterActive = !isSelf && hasAnyFilter();

        const rowsHtml = META.days.map((dayAr, dIdx) => {
          const dayLessons = teacher.lessons.filter(l => l.dayIdx === dIdx);
          const unavailSet = new Set((teacher.unavailGrid && teacher.unavailGrid[dIdx]) || []);
          const byStart = new Map();
          const covered = new Set();
          dayLessons.forEach(l => {
            byStart.set(l.pStart, l);
            for (let p = l.pStart + 1; p <= l.pEnd; p++) covered.add(p);
          });

          const cells = [];
          for (let p = 0; p < 5; p++) {
            if (covered.has(p)) continue;
            if (byStart.has(p)) {
              const l = byStart.get(p);
              const matched = filterActive && lessonMatches(l);
              const dimClass = filterActive && !matched ? 'dimmed' : '';
              const hlClass = matched ? 'matched-highlight' : '';
              cells.push(`
                <td colspan="${l.span}" class="tt-cell lesson-slot ${dimClass} ${hlClass}"
                    style="background:${escapeHtml(l.bg)}; color:${escapeHtml(l.fg)};"
                    data-jump-class="${escapeHtml(l.cls)}">
                  <div class="cell-top-line" dir="rtl">${escapeHtml(l.cls)}</div>
                  <div class="cell-bottom-line" dir="rtl">${escapeHtml(l.subj)}</div>
                  ${l.span > 1 ? `<span class="cell-span-tag">${escapeHtml(tr.spanContTag(l.span))}</span>` : ''}
                </td>
              `);
            } else if (unavailSet.has(p)) {
              cells.push(`<td class="tt-cell unavail-slot" title="${escapeHtml(tr.unavailSlotLabel)} (-x-)"><span class="ltr-token">-x-</span></td>`);
            } else {
              cells.push(`<td class="tt-cell free-slot" title="${escapeHtml(tr.freeSlotLabel)} (---)"><span class="ltr-token">---</span></td>`);
            }
          }

          return `
            <tr>
              <th scope="row" class="day-header">
                ${buildDayHeaderCellHtml(dayAr, dIdx)}
              </th>
              ${cells.join('')}
            </tr>
          `;
        }).join('');

        const navRightHtml = isModal
          ? `
            <div class="tt-nav-controls">
              <button type="button" class="btn" data-switch-full-teacher="${teacher.id}">${escapeHtml(tr.btnOpenTeacherTab)}</button>
              <button type="button" class="btn" data-close-modal="true">${escapeHtml(tr.btnCloseModal)}</button>
            </div>
          `
          : isSelf
          ? `
            <div class="tt-nav-controls">
              <button type="button" class="btn" data-self-reset-teacher="true">${escapeHtml(tr.btnChangeTeacher)}</button>
            </div>
          `
          : `
            <div class="tt-nav-controls">
              <button type="button" class="btn" id="prevTeacherBtn" ${teacher.id <= 1 ? 'disabled' : ''}>${escapeHtml(tr.btnPrevTeacher)}</button>
              <button type="button" class="btn" id="nextTeacherBtn" ${teacher.id >= TEACHERS.length ? 'disabled' : ''}>${escapeHtml(tr.btnNextTeacher)}</button>
            </div>
          `;

        return `
          <div class="tt-card-top">
            <div class="tt-identity">
              <span class="tt-institution-sub ar-text">${escapeHtml(META.title || '')}</span>
              <h2 class="tt-main-heading" ${isModal ? 'id="modalTeacherHeading"' : ''}>
                <span class="ar-text">${escapeHtml(teacher.name)}</span>
                <span class="page-pill">${escapeHtml(tr.colPage)} ${teacher.id} • ${teacher.periods} ${escapeHtml(tr.unitPeriodsWeek)}</span>
              </h2>
            </div>
            ${navRightHtml}
          </div>

          <div class="tt-scroll-wrap">
            <table class="fet-grid" aria-label="${escapeHtml(teacher.name)}">
              <thead>
                <tr>
                  <th class="corner-cell">${escapeHtml(tr.cornerDayTime)}</th>
                  ${META.periods.map((pTime, idx) => `
                    <th>
                      <span class="period-num-label">${escapeHtml(tr.periodOrdinal(idx + 1))}</span>
                      <span class="period-time-label ltr-token">${escapeHtml(pTime)}</span>
                    </th>
                  `).join('')}
                </tr>
              </thead>
              <tbody>
                ${rowsHtml}
              </tbody>
            </table>
          </div>

          <div class="tt-footer">
            <div class="tt-legend">
              <span class="legend-item">
                <span class="legend-box ltr-token" style="background:#ffffff; color:#98a29c;">---</span>
                <span>${escapeHtml(tr.freeSlotLabel)} (${teacher.free} ${escapeHtml(tr.unitPeriods)})</span>
              </span>
              <span class="legend-item">
                <span class="legend-box ltr-token" style="background:#f3f4f3; color:#7d8781;">-x-</span>
                <span>${escapeHtml(tr.unavailSlotLabel)} (${teacher.unavail} ${escapeHtml(tr.unitPeriods)})</span>
              </span>
              <span class="legend-item">
                <span>${escapeHtml(tr.hintClickCellToClass)}</span>
              </span>
            </div>
            <span class="ltr-token">${escapeHtml(META.generated || '')}</span>
          </div>
        `;
      }

      // Render Teacher View
      function renderTeacherView(filteredLessons) {
        const tr = T();
        const matchedTeacherIds = hasAnyFilter()
          ? new Set(filteredLessons.map(l => l.page))
          : new Set(TEACHERS.map(t => t.id));

        const qNorm = normalizeText(state.teacherQuickFilter);
        const visibleTeachers = TEACHERS.filter(t => {
          if (!matchedTeacherIds.has(t.id)) return false;
          if (!qNorm) return true;
          return t.normName.includes(qNorm) || String(t.id).includes(qNorm);
        });

        if (state.lang === 'ar') {
          liveResultSummary.innerHTML = `المعلمون المطابقون: <strong>${visibleTeachers.length}</strong> من ${TEACHERS.length}`;
        } else if (state.lang === 'jawi') {
          liveResultSummary.innerHTML = `ڬورو يڠ سفادن: <strong>${visibleTeachers.length}</strong> درفد ${TEACHERS.length} ${escapeHtml(tr.unitPersons)}`;
        } else {
          liveResultSummary.innerHTML = `ครูที่ตรงตามเงื่อนไข <strong>${visibleTeachers.length}</strong> จาก ${TEACHERS.length} ท่าน`;
        }
        teacherDirCount.textContent = `${visibleTeachers.length} ${tr.unitPersons}`;

        if (visibleTeachers.length > 0 && !visibleTeachers.some(t => t.id === state.selectedTeacherId)) {
          state.selectedTeacherId = visibleTeachers[0].id;
        }

        if (visibleTeachers.length === 0) {
          teacherDirList.innerHTML = `<div style="padding:16px; text-align:center; color:var(--muted); font-size:13.5px;">${escapeHtml(tr.teacherEmptyDir)}</div>`;
          teacherTimetableContainer.innerHTML = `
            <div class="empty-state">
              <h3>${escapeHtml(tr.teacherEmptyTitle)}</h3>
              <p>${escapeHtml(tr.teacherEmptySub)}</p>
            </div>
          `;
          return;
        }

        teacherDirList.innerHTML = visibleTeachers.map(t => `
          <button type="button" class="dir-item ${t.id === state.selectedTeacherId ? 'active' : ''}" data-select-teacher="${t.id}">
            <span class="dir-item-main">
              <span class="dir-num ltr-token">#${String(t.id).padStart(2, '0')}</span>
              <span class="dir-name ar-text">${escapeHtml(t.name)}</span>
            </span>
            <span class="dir-meta">${t.periods} ${escapeHtml(tr.unitPeriods)}</span>
          </button>
        `).join('');

        const currentTeacher = teacherById.get(state.selectedTeacherId) || visibleTeachers[0];
        teacherTimetableContainer.innerHTML = buildTeacherTimetableHtml(currentTeacher);

        const prevBtn = document.getElementById('prevTeacherBtn');
        const nextBtn = document.getElementById('nextTeacherBtn');
        if (prevBtn) {
          prevBtn.onclick = () => {
            if (state.selectedTeacherId > 1) {
              state.selectedTeacherId -= 1;
              if (state.teacherId !== '') {
                state.teacherId = String(state.selectedTeacherId);
                teacherFilter.value = state.teacherId;
              }
              renderAll();
            }
          };
        }
        if (nextBtn) {
          nextBtn.onclick = () => {
            if (state.selectedTeacherId < TEACHERS.length) {
              state.selectedTeacherId += 1;
              if (state.teacherId !== '') {
                state.teacherId = String(state.selectedTeacherId);
                teacherFilter.value = state.teacherId;
              }
              renderAll();
            }
          };
        }
      }

      // Render Class View
      function renderClassView(filteredLessons) {
        const tr = T();
        const matchedClassNames = hasAnyFilter()
          ? new Set(filteredLessons.map(l => l.cls))
          : new Set(CLASSES.map(c => c.name));

        const qNorm = normalizeText(state.classQuickFilter);
        const visibleClasses = CLASSES.filter(c => {
          if (!matchedClassNames.has(c.name)) return false;
          if (!qNorm) return true;
          return c.normName.includes(qNorm);
        });

        if (state.lang === 'ar') {
          liveResultSummary.innerHTML = `الفصول المطابقة: <strong>${visibleClasses.length}</strong> من ${CLASSES.length}`;
        } else if (state.lang === 'jawi') {
          liveResultSummary.innerHTML = `كلس يڠ سفادن: <strong>${visibleClasses.length}</strong> درفد ${CLASSES.length} ${escapeHtml(tr.unitRooms)}`;
        } else {
          liveResultSummary.innerHTML = `ห้องเรียนที่ตรงตามเงื่อนไข <strong>${visibleClasses.length}</strong> จาก ${CLASSES.length} ห้อง`;
        }
        classDirCount.textContent = `${visibleClasses.length} ${tr.unitRooms}`;

        if (visibleClasses.length > 0 && !visibleClasses.some(c => c.name === state.selectedClass)) {
          state.selectedClass = visibleClasses[0].name;
        }

        if (visibleClasses.length === 0) {
          classDirList.innerHTML = `<div style="padding:16px; text-align:center; color:var(--muted); font-size:13.5px;">${escapeHtml(tr.classEmptyDir)}</div>`;
          classTimetableContainer.innerHTML = `
            <div class="empty-state">
              <h3>${escapeHtml(tr.classEmptyTitle)}</h3>
              <p>${escapeHtml(tr.classEmptySub)}</p>
            </div>
          `;
          return;
        }

        classDirList.innerHTML = visibleClasses.map(c => `
          <button type="button" class="dir-item ${c.name === state.selectedClass ? 'active' : ''}" data-select-class="${escapeHtml(c.name)}">
            <span class="dir-item-main">
              <span class="dir-name ar-text">${escapeHtml(c.name)}</span>
            </span>
            <span class="dir-meta">${c.periods} ${escapeHtml(tr.unitPeriodsWeek)}</span>
          </button>
        `).join('');

        const clsObj = classMap.get(state.selectedClass) || visibleClasses[0];
        const idxInAll = CLASSES.findIndex(c => c.name === clsObj.name);
        const filterActive = hasAnyFilter();

        const rowsHtml = META.days.map((dayAr, dIdx) => {
          const dayLessons = clsObj.lessons.filter(l => l.dayIdx === dIdx);
          const byStart = new Map();
          const covered = new Set();
          dayLessons.forEach(l => {
            byStart.set(l.pStart, l);
            for (let p = l.pStart + 1; p <= l.pEnd; p++) covered.add(p);
          });

          const cells = [];
          for (let p = 0; p < 5; p++) {
            if (covered.has(p)) continue;
            if (byStart.has(p)) {
              const l = byStart.get(p);
              const matched = filterActive && lessonMatches(l);
              const dimClass = filterActive && !matched ? 'dimmed' : '';
              const hlClass = matched ? 'matched-highlight' : '';
              cells.push(`
                <td colspan="${l.span}" class="tt-cell lesson-slot ${dimClass} ${hlClass}"
                    style="background:${escapeHtml(l.bg)}; color:${escapeHtml(l.fg)};"
                    data-jump-teacher="${l.page}">
                  <div class="cell-top-line" dir="rtl">${escapeHtml(l.subj)}</div>
                  <div class="cell-bottom-line" dir="rtl" style="font-size:13.5px; opacity:0.94;">${escapeHtml(l.teacher)}</div>
                </td>
              `);
            } else {
              cells.push(`<td class="tt-cell free-slot" title="${escapeHtml(tr.noLessonSlot)}"><span class="ltr-token">---</span></td>`);
            }
          }

          return `
            <tr>
              <th scope="row" class="day-header">
                ${buildDayHeaderCellHtml(dayAr, dIdx)}
              </th>
              ${cells.join('')}
            </tr>
          `;
        }).join('');

        classTimetableContainer.innerHTML = `
          <div class="tt-card-top">
            <div class="tt-identity">
              <span class="tt-institution-sub">${escapeHtml(tr.classSheetSub)}</span>
              <h2 class="tt-main-heading">
                <span>${escapeHtml(tr.classHeadingPrefix)}</span>
                <span class="ar-text">${escapeHtml(clsObj.name)}</span>
                <span class="page-pill">${clsObj.periods} ${escapeHtml(tr.unitPeriodsWeek)}</span>
              </h2>
            </div>
            <div class="tt-nav-controls">
              <button type="button" class="btn" id="prevClassBtn" ${idxInAll <= 0 ? 'disabled' : ''}>${escapeHtml(tr.btnPrevClass)}</button>
              <button type="button" class="btn" id="nextClassBtn" ${idxInAll >= CLASSES.length - 1 ? 'disabled' : ''}>${escapeHtml(tr.btnNextClass)}</button>
            </div>
          </div>

          <div class="tt-scroll-wrap">
            <table class="fet-grid" aria-label="${escapeHtml(clsObj.name)}">
              <thead>
                <tr>
                  <th class="corner-cell">${escapeHtml(tr.cornerDayTime)}</th>
                  ${META.periods.map((pTime, idx) => `
                    <th>
                      <span class="period-num-label">${escapeHtml(tr.periodOrdinal(idx + 1))}</span>
                      <span class="period-time-label ltr-token">${escapeHtml(pTime)}</span>
                    </th>
                  `).join('')}
                </tr>
              </thead>
              <tbody>
                ${rowsHtml}
              </tbody>
            </table>
          </div>

          <div class="tt-footer">
            <div class="tt-legend">
              <span>${escapeHtml(tr.hintClassFooter)}</span>
            </div>
            <span class="ltr-token">${escapeHtml(META.generated || '')}</span>
          </div>
        `;

        const prevCBtn = document.getElementById('prevClassBtn');
        const nextCBtn = document.getElementById('nextClassBtn');
        if (prevCBtn) {
          prevCBtn.onclick = () => {
            if (idxInAll > 0) {
              state.selectedClass = CLASSES[idxInAll - 1].name;
              if (state.cls !== '') {
                state.cls = state.selectedClass;
                classFilter.value = state.cls;
              }
              renderAll();
            }
          };
        }
        if (nextCBtn) {
          nextCBtn.onclick = () => {
            if (idxInAll < CLASSES.length - 1) {
              state.selectedClass = CLASSES[idxInAll + 1].name;
              if (state.cls !== '') {
                state.cls = state.selectedClass;
                classFilter.value = state.cls;
              }
              renderAll();
            }
          };
        }
      }

      // Render Free / Substitute Teacher Finder View
      function renderFreeView() {
        const tr = T();
        const dIdx = state.dayIdx !== '' ? Number(state.dayIdx) : state.subDayIdx;
        const pIdx = state.periodIdx !== '' ? Number(state.periodIdx) : state.subPeriodIdx;

        subDayPills.innerHTML = META.days.map((_, idx) => `
          <button type="button" class="slot-pill-btn ${idx === dIdx ? 'active' : ''}" data-pick-sub-day="${idx}" aria-pressed="${idx === dIdx ? 'true' : 'false'}">
            ${getDayPillHtml(idx)}
          </button>
        `).join('');

        subPeriodPills.innerHTML = META.periods.map((pTime, idx) => `
          <button type="button" class="slot-pill-btn ${idx === pIdx ? 'active' : ''}" data-pick-sub-period="${idx}" aria-pressed="${idx === pIdx ? 'true' : 'false'}">
            <span>${escapeHtml(tr.periodShort(idx + 1))}</span>
            <span class="ltr-token" style="opacity:0.86; font-weight:500;">(${escapeHtml(pTime)})</span>
          </button>
        `).join('');

        let targetClassLesson = null;
        if (state.cls !== '') {
          const cObj = classMap.get(state.cls);
          if (cObj) {
            targetClassLesson = cObj.lessons.find(l => l.dayIdx === dIdx && pIdx >= l.pStart && pIdx <= l.pEnd) || null;
          }
          subClassContext.classList.remove('hidden');
          if (targetClassLesson) {
            const canQuickFilterSubj = state.subj !== targetClassLesson.subj;
            if (state.lang === 'ar') {
              subClassContext.innerHTML = `
                <span>الفصل <strong class="ar-text">${escapeHtml(state.cls)}</strong> يدرس في هذه الحصة مادة <strong class="ar-text">${escapeHtml(targetClassLesson.subj)}</strong> (معلم المادة: <strong class="ar-text">${escapeHtml(targetClassLesson.teacher)}</strong>)</span>
                ${canQuickFilterSubj ? `<button type="button" class="btn" style="padding:3px 10px; font-size:13px;" data-filter-target-subj="${escapeHtml(targetClassLesson.subj)}">تصفية معلمي مادة ${escapeHtml(targetClassLesson.subj)}</button>` : ''}
              `;
            } else if (state.lang === 'jawi') {
              subClassContext.innerHTML = `
                <span>كلس <strong class="ar-text">${escapeHtml(state.cls)}</strong> فد وقتو اين بليجر مات فلاجرن <strong class="ar-text">${escapeHtml(targetClassLesson.subj)}</strong> (ڬورو تتف: <strong class="ar-text">${escapeHtml(targetClassLesson.teacher)}</strong>)</span>
                ${canQuickFilterSubj ? `<button type="button" class="btn" style="padding:3px 10px; font-size:13px;" data-filter-target-subj="${escapeHtml(targetClassLesson.subj)}">تافيس هاڽ ڬورو مات فلاجرن ${escapeHtml(targetClassLesson.subj)}</button>` : ''}
              `;
            } else {
              subClassContext.innerHTML = `
                <span>ห้อง <strong class="ar-text">${escapeHtml(state.cls)}</strong> ในคาบนี้เรียนวิชา <strong class="ar-text">${escapeHtml(targetClassLesson.subj)}</strong> (ครูประจำวิชา: <strong class="ar-text">${escapeHtml(targetClassLesson.teacher)}</strong>)</span>
                ${canQuickFilterSubj ? `<button type="button" class="btn" style="padding:3px 10px; font-size:12.5px;" data-filter-target-subj="${escapeHtml(targetClassLesson.subj)}">กรองเฉพาะครูที่สอนวิชา ${escapeHtml(targetClassLesson.subj)}</button>` : ''}
              `;
            }
          } else {
            if (state.lang === 'ar') {
              subClassContext.innerHTML = `<span>الفصل <strong class="ar-text">${escapeHtml(state.cls)}</strong> ليس لديه حصة في ${escapeHtml(getDayPlainText(dIdx))} (${escapeHtml(tr.periodOrdinal(pIdx + 1))})</span>`;
            } else if (state.lang === 'jawi') {
              subClassContext.innerHTML = `<span>كلس <strong class="ar-text">${escapeHtml(state.cls)}</strong> تياد وقتو بليجر فد هاري ${escapeHtml(getDayPlainText(dIdx))} (${escapeHtml(tr.periodOrdinal(pIdx + 1))})</span>`;
            } else {
              subClassContext.innerHTML = `<span>ห้อง <strong class="ar-text">${escapeHtml(state.cls)}</strong> ไม่มีคาบเรียนในวัน ${escapeHtml(getDayPlainText(dIdx))} คาบที่ ${pIdx + 1}</span>`;
            }
          }
        } else {
          subClassContext.classList.add('hidden');
          subClassContext.innerHTML = '';
        }

        const qTokens = state.query.trim() ? normalizeText(state.query).split(' ').filter(Boolean) : [];
        const highlightSubj = state.subj || (targetClassLesson ? targetClassLesson.subj : '');

        const candidates = [];
        TEACHERS.forEach(t => {
          const unavailSet = new Set((t.unavailGrid && t.unavailGrid[dIdx]) || []);
          if (unavailSet.has(pIdx)) return;

          const dayLessons = t.lessons.filter(l => l.dayIdx === dIdx);
          const isBusy = dayLessons.some(l => pIdx >= l.pStart && pIdx <= l.pEnd);
          if (isBusy) return;

          if (state.teacherId !== '' && t.id !== Number(state.teacherId)) return;
          if (state.subj !== '' && !t.subjects.includes(state.subj)) return;
          if (qTokens.length > 0) {
            for (const tk of qTokens) {
              if (!t.searchBlob.includes(tk)) return;
            }
          }

          const slotByPeriod = [null, null, null, null, null];
          dayLessons.forEach(l => {
            for (let p = l.pStart; p <= l.pEnd; p++) {
              if (p >= 0 && p < 5) slotByPeriod[p] = l;
            }
          });

          const dayBusyCount = dayLessons.reduce((acc, l) => acc + l.span, 0);
          candidates.push({
            teacher: t,
            dayBusy: dayBusyCount,
            slotByPeriod,
            unavailSet
          });
        });

        const dir = state.subSortDir === 'asc' ? 1 : -1;
        candidates.sort((a, b) => {
          let cmp = 0;
          switch (state.subSortKey) {
            case 'id':
              cmp = a.teacher.id - b.teacher.id;
              break;
            case 'name':
              cmp = a.teacher.name.localeCompare(b.teacher.name, 'ar') || a.teacher.id - b.teacher.id;
              break;
            case 'periods':
              cmp = a.teacher.periods - b.teacher.periods || a.dayBusy - b.dayBusy || a.teacher.id - b.teacher.id;
              break;
            case 'dayBusy':
            default:
              cmp = a.dayBusy - b.dayBusy || a.teacher.periods - b.teacher.periods || a.teacher.id - b.teacher.id;
              break;
          }
          return cmp * dir;
        });

        document.querySelectorAll('#freeTeachersTable thead th.sortable').forEach(th => {
          const key = th.getAttribute('data-sub-sort');
          const ind = th.querySelector('.sort-ind');
          if (key === state.subSortKey) {
            th.classList.add('sorted');
            if (ind) ind.textContent = state.subSortDir === 'asc' ? '↑' : '↓';
          } else {
            th.classList.remove('sorted');
            if (ind) ind.textContent = '↕';
          }
        });

        if (state.lang === 'ar') {
          liveResultSummary.innerHTML = `المعلمون المتاحون للبديل: <strong>${candidates.length}</strong> • ${escapeHtml(getDayPlainText(dIdx))} (${escapeHtml(tr.periodOrdinal(pIdx + 1))})`;
        } else if (state.lang === 'jawi') {
          liveResultSummary.innerHTML = `ڬورو كوسوڠ سديا مڠڬنتي: <strong>${candidates.length}</strong> ${escapeHtml(tr.unitPersons)} • ${escapeHtml(getDayPlainText(dIdx))} (${escapeHtml(tr.periodOrdinal(pIdx + 1))})`;
        } else {
          liveResultSummary.innerHTML = `ครูว่างพร้อมสอนแทน <strong>${candidates.length}</strong> ท่าน • ${escapeHtml(getDayPlainText(dIdx))} คาบที่ ${pIdx + 1}`;
        }

        if (candidates.length === 0) {
          freeTableBody.innerHTML = '';
          freeTeachersTable.classList.add('hidden');
          freeEmptyState.classList.remove('hidden');
          return;
        }

        freeTeachersTable.classList.remove('hidden');
        freeEmptyState.classList.add('hidden');

        freeTableBody.innerHTML = candidates.map(({ teacher: t, dayBusy, slotByPeriod, unavailSet }) => {
          const miniCellsHtml = [0, 1, 2, 3, 4].map(p => {
            if (p === pIdx) {
              return `<span class="mini-slot is-target-free">${escapeHtml(tr.miniFreeWord)}</span>`;
            }
            if (slotByPeriod[p]) {
              const l = slotByPeriod[p];
              return `<span class="mini-slot is-busy ar-text" title="${escapeHtml(l.cls)} - ${escapeHtml(l.subj)}">${escapeHtml(l.cls)}</span>`;
            }
            if (unavailSet.has(p)) {
              return `<span class="mini-slot is-unavail ltr-token">-x-</span>`;
            }
            return `<span class="mini-slot is-free ltr-token">---</span>`;
          }).join('');

          const subjTagsHtml = t.subjects.map(s => `
            <span class="subj-mini-tag ${highlightSubj && s === highlightSubj ? 'matched' : ''}">${escapeHtml(s)}</span>
          `).join('');

          return `
            <tr data-open-teacher="${t.id}">
              <td class="num-col"><span class="dir-num ltr-token">#${String(t.id).padStart(2, '0')}</span></td>
              <td><strong class="ar-text" style="font-size:15.5px;">${escapeHtml(t.name)}</strong></td>
              <td><div class="subj-tag-list">${subjTagsHtml}</div></td>
              <td><div class="day-mini-track">${miniCellsHtml}</div></td>
              <td class="num-col">${dayBusy} ${escapeHtml(tr.unitPeriods)}</td>
              <td class="num-col">${t.periods} ${escapeHtml(tr.unitPeriods)}</td>
            </tr>
          `;
        }).join('');
      }

      function buildSelfResultHtml(teacher) {
        const tr = T();
        const dayPillsHtml = `
          <div class="self-day-filter-bar">
            <span class="sub-picker-label" style="min-width:auto; margin-right:4px;">${escapeHtml(tr.lblPickViewDay)}</span>
            <div class="pill-btn-row" role="group">
              <button type="button" class="slot-pill-btn ${state.selfDayFilter === 'all' ? 'active' : ''}" data-self-day="all">${escapeHtml(tr.wholeWeek)}</button>
              ${META.days.map((_, idx) => `
                <button type="button" class="slot-pill-btn ${state.selfDayFilter === String(idx) ? 'active' : ''}" data-self-day="${idx}">
                  ${getDayPillHtml(idx)}
                </button>
              `).join('')}
            </div>
          </div>
        `;

        if (state.selfDayFilter === 'all') {
          const baseHtml = buildTeacherTimetableHtml(teacher, { isSelf: true });
          return baseHtml.replace('<div class="tt-scroll-wrap">', dayPillsHtml + '<div class="tt-scroll-wrap">');
        }

        const dIdx = Number(state.selfDayFilter);
        const dayLessons = teacher.lessons.filter(l => l.dayIdx === dIdx);
        const unavailSet = new Set((teacher.unavailGrid && teacher.unavailGrid[dIdx]) || []);
        const byStart = new Map();
        const covered = new Set();
        dayLessons.forEach(l => {
          byStart.set(l.pStart, l);
          for (let p = l.pStart + 1; p <= l.pEnd; p++) covered.add(p);
        });

        const slotsHtml = [];
        for (let p = 0; p < 5; p++) {
          if (covered.has(p)) continue;
          if (byStart.has(p)) {
            const l = byStart.get(p);
            const pLabel = l.span > 1 ? tr.periodSpanOrdinal(l.pStart + 1, l.pEnd + 1) : tr.periodOrdinal(p + 1);
            slotsHtml.push(`
              <div class="daily-slot-row">
                <div class="daily-slot-time">
                  <span class="period-num-label" style="font-size:12.5px;">${escapeHtml(pLabel)}</span>
                  <span class="period-time-label ltr-token" style="font-weight:700; color:var(--ink);">${escapeHtml(l.timeRange)}</span>
                </div>
                <div class="daily-slot-badge" style="background:${escapeHtml(l.bg)}; color:${escapeHtml(l.fg)};" data-jump-class="${escapeHtml(l.cls)}">
                  <div>
                    <div style="font-size:13px; opacity:0.9;">${escapeHtml(tr.classHeadingPrefix)} <strong class="ar-text" style="font-size:17px;">${escapeHtml(l.cls)}</strong></div>
                    <div class="ar-text" style="font-size:18px; font-weight:700;">${escapeHtml(l.subj)}</div>
                  </div>
                  ${l.span > 1 ? `<span class="cell-span-tag">${escapeHtml(tr.spanContTag(l.span))}</span>` : ''}
                </div>
              </div>
            `);
          } else if (unavailSet.has(p)) {
            slotsHtml.push(`
              <div class="daily-slot-row" style="background:var(--surface-subtle);">
                <div class="daily-slot-time">
                  <span class="period-num-label" style="font-size:12.5px;">${escapeHtml(tr.periodOrdinal(p + 1))}</span>
                  <span class="period-time-label ltr-token" style="color:var(--muted);">${escapeHtml(META.periods[p] || '')}</span>
                </div>
                <div style="color:var(--muted); font-weight:600;">${escapeHtml(tr.unavailSlotLabel)} <span class="ltr-token">(-x-)</span></div>
              </div>
            `);
          } else {
            slotsHtml.push(`
              <div class="daily-slot-row">
                <div class="daily-slot-time">
                  <span class="period-num-label" style="font-size:12.5px;">${escapeHtml(tr.periodOrdinal(p + 1))}</span>
                  <span class="period-time-label ltr-token" style="color:var(--muted);">${escapeHtml(META.periods[p] || '')}</span>
                </div>
                <div style="color:var(--muted);">${escapeHtml(tr.freeSlotLabel)} <span class="ltr-token">(---)</span></div>
              </div>
            `);
          }
        }

        return `
          <div class="tt-card-top">
            <div class="tt-identity">
              <span class="tt-institution-sub ar-text">${escapeHtml(META.title || '')}</span>
              <h2 class="tt-main-heading">
                <span class="ar-text">${escapeHtml(teacher.name)}</span>
                <span class="page-pill">${escapeHtml(tr.colPage)} ${teacher.id} • ${escapeHtml(getDayPlainText(dIdx))}</span>
              </h2>
            </div>
            <div class="tt-nav-controls">
              <button type="button" class="btn" data-self-reset-teacher="true">${escapeHtml(tr.btnChangeTeacher)}</button>
            </div>
          </div>
          ${dayPillsHtml}
          <div class="daily-cards-wrap">
            ${slotsHtml.join('')}
          </div>
          <div class="tt-footer">
            <span>${escapeHtml(tr.selfFooterDaily)}</span>
            <span class="ltr-token">${escapeHtml(META.generated || '')}</span>
          </div>
        `;
      }

      // Render Self-Service Teacher Lookup View
      function renderSelfView() {
        const tr = T();
        const qTrim = state.selfQuery.trim();
        selfClearInputBtn.classList.toggle('visible', state.selfQuery.length > 0);

        selfLetterRow.innerHTML = `
          <button type="button" class="letter-pill ${state.selfLetter === '' ? 'active' : ''}" data-self-letter="">${escapeHtml(tr.allLetters)}</button>
          ${INITIAL_LETTERS.map(ltr => `
            <button type="button" class="letter-pill ar-letter ${state.selfLetter === ltr ? 'active' : ''}" data-self-letter="${escapeHtml(ltr)}">${escapeHtml(ltr)}</button>
          `).join('')}
        `;

        let matchedTeachers = TEACHERS;
        if (state.selfLetter !== '') {
          matchedTeachers = matchedTeachers.filter(t => t.firstLetter === state.selfLetter);
        }
        if (qTrim) {
          const cleanNumStr = qTrim.replace(/^#/, '').trim();
          const exactNum = /^\d+$/.test(cleanNumStr) ? Number(cleanNumStr) : null;
          const tokens = normalizeText(qTrim).split(' ').filter(Boolean);
          matchedTeachers = matchedTeachers.filter(t => {
            if (exactNum !== null && t.id === exactNum) return true;
            return tokens.every(tk => t.searchBlob.includes(tk));
          });
          if (exactNum !== null) {
            matchedTeachers = matchedTeachers.slice().sort((a, b) => (a.id === exactNum ? -1 : b.id === exactNum ? 1 : a.id - b.id));
          }
        }

        let activeTeacher = null;
        if (state.selfPickedTeacherId !== null) {
          activeTeacher = teacherById.get(state.selfPickedTeacherId) || null;
        } else if (qTrim && matchedTeachers.length === 1) {
          activeTeacher = matchedTeachers[0];
        }

        selfTeacherSelect.value = activeTeacher ? String(activeTeacher.id) : '';
        selfClearTeacherBtn.classList.toggle('hidden', !activeTeacher && !qTrim && !state.selfLetter);

        const collapseDirectory = Boolean(activeTeacher && !state.selfShowList);
        selfLetterWrap.classList.toggle('hidden', collapseDirectory);
        selfMatchSection.classList.toggle('hidden', collapseDirectory);
        selfSelectedBanner.classList.toggle('hidden', !collapseDirectory);

        if (collapseDirectory && activeTeacher) {
          const bannerLabelHtml = state.lang === 'ar'
            ? `يتم عرض جدول المعلم: <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (${escapeHtml(tr.colPage)} ${activeTeacher.id} • ${activeTeacher.periods} ${escapeHtml(tr.unitPeriodsWeek)})`
            : state.lang === 'jawi'
            ? `سدڠ ممفافركن جدول مڠاجر: <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (${escapeHtml(tr.colPage)} ${activeTeacher.id} • ${activeTeacher.periods} ${escapeHtml(tr.unitPeriodsWeek)})`
            : `กำลังแสดงตารางสอนของ <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (หน้า ${activeTeacher.id} • ${activeTeacher.periods} คาบ/สัปดาห์)`;

          selfSelectedBanner.innerHTML = `
            <span>${bannerLabelHtml}</span>
            <button type="button" class="btn" style="padding:5px 12px; font-size:13px;" data-self-expand-list="true">${escapeHtml(tr.btnExpandList)}</button>
          `;
        } else if (matchedTeachers.length === 0) {
          selfTeacherGrid.innerHTML = '';
          selfTeacherGrid.classList.add('hidden');
          selfNoMatch.classList.remove('hidden');
        } else {
          selfTeacherGrid.classList.remove('hidden');
          selfNoMatch.classList.add('hidden');
          selfTeacherGrid.innerHTML = matchedTeachers.map(t => `
            <button type="button" class="self-teacher-btn ${activeTeacher && t.id === activeTeacher.id ? 'active' : ''}" data-self-pick="${t.id}" role="option" aria-selected="${activeTeacher && t.id === activeTeacher.id ? 'true' : 'false'}">
              <span class="self-teacher-btn-top">
                <span class="dir-item-main">
                  <span class="dir-num ltr-token">#${String(t.id).padStart(2, '0')}</span>
                  <span class="dir-name ar-text">${escapeHtml(t.name)}</span>
                </span>
                <span class="dir-meta">${t.periods} ${escapeHtml(tr.unitPeriods)}</span>
              </span>
              <span class="self-teacher-sub ar-text">${escapeHtml(t.subjects.join(' • '))}</span>
            </button>
          `).join('');
        }

        if (activeTeacher) {
          selfTimetableResult.classList.remove('hidden');
          selfTimetableResult.innerHTML = buildSelfResultHtml(activeTeacher);
          if (state.lang === 'ar') {
            liveResultSummary.innerHTML = `جدول المعلم <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (${escapeHtml(tr.colPage)} ${activeTeacher.id} • ${activeTeacher.periods} ${escapeHtml(tr.unitPeriodsWeek)})`;
          } else if (state.lang === 'jawi') {
            liveResultSummary.innerHTML = `جدول مڠاجر <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (${escapeHtml(tr.colPage)} ${activeTeacher.id} • ${activeTeacher.periods} ${escapeHtml(tr.unitPeriodsWeek)})`;
          } else {
            liveResultSummary.innerHTML = `ตารางสอนของ <strong class="ar-text">${escapeHtml(activeTeacher.name)}</strong> (หน้า ${activeTeacher.id} • ${activeTeacher.periods} คาบ/สัปดาห์)`;
          }
        } else {
          selfTimetableResult.classList.add('hidden');
          selfTimetableResult.innerHTML = '';
          if (state.lang === 'ar') {
            liveResultSummary.innerHTML = `اختر اسم المعلم لعرض الجدول • النتائج: <strong>${matchedTeachers.length}</strong> من ${TEACHERS.length}`;
          } else if (state.lang === 'jawi') {
            liveResultSummary.innerHTML = `فيليه نام ڬورو اونتوق مليهت جدول • دجومفأي <strong>${matchedTeachers.length}</strong> درفد ${TEACHERS.length} ${escapeHtml(tr.unitPersons)}`;
          } else {
            liveResultSummary.innerHTML = `เลือกชื่อครูเพื่อดูตารางสอน • พบ <strong>${matchedTeachers.length}</strong> จาก ${TEACHERS.length} ท่าน`;
          }
        }
      }

      function resetSelfLookup() {
        state.selfQuery = '';
        state.selfLetter = '';
        state.selfPickedTeacherId = null;
        state.selfShowList = true;
        state.selfDayFilter = 'all';
        selfSearchInput.value = '';
        selfTeacherSelect.value = '';
        renderAll();
        selfSearchInput.focus();
      }

      // Academic Affairs Editor Elements & Logic
      const manageView = document.getElementById('manageView');
      const manageTeacherSelect = document.getElementById('manageTeacherSelect');
      const editTeacherNameBtn = document.getElementById('editTeacherNameBtn');
      const addNewTeacherBtn = document.getElementById('addNewTeacherBtn');
      const customModifiedBadge = document.getElementById('customModifiedBadge');
      const openAddSlotBtn = document.getElementById('openAddSlotBtn');
      const resetDefaultDataBtn = document.getElementById('resetDefaultDataBtn');
      const resetConfirmBox = document.getElementById('resetConfirmBox');
      const confirmResetYesBtn = document.getElementById('confirmResetYesBtn');
      const confirmResetNoBtn = document.getElementById('confirmResetNoBtn');
      const manageGridContainer = document.getElementById('manageGridContainer');
      const classDatalist = document.getElementById('classDatalist');
      const subjectDatalist = document.getElementById('subjectDatalist');

      const slotEditorModal = document.getElementById('slotEditorModal');
      const slotEditorForm = document.getElementById('slotEditorForm');
      const slotTypeTabs = document.getElementById('slotTypeTabs');
      const slotTeacherSelect = document.getElementById('slotTeacherSelect');
      const slotDaySelect = document.getElementById('slotDaySelect');
      const slotPeriodSelect = document.getElementById('slotPeriodSelect');
      const lessonSpecificFields = document.getElementById('lessonSpecificFields');
      const slotClassInput = document.getElementById('slotClassInput');
      const slotSpanSelect = document.getElementById('slotSpanSelect');
      const slotSubjectInput = document.getElementById('slotSubjectInput');
      const slotColorInput = document.getElementById('slotColorInput');
      const presetColorSwatches = document.getElementById('presetColorSwatches');
      const slotFormAlert = document.getElementById('slotFormAlert');
      const deleteLessonBtn = document.getElementById('deleteLessonBtn');
      const closeSlotModalTopBtn = document.getElementById('closeSlotModalTopBtn');
      const cancelSlotModalBtn = document.getElementById('cancelSlotModalBtn');

      const teacherProfileModal = document.getElementById('teacherProfileModal');
      const teacherProfileForm = document.getElementById('teacherProfileForm');
      const teacherProfileModalTitle = document.getElementById('teacherProfileModalTitle');
      const teacherProfileNameInput = document.getElementById('teacherProfileNameInput');
      const teacherProfileAlert = document.getElementById('teacherProfileAlert');
      const closeTeacherProfileTopBtn = document.getElementById('closeTeacherProfileTopBtn');
      const cancelTeacherProfileBtn = document.getElementById('cancelTeacherProfileBtn');

      const PRESET_COLORS = ['#E6BD72', '#79C265', '#60F189', '#FF8E9E', '#F65244', '#1E662D', '#5BBFF2', '#BB97CD', '#3BC898', '#FDA548', '#2F74FE', '#9A83E4'];
      state.manageTeacherId = TEACHERS[0] ? TEACHERS[0].id : 1;
      let currentSlotType = 'lesson';
      let editingExistingRawIdx = null;
      let teacherProfileMode = 'add';

      function computeIsWhiteFg(hex) {
        const clean = String(hex || '#E6BD72').replace('#', '');
        if (clean.length !== 6) return 0;
        const r = parseInt(clean.slice(0, 2), 16);
        const g = parseInt(clean.slice(2, 4), 16);
        const b = parseInt(clean.slice(4, 6), 16);
        const lum = 0.299 * r + 0.587 * g + 0.114 * b;
        return lum < 145 ? 1 : 0;
      }

      function persistCustomTimetable() {
        hasCustomEdits = true;
        try {
          const cleanTeachers = TEACHERS.map(t => ({
            id: t.id,
            name: t.name,
            periods: t.periods,
            free: t.free,
            unavail: t.unavail,
            unavailGrid: t.unavailGrid
          }));
          localStorage.setItem('thaqafah_tt_custom_v1', JSON.stringify({
            teachers: cleanTeachers,
            lessons: RAW_LESSONS
          }));
        } catch (e) {}
      }

      function updateDynamicCountsAndDropdowns() {
        I18N.th.allTeachers = `ทั้งหมด (${TEACHERS.length} ท่าน)`;
        I18N.th.lblSelfSelect = `หรือเลือกจากรายชื่อครูทั้งหมด (${TEACHERS.length} ท่าน)`;
        I18N.th.allClasses = `ทั้งหมด (${CLASSES.length} ห้อง)`;
        I18N.th.allSubjects = `ทั้งหมด (${SUBJECTS.length} วิชา)`;
        I18N.th.headerMetaHtml = `<span>ข้อมูลจากไฟล์: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• ครูผู้สอน ${TEACHERS.length} ท่าน • ${CLASSES.length} ห้องเรียน • ${SUBJECTS.length} รายวิชา</span>`;

        I18N.ar.allTeachers = `الكل (${TEACHERS.length} معلماً)`;
        I18N.ar.lblSelfSelect = `أو اختر من قائمة جميع المعلمين (${TEACHERS.length} معلماً)`;
        I18N.ar.allClasses = `الكل (${CLASSES.length} فصلاً)`;
        I18N.ar.allSubjects = `الكل (${SUBJECTS.length} مادة)`;
        I18N.ar.headerMetaHtml = `<span>المصدر: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• ${TEACHERS.length} معلماً • ${CLASSES.length} فصلاً • ${SUBJECTS.length} مادة دراسية</span>`;

        I18N.jawi.allTeachers = `سموا (${TEACHERS.length} ڬورو)`;
        I18N.jawi.lblSelfSelect = `اتاو فيليه درفد سناراي سموا ڬورو (${TEACHERS.length} اورڠ)`;
        I18N.jawi.allClasses = `سموا (${CLASSES.length} كلس)`;
        I18N.jawi.allSubjects = `سموا (${SUBJECTS.length} مات فلاجرن)`;
        I18N.jawi.headerMetaHtml = `<span>سومبر فايل: <strong class="ar-text">جدول-كورو-ملون.pdf</strong></span><span>• ${TEACHERS.length} ڬورو فڠاجر • ${CLASSES.length} كلس • ${SUBJECTS.length} مات فلاجرن</span>`;

        const tr = T();
        if (headerMetaBox) headerMetaBox.innerHTML = tr.headerMetaHtml;

        const prevT = state.teacherId;
        const prevC = state.cls;
        const prevS = state.subj;
        const prevD = state.dayIdx;
        const prevP = state.periodIdx;

        teacherFilter.innerHTML = `<option value="">${escapeHtml(tr.allTeachers)}</option>` +
          TEACHERS.map(t => `<option value="${t.id}">${escapeHtml(`${String(t.id).padStart(2, '0')}. ${t.name}`)}</option>`).join('');
        teacherFilter.value = prevT;

        selfTeacherSelect.innerHTML = `<option value="">${escapeHtml(tr.optSelfPrompt)}</option>` +
          TEACHERS.map(t => `<option value="${t.id}">${escapeHtml(`${String(t.id).padStart(2, '0')}. ${t.name}`)}</option>`).join('');

        const teacherOptionsOnly = TEACHERS.map(t => `<option value="${t.id}">${escapeHtml(`${String(t.id).padStart(2, '0')}. ${t.name}`)}</option>`).join('');
        manageTeacherSelect.innerHTML = teacherOptionsOnly;
        manageTeacherSelect.value = String(state.manageTeacherId);
        slotTeacherSelect.innerHTML = teacherOptionsOnly;

        classFilter.innerHTML = `<option value="">${escapeHtml(tr.allClasses)}</option>` +
          CLASSES.map(c => `<option value="${escapeHtml(c.name)}">${escapeHtml(c.name)}</option>`).join('');
        classFilter.value = prevC;
        classDatalist.innerHTML = CLASSES.map(c => `<option value="${escapeHtml(c.name)}"></option>`).join('');

        subjectFilter.innerHTML = `<option value="">${escapeHtml(tr.allSubjects)}</option>` +
          SUBJECTS.map(s => `<option value="${escapeHtml(s)}">${escapeHtml(s)}</option>`).join('');
        subjectFilter.value = prevS;
        subjectDatalist.innerHTML = SUBJECTS.map(s => `<option value="${escapeHtml(s)}"></option>`).join('');

        dayFilter.innerHTML = `<option value="">${escapeHtml(tr.allDays)}</option>` +
          META.days.map((_, i) => `<option value="${i}">${escapeHtml(getDayPlainText(i))}</option>`).join('');
        dayFilter.value = prevD;
        slotDaySelect.innerHTML = META.days.map((_, i) => `<option value="${i}">${escapeHtml(getDayPlainText(i))}</option>`).join('');

        periodFilter.innerHTML = `<option value="">${escapeHtml(tr.allPeriods)}</option>` +
          META.periods.map((p, i) => `<option value="${i}">${escapeHtml(`${tr.periodShort(i + 1)}: ${p}`)}</option>`).join('');
        periodFilter.value = prevP;
        slotPeriodSelect.innerHTML = META.periods.map((p, i) => `<option value="${i}">${escapeHtml(`${tr.periodShort(i + 1)} (${p})`)}</option>`).join('');
      }

      function syncEditorTranslations() {
        const tr = T();
        const setTxt = (id, val) => {
          const el = document.getElementById(id);
          if (el) el.textContent = val;
        };
        setTxt('lblManageTeacher', tr.lblManageTeacher);
        setTxt('editTeacherNameBtn', tr.btnEditTeacherName);
        setTxt('addNewTeacherBtn', tr.btnAddTeacher);
        setTxt('customModifiedBadge', tr.badgeModified);
        setTxt('openAddSlotBtn', tr.btnOpenAddSlot);
        setTxt('resetDefaultDataBtn', tr.btnResetDefault);
        setTxt('resetConfirmLabel', tr.lblConfirmReset);
        setTxt('confirmResetYesBtn', tr.btnConfirmYes);
        setTxt('confirmResetNoBtn', tr.btnCancel);
        setTxt('manageHintText', tr.manageHint);
        setTxt('slotModalTitle', tr.slotModalTitle);
        setTxt('tabTypeLesson', tr.tabTypeLesson);
        setTxt('tabTypeFree', tr.tabTypeFree);
        setTxt('tabTypeUnavail', tr.tabTypeUnavail);
        setTxt('lblSlotTeacher', tr.lblTeacher);
        setTxt('lblSlotDay', tr.lblDay);
        setTxt('lblSlotPeriod', tr.lblSlotStartPeriod);
        setTxt('lblSlotClass', tr.lblClass);
        setTxt('lblSlotSpan', tr.lblSlotSpan);
        setTxt('optSpan1', tr.optSpan1);
        setTxt('optSpan2', tr.optSpan2);
        setTxt('lblSlotSubject', tr.lblSubject);
        setTxt('lblSlotColor', tr.lblSlotColor);
        setTxt('deleteLessonBtn', tr.btnDeleteLesson);
        setTxt('cancelSlotModalBtn', tr.btnCancel);
        setTxt('saveSlotBtn', tr.btnSaveChanges);
        setTxt('lblTeacherProfileName', tr.lblTeacherProfileName);
        setTxt('cancelTeacherProfileBtn', tr.btnCancel);
        setTxt('saveTeacherProfileBtn', tr.btnSaveChanges);
      }

      function renderManageView() {
        const tr = T();
        syncEditorTranslations();
        if (!teacherById.has(state.manageTeacherId) && TEACHERS.length > 0) {
          state.manageTeacherId = TEACHERS[0].id;
        }
        manageTeacherSelect.value = String(state.manageTeacherId);
        customModifiedBadge.classList.toggle('hidden', !hasCustomEdits);
        resetDefaultDataBtn.classList.toggle('hidden', !hasCustomEdits || !resetConfirmBox.classList.contains('hidden'));

        const teacher = teacherById.get(state.manageTeacherId);
        if (!teacher) return;

        liveResultSummary.innerHTML = escapeHtml(tr.manageStatusText(teacher.name, teacher.periods));

        const rowsHtml = META.days.map((dayAr, dIdx) => {
          const dayLessons = teacher.lessons.filter(l => l.dayIdx === dIdx);
          const unavailSet = new Set((teacher.unavailGrid && teacher.unavailGrid[dIdx]) || []);
          const byStart = new Map();
          const covered = new Set();
          dayLessons.forEach(l => {
            byStart.set(l.pStart, l);
            for (let p = l.pStart + 1; p <= l.pEnd; p++) covered.add(p);
          });

          const cells = [];
          for (let p = 0; p < 5; p++) {
            if (covered.has(p)) continue;
            if (byStart.has(p)) {
              const l = byStart.get(p);
              cells.push(`
                <td colspan="${l.span}" class="tt-cell lesson-slot editable-cell"
                    style="background:${escapeHtml(l.bg)}; color:${escapeHtml(l.fg)};"
                    data-edit-slot="${dIdx}:${l.pStart}">
                  <div class="cell-top-line" dir="rtl">${escapeHtml(l.cls)}</div>
                  <div class="cell-bottom-line" dir="rtl">${escapeHtml(l.subj)}</div>
                  ${l.span > 1 ? `<span class="cell-span-tag">${escapeHtml(tr.spanContTag(l.span))}</span>` : ''}
                </td>
              `);
            } else if (unavailSet.has(p)) {
              cells.push(`<td class="tt-cell unavail-slot editable-cell" data-edit-slot="${dIdx}:${p}"><span class="ltr-token">-x-</span></td>`);
            } else {
              cells.push(`<td class="tt-cell free-slot editable-cell" data-edit-slot="${dIdx}:${p}"><span class="ltr-token">+ ---</span></td>`);
            }
          }

          return `
            <tr>
              <th scope="row" class="day-header">${buildDayHeaderCellHtml(dayAr, dIdx)}</th>
              ${cells.join('')}
            </tr>
          `;
        }).join('');

        manageGridContainer.innerHTML = `
          <div class="tt-card-top">
            <div class="tt-identity">
              <span class="tt-institution-sub ar-text">${escapeHtml(META.title || '')}</span>
              <h2 class="tt-main-heading">
                <span class="ar-text">${escapeHtml(teacher.name)}</span>
                <span class="page-pill">${escapeHtml(tr.colPage)} ${teacher.id} • ${teacher.periods} ${escapeHtml(tr.unitPeriodsWeek)}</span>
              </h2>
            </div>
          </div>
          <div class="tt-scroll-wrap">
            <table class="fet-grid" aria-label="${escapeHtml(teacher.name)}">
              <thead>
                <tr>
                  <th class="corner-cell">${escapeHtml(tr.cornerDayTime)}</th>
                  ${META.periods.map((pTime, idx) => `
                    <th>
                      <span class="period-num-label">${escapeHtml(tr.periodOrdinal(idx + 1))}</span>
                      <span class="period-time-label ltr-token">${escapeHtml(pTime)}</span>
                    </th>
                  `).join('')}
                </tr>
              </thead>
              <tbody>${rowsHtml}</tbody>
            </table>
          </div>
          <div class="tt-footer">
            <div class="tt-legend">
              <span class="legend-item">
                <span class="legend-box ltr-token" style="background:#ffffff; color:#98a29c;">---</span>
                <span>${escapeHtml(tr.freeSlotLabel)} (${teacher.free} ${escapeHtml(tr.unitPeriods)})</span>
              </span>
              <span class="legend-item">
                <span class="legend-box ltr-token" style="background:#f3f4f3; color:#7d8781;">-x-</span>
                <span>${escapeHtml(tr.unavailSlotLabel)} (${teacher.unavail} ${escapeHtml(tr.unitPeriods)})</span>
              </span>
            </div>
            <span class="ltr-token">${escapeHtml(META.generated || '')}</span>
          </div>
        `;
      }

      function renderColorSwatches() {
        const cur = (slotColorInput.value || '#E6BD72').toUpperCase();
        presetColorSwatches.innerHTML = PRESET_COLORS.map(c => `
          <button type="button" class="preset-color-dot ${c.toUpperCase() === cur ? 'active' : ''}"
                  data-pick-color="${c}" style="background:${c};" aria-label="${c}"></button>
        `).join('');
      }

      function setSlotTypeTab(type) {
        currentSlotType = type;
        slotTypeTabs.querySelectorAll('[data-slot-type]').forEach(btn => {
          btn.classList.toggle('active', btn.getAttribute('data-slot-type') === type);
        });
        lessonSpecificFields.classList.toggle('hidden', type !== 'lesson');
        slotFormAlert.classList.add('hidden');
      }

      function syncSlotModalFromSelection(tId, dIdx, pIdx) {
        const teacher = teacherById.get(Number(tId));
        slotFormAlert.classList.add('hidden');
        editingExistingRawIdx = null;
        if (!teacher) return;

        const existingLesson = teacher.lessons.find(l => l.dayIdx === Number(dIdx) && Number(pIdx) >= l.pStart && Number(pIdx) <= l.pEnd);
        const unavailSet = new Set((teacher.unavailGrid && teacher.unavailGrid[Number(dIdx)]) || []);

        slotTeacherSelect.value = String(teacher.id);
        slotDaySelect.value = String(dIdx);

        if (existingLesson) {
          editingExistingRawIdx = existingLesson.rawIdx;
          slotPeriodSelect.value = String(existingLesson.pStart);
          slotSpanSelect.value = String(existingLesson.span);
          slotClassInput.value = existingLesson.cls;
          slotSubjectInput.value = existingLesson.subj;
          slotColorInput.value = existingLesson.bg;
          deleteLessonBtn.classList.remove('hidden');
          setSlotTypeTab('lesson');
        } else {
          slotPeriodSelect.value = String(pIdx);
          slotSpanSelect.value = '1';
          slotClassInput.value = '';
          slotSubjectInput.value = teacher.subjects[0] || '';
          slotColorInput.value = PRESET_COLORS[(teacher.id + Number(dIdx) + Number(pIdx)) % PRESET_COLORS.length];
          deleteLessonBtn.classList.add('hidden');
          setSlotTypeTab(unavailSet.has(Number(pIdx)) ? 'unavail' : 'lesson');
        }
        slotSpanSelect.options[1].disabled = Number(slotPeriodSelect.value) >= 4;
        if (Number(slotPeriodSelect.value) >= 4) slotSpanSelect.value = '1';
        renderColorSwatches();
      }

      function openSlotEditor(tId, dIdx, pIdx) {
        updateDynamicCountsAndDropdowns();
        syncEditorTranslations();
        syncSlotModalFromSelection(tId, dIdx, pIdx);
        slotEditorModal.classList.add('open');
      }

      function closeSlotEditor() {
        slotEditorModal.classList.remove('open');
      }

      function clearSlotsForTeacherRange(teacherId, dayIdx, pStart, pEnd) {
        RAW_LESSONS = RAW_LESSONS.filter(row => {
          if (row[0] !== teacherId || row[1] !== dayIdx) return true;
          const rStart = row[2];
          const rEnd = row[2] + row[3] - 1;
          return rEnd < pStart || rStart > pEnd;
        });
        const t = teacherById.get(teacherId);
        if (t && Array.isArray(t.unavailGrid[dayIdx])) {
          t.unavailGrid[dayIdx] = t.unavailGrid[dayIdx].filter(p => p < pStart || p > pEnd);
        }
      }

      function openTeacherModal(teacherId) {
        const teacher = teacherById.get(Number(teacherId));
        if (!teacher) return;
        state.modalTeacherId = teacher.id;
        modalContentArea.innerHTML = buildTeacherTimetableHtml(teacher, { isModal: true });
        teacherModal.classList.add('open');
      }

      function closeTeacherModal() {
        state.modalTeacherId = null;
        teacherModal.classList.remove('open');
      }

      function setView(viewName) {
        state.view = viewName;
        document.querySelectorAll('.view-tab').forEach(btn => {
          const isMatch = btn.getAttribute('data-view') === viewName;
          btn.classList.toggle('active', isMatch);
          btn.setAttribute('aria-selected', isMatch ? 'true' : 'false');
        });
        adminFilterGrid.classList.toggle('hidden', viewName === 'self' || viewName === 'manage');
        selfView.classList.toggle('hidden', viewName !== 'self');
        explorerView.classList.toggle('hidden', viewName !== 'explorer');
        teacherView.classList.toggle('hidden', viewName !== 'teacher');
        classView.classList.toggle('hidden', viewName !== 'class');
        freeView.classList.toggle('hidden', viewName !== 'free');
        manageView.classList.toggle('hidden', viewName !== 'manage');
        renderAll();
      }

      function resetAllFilters() {
        state.query = '';
        state.teacherId = '';
        state.cls = '';
        state.subj = '';
        state.dayIdx = '';
        state.periodIdx = '';
        state.page = 1;
        searchInput.value = '';
        teacherFilter.value = '';
        classFilter.value = '';
        subjectFilter.value = '';
        dayFilter.value = '';
        periodFilter.value = '';
        renderAll();
      }

      function renderAll() {
        if (state.view === 'manage') {
          activeFiltersBar.classList.remove('visible');
          renderManageView();
          return;
        }
        renderFilterChips();
        if (state.view === 'self') {
          renderSelfView();
          return;
        }
        const filtered = getFilteredLessons();
        if (state.view === 'explorer') {
          renderExplorer(filtered);
        } else if (state.view === 'teacher') {
          renderTeacherView(filtered);
        } else if (state.view === 'class') {
          renderClassView(filtered);
        } else if (state.view === 'free') {
          renderFreeView();
        }
      }

      // Language & Theme Switcher Listeners
      if (langSwitcher) {
        langSwitcher.addEventListener('click', (e) => {
          const btn = e.target.closest('[data-set-lang]');
          if (!btn) return;
          setLanguage(btn.getAttribute('data-set-lang'));
          updateDynamicCountsAndDropdowns();
          syncEditorTranslations();
          renderAll();
        });
      }

      if (themeSwitcher) {
        themeSwitcher.addEventListener('click', (e) => {
          const btn = e.target.closest('[data-set-theme]');
          if (!btn) return;
          applyTheme(btn.getAttribute('data-set-theme'));
        });
      }

      // Event Listeners
      document.querySelectorAll('.view-tab').forEach(btn => {
        btn.addEventListener('click', () => setView(btn.getAttribute('data-view')));
      });

      searchInput.addEventListener('input', (e) => {
        state.query = e.target.value;
        state.page = 1;
        renderAll();
      });

      clearSearchBtn.addEventListener('click', () => {
        state.query = '';
        searchInput.value = '';
        state.page = 1;
        searchInput.focus();
        renderAll();
      });

      teacherFilter.addEventListener('change', (e) => {
        state.teacherId = e.target.value;
        if (state.teacherId !== '') {
          state.selectedTeacherId = Number(state.teacherId);
        }
        state.page = 1;
        renderAll();
      });

      classFilter.addEventListener('change', (e) => {
        state.cls = e.target.value;
        if (state.cls !== '') {
          state.selectedClass = state.cls;
        }
        state.page = 1;
        renderAll();
      });

      subjectFilter.addEventListener('change', (e) => {
        state.subj = e.target.value;
        state.page = 1;
        renderAll();
      });

      dayFilter.addEventListener('change', (e) => {
        state.dayIdx = e.target.value;
        if (state.dayIdx !== '') {
          state.subDayIdx = Number(state.dayIdx);
        }
        state.page = 1;
        renderAll();
      });

      periodFilter.addEventListener('change', (e) => {
        state.periodIdx = e.target.value;
        if (state.periodIdx !== '') {
          state.subPeriodIdx = Number(state.periodIdx);
        }
        state.page = 1;
        renderAll();
      });

      filterChipsContainer.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-clear-key]');
        if (!btn) return;
        const key = btn.getAttribute('data-clear-key');
        state[key] = '';
        if (key === 'query') searchInput.value = '';
        if (key === 'teacherId') teacherFilter.value = '';
        if (key === 'cls') classFilter.value = '';
        if (key === 'subj') subjectFilter.value = '';
        if (key === 'dayIdx') dayFilter.value = '';
        if (key === 'periodIdx') periodFilter.value = '';
        state.page = 1;
        renderAll();
      });

      resetAllBtn.addEventListener('click', resetAllFilters);
      emptyResetBtn.addEventListener('click', resetAllFilters);
      freeEmptyResetBtn.addEventListener('click', resetAllFilters);

      // Substitute View Day/Period Pills, Sorting & Row Click
      subDayPills.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-pick-sub-day]');
        if (!btn) return;
        const idx = Number(btn.getAttribute('data-pick-sub-day'));
        state.subDayIdx = idx;
        if (state.dayIdx !== '') {
          state.dayIdx = String(idx);
          dayFilter.value = state.dayIdx;
        }
        renderAll();
      });

      subPeriodPills.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-pick-sub-period]');
        if (!btn) return;
        const idx = Number(btn.getAttribute('data-pick-sub-period'));
        state.subPeriodIdx = idx;
        if (state.periodIdx !== '') {
          state.periodIdx = String(idx);
          periodFilter.value = state.periodIdx;
        }
        renderAll();
      });

      subClassContext.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-filter-target-subj]');
        if (!btn) return;
        state.subj = btn.getAttribute('data-filter-target-subj');
        subjectFilter.value = state.subj;
        renderAll();
      });

      document.querySelectorAll('#freeTeachersTable thead th.sortable').forEach(th => {
        th.addEventListener('click', () => {
          const key = th.getAttribute('data-sub-sort');
          if (state.subSortKey === key) {
            state.subSortDir = state.subSortDir === 'asc' ? 'desc' : 'asc';
          } else {
            state.subSortKey = key;
            state.subSortDir = 'asc';
          }
          renderAll();
        });
      });

      freeTableBody.addEventListener('click', (e) => {
        const tr = e.target.closest('[data-open-teacher]');
        if (!tr) return;
        openTeacherModal(tr.getAttribute('data-open-teacher'));
      });

      // Sorting
      document.querySelectorAll('#lessonsTable thead th.sortable').forEach(th => {
        th.addEventListener('click', () => {
          const key = th.getAttribute('data-sort');
          if (state.sortKey === key) {
            state.sortDir = state.sortDir === 'asc' ? 'desc' : 'asc';
          } else {
            state.sortKey = key;
            state.sortDir = 'asc';
          }
          renderAll();
        });
      });

      // Pagination
      pageSizeSelect.addEventListener('change', (e) => {
        state.pageSize = Number(e.target.value) || 25;
        state.page = 1;
        renderAll();
      });

      prevPageBtn.addEventListener('click', () => {
        if (state.page > 1) {
          state.page -= 1;
          renderAll();
        }
      });

      nextPageBtn.addEventListener('click', () => {
        state.page += 1;
        renderAll();
      });

      // Table Row Click -> Open Teacher Modal
      explorerTableBody.addEventListener('click', (e) => {
        const tr = e.target.closest('[data-open-teacher]');
        if (!tr) return;
        openTeacherModal(tr.getAttribute('data-open-teacher'));
      });

      // Sidebar Directory Quick Searches & Selection
      teacherQuickSearch.addEventListener('input', (e) => {
        state.teacherQuickFilter = e.target.value;
        renderAll();
      });

      teacherDirList.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-select-teacher]');
        if (!btn) return;
        state.selectedTeacherId = Number(btn.getAttribute('data-select-teacher'));
        renderAll();
      });

      classQuickSearch.addEventListener('input', (e) => {
        state.classQuickFilter = e.target.value;
        renderAll();
      });

      classDirList.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-select-class]');
        if (!btn) return;
        state.selectedClass = btn.getAttribute('data-select-class');
        renderAll();
      });

      // Academic Affairs Manage View & Modals Listeners
      manageTeacherSelect.addEventListener('change', (e) => {
        state.manageTeacherId = Number(e.target.value);
        renderAll();
      });

      openAddSlotBtn.addEventListener('click', () => {
        openSlotEditor(state.manageTeacherId, 0, 0);
      });

      manageGridContainer.addEventListener('click', (e) => {
        const cell = e.target.closest('[data-edit-slot]');
        if (!cell) return;
        const [dStr, pStr] = cell.getAttribute('data-edit-slot').split(':');
        openSlotEditor(state.manageTeacherId, Number(dStr), Number(pStr));
      });

      slotTypeTabs.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-slot-type]');
        if (!btn) return;
        setSlotTypeTab(btn.getAttribute('data-slot-type'));
      });

      slotTeacherSelect.addEventListener('change', () => {
        syncSlotModalFromSelection(slotTeacherSelect.value, slotDaySelect.value, slotPeriodSelect.value);
      });

      slotDaySelect.addEventListener('change', () => {
        syncSlotModalFromSelection(slotTeacherSelect.value, slotDaySelect.value, slotPeriodSelect.value);
      });

      slotPeriodSelect.addEventListener('change', () => {
        const pVal = Number(slotPeriodSelect.value);
        slotSpanSelect.options[1].disabled = pVal >= 4;
        if (pVal >= 4) slotSpanSelect.value = '1';
        syncSlotModalFromSelection(slotTeacherSelect.value, slotDaySelect.value, pVal);
      });

      presetColorSwatches.addEventListener('click', (e) => {
        const dot = e.target.closest('[data-pick-color]');
        if (!dot) return;
        slotColorInput.value = dot.getAttribute('data-pick-color');
        renderColorSwatches();
      });

      slotColorInput.addEventListener('input', renderColorSwatches);
      closeSlotModalTopBtn.addEventListener('click', closeSlotEditor);
      cancelSlotModalBtn.addEventListener('click', closeSlotEditor);

      deleteLessonBtn.addEventListener('click', () => {
        const tId = Number(slotTeacherSelect.value);
        const dIdx = Number(slotDaySelect.value);
        const pStart = Number(slotPeriodSelect.value);
        const tObj = teacherById.get(tId);
        const existing = tObj ? tObj.lessons.find(l => l.dayIdx === dIdx && pStart >= l.pStart && pStart <= l.pEnd) : null;
        if (existing) {
          clearSlotsForTeacherRange(tId, dIdx, existing.pStart, existing.pEnd);
        } else {
          clearSlotsForTeacherRange(tId, dIdx, pStart, pStart);
        }
        state.manageTeacherId = tId;
        rebuildDataIndexes();
        persistCustomTimetable();
        updateDynamicCountsAndDropdowns();
        closeSlotEditor();
        renderAll();
      });

      slotEditorForm.addEventListener('submit', (e) => {
        e.preventDefault();
        const tr = T();
        const tId = Number(slotTeacherSelect.value);
        const dIdx = Number(slotDaySelect.value);
        const pStart = Number(slotPeriodSelect.value);

        if (currentSlotType === 'lesson') {
          const span = Number(slotSpanSelect.value) || 1;
          const pEnd = pStart + span - 1;
          const cls = slotClassInput.value.trim();
          const subj = slotSubjectInput.value.trim();
          const bg = (slotColorInput.value || '#E6BD72').toUpperCase();

          if (!cls || !subj) {
            slotFormAlert.textContent = tr.errReqClassSubj;
            slotFormAlert.classList.remove('hidden');
            return;
          }
          if (pEnd > 4) {
            slotFormAlert.textContent = tr.errSpanOverflow;
            slotFormAlert.classList.remove('hidden');
            return;
          }

          // Check class collision with other teachers
          const conflict = LESSONS.find(l => l.page !== tId && l.cls === cls && l.dayIdx === dIdx && !(l.pEnd < pStart || l.pStart > pEnd));
          if (conflict) {
            slotFormAlert.textContent = tr.errClassConflict(cls, conflict.subj, conflict.teacher);
            slotFormAlert.classList.remove('hidden');
            return;
          }

          clearSlotsForTeacherRange(tId, dIdx, pStart, pEnd);
          RAW_LESSONS.push([tId, dIdx, pStart, span, cls, subj, bg, computeIsWhiteFg(bg)]);
          RAW_LESSONS.sort((a, b) => a[0] - b[0] || a[1] - b[1] || a[2] - b[2]);
        } else if (currentSlotType === 'free') {
          clearSlotsForTeacherRange(tId, dIdx, pStart, pStart);
        } else if (currentSlotType === 'unavail') {
          clearSlotsForTeacherRange(tId, dIdx, pStart, pStart);
          const tObj = teacherById.get(tId);
          if (tObj) {
            if (!tObj.unavailGrid[dIdx].includes(pStart)) {
              tObj.unavailGrid[dIdx].push(pStart);
              tObj.unavailGrid[dIdx].sort((a, b) => a - b);
            }
          }
        }

        state.manageTeacherId = tId;
        rebuildDataIndexes();
        persistCustomTimetable();
        updateDynamicCountsAndDropdowns();
        closeSlotEditor();
        renderAll();
      });

      function openTeacherProfile(mode) {
        const tr = T();
        teacherProfileMode = mode;
        syncEditorTranslations();
        teacherProfileAlert.classList.add('hidden');
        if (mode === 'edit') {
          const tObj = teacherById.get(state.manageTeacherId);
          teacherProfileModalTitle.textContent = tr.teacherEditTitle;
          teacherProfileNameInput.value = tObj ? tObj.name : '';
        } else {
          teacherProfileModalTitle.textContent = tr.teacherAddTitle;
          teacherProfileNameInput.value = '';
        }
        teacherProfileModal.classList.add('open');
        teacherProfileNameInput.focus();
      }

      function closeTeacherProfile() {
        teacherProfileModal.classList.remove('open');
      }

      editTeacherNameBtn.addEventListener('click', () => openTeacherProfile('edit'));
      addNewTeacherBtn.addEventListener('click', () => openTeacherProfile('add'));
      closeTeacherProfileTopBtn.addEventListener('click', closeTeacherProfile);
      cancelTeacherProfileBtn.addEventListener('click', closeTeacherProfile);

      teacherProfileForm.addEventListener('submit', (e) => {
        e.preventDefault();
        const tr = T();
        const nameVal = teacherProfileNameInput.value.trim();
        if (!nameVal) {
          teacherProfileAlert.textContent = tr.errReqTeacherName;
          teacherProfileAlert.classList.remove('hidden');
          return;
        }
        if (teacherProfileMode === 'edit') {
          const tObj = teacherById.get(state.manageTeacherId);
          if (tObj) tObj.name = nameVal;
        } else {
          const nextId = TEACHERS.reduce((mx, t) => Math.max(mx, t.id), 0) + 1;
          TEACHERS.push({
            id: nextId,
            name: nameVal,
            periods: 0,
            free: 30,
            unavail: 0,
            unavailGrid: [[], [], [], [], [], []]
          });
          state.manageTeacherId = nextId;
          state.selectedTeacherId = nextId;
        }
        rebuildDataIndexes();
        persistCustomTimetable();
        updateDynamicCountsAndDropdowns();
        closeTeacherProfile();
        renderAll();
      });

      resetDefaultDataBtn.addEventListener('click', () => {
        resetDefaultDataBtn.classList.add('hidden');
        resetConfirmBox.classList.remove('hidden');
      });

      confirmResetNoBtn.addEventListener('click', () => {
        resetConfirmBox.classList.add('hidden');
        resetDefaultDataBtn.classList.toggle('hidden', !hasCustomEdits);
      });

      confirmResetYesBtn.addEventListener('click', () => {
        TEACHERS = JSON.parse(DEFAULT_TEACHERS_JSON);
        RAW_LESSONS = JSON.parse(DEFAULT_LESSONS_JSON);
        hasCustomEdits = false;
        try {
          localStorage.removeItem('thaqafah_tt_custom_v1');
        } catch (e) {}
        resetConfirmBox.classList.add('hidden');
        rebuildDataIndexes();
        if (!teacherById.has(state.manageTeacherId)) {
          state.manageTeacherId = TEACHERS[0] ? TEACHERS[0].id : 1;
        }
        updateDynamicCountsAndDropdowns();
        renderAll();
      });

      // Delegated clicks inside Timetable Grids & Modal
      document.addEventListener('click', (e) => {
        const jumpClsEl = e.target.closest('[data-jump-class]');
        if (jumpClsEl) {
          const targetCls = jumpClsEl.getAttribute('data-jump-class');
          closeTeacherModal();
          state.selectedClass = targetCls;
          setView('class');
          return;
        }

        const jumpTeacherEl = e.target.closest('[data-jump-teacher]');
        if (jumpTeacherEl) {
          const targetId = Number(jumpTeacherEl.getAttribute('data-jump-teacher'));
          state.selectedTeacherId = targetId;
          setView('teacher');
          return;
        }

        const fullTeacherBtn = e.target.closest('[data-switch-full-teacher]');
        if (fullTeacherBtn) {
          const targetId = Number(fullTeacherBtn.getAttribute('data-switch-full-teacher'));
          closeTeacherModal();
          state.selectedTeacherId = targetId;
          setView('teacher');
          return;
        }

        if (e.target.closest('[data-self-reset-teacher]')) {
          resetSelfLookup();
          return;
        }

        if (e.target.closest('[data-self-expand-list]')) {
          state.selfShowList = true;
          renderAll();
          return;
        }

        const dayBtn = e.target.closest('[data-self-day]');
        if (dayBtn) {
          state.selfDayFilter = dayBtn.getAttribute('data-self-day');
          renderAll();
          return;
        }

        if (e.target.closest('[data-close-modal]') || e.target === teacherModal) {
          closeTeacherModal();
        }
        if (e.target === slotEditorModal) {
          closeSlotEditor();
        }
        if (e.target === teacherProfileModal) {
          closeTeacherProfile();
        }
      });

      // Self-Service Teacher Lookup Listeners
      selfSearchInput.addEventListener('input', (e) => {
        state.selfQuery = e.target.value;
        state.selfPickedTeacherId = null;
        state.selfShowList = true;
        renderAll();
      });

      selfClearInputBtn.addEventListener('click', () => {
        state.selfQuery = '';
        state.selfPickedTeacherId = null;
        state.selfShowList = true;
        selfSearchInput.value = '';
        renderAll();
        selfSearchInput.focus();
      });

      selfLetterRow.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-self-letter]');
        if (!btn) return;
        state.selfLetter = btn.getAttribute('data-self-letter');
        state.selfPickedTeacherId = null;
        state.selfShowList = true;
        renderAll();
      });

      selfTeacherSelect.addEventListener('change', (e) => {
        state.selfPickedTeacherId = e.target.value ? Number(e.target.value) : null;
        state.selfShowList = !state.selfPickedTeacherId;
        state.selfDayFilter = 'all';
        renderAll();
      });

      selfClearTeacherBtn.addEventListener('click', resetSelfLookup);

      selfTeacherGrid.addEventListener('click', (e) => {
        const btn = e.target.closest('[data-self-pick]');
        if (!btn) return;
        state.selfPickedTeacherId = Number(btn.getAttribute('data-self-pick'));
        state.selfShowList = false;
        state.selfDayFilter = 'all';
        renderAll();
      });

      document.addEventListener('keydown', (e) => {
        if (e.key === 'Escape') {
          if (teacherModal.classList.contains('open')) closeTeacherModal();
          if (slotEditorModal.classList.contains('open')) closeSlotEditor();
          if (teacherProfileModal.classList.contains('open')) closeTeacherProfile();
        }
      });

      applyTheme(state.theme);
      applyStaticTranslations();
      updateDynamicCountsAndDropdowns();
      syncEditorTranslations();
      renderAll();
    })();
  </script>
</body>
</html>
