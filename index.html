<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Planing QA Sliman & Dashboard Direction</title>
    <!-- ===== HORODATAGE DE BUILD (ne pas modifier à la main) =====
         Date de dernière modification du fichier : vendredi 23 octobre 2026 (heure locale +02:00)
         Semaine ISO correspondante : 43 (lundi 19/10/2026 -> dimanche 25/10/2026)
         Pour l'IA : relire cette balise meta permet de dater la version sans ouvrir le fichier. -->
    <meta name="build-horodatage" content="2026-10-23; semaine-iso=43; v10=verrou-2704+brouillons+equipe-mobile">
    <!-- Chargeur local-first : si le dossier libs/ est copié à côté du HTML, tout fonctionne hors-ligne ; sinon repli CDN automatique -->
    <script>
        function loadLibScriptFallback(cdnUrl) {
            var s = document.createElement('script');
            s.src = cdnUrl;
            s.onerror = function () { console.error('Librairie injoignable (local + CDN) : ' + cdnUrl); };
            document.head.appendChild(s);
        }
        function loadLibStyleFallback(cdnUrl) {
            var l = document.createElement('link');
            l.rel = 'stylesheet'; l.href = cdnUrl;
            document.head.appendChild(l);
        }
    </script>
    <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Crect width='64' height='64' rx='14' fill='%230F172A'/%3E%3Cpath d='M14 36l36-14-14 36-5-15-17-7z' fill='%2338BDF8'/%3E%3C/svg%3E">
    <meta name="theme-color" content="#0F172A">
    <link rel="stylesheet" href="libs/css/all.min.css" onerror="this.onerror=null;loadLibStyleFallback('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css')">
    <script src="libs/tailwind.js" onerror="this.onerror=null;loadLibScriptFallback('https://cdn.tailwindcss.com')"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&family=JetBrains+Mono:wght@600;800;900&display=swap" rel="stylesheet">
    <script src="libs/chart.umd.min.js" onerror="this.onerror=null;loadLibScriptFallback('https://cdn.jsdelivr.net/npm/chart.js@4.4.9/dist/chart.umd.min.js')"></script>

    <style>
        body { font-family: 'Inter', sans-serif; background-color: #F4F7F9; color: #0F172A; margin: 0; -webkit-font-smoothing: antialiased; }
        .mono { font-family: 'JetBrains Mono', monospace; }

        ::-webkit-scrollbar { width: 8px; height: 8px; }
        ::-webkit-scrollbar-track { background: transparent; }
        ::-webkit-scrollbar-thumb { background: #CBD5E1; border-radius: 10px; }
        ::-webkit-scrollbar-thumb:hover { background: #94A3B8; }
        .hide-scrollbar::-webkit-scrollbar { display: none; }
        .hide-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }

        .q-card {
            display: inline-flex; flex-direction: column; width: 100%; max-width: 320px;
            background: #FFFFFF; border-radius: 8px; margin: 6px 0;
            border: 1px solid #E2E8F0; box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
            transition: all 0.2s; cursor: pointer; overflow: hidden; border-left-width: 12px; position: relative;
        }
        @media (min-width: 640px) { .q-card { margin: 6px; } }
        .q-card:hover { box-shadow: 0 8px 16px rgba(15, 23, 42, 0.1); transform: translateY(-2px); }

        .card-ini { border-left-color: #0EA5E9; }
        .card-pro { border-left-color: #F97316; }

        .q-header { padding: 10px 12px; border-bottom: 1px solid #F1F5F9; display: flex; justify-content: space-between; align-items: center; }
        .q-code { font-family: 'JetBrains Mono', monospace; font-size: 12px; font-weight: 900; color: #1E293B; }
        .q-body { padding: 14px 12px; flex-grow: 1; display: flex; flex-direction: column; align-items: flex-start; gap: 8px; }
        .q-title-row { display: flex; align-items: flex-start; gap: 8px; width: 100%; }
        .q-title { font-size: 12px; font-weight: 900; color: #0F172A; line-height: 1.4; text-transform: uppercase; flex-grow: 1; display: block; }

        .q-note { font-size: 12px !important; color: #1E293B !important; font-weight: 800; background-color: #FEF3C7 !important; padding: 8px 10px; border-radius: 6px; width: 100%; border: 1px solid #FDE68A !important; border-left: 4px solid #F59E0B !important; margin-top: 6px; }
        .status-expired .q-note { background: #FEF2F2 !important; border-color: #FCA5A5 !important; border-left-color: #EF4444 !important; color: #7F1D1D !important; }

        .q-footer { padding: 10px 12px; background: rgba(0,0,0,0.02); display: flex; justify-content: space-between; align-items: center; }
        .q-date { font-family: 'JetBrains Mono', monospace; font-size: 12px; font-weight: 800; color: #475569; }

        .badge-type { padding: 3px 6px; border-radius: 4px; font-size: 10px; font-weight: 900; }
        .type-ini { background: #E0F2FE; color: #0369A1; }
        .type-pro { background: #FFEDD5; color: #B45309; }

        .state-validated { border: none !important; background: #000 !important; padding: 6px !important; position: relative; z-index: 1; }
        .state-validated::before { content: ''; position: absolute; height: 300%; width: 300%; background-image: conic-gradient(#00ff00, #22c55e, transparent 25%, #22c55e, #00ff00); top: -100%; left: -100%; animation: rotate-laser 4s linear infinite; z-index: -1; }
        @keyframes rotate-laser { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
        .state-validated .q-header, .state-validated .q-body, .state-validated .q-footer { background-color: #F0FDF4 !important; border: none; border-radius: 0; }
        .state-validated .q-title { color: #166534 !important; }
        .state-validated .q-icon { color: #10B981 !important; font-size: 16px; }

        .state-priority { border-left-width: 16px !important; border-left-color: #00E5FF !important; background-color: #F0F9FF !important; border-color: #00E5FF !important; box-shadow: 0 0 15px rgba(0, 229, 255, 0.4); z-index: 10; }
        .state-priority .priority-sky { display: block !important; background: #E0F2FE; height: 40px; position: relative; overflow: hidden; border-bottom: 1px dashed #7DD3FC; padding: 0 !important; }
        .plane-wrapper { position: absolute; top: 0; left: -350px; height: 100%; display: flex; align-items: center; animation: fly-right 3.5s linear infinite; white-space: nowrap; }
        .plane-icon { filter: drop-shadow(2px 4px 2px rgba(0,0,0,0.2)); z-index: 3; margin-bottom: 2px; }
        .plane-cable { width: 15px; height: 2px; background-color: #475569; z-index: 1; }
        .plane-banner-content { background-color: #FFFFFF; color: #0369A1; background-image: linear-gradient(115deg, rgba(255,255,255,0) 40%, rgba(14, 165, 233, 0.15) 45%, rgba(14, 165, 233, 0.6) 50%, rgba(14, 165, 233, 0.15) 55%, rgba(255,255,255,0) 60%); background-size: 200% 100%; border: 2px solid #0EA5E9; box-shadow: 0 4px 8px rgba(2, 132, 199, 0.15); padding: 4px 10px; font-weight: 900; font-size: 11px; border-radius: 4px; display: flex; align-items: center; gap: 6px; position: relative; z-index: 2; letter-spacing: 1px; animation: lightning-strike 2.5s infinite linear; }
        @keyframes lightning-strike { 0% { background-position: 200% 0; } 100% { background-position: -200% 0; } }
        .state-priority .q-title { color: #0369A1 !important; font-weight: 900; }
        .state-priority .q-icon { color: #0284C7 !important; font-size: 18px; }
        @keyframes fly-right { 0% { left: -350px; transform: translateY(0px); } 25% { transform: translateY(-2px); } 50% { transform: translateY(2px); } 75% { transform: translateY(-2px); } 100% { left: 100%; transform: translateY(0px); } }

        .state-disabled { border-left-width: 24px !important; border-left-color: #F59E0B !important; background-color: #FFFBEB !important; border-color: #FCD34D !important; }
        .state-disabled .q-banner { display: block; background: repeating-linear-gradient(-45deg, #F59E0B, #F59E0B 10px, #1E293B 10px, #1E293B 20px); background-size: 28.28px 28.28px; color: #FFFFFF; text-shadow: 1px 1px 2px rgba(0,0,0,0.8); animation: zebra-move 1.5s linear infinite; }
        @keyframes zebra-move { 0% { background-position: 0 0; } 100% { background-position: 28.28px 0; } }
        .state-disabled .q-body { background-color: rgba(255, 255, 255, 0.9); margin: 6px; border-radius: 6px; padding: 12px; border: 1px solid #FDE68A; }

        .state-standby { border-left-color: #64748B !important; background-color: #F1F5F9 !important; border: 1px solid #CBD5E1 !important; border-left-width: 12px !important; background-image: linear-gradient(rgba(100, 116, 139, 0.15) 2px, transparent 2px), linear-gradient(90deg, rgba(100, 116, 139, 0.15) 2px, transparent 2px) !important; background-size: 20px 20px !important; }
        .state-standby .q-banner { display: block; background-color: #334155; color: #FFFFFF; letter-spacing: 2px; text-align: center; font-size: 11px; padding: 4px 0; font-weight: 900; }
        .state-standby .q-body { background-color: rgba(255, 255, 255, 0.95); margin: 6px; border-radius: 6px; padding: 12px; border: 1px solid #E2E8F0; }

        .status-expired { border-left-color: #EF4444 !important; background-color: #7F1D1D !important; border-color: #B91C1C !important; animation: alarm-breathe 3s ease-in-out infinite; }
        .status-expired .q-banner { display: block; background-color: #450A0A; color: #FCA5A5; text-align: center; font-size: 11px; padding: 4px 0; font-weight: 900; border-bottom: 1px solid #991B1B; }
        .status-expired .q-title { color: #FFFFFF !important; }
        .status-expired .q-code { color: #FECACA !important; }
        .status-expired .q-date { color: #FCA5A5 !important; }
        .status-expired .q-icon { color: #FCA5A5 !important; }
        @keyframes alarm-breathe { 0%, 100% { box-shadow: 0 0 5px rgba(220, 38, 38, 0.2); } 50% { box-shadow: 0 0 15px rgba(220, 38, 38, 0.6); } }

        .timer-badge { font-size: 11px; padding: 2px 6px; border-radius: 4px; font-weight: 900; }
        .timer-ok { background: #E2E8F0; color: #475569; }
        .timer-soon { background: #FEF3C7; color: #B45309; }
        .timer-expired { background: #FEE2E2; color: #DC2626; border: 1px solid #FCA5A5; }

        .excel-table th { background: #1E293B; color: white; font-size: 10px; text-transform: uppercase; padding: 10px; text-align: left; }
        .excel-table td { border-bottom: 1px solid #E2E8F0; padding: 8px 10px; font-size: 11px; }

        .qls-table { border-collapse: collapse; margin: 0 auto; }
        .qls-table th, .qls-table td { border: 1px solid #94A3B8; padding: 4px 6px; font-size: 10px; }

        .tour-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(15, 23, 42, 0.85); z-index: 9990; display: none; backdrop-filter: blur(2px); }
        .tour-focus-box { position: fixed; border-radius: 12px; pointer-events: none; z-index: 9992; transition: all 0.3s cubic-bezier(0.25, 1, 0.5, 1); opacity: 0; visibility: hidden; border: 4px solid transparent; box-shadow: 0 0 0 9999px rgba(15, 23, 42, 0.75), 0 0 20px rgba(239, 68, 68, 1); }
        .tour-focus-box.active { opacity: 1; visibility: visible; animation: tour-blink-red 0.8s infinite alternate; }
        @keyframes tour-blink-red { from { border-color: #ef4444; box-shadow: 0 0 0 9999px rgba(15, 23, 42, 0.75), 0 0 25px 5px rgba(239, 68, 68, 0.8); } to { border-color: rgba(239, 68, 68, 0.3); box-shadow: 0 0 0 9999px rgba(15, 23, 42, 0.85), 0 0 5px 0px rgba(239, 68, 68, 0); } }
        .tour-dialog { position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 9995; background: white; padding: 24px; border-radius: 16px; box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5); width: 90%; max-width: 400px; display: none; border: 2px solid #BFDBFE; text-align: center; }

        /* ===== NOUVEAU : modales, toast, formulaires, accessibilité ===== */
        .modal-backdrop { position: fixed; inset: 0; background: rgba(15, 23, 42, 0.6); backdrop-filter: blur(2px); z-index: 9980; display: none; align-items: center; justify-content: center; padding: 16px; }
        .modal-backdrop.open { display: flex; }
        .modal-panel { background: #fff; border-radius: 16px; box-shadow: 0 25px 50px -12px rgba(0,0,0,0.5); width: 100%; max-width: 600px; max-height: 88vh; display: flex; flex-direction: column; overflow: hidden; }
        .modal-head { padding: 14px 18px; border-bottom: 1px solid #E2E8F0; display: flex; justify-content: space-between; align-items: center; background: #F8FAFC; gap: 12px; }
        .modal-title { font-weight: 900; text-transform: uppercase; font-size: 13px; letter-spacing: 0.05em; color: #0F172A; display: inline-flex; align-items: center; }
        .modal-body { padding: 16px 18px; overflow-y: auto; flex-grow: 1; }
        .modal-foot { padding: 12px 18px; border-top: 1px solid #E2E8F0; display: flex; justify-content: flex-end; gap: 8px; background: #F8FAFC; }
        .modal-close { width: 30px; height: 30px; border-radius: 8px; display: flex; align-items: center; justify-content: center; color: #64748B; flex-shrink: 0; }
        .modal-close:hover { background: #E2E8F0; color: #0F172A; }

        .toast-box { position: fixed; bottom: 20px; right: 20px; z-index: 9999; display: flex; flex-direction: column; gap: 8px; align-items: flex-end; }
        .toast { background: #0F172A; color: #fff; padding: 10px 14px; border-radius: 10px; font-size: 12px; font-weight: 700; box-shadow: 0 10px 25px rgba(0,0,0,0.3); border-left: 4px solid #22C55E; max-width: 320px; animation: toast-in 0.25s ease; }
        .toast.err { border-left-color: #EF4444; }
        @keyframes toast-in { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        .form-label { display: block; font-size: 10px; font-weight: 900; text-transform: uppercase; color: #64748B; margin-bottom: 4px; letter-spacing: 0.05em; }
        .form-input { width: 100%; border: 1px solid #CBD5E1; border-radius: 8px; padding: 8px 10px; font-size: 12px; font-weight: 600; background: #fff; color: #0F172A; }
        .form-input:focus { outline: 2px solid #0EA5E9; border-color: transparent; }

        .state-btn { padding: 8px 12px; border-radius: 8px; font-size: 11px; font-weight: 900; border: 1px solid #CBD5E1; background: #fff; color: #475569; text-transform: uppercase; cursor: pointer; }
        .state-btn:hover { background: #F1F5F9; }
        .state-btn.active { outline: 2px solid #0EA5E9; background: #E0F2FE; color: #0369A1; border-color: #0EA5E9; }

        .op-flash { animation: opFlash 2s ease; }
        @keyframes opFlash { 0%, 100% { background: #fff; } 20%, 60% { background: #DBEAFE; } }

        @media (prefers-reduced-motion: reduce) {
            *, *::before, *::after { animation-duration: 0.01ms !important; animation-iteration-count: 1 !important; transition-duration: 0.01ms !important; }
        }
        /* ===== VAGUE DESIGN & FONCTIONS (D1-D5, F1-F4) ===== */
        /* D1 : compteurs de statut cliquables */
        .cnt-badge { display: inline-flex; align-items: center; gap: 6px; padding: 6px 12px; border-radius: 9999px; font-size: 11px; font-weight: 900; text-transform: uppercase; letter-spacing: .04em; background: #fff; border: 1px solid #E2E8F0; box-shadow: 0 1px 2px rgba(15,23,42,.05); transition: transform .15s, box-shadow .15s; cursor: pointer; }
        .cnt-badge:hover { transform: translateY(-1px); box-shadow: 0 6px 14px rgba(15,23,42,.10); }
        .cnt-badge .cnt-n { font-family: 'JetBrains Mono', monospace; font-size: 14px; }
        .cnt-badge.cnt-expired { color: #B91C1C; border-color: #FECACA; background: #FEF2F2; }
        .cnt-badge.cnt-soon { color: #92400E; border-color: #FDE68A; background: #FFFBEB; }
        .cnt-badge.cnt-aqual { color: #075985; border-color: #BAE6FD; background: #F0F9FF; }
        .cnt-badge.cnt-validated { color: #065F46; border-color: #A7F3D0; background: #ECFDF5; }
        .cnt-badge.cnt-active { outline: 2px solid currentColor; outline-offset: 1px; transform: translateY(-1px); }
        .cnt-badge.cnt-zero { opacity: .55; }
        /* D2 : pastille initiales + barre de progression */
        .op-pastille { width: 34px; height: 34px; border-radius: 9999px; color: #fff; font-size: 11px; font-weight: 900; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
        .op-progress { height: 6px; border-radius: 9999px; background: #E2E8F0; overflow: hidden; margin-top: 6px; }
        .op-progress > i { display: block; height: 100%; border-radius: 9999px; transition: width .4s ease; }
        /* D3 : bandeau du jour */
        #today-banner { animation: fadeSlide .25s ease; }
        @keyframes fadeSlide { from { opacity: 0; transform: translateY(-4px); } to { opacity: 1; transform: none; } }
        /* D5 : micro-interactions */
        .view-in { animation: viewIn .18s ease; }
        @keyframes viewIn { from { opacity: 0; transform: translateY(6px); } to { opacity: 1; transform: none; } }
        #tableBody tr { transition: box-shadow .15s; }
        #tableBody tr:hover { box-shadow: inset 0 0 0 2px rgba(56,189,248,.35); }
        /* F1 : lignes d'échéances */
        .ech-row { transition: background .15s, transform .15s; cursor: pointer; }
        .ech-row:hover { background: #F8FAFC; transform: translateX(2px); }
        /* D5 : retour en haut */
        #back-to-top { position: fixed; right: 18px; bottom: 18px; z-index: 60; width: 42px; height: 42px; border-radius: 12px; background: #0F172A; color: #fff; border: none; box-shadow: 0 8px 20px rgba(15,23,42,.30); display: none; align-items: center; justify-content: center; cursor: pointer; font-size: 15px; }
        #back-to-top.show { display: flex; }
        #back-to-top:hover { background: #1E293B; transform: translateY(-2px); }
        /* F2 : fiche opérateur (écran + impression dédiée) */
        #fiche-print { position: fixed; inset: 0; z-index: 70; background: rgba(15,23,42,.55); overflow: auto; padding: 20px; display: none; }
        #fiche-print.fiche-open { display: block; }
        .fiche-sheet { background: #fff; max-width: 880px; margin: 10px auto; padding: 26px 30px; border-radius: 14px; box-shadow: 0 20px 50px rgba(15,23,42,.35); }
        .fiche-sheet table { width: 100%; border-collapse: collapse; font-size: 12px; }
        .fiche-sheet th { background: #0F172A; color: #fff; text-align: left; padding: 7px 9px; font-size: 10px; text-transform: uppercase; letter-spacing: .06em; }
        .fiche-sheet td { border: 1px solid #E2E8F0; padding: 6px 9px; }
        @media print {
            header, #filters-container, .no-print, #tour-overlay, #tour-dialog, #tour-focus-box, .toast-box { display: none !important; }
            body { background: #fff; }
            main { padding: 0 !important; }
            .modal-backdrop { display: none !important; }
            /* F2 : si une fiche est ouverte mais que l'impression n'est pas lancée via son
               bouton (Ctrl+P normal), l'overlay n'est PAS imprimée — seule la classe
               body.print-fiche (spécificité supérieure) l'affiche à l'impression. */
            #fiche-print.fiche-open { display: none !important; }
            /* F2 : n'imprimer QUE la fiche quand le corps porte la classe dédiée */
            body.print-fiche > *:not(#fiche-print) { display: none !important; }
            body.print-fiche #fiche-print { display: block !important; position: static !important; background: #fff; padding: 0; overflow: visible; }
            body.print-fiche .fiche-sheet { box-shadow: none; border-radius: 0; margin: 0; max-width: none; padding: 0; }
        }

        /* ===== CSS DE SECOURS =====
           Si Tailwind ne se charge ni en local ni via le CDN (poste coupé),
           ces règles (spécificité élément, battues par les classes Tailwind quand
           elles sont présentes) gardent la page lisible et utilisable. */
        .hidden { display: none !important; }
        html, body { background: #F4F7F9; color: #0F172A; margin: 0; }
        header { background: #0F172A; color: #fff; padding: 10px 16px; }
        header h1 { font-size: 18px; font-weight: 900; margin: 0; text-transform: uppercase; }
        main { padding: 16px; }
        table { border-collapse: collapse; width: 100%; background: #fff; }
        th, td { border: 1px solid #CBD5E1; padding: 6px 8px; font-size: 12px; text-align: left; }
        thead th { background: #1E293B; color: #fff; }
        button { cursor: pointer; border: 1px solid #CBD5E1; background: #fff; border-radius: 8px; padding: 6px 10px; font-weight: 700; font-size: 12px; }
        input, select, textarea { border: 1px solid #CBD5E1; border-radius: 8px; padding: 6px 8px; font-size: 12px; font-family: inherit; }
        #view-reporting, #view-hebdo, #view-tuto, #filters-container { margin-top: 12px; }
        #searchResults { background: #fff; border: 1px solid #CBD5E1; }

        /* ===== VAGUE VIZ EXPERT (V1, V2, V6, V7, I1, I2) ===== */
        /* I1 : fond dégradé subtil */
        html, body { background: linear-gradient(160deg, #EEF3F8 0%, #F4F7F9 45%, #E9F0F7 100%); background-attachment: fixed; }
        /* V7 : confettis (sous les modales z9980, au-dessus du reste) */
        #confetti-canvas { position: fixed; inset: 0; z-index: 9970; pointer-events: none; }
        /* V7 : tampon d'état dans la modale carte */
        .state-stamp { position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%) rotate(-14deg) scale(2.6); opacity: 0; font-size: 42px; font-weight: 900; letter-spacing: .06em; border: 6px solid currentColor; border-radius: 16px; padding: 8px 28px; pointer-events: none; z-index: 9985; text-transform: uppercase; background: rgba(255,255,255,.85); }
        .state-stamp.play { animation: stampIn .55s cubic-bezier(.2, 1.4, .4, 1) forwards; }
        @keyframes stampIn {
            0% { opacity: 0; transform: translate(-50%, -50%) rotate(-14deg) scale(2.6); }
            55% { opacity: 1; transform: translate(-50%, -50%) rotate(-14deg) scale(1); }
            100% { opacity: .9; transform: translate(-50%, -50%) rotate(-14deg) scale(1); }
        }
        .stamp-validated { color: #059669; }
        .stamp-priority { color: #2563EB; }
        .stamp-standby { color: #64748B; }
        .stamp-disabled { color: #DC2626; }
        /* V1 : timeline Gantt */
        .tl-scroll { max-height: 62vh; overflow-y: auto; overflow-x: hidden; }
        .tl-row { display: flex; align-items: center; border-bottom: 1px solid #F1F5F9; }
        .tl-row:hover { background: #F8FAFC; }
        .tl-name { width: 148px; flex-shrink: 0; position: sticky; left: 0; background: inherit; z-index: 1; font-size: 10px; font-weight: 900; text-transform: uppercase; color: #334155; padding: 0 8px; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
        .tl-row { background: #fff; }
        .tl-track { position: relative; flex-grow: 1; height: 27px; }
        .tl-grid { position: absolute; top: 0; bottom: 0; width: 1px; background: #E2E8F0; }
        .tl-grid.month-start { background: #CBD5E1; }
        .tl-today { position: absolute; top: 0; bottom: 0; width: 2px; background: #2563EB; opacity: .55; }
        .tl-bar { position: absolute; top: 4px; height: 19px; border-radius: 6px; font-size: 9px; font-weight: 900; color: #fff; display: flex; align-items: center; gap: 4px; padding: 0 6px; white-space: nowrap; overflow: hidden; cursor: pointer; box-shadow: 0 1px 3px rgba(15,23,42,.25); transition: filter .15s, transform .15s; z-index: 1; }
        .tl-bar:hover { transform: translateY(-1px); filter: brightness(1.1); }
        .tl-bar.bar-exp { background: #DC2626; }
        .tl-bar.bar-30 { background: #EA580C; }
        .tl-bar.bar-90 { background: #D97706; }
        .tl-bar.bar-far { background: #2563EB; }
        .tl-months { display: flex; position: relative; height: 18px; margin-left: 148px; }
        .tl-month-lbl { position: absolute; font-size: 9px; font-weight: 900; text-transform: uppercase; color: #64748B; letter-spacing: .05em; padding-left: 4px; border-left: 1px solid #CBD5E1; }
        /* V2 : heatmap */
        .hm-grid { display: grid; gap: 2px; }
        .hm-cell { height: 24px; border-radius: 4px; display: flex; align-items: center; justify-content: center; font-size: 9px; font-weight: 900; color: #fff; background: #F1F5F9; cursor: default; transition: transform .1s; }
        .hm-cell:hover { transform: scale(1.15); z-index: 2; }
        .hm-cell.lvl-1 { background: #FCD34D; color: #78350F; }
        .hm-cell.lvl-2 { background: #FB923C; }
        .hm-cell.lvl-3 { background: #EA580C; }
        .hm-cell.lvl-4 { background: #DC2626; }
        .hm-cell.crit { outline: 2px solid #991B1B; outline-offset: -2px; }
        /* I2 : validation rapide */
        .ech-fast { width: 26px; height: 26px; border-radius: 8px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; background: #ECFDF5; border: 1px solid #A7F3D0; color: #059669; cursor: pointer; transition: all .15s; }
        .ech-fast:hover { background: #059669; color: #fff; transform: scale(1.12); }
        /* drop overlay */
        #drop-overlay { position: fixed; inset: 0; z-index: 9998; background: rgba(15,23,42,.62); display: none; align-items: center; justify-content: center; pointer-events: none; backdrop-filter: blur(2px); }
        #drop-overlay.show { display: flex; }
        .drop-card { background: #fff; border: 3px dashed #2563EB; border-radius: 18px; padding: 34px 44px; text-align: center; box-shadow: 0 25px 60px rgba(15,23,42,.5); }

        /* ============================================================
           VAGUE DIRECTION ARTISTIQUE — « FICHE DE CONTRÔLE »
           Papier technique ivoire + encre bleu-noir, bleu de plan,
           filets fins, chiffres machine. Couche d'surcharge ciblée :
           uniquement des classes/IDs propres (aucune règle générique
           partagée avec KPI & Direction / Résumé Hebdo).
           Animations A1-A8 : transform/opacity uniquement (GPU), sauf
           a-ruban (reflet au survol, une seule carte à la fois) ;
           infinis réservés aux états d'échéance, one-shots déclenchés
           par .card-just-changed (changement d'état réel, jamais au
           simple rendu du tableau).
           ============================================================ */
        :root {
            --papier: #F1EDE4;      /* fond de page */
            --surface: #FBF9F4;     /* cartes, panneaux */
            --surface-2: #FFFFFF;   /* champs, feuille d'impression */
            --encre: #17212B;       /* texte principal */
            --encre-2: #5A6672;     /* texte secondaire */
            --filet: #DDD6C8;       /* bordures */
            --plan: #1D4E89;        /* accent principal */
            --plan-clair: #2E6B9E;  /* accent secondaire */
            --cuivre: #B4622A;      /* accent chaud (INI, pas capable) */
            --valide: #1D6B4F;      /* encre verte */
            --urgence: #C2410C;     /* orange urgence */
            --alerte: #B42318;      /* rouge alerte */
            --neutre: #8A8578;      /* gris chaud (standby) */
            --attente: #2E6B9E;     /* bleu attente (à qualifier) */
            --r: 4px;               /* rayon signature */
            --o1: 0 1px 2px rgba(23,33,43,.06);
            --o2: 0 1px 2px rgba(23,33,43,.09), 0 3px 8px rgba(23,33,43,.07);
            --d1: 120ms; --d2: 180ms; --d3: 260ms;
            --courbe: cubic-bezier(.2, 0, 0, 1);        /* précision machinée */
            --courbe-out: cubic-bezier(.16, 1, .3, 1);  /* sortie amortie */
        }
        /* ---- Fond papier ivoire + texture 45° très subtile ---- */
        html { background: var(--papier); }
        body { background: var(--papier) repeating-linear-gradient(45deg, rgba(23,33,43,.02) 0 1px, transparent 1px 7px); background-attachment: fixed; color: var(--encre); font-family: 'Inter', 'Segoe UI', system-ui, sans-serif; }
        .mono { font-family: 'JetBrains Mono', Consolas, monospace; }
        ::-webkit-scrollbar-thumb { background: #C9C0AE; }
        ::-webkit-scrollbar-thumb:hover { background: #A89E8A; }
        input, select, textarea { border-color: var(--filet); border-radius: var(--r); }
        /* ---- Chrome : bandeau d'encre, filet de plan, boutons gravés ---- */
        header { background-color: #17212B !important; border-bottom: 2px solid var(--plan); box-shadow: 0 10px 28px rgba(23,33,43,.14); }
        header .rounded-lg { border-radius: var(--r) !important; }
        header .bg-slate-800, header .bg-slate-900 { background-color: #101A22 !important; border-color: #2B3945 !important; }
        header .bg-slate-800:hover, header .bg-slate-900:hover { background-color: #16222C !important; }
        header .bg-blue-600 { background: var(--papier) !important; box-shadow: none !important; border: 1px solid rgba(221,214,200,.45); }
        header .bg-blue-600 i { color: var(--plan) !important; }
        header .bg-blue-100 { background: var(--surface) !important; border-color: var(--filet) !important; color: var(--plan) !important; }
        header .bg-blue-100:hover { background: #F3EEE3 !important; }
        header h1 { letter-spacing: .02em; }
        header h1 span { color: #C97A3D !important; }
        header p { color: #8E9AA6 !important; }
        #btn-validated-modal { border: 1px solid #2B3945 !important; }
        #btn-validated-modal .bg-emerald-500 { animation: a-veille-verte 2.8s ease-in-out infinite; }
        @keyframes a-veille-verte { 0%, 100% { opacity: .45; } 50% { opacity: 1; } }
        #search-container input { background-color: #101A22 !important; border-color: #2B3945 !important; }
        #search-container input:focus { border-color: var(--plan-clair) !important; }
        #search-container .fa-search { color: #7C8B99 !important; }
        #tab-bar button { border-radius: var(--r) !important; transition: background var(--d1) var(--courbe), color var(--d1) var(--courbe), border-color var(--d1) var(--courbe); }
        #tab-bar .bg-blue-600 { background: var(--plan) !important; }
        #tab-bar .bg-white { background: var(--surface) !important; border-color: var(--filet) !important; color: var(--encre-2) !important; }
        #back-to-top { background: var(--encre); border-radius: var(--r); }
        /* ---- Pastilles de compteurs (papier encré) ---- */
        .cnt-badge { background: var(--surface); border-color: var(--filet); color: var(--encre-2); border-radius: var(--r); box-shadow: var(--o1); }
        .cnt-badge .cnt-n { color: inherit; }
        .cnt-badge.cnt-expired { color: var(--alerte); border-color: #E5B9B4; background: #F9EDEB; }
        .cnt-badge.cnt-soon { color: var(--urgence); border-color: #E6C9A8; background: #F7EFE3; }
        .cnt-badge.cnt-aqual { color: var(--attente); border-color: #B9CBDC; background: #EDF2F7; }
        .cnt-badge.cnt-validated { color: var(--valide); border-color: #AECBBB; background: #EAF2ED; }
        .state-btn { border-radius: var(--r); border-color: var(--filet); background: var(--surface); color: var(--encre-2); }
        .state-btn.active { outline: 2px solid var(--plan); background: #E7EDF4; color: var(--plan); border-color: var(--plan); }
        /* ---- Surfaces : cartes, table, échéances, modales, fiche ---- */
        .q-card { background: var(--surface); border-color: var(--filet); border-radius: var(--r); box-shadow: var(--o1); transition: box-shadow var(--d2) var(--courbe), transform var(--d2) var(--courbe); }
        .q-card:hover { box-shadow: var(--o2); transform: translateY(-2px); }
        .card-ini { border-left-color: var(--plan-clair); }
        .card-pro { border-left-color: var(--cuivre); }
        .q-header { background: transparent; border-bottom-color: var(--filet); }
        .q-code { color: var(--encre); letter-spacing: .04em; }
        .q-body { background: transparent; }
        .q-title { color: var(--encre); letter-spacing: .02em; }
        .q-footer { background: rgba(23,33,43,.03); border-top: 1px solid var(--filet); }
        .q-date { color: var(--encre-2); }
        .q-note { background: #F7EEDD !important; border-color: #E6D3AE !important; border-left-color: var(--cuivre) !important; color: #5C421F !important; border-radius: 3px !important; }
        .badge-type { border-radius: 3px; }
        .type-ini { background: #E4EDF5; color: var(--plan); }
        .type-pro { background: #F5E7D8; color: #8A4B1B; }
        .timer-badge { border-radius: 3px; font-family: 'JetBrains Mono', Consolas, monospace; letter-spacing: .02em; }
        #tableBody tr { background: var(--surface); border-bottom-color: var(--filet) !important; transition: box-shadow var(--d1) var(--courbe); }
        #tableBody tr:hover { box-shadow: inset 0 0 0 2px rgba(29,78,137,.25); }
        #tableBody td { border-color: var(--filet) !important; }
        .op-pastille { border-radius: 3px; box-shadow: inset 0 0 0 1px rgba(23,33,43,.15); }
        .op-progress { background: #E7E0D2; border-radius: 2px; }
        .op-progress > i { border-radius: 2px; }
        .ech-row { background: var(--surface) !important; border-color: var(--filet) !important; border-radius: var(--r) !important; }
        .ech-row:hover { background: #F6F2E9 !important; }
        .ech-fast { border-radius: 3px; background: #EAF2ED; border-color: #AECBBB; color: var(--valide); }
        .ech-fast:hover { background: var(--valide); border-color: var(--valide); }
        .modal-panel { background: var(--surface); border-radius: 6px; border: 1px solid var(--filet); box-shadow: 0 24px 60px rgba(23,33,43,.25); }
        .fiche-sheet { border-radius: 6px; border: 1px solid var(--filet); box-shadow: 0 18px 44px rgba(23,33,42,.28); }
        .drop-card { border-radius: 6px; border-color: var(--plan); }
        /* Timeline / heatmap : harmonisation papier (couleurs sémantiques conservées) */
        .tl-row { background: var(--surface); border-bottom-color: var(--filet); }
        .tl-name { color: var(--encre-2); }
        .tl-row:hover { background: #F6F2E9; }
        .tl-bar { border-radius: 3px; }
        .hm-cell { border-radius: 2px; background: #EFE9DC; }
        /* ---- Tampon d'état : encre de fiche contrôle ---- */
        .state-stamp { border-width: 5px !important; border-radius: 6px !important; font-family: 'JetBrains Mono', Consolas, monospace; font-size: 38px; background: rgba(251,249,244,.92); letter-spacing: .1em; }
        .stamp-validated { color: var(--valide); }
        .stamp-priority { color: var(--urgence); }
        .stamp-standby { color: var(--encre-2); }
        .stamp-disabled { color: var(--cuivre); }
        .play-noanim { animation: none !important; }        /* correctif : classe manquante */
        .state-stamp.play-noanim { opacity: .9; }

        /* ===================== A1 — VALIDÉE : « verrouillage » =====================
           Trait d'encre verte fixe + léger enfoncement une seule fois au changement. */
        .q-card.state-validated { border: 1px solid var(--filet) !important; border-left: 12px solid var(--valide) !important; background: var(--surface) !important; padding: 0 !important; }
        .q-card.state-validated::before { content: none !important; }          /* coupe l'anneau laser */
        .state-validated .q-header, .state-validated .q-body, .state-validated .q-footer { background-color: transparent !important; border: none; border-radius: 0; }
        .state-validated .q-title { color: var(--valide) !important; }
        .state-validated .q-icon { color: var(--valide) !important; font-size: 15px; }
        .q-card.card-just-changed.state-validated { animation: a-verrou var(--d3) var(--courbe-out); }
        @keyframes a-verrou { 0% { transform: scale(1.035); } 55% { transform: scale(.985); } 100% { transform: scale(1); } }

        /* ===================== A2 — PRIORITÉ : « dossier de priorité » =====================
           La carte devient un DOSSIER : dos ambre vertical (26 px) le long du
           bord gauche avec le mot PRIORITÉ écrit de bas en haut, et coin
           replié en triangle — seule carte à texte vertical de l'application,
           l'œil y va tout de suite à 2 mètres. Rien à voir avec l'échue
           (bandeau ROUGE horizontal « verdict »). Le reste de la fiche reste
           en papier net : seule la structure change, pas la couleur de l'encre.
           Au changement d'état, le dos se range depuis le haut (une fois).
           L'avion est neutralisé en CSS pur. */
        .q-card.state-priority { border-color: var(--filet) !important; border-left-width: 0 !important; background: var(--surface) !important; background-image: none !important; box-shadow: 0 2px 4px rgba(23,33,43,.10), 0 6px 16px rgba(180,83,9,.13); }
        .q-card.state-priority::before { content: ''; position: absolute; top: 0; right: 0; width: 0; height: 0; border-left: 15px solid transparent; border-top: 15px solid #B45309; z-index: 3; }
        .state-priority .priority-sky { display: block !important; position: static !important; height: 0 !important; overflow: visible !important; background: transparent !important; border: none !important; padding: 0 !important; }
        .state-priority .plane-wrapper { position: absolute !important; top: 0 !important; left: 0 !important; width: 100% !important; height: 100% !important; display: block; animation: none !important; transform: none !important; }
        .state-priority .plane-icon, .state-priority .plane-cable { display: none !important; }
        .state-priority .plane-banner-content { position: absolute !important; left: 0 !important; top: 0 !important; bottom: 0 !important; width: 26px; display: flex; align-items: center; justify-content: center; writing-mode: vertical-rl; transform: rotate(180deg); background: #B45309 !important; color: #fff !important; border: none !important; box-shadow: none !important; border-radius: 0 !important; padding: 8px 0 !important; letter-spacing: .18em; font-size: 10px; animation: none; background-image: none !important; clip-path: none; z-index: 2; }
        .state-priority .plane-banner-content i { display: none; }
        .q-card.card-just-changed.state-priority .plane-banner-content { animation: a-dossier .34s var(--courbe-out) both; }
        @keyframes a-dossier { 0% { transform: rotate(180deg) translateY(104%); } 100% { transform: rotate(180deg) translateY(0); } }
        .state-priority .q-header, .state-priority .q-body, .state-priority .q-footer { padding-left: 36px; }
        .state-priority .q-header { border-bottom-color: rgba(180,83,9,.22); }

        /* ===================== A3 — STANDBY : « LED qui respire » =====================
           Témoin rond qui monte et descend lentement (4,2 s) — état en veille. */
        .q-card.state-standby { border: 1px solid var(--filet) !important; border-left: 12px solid var(--neutre) !important; background: var(--surface) !important; background-image: none !important; }
        .state-standby .q-banner { display: block; background: transparent !important; color: var(--encre-2); letter-spacing: .18em; text-align: left; font-size: 10px; padding: 5px 12px; font-weight: 900; border-bottom: 1px solid var(--filet); }
        .state-standby .q-banner::before { content: ''; display: inline-block; width: 7px; height: 7px; border-radius: 50%; background: var(--neutre); margin-right: 8px; animation: a-led 4.2s ease-in-out infinite; }
        @keyframes a-led { 0%, 100% { opacity: .25; } 50% { opacity: .95; } }
        .state-standby .q-body { background-color: transparent; margin: 0; border: none; padding: 14px 12px; }
        .state-standby .q-title { color: var(--encre-2) !important; }

        /* ===================== A4 — PAS CAPABLE : « blocage » =====================
           Hachures inclinées figées (zèbre remplacée) + chute sans rebond au
           changement d'état, titre barré : le verrou est posé. */
        .q-card.state-disabled { border: 1px solid #E0C5A5 !important; border-left: 12px solid var(--cuivre) !important; background: var(--surface) !important; }
        .state-disabled .q-banner { display: block; background: repeating-linear-gradient(-45deg, var(--cuivre) 0 8px, #8A4B1B 8px 16px) !important; background-size: auto !important; color: #FFF !important; text-shadow: none; letter-spacing: .22em; animation: none !important; }
        .state-disabled .q-body { background-color: transparent; margin: 0; border: none; padding: 14px 12px; }
        .state-disabled .q-title { color: var(--encre-2) !important; text-decoration: line-through; text-decoration-thickness: 1px; }
        .q-card.card-just-changed.state-disabled { animation: a-blocage .3s var(--courbe-out); }
        @keyframes a-blocage { 0% { transform: translateY(-9px); opacity: .35; } 72% { transform: translateY(1px); opacity: 1; } 100% { transform: none; opacity: 1; } }

        /* ===================== A5 — ÉCHUE : « compteur figé » =====================
           Bandeau rouge plein qui bascule en place une fois (pas de respiration
           permanente : le rouge + les hachures statiques suffisent à 2 m). */
        .q-card.status-expired { animation: none !important; border: 1px solid #E0B4AF !important; border-left: 12px solid var(--alerte) !important; background: var(--surface) !important; background-image: repeating-linear-gradient(-45deg, rgba(180,35,24,.05) 0 6px, transparent 6px 13px) !important; }
        .q-card.status-expired.op-flash { animation: a-flash 2s ease !important; }   /* le halo passe aussi sur les cartes échues */
        .status-expired .q-banner { display: block; background: var(--alerte) !important; color: #fff !important; text-align: center; font-size: 11px; padding: 4px 0; font-weight: 900; letter-spacing: .2em; border-bottom: none !important; }
        .status-expired .q-title { color: var(--encre) !important; }
        .status-expired .q-code { color: var(--alerte) !important; }
        .status-expired .q-date { color: var(--alerte) !important; }
        .status-expired .q-icon { color: var(--alerte) !important; }
        .status-expired .q-note { background: #F7E9E6 !important; border-color: #E0B4AF !important; border-left-color: var(--alerte) !important; color: #6B241C !important; }
        .q-card.card-just-changed.status-expired .q-banner { animation: a-flip .3s var(--courbe-out); }
        @keyframes a-flip { 0% { transform: scaleY(.15); opacity: 0; } 100% { transform: none; opacity: 1; } }

        /* ===================== A6 — CRITIQUE (≤ 5 j) : « balise » =====================
           Liseré rouge qui pulse doucement (1,3 s) + pastille J-x qui bat :
           détectable à 2 m sans gêner la lecture. */
        .q-card.status-critical { border-left-color: var(--alerte) !important; }
        .q-card.status-critical::after { content: ''; position: absolute; inset: 0; border-radius: inherit; pointer-events: none; box-shadow: inset 0 0 0 2px var(--alerte); animation: a-balise 1.3s ease-in-out infinite; }
        @keyframes a-balise { 0%, 100% { opacity: 0; } 50% { opacity: .38; } }
        .timer-badge.timer-expired { background: #F9E7E3 !important; color: var(--alerte) !important; border: 1px solid #E5B9B4 !important; animation: a-bat 1.3s ease-in-out infinite; }
        @keyframes a-bat { 0%, 100% { transform: scale(1); } 50% { transform: scale(1.09); } }

        /* ===================== A7 — AVERTISSEMENT (≤ 15 j) : « sablier » =====================
           Filet cuivre qui se remplit lentement sous la pastille J-x (2,6 s),
           puis s'efface : le temps s'écoule, sans urgence criée. */
        .q-card.status-warning { border-left-color: #D9B98C !important; }
        .timer-badge.timer-soon { background: #F5EDDF !important; color: #7A4A12 !important; border: 1px solid #E3CFA3 !important; position: relative; overflow: hidden; }
        .timer-badge.timer-soon::after { content: ''; position: absolute; left: 0; bottom: 0; width: 100%; height: 2px; background: var(--cuivre); transform-origin: left; animation: a-sablier 2.6s var(--courbe) infinite; }
        @keyframes a-sablier { 0% { transform: scaleX(0); opacity: 1; } 72% { transform: scaleX(1); opacity: 1; } 100% { transform: scaleX(1); opacity: 0; } }

        /* ===================== A8 — À QUALIFIER : « ruban » =====================
           Bordure pointillée (attente) + reflet de ruban au survol uniquement :
           c'est le statut le plus nombreux, jamais d'animation automatique. */
        .q-card.status-aqual { border-style: dashed; border-left-style: solid !important; border-left-color: var(--attente) !important; }
        .q-card.status-aqual .q-date { color: var(--attente); font-style: italic; }
        .q-card.status-aqual::after { content: ''; position: absolute; inset: 0; border-radius: inherit; pointer-events: none; background: linear-gradient(115deg, transparent 42%, rgba(46,107,158,.12) 50%, transparent 58%); background-size: 260% 100%; background-position: 135% 0; }
        .q-card.status-aqual:hover::after { animation: a-ruban .75s var(--courbe-out); }
        @keyframes a-ruban { from { background-position: 135% 0; } to { background-position: -35% 0; } }

        /* ---- M1 : halo d'encre pour le flash de repérage (remplace le bleu
           de fond, qui était étouffé par les fonds papier des cartes à état) ---- */
        .op-flash { animation: a-flash 2s ease; }
        @keyframes a-flash { 0%, 100% { box-shadow: none; } 20%, 60% { box-shadow: inset 0 0 0 3px rgba(29,78,137,.45); } }
        @media (prefers-reduced-motion: reduce) { .q-card.status-expired.op-flash { animation: none !important; } }  /* cohérent avec les lignes */

        /* ---- Garde perf : au-delà de 40 cartes, les infinis d'état passent statiques ---- */
        body.motion-soft .q-card.status-critical::after, body.motion-soft .timer-badge.timer-expired, body.motion-soft .timer-badge.timer-soon::after { animation: none !important; }

        /* ---- Garde impression : aucune texture/animation sur le papier ---- */
        @media print {
            html, body { background: #fff !important; background-image: none !important; }
            .q-card::before, .q-card::after, .timer-badge::after, .state-standby .q-banner::before { display: none !important; }
            .q-card, .ech-row, .tl-row, .fiche-sheet, #tableBody tr { box-shadow: none !important; }
            .fiche-sheet { background: #fff !important; }
        }

        /* ===================== V8-4 — CONTRÔLES ÉCHÉANCES : gravure papier =====================
           Les bascules Liste/Timeline, fenêtres et filtres passent en papier gravé
           (même famille que les onglets). L'état actif est piloté par le JS via les
           classes Tailwind existantes (bg-blue-600…) : on ne crée AUCUNE nouvelle
           classe d'activation pour ne pas désynchroniser les toggles — on redéfinit
           seulement leur rendu, en !important, par ID. */
        #ech-modes, #ech-windows, #ech-filters { background: #EBE5D8 !important; border: 1px solid var(--filet) !important; border-radius: 4px !important; padding: 3px !important; }
        #ech-modes button, #ech-windows button, #ech-filters button {
            background: transparent !important; color: var(--encre-2) !important; border: none !important;
            border-radius: 3px !important; box-shadow: none !important; font-family: 'JetBrains Mono', Consolas, monospace;
            letter-spacing: .04em; transition: background .12s ease, color .12s ease;
        }
        #ech-modes button:hover, #ech-windows button:hover, #ech-filters button:hover { background: #DDD6C8 !important; }
        #btn-echm-list.bg-blue-600, #btn-echm-timeline.bg-blue-600, #btn-echw-3.bg-blue-600, #btn-echw-6.bg-blue-600, #btn-echw-12.bg-blue-600,
        #btn-ech-all.bg-blue-600, #btn-ech-expired.bg-blue-600, #btn-ech-7.bg-blue-600, #btn-ech-30.bg-blue-600, #btn-ech-90.bg-blue-600 {
            background: var(--plan) !important; color: #fff !important;
        }
        #ech-modes button.bg-blue-600:hover, #ech-windows button.bg-blue-600:hover, #ech-filters button.bg-blue-600:hover { background: #163F6F !important; }
        #btn-ech-csv, #btn-ech-print {
            font-family: 'JetBrains Mono', Consolas, monospace; font-size: 11px; font-weight: 900; text-transform: uppercase;
            letter-spacing: .06em; border-radius: 4px !important; padding: 8px 12px !important; transition: background .12s ease, transform .12s ease;
        }
        #btn-ech-csv { background: var(--surface) !important; color: var(--encre) !important; border: 1px solid var(--filet) !important; }
        #btn-ech-csv:hover { background: #E7E0D0 !important; }
        #btn-ech-print { background: var(--encre) !important; color: #fff !important; border: 1px solid var(--encre) !important; }
        #btn-ech-print:hover { background: #24303C !important; border-color: #24303C !important; }
        #btn-ech-csv:active, #btn-ech-print:active { transform: translateY(1px); }

        /* ===================== V8-2 — OPÉRATEUR « COMPLET » =====================
           Petit sceau sous l'indicateur quand tout est validé + tampon dédié
           (17 caractères : taille et ouverture réduites pour rester à l'écran). */
        .op-complet { display: inline-flex; align-items: center; gap: 4px; margin-top: 6px; padding: 2px 8px; border-radius: 999px; background: #E4EFE7; border: 1px solid #B7D8C3; color: #1D6B45; font-size: 9px; font-weight: 900; letter-spacing: .12em; font-family: 'JetBrains Mono', Consolas, monospace; }
        .stamp-complete { color: var(--valide); }
        .state-stamp.stamp-complete { font-size: 26px; letter-spacing: .06em; }
        .state-stamp.stamp-complete.play { animation: stampInComplete .55s cubic-bezier(.2, 1.4, .4, 1) forwards; }
        @keyframes stampInComplete {
            0% { opacity: 0; transform: translate(-50%, -50%) rotate(-14deg) scale(1.7); }
            55% { opacity: 1; transform: translate(-50%, -50%) rotate(-14deg) scale(1); }
            100% { opacity: .9; transform: translate(-50%, -50%) rotate(-14deg) scale(1); }
        }

        /* ---- V8-3 : feuille des échéances — masquée à l'écran, imprimable seule ---- */
        #ech-print { display: none; }
        @media print {
            /* flux exclusif : la classe body « print-ech » ne coexiste jamais avec « print-fiche »
               (chaque fonction retire la classe de l'autre) — ici, seuls #ech-print vit. */
            body.print-ech > *:not(#ech-print) { display: none !important; }
            body.print-ech > #ech-print { display: block !important; background: #fff; color: #17212B; padding: 0; font-family: 'JetBrains Mono', Consolas, monospace; }
            body.print-ech #fiche-print { display: none !important; }   /* au cas où une fiche serait restée ouverte */
            #ech-print .ep-head { display: flex; justify-content: space-between; align-items: flex-end; gap: 12px; border-bottom: 3px solid #17212B; padding-bottom: 10px; margin-bottom: 14px; }
            #ech-print .ep-title { font-weight: 900; text-transform: uppercase; font-size: 17px; letter-spacing: -.02em; }
            #ech-print .ep-sub { font-size: 11px; font-weight: 800; color: #64748B; text-transform: uppercase; letter-spacing: .08em; }
            #ech-print .ep-meta { font-size: 11px; font-weight: 800; color: #64748B; text-align: right; line-height: 1.6; }
            #ech-print .ep-table { width: 100%; border-collapse: collapse; font-size: 11px; }
            #ech-print .ep-table th { text-align: left; font-size: 10px; text-transform: uppercase; letter-spacing: .08em; border-bottom: 2px solid #17212B; padding: 6px 8px; }
            #ech-print .ep-table td { border-bottom: 1px solid #DDD6C8; padding: 6px 8px; font-weight: 700; }
            #ech-print .ep-table .c { text-align: center; white-space: nowrap; }
            #ech-print .ep-table tbody tr { page-break-inside: avoid; }
            #ech-print .etat-echue { color: #B42318; font-weight: 900; }
            #ech-print .etat-valide { color: #1D6B45; font-weight: 900; }
            #ech-print .ep-foot { margin-top: 14px; font-size: 10px; font-weight: 700; color: #94A3B8; text-align: right; }
        }

        /* ===================== V9 — REMISE EN QUESTION : zones restantes ===================== */

        /* ---- Filtres opérateurs (programme / ligne / secteur / équipe) — gravure papier.
               Même motif que #ech-filters : classes propres par préfixe d'ID, l'état actif
               reste la classe déjà basculée par setBtnActive (bg-blue-600) — aucune classe
               d'activation inventée, aucun attribut HTML modifié. ---- */
        [id^="btn-prog-"], [id^="btn-zone-"], [id^="btn-secteur-"], [id^="btn-team-"] {
            border: 1px solid var(--filet) !important;
            border-radius: var(--r) !important;
            background: var(--surface) !important;
            transition: background var(--d1) var(--courbe), color var(--d1) var(--courbe), border-color var(--d1) var(--courbe);
        }
        [id^="btn-prog-"]:not(.bg-blue-600), [id^="btn-zone-"]:not(.bg-blue-600),
        [id^="btn-secteur-"]:not(.bg-blue-600), [id^="btn-team-"]:not(.bg-blue-600) {
            color: var(--encre-2) !important;
        }
        [id^="btn-prog-"]:not(.bg-blue-600):hover, [id^="btn-zone-"]:not(.bg-blue-600):hover,
        [id^="btn-secteur-"]:not(.bg-blue-600):hover, [id^="btn-team-"]:not(.bg-blue-600):hover {
            background: var(--papier) !important;
        }
        [id^="btn-prog-"].bg-blue-600, [id^="btn-zone-"].bg-blue-600,
        [id^="btn-secteur-"].bg-blue-600, [id^="btn-team-"].bg-blue-600 {
            background: var(--plan) !important;
            color: #fff !important;
            border-color: #123A68 !important;
        }

        /* ---- Bandeau « Aujourd'hui » — papier, filet cuivre. Les DEUX états restent
               lisibles : l'état « rien d'urgent » garde sa teinte verte (className
               bg-emerald-50 posée par renderTodayBanner — classe déjà toggles).
               Les chips rouge/ambre conservent leurs couleurs sémantiques. ---- */
        #today-banner {
            border-radius: var(--r) !important;
            background: var(--papier) !important;
            border: 1px solid var(--filet) !important;
            border-left: 3px solid var(--cuivre) !important;
            box-shadow: none !important;
        }
        #today-banner.bg-emerald-50 {
            background: #F1F5EF !important;
            border-color: #C6D4C2 !important;
            border-left: 3px solid #6E9A6A !important;
        }
        #today-banner button.bg-amber-100 {          /* « Voir les échues » */
            background: var(--surface) !important;
            border-color: var(--filet) !important;
            color: var(--encre) !important;
        }
        #today-banner button.bg-amber-100:hover { background: var(--papier) !important; }

        /* ---- Chrome des modales — papier gravé (même précédent que .modal-panel,
               déjà accepté : seuls les éléments de chrome sont retokenisés,
               .modal-body reste inchangé pour ne rien casser aux vues Direction). ---- */
        .modal-head {
            background: var(--papier) !important;
            border-bottom: 1px solid var(--filet) !important;
        }
        .modal-title {
            color: var(--encre) !important;
            font-family: 'JetBrains Mono', Consolas, monospace !important;
            letter-spacing: .02em !important;
        }
        .modal-foot {
            background: var(--papier) !important;
            border-top: 1px solid var(--filet) !important;
        }

        /* ==== V10 — MOBILE (téléphone ~390px) : cibles tactiles + timeline ====
           Couche minérale posée PAR-DESSUS le reste (aucune règle existante
           n'est modifiée) : uniquement @media (max-width:480px), donc le
           bureau (≥481px) est strictement inchangé. */
        @media (max-width: 480px) {
            /* Onglets : hauteur tactile 44px (guides Apple/Google) */
            #tab-bar button { min-height: 44px; }
            /* Compteurs cliquables (échues / sous 7j / ...) */
            .cnt-badge { min-height: 44px; padding: 8px 14px; }
            /* Bouton rapide des lignes échéances + fermeture modales */
            .ech-fast { width: 40px; height: 40px; }
            .modal-close { width: 40px; height: 40px; }
            /* Micro-boutons par opérateur (+, ✍, ↔) */
            #tableBody button { min-width: 40px; min-height: 40px; }
            /* Boutons d'en-tête (aide, gestion, PIN) : 40 → 44 */
            header button.w-10 { width: 44px; height: 44px; }
            /* Timeline Échéances : noms 148px → 90px + défilement horizontal
               (aujourd'hui overflow-x:hidden écrêtait les mois à 390px) */
            .tl-name { width: 90px; }
            .tl-months { margin-left: 90px; }
            .tl-scroll { overflow-x: auto; }
            /* Modale Brouillons : zone de texte confortable */
            #br-text { min-height: 140px; }
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">
    <header class="bg-slate-900 text-white sticky top-0 z-50 shadow-md py-3 lg:h-20 flex flex-col justify-center px-4 lg:px-6">
        <div class="max-w-[1920px] mx-auto w-full flex flex-wrap items-center justify-between gap-y-3">
            <div class="flex items-center gap-3">
                <div class="bg-blue-600 w-9 h-9 lg:w-10 lg:h-10 rounded-lg flex items-center justify-center shadow-lg shadow-blue-500/20"><i class="fa-solid fa-plane-up text-lg lg:text-xl"></i></div>
                <div>
                    <h1 class="text-lg lg:text-xl font-black uppercase tracking-tight leading-tight">Planing QA <span class="text-blue-400">Sliman</span></h1>
                    <p class="text-[9px] lg:text-[10px] text-slate-400 uppercase tracking-widest font-bold hidden sm:block">Pilotage Opérationnel · P40 · P50 · P28</p>
                </div>
            </div>

            <button id="btn-validated-modal" onclick="openValidatedModal()" class="flex items-center bg-slate-800 border border-slate-700 px-3 lg:px-6 py-2 rounded-lg gap-2 lg:gap-4 hover:bg-slate-700 transition-colors shadow-sm ml-auto sm:ml-0">
                <div class="w-2 h-2 rounded-full bg-emerald-500 shadow-[0_0_8px_#10B981]"></div>
                <span class="hidden sm:inline text-xs font-bold uppercase text-slate-300">Validations</span>
                <span id="global-counter" class="text-lg lg:text-xl font-black text-emerald-400 mono">0</span>
            </button>

            <div class="flex items-center gap-2 lg:gap-3 w-full sm:w-auto order-last sm:order-none justify-between sm:justify-end">
                <div id="search-container" class="relative flex-grow sm:flex-grow-0 z-50">
                    <i class="fa-solid fa-search absolute left-3 top-1/2 -translate-y-1/2 text-slate-500 text-sm"></i>
                    <input type="text" id="searchInput" oninput="debouncedSearch()" placeholder="Rechercher..." class="pl-9 pr-8 py-2.5 sm:py-2 bg-slate-800 border border-slate-700 rounded-lg text-sm text-white focus:border-blue-500 focus:outline-none w-full sm:w-64 transition-all" autocomplete="off">
                    <button onclick="clearSearch()" id="clearSearchBtn" class="absolute right-3 top-1/2 -translate-y-1/2 text-slate-400 hover:text-white hidden"><i class="fa-solid fa-xmark"></i></button>
                    <ul id="searchResults" class="absolute top-full left-0 w-full mt-2 bg-white border border-slate-200 rounded-lg shadow-2xl hidden max-h-64 overflow-y-auto divide-y divide-slate-100 text-slate-800"></ul>
                </div>
                <div class="hidden lg:flex items-center bg-slate-800 border border-slate-700 rounded-lg overflow-hidden shadow-sm h-10">
                    <button onclick="zoomOut()" class="w-8 h-full flex items-center justify-center hover:bg-slate-700 text-slate-400 hover:text-white transition-colors" title="Réduire"><i class="fa-solid fa-minus text-xs"></i></button>
                    <span id="zoom-level" class="text-xs font-bold text-slate-300 w-10 text-center select-none">100%</span>
                    <button onclick="zoomIn()" class="w-8 h-full flex items-center justify-center hover:bg-slate-700 text-slate-400 hover:text-white transition-colors" title="Agrandir"><i class="fa-solid fa-plus text-xs"></i></button>
                </div>
                <div class="flex gap-2">
                    <button type="button" onclick="startTour()" title="Guide de démarrage" class="w-10 h-10 rounded-lg bg-blue-100 border border-blue-200 flex items-center justify-center text-blue-700 hover:bg-blue-200 shadow-sm"><i class="fa-solid fa-question text-lg"></i></button>
                    <button onclick="openManageModal()" title="Gérer les opérateurs" class="w-10 h-10 rounded-lg bg-slate-800 border border-slate-700 flex items-center justify-center hover:bg-slate-700 text-slate-300"><i class="fa-solid fa-users-gear"></i></button>
                    <button onclick="openPinModal()" title="Code de verrouillage" class="w-10 h-10 rounded-lg bg-slate-900 border border-slate-800 flex items-center justify-center hover:bg-slate-800 text-slate-600 hover:text-blue-400"><i class="fa-solid fa-code"></i></button>
                </div>
            </div>
        </div>
    </header>

    <main class="flex-grow p-3 sm:p-4 lg:p-6 overflow-x-hidden flex flex-col max-w-[1920px] mx-auto w-full">

        <!-- D1 : compteurs globaux cliquables (filtrent le tableau opérateurs) -->
        <div id="status-counters" class="flex flex-wrap items-center gap-2 mb-3 no-print">
            <button id="cnt-expired" onclick="setStatusFilter('expired')" class="cnt-badge cnt-expired" title="Qualifications échues (date passée), toutes équipes confondues — cliquer pour filtrer les opérateurs concernés"><i class="fa-solid fa-triangle-exclamation"></i><span class="cnt-n" id="cnt-expired-n">0</span>Échues</button>
            <button id="cnt-soon" onclick="setStatusFilter('soon')" class="cnt-badge cnt-soon" title="Qualifications qui expirent dans 7 jours ou moins, toutes équipes confondues — cliquer pour filtrer"><i class="fa-solid fa-fire"></i><span class="cnt-n" id="cnt-soon-n">0</span>Sous 7 j</button>
            <button id="cnt-aqual" onclick="setStatusFilter('aqual')" class="cnt-badge cnt-aqual" title="Qualifications sans date (à qualifier), toutes équipes confondues — cliquer pour filtrer"><i class="fa-solid fa-hourglass-half"></i><span class="cnt-n" id="cnt-aqual-n">0</span>À qualifier</button>
            <button id="cnt-validated" onclick="setStatusFilter('validated')" class="cnt-badge cnt-validated" title="Qualifications passées en Validée, toutes équipes confondues — cliquer pour filtrer"><i class="fa-solid fa-circle-check"></i><span class="cnt-n" id="cnt-validated-n">0</span>Validées</button>
            <button id="cnt-reset" onclick="resetAllFilters()" class="cnt-badge hidden" style="color:#475569" title="Réinitialiser tous les filtres (équipe + statut + recherche)"><i class="fa-solid fa-rotate-left"></i>Réinitialiser</button>
        </div>

        <div id="tab-bar" class="flex overflow-x-auto items-center gap-2 mb-4 pb-2 hide-scrollbar w-full whitespace-nowrap snap-x">
            <button onclick="switchTab('operators')" id="tab-operators" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-blue-600 text-white rounded-xl font-bold shadow-md text-sm flex items-center gap-2">
                <i class="fa-solid fa-users"></i> Suivi Opérateurs
            </button>
            <button onclick="switchTab('reporting')" id="tab-reporting" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-white text-slate-600 rounded-xl font-bold shadow-sm hover:bg-slate-50 border border-slate-200 text-sm flex items-center gap-2">
                <i class="fa-solid fa-chart-pie text-emerald-500"></i> KPI & Direction
            </button>
            <button onclick="switchTab('hebdo')" id="tab-hebdo" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-white text-slate-600 rounded-xl font-bold shadow-sm hover:bg-slate-50 border border-slate-200 text-sm flex items-center gap-2">
                <i class="fa-solid fa-calendar-week"></i> Résumé Hebdo
            </button>
            <button onclick="switchTab('echances')" id="tab-echances" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-white text-slate-600 rounded-xl font-bold shadow-sm hover:bg-slate-50 border border-slate-200 text-sm flex items-center gap-2">
                <i class="fa-solid fa-hourglass-half text-amber-500"></i> Échéances
            </button>
            <button onclick="switchTab('brouillons'); renderBrouillons();" id="tab-brouillons" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-white text-slate-600 rounded-xl font-bold shadow-sm hover:bg-slate-50 border border-slate-200 text-sm flex items-center gap-2">
                <i class="fa-solid fa-note-sticky text-rose-500"></i> Brouillons
            </button>
            <button onclick="switchTab('tuto')" id="tab-tuto" class="flex-shrink-0 snap-start px-4 sm:px-5 py-2.5 bg-white text-slate-600 rounded-xl font-bold shadow-sm hover:bg-slate-50 border border-slate-200 text-sm flex items-center gap-2 lg:ml-auto">
                <i class="fa-solid fa-book"></i> Procédures
            </button>
        </div>

        <!-- ONGLET 1: OPERATEURS -->
        <div id="view-operators" class="flex flex-col gap-4">
            <div id="filters-container" class="flex flex-col gap-3 bg-slate-50 p-3 rounded-xl border border-slate-200 shadow-sm w-full lg:w-fit">
                <div class="flex items-center overflow-x-auto hide-scrollbar gap-4 pb-1">
                    <div class="flex items-center gap-2 flex-shrink-0">
                        <span class="text-[10px] font-black text-slate-400 uppercase">Programme</span>
                        <div class="flex gap-1 bg-slate-200/50 p-1 rounded-lg">
                            <button onclick="setProgramme('A350')" id="btn-prog-A350" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">A350</button>
                            <button onclick="setProgramme('A330')" id="btn-prog-A330" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">A330</button>
                        </div>
                    </div>
                    <div class="flex items-center gap-2 flex-shrink-0 border-l border-slate-200 pl-4">
                        <span class="text-[10px] font-black text-slate-400 uppercase">Sous-section</span>
                        <div class="flex gap-1 bg-slate-200/50 p-1 rounded-lg">
                            <button onclick="setZone('P40')" id="btn-zone-P40" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">P40</button>
                            <button onclick="setZone('P50')" id="btn-zone-P50" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">P50</button>
                            <button onclick="setZone('P28')" id="btn-zone-P28" class="hidden px-3 sm:px-4 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">P28</button>
                        </div>
                    </div>
                    <div class="flex items-center gap-2 flex-shrink-0 border-l border-slate-200 pl-4">
                        <span class="text-[10px] font-black text-slate-400 uppercase">Ligne</span>
                        <div class="flex gap-1 bg-slate-200/50 p-1 rounded-lg">
                            <button onclick="setSecteur('A')" id="btn-secteur-A" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">A</button>
                            <button onclick="setSecteur('B')" id="btn-secteur-B" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">B</button>
                            <button onclick="setSecteur('C')" id="btn-secteur-C" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">C</button>
                        </div>
                    </div>
                    <div class="flex items-center gap-2 flex-shrink-0 border-l border-slate-200 pl-4 pr-2">
                        <span class="text-[10px] font-black text-slate-400 uppercase">Équipe</span>
                        <div class="flex gap-1 bg-slate-200/50 p-1 rounded-lg">
                            <button onclick="setTeam('A')" id="btn-team-A" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">Équipe A</button>
                            <button onclick="setTeam('B')" id="btn-team-B" class="px-3 sm:px-4 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">Équipe B</button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- D3 : bandeau « Aujourd'hui » (alertes globales nominales) -->
            <div id="today-banner" class="hidden rounded-xl border px-4 py-3 flex flex-col gap-2"></div>

            <div id="table-container" class="bg-transparent lg:bg-white lg:border lg:border-slate-200 overflow-visible lg:overflow-auto flex-grow rounded-xl lg:shadow-sm flex flex-col">
                <table class="w-full text-sm border-separate border-spacing-0">
                    <thead class="bg-slate-50 sticky top-0 z-10 border-b-2 border-slate-200 shadow-sm hidden lg:table-header-group">
                        <tr class="text-slate-500 uppercase font-black text-[11px] tracking-widest">
                            <th class="px-6 py-4 w-[15%] border-r-2 border-slate-200 text-left">Opérateur</th>
                            <th class="px-6 py-4 w-[78%] text-left">Cartographie des Qualifications</th>
                            <th class="px-4 py-4 w-[7%] border-l-2 border-slate-200 text-center">Indicateur</th>
                        </tr>
                    </thead>
                    <tbody id="tableBody" class="lg:divide-y-4 lg:divide-slate-200 block lg:table-row-group"></tbody>
                </table>
            </div>
        </div>

        <!-- ONGLET 2 : KPI & DIRECTION -->
        <div id="view-reporting" class="hidden flex-col gap-6">
            <div class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200 flex flex-col md:flex-row justify-between items-start md:items-center gap-4">
                <div>
                    <h2 class="text-xl font-black text-slate-800 uppercase tracking-tight">Tableau de Bord Direction</h2>
                    <p class="text-xs text-slate-500 font-medium">Visualisation consolidée P40 & P50</p>
                </div>
                <div class="flex bg-slate-100 p-1 rounded-lg border border-slate-200 w-full md:w-auto">
                    <button onclick="changeKpiView('Tout')" id="btn-kpi-Tout" class="flex-1 px-5 py-2 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">Tout</button>
                    <button onclick="changeKpiView('P40')" id="btn-kpi-P40" class="flex-1 px-5 py-2 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">P40</button>
                    <button onclick="changeKpiView('P50')" id="btn-kpi-P50" class="flex-1 px-5 py-2 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">P50</button>
                </div>
            </div>

            <div class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                <h3 class="text-sm font-black text-slate-800 uppercase tracking-widest mb-4 flex items-center gap-2">
                    <i class="fa-solid fa-users-viewfinder text-blue-500"></i> Performance par Validateur
                </h3>
                <div id="qls-table-container" class="overflow-x-auto flex justify-center pb-2"></div>
            </div>

            <div id="kpi-charts-wrapper" class="grid grid-cols-1 xl:grid-cols-2 gap-6">
                <div id="kpi-section-p40" class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200 flex flex-col">
                    <div class="flex justify-between items-center mb-4">
                        <h3 class="text-blue-600 font-black uppercase text-sm"><i class="fa-solid fa-industry mr-2"></i> Historique P40</h3>
                        <div class="text-center"><span class="block text-[10px] uppercase font-bold text-slate-400">Total Validations</span><span id="kpi-p40-total" class="text-lg font-black text-blue-700 mono">0</span><span id="kpi-p40-trend" class="block text-[10px] font-bold text-slate-400 mt-0.5"></span></div>
                    </div>
                    <div class="h-64"><canvas id="bossKpiChartP40"></canvas></div>
                </div>
                <div id="kpi-section-p50" class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200 flex flex-col">
                    <div class="flex justify-between items-center mb-4">
                        <h3 class="text-indigo-600 font-black uppercase text-sm"><i class="fa-solid fa-gears mr-2"></i> Historique P50</h3>
                        <div class="text-center"><span class="block text-[10px] uppercase font-bold text-slate-400">Total Validations</span><span id="kpi-p50-total" class="text-lg font-black text-indigo-700 mono">0</span><span id="kpi-p50-trend" class="block text-[10px] font-bold text-slate-400 mt-0.5"></span></div>
                    </div>
                    <div class="h-64"><canvas id="bossKpiChartP50"></canvas></div>
                </div>
            </div>

            <div class="bg-white rounded-2xl shadow-sm border border-slate-200 overflow-hidden flex flex-col">
                <div class="p-5 border-b border-slate-200 bg-slate-800 text-white flex flex-col sm:flex-row justify-between items-start sm:items-center gap-3">
                    <div>
                        <h3 class="text-base font-black uppercase tracking-widest"><i class="fa-solid fa-table-list text-blue-400 mr-2"></i> Registre Officiel des Validations</h3>
                        <p class="text-[10px] text-slate-400 font-medium mt-1">Généré automatiquement ou via l'ajout manuel.</p>
                    </div>
                    <div class="flex gap-2">
                        <button onclick="openManualLogModal()" class="bg-blue-600 hover:bg-blue-500 text-white px-3 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-plus"></i> Ajout Manuel</button>
                        <button onclick="exportBossCSV()" class="bg-emerald-600 hover:bg-emerald-500 text-white px-3 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-file-excel"></i> Exporter CSV</button>
                    </div>
                </div>
                <div class="px-5 py-3 bg-slate-50 border-b border-slate-200 flex flex-wrap items-center gap-3 no-print">
                    <div class="flex items-center gap-2">
                        <span class="text-[10px] font-black text-slate-400 uppercase">Validée par</span>
                        <select id="reg-validator-filter" onchange="renderReporting()" class="form-input" style="width:170px;padding:6px 8px"><option value="">Tous</option></select>
                    </div>
                    <div class="flex items-center gap-2 flex-grow min-w-[180px]">
                        <i class="fa-solid fa-search text-slate-400 text-xs"></i>
                        <input id="reg-search-filter" oninput="debouncedRegSearch()" placeholder="Filtrer (QA, compagnon, station...)" class="form-input" style="padding:6px 8px" autocomplete="off">
                    </div>
                    <span id="reg-count" class="text-[10px] font-black text-slate-400"></span>
                </div>
                <div class="overflow-x-auto max-h-[500px] border-b border-slate-200">
                    <table class="w-full text-[11px] text-left border-collapse excel-table">
                        <thead class="bg-slate-800 text-white font-bold uppercase tracking-wider sticky top-0 z-10 shadow-sm">
                            <tr>
                                <th class="px-4 py-3 border-r border-slate-700">Poste</th><th class="px-4 py-3 border-r border-slate-700">Station</th><th class="px-4 py-3 border-r border-slate-700">Nom de la QA</th><th class="px-4 py-3 border-r border-slate-700">Nom du Compagnon</th><th class="px-4 py-3 border-r border-slate-700">Init / Proro</th><th class="px-4 py-3 border-r border-slate-700 text-center">QLS1/QLS2</th><th class="px-4 py-3 border-r border-slate-700">Validée Par</th><th class="px-4 py-3 border-r border-slate-700 text-center">Date Val. QA</th><th class="text-center border-r border-slate-700">QCM / Com.</th><th class="text-center">CW</th>
                            </tr>
                        </thead>
                        <tbody id="boss-registry-tbody" class="bg-white divide-y divide-slate-200 text-slate-800 font-medium"></tbody>
                    </table>
                </div>
            </div>
        </div>

        <!-- ONGLET 3 : RÉSUMÉ HEBDO -->
        <div id="view-hebdo" class="hidden bg-white border border-slate-200 overflow-x-hidden overflow-y-auto flex-grow rounded-xl shadow-sm flex flex-col p-4 sm:p-6">
            <div class="flex flex-wrap justify-between items-center gap-3 mb-4 no-print">
                <h2 class="text-lg font-black uppercase tracking-tight text-slate-800"><i class="fa-solid fa-calendar-week text-blue-500 mr-2"></i>Résumé Hebdomadaire</h2>
                <div class="flex gap-2">
                    <button onclick="copyHebdo()" class="bg-slate-800 hover:bg-slate-700 text-white px-3 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-copy"></i> Copier le résumé</button>
                    <button onclick="window.print()" class="bg-slate-100 hover:bg-slate-200 text-slate-700 px-3 py-2 rounded-lg text-xs font-black uppercase border border-slate-300 flex items-center gap-2"><i class="fa-solid fa-print"></i> Imprimer</button>
                </div>
            </div>
            <div id="hebdo-container" class="flex flex-col gap-6 w-full"></div>
        </div>

        <!-- ONGLET 4 : ÉCHÉANCES (F1) -->
        <div id="view-echances" class="hidden flex flex-col gap-4">
            <div class="bg-white p-4 sm:p-5 rounded-2xl shadow-sm border border-slate-200 flex flex-col md:flex-row justify-between items-start md:items-center gap-3">
                <div>
                    <h2 class="text-lg sm:text-xl font-black text-slate-800 uppercase tracking-tight"><i class="fa-solid fa-hourglass-half text-amber-500 mr-2"></i>Prochaines Échéances</h2>
                    <p class="text-xs text-slate-500 font-medium">Toutes les prorogations datées, de la plus proche à la plus lointaine — <span class="font-bold">clique une ligne</span> pour agir sur la qualification.</p>
                </div>
                <div class="flex flex-wrap gap-2 items-center no-print">
                    <div class="flex bg-slate-100 p-1 rounded-lg border border-slate-200" id="ech-modes">
                        <button onclick="setEchViewMode('list')" id="btn-echm-list" class="px-3 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm"><i class="fa-solid fa-list mr-1"></i>Liste</button>
                        <button onclick="setEchViewMode('timeline')" id="btn-echm-timeline" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200"><i class="fa-solid fa-chart-gantt mr-1"></i>Timeline</button>
                    </div>
                    <div class="flex bg-slate-100 p-1 rounded-lg border border-slate-200 hidden" id="ech-windows">
                        <button onclick="setEchWindow(3)" id="btn-echw-3" class="px-3 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">3 mois</button>
                        <button onclick="setEchWindow(6)" id="btn-echw-6" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">6 mois</button>
                        <button onclick="setEchWindow(12)" id="btn-echw-12" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">12 mois</button>
                    </div>
                    <div class="flex bg-slate-100 p-1 rounded-lg border border-slate-200" id="ech-filters">
                        <button onclick="setEchanceFilter('all')" id="btn-ech-all" class="px-3 py-1.5 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm">Tout</button>
                        <button onclick="setEchanceFilter('expired')" id="btn-ech-expired" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">Échues</button>
                        <button onclick="setEchanceFilter('7')" id="btn-ech-7" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">≤ 7 j</button>
                        <button onclick="setEchanceFilter('30')" id="btn-ech-30" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">≤ 30 j</button>
                        <button onclick="setEchanceFilter('90')" id="btn-ech-90" class="px-3 py-1.5 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200">≤ 90 j</button>
                    </div>
                    <button id="btn-ech-print" onclick="printEcheancesListe()" title="Imprimer la liste filtrée pour le tableau de l'atelier"><i class="fa-solid fa-print mr-1"></i> Imprimer la liste</button>
                    <button id="btn-ech-csv" onclick="exportEcheancesCSV()" title="Exporter la liste filtrée en CSV"><i class="fa-solid fa-file-csv mr-1"></i> Export CSV</button>
                </div>
            </div>
            <div id="echances-list" class="flex flex-col gap-1.5"></div>
            <div id="ech-timeline" class="hidden flex flex-col gap-3"></div>
        </div>

        <!-- ONGLET 6 : BROUILLONS (cahier de texte — notes + photos) -->
        <div id="view-brouillons" class="hidden flex flex-col gap-4">
            <div class="bg-white border border-slate-200 rounded-xl shadow-sm p-4 flex flex-col gap-3">
                <div class="flex flex-wrap items-center justify-between gap-3">
                    <div>
                        <h2 class="text-base sm:text-lg font-black text-slate-800 uppercase tracking-tight"><i class="fa-solid fa-note-sticky text-rose-500 mr-2"></i>Brouillons — cahier de texte</h2>
                        <p class="text-[10px] font-bold text-slate-400 mt-1">Notes libres et extraits (photos) rangés sur CE POSTE — hors des qualifications.</p>
                    </div>
                    <div class="flex items-center gap-2 flex-wrap">
                        <input id="br-search" oninput="renderBrouillons()" placeholder="Rechercher…" class="form-input" style="width:150px; padding:8px 10px; font-size:12px;">
                        <button onclick="newBrouillon()" class="px-4 py-2.5 rounded-lg text-xs font-black bg-blue-600 text-white hover:bg-blue-500 shadow-md flex items-center gap-2"><i class="fa-solid fa-plus"></i> Nouvelle note</button>
                    </div>
                </div>
                <div id="brouillons-list" class="flex flex-col gap-2"></div>
            </div>
        </div>

        <!-- ONGLET 5 : TUTO -->
        <div id="view-tuto" class="hidden bg-slate-50 border border-slate-200 overflow-x-hidden overflow-y-auto flex-grow rounded-xl shadow-inner flex flex-col p-4 sm:p-6 lg:p-8 gap-8">
            <div class="text-center max-w-3xl mx-auto bg-white p-6 rounded-2xl shadow-sm border border-slate-200 relative overflow-hidden w-full">
                <div class="absolute top-0 left-0 w-full h-2 bg-gradient-to-r from-blue-500 via-blue-400 to-emerald-400"></div>
                <h2 class="text-2xl sm:text-3xl font-black text-slate-800 uppercase tracking-tight mt-2"><i class="fa-solid fa-route text-blue-500 mr-3"></i>Centre de Procédures QA</h2>
            </div>
            <div class="flex flex-col items-center w-full bg-white p-4 rounded-2xl shadow-sm border border-slate-200">
                <img src="arbre.jpg" alt="Organigramme" class="max-w-full h-auto rounded-lg shadow-inner" onerror="this.onerror=null; this.src='data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 width=%22800%22 height=%22400%22%3E%3Crect width=%22800%22 height=%22400%22 fill=%22%23f8fafc%22/%3E%3Ctext x=%22400%22 y=%22195%22 font-family=%22sans-serif%22 font-size=%2222%22 font-weight=%22bold%22 fill=%22%23ef4444%22 text-anchor=%22middle%22%3EIMAGE arbre.jpg INTROUVABLE%3C/text%3E%3Ctext x=%22400%22 y=%22230%22 font-family=%22sans-serif%22 font-size=%2214%22 fill=%22%2364748b%22 text-anchor=%22middle%22%3EDépose arbre.jpg à côté du fichier HTML%3C/text%3E%3C/svg%3E';">
                <p class="text-[11px] font-bold text-slate-400 mt-3 text-center">Pour afficher l'organigramme : dépose le fichier <b>arbre.jpg</b> dans le même dossier que ce fichier HTML.</p>
                <p class="text-[10px] text-slate-400 mt-4 text-center border-t border-slate-100 pt-3">Version du 23 octobre 2026 · Semaine 43</p>
            </div>
        </div>
    </main>
    <!-- ===== MODALES ===== -->
    <div id="tour-overlay" class="tour-overlay" onclick="endTour()"></div>
    <div id="tour-focus-box" class="tour-focus-box"></div>
    <div id="tour-dialog" class="tour-dialog">
        <h3 id="tour-title" class="font-black text-blue-600 mb-3 text-lg"></h3>
        <p id="tour-text" class="text-sm text-slate-600 mb-6 leading-relaxed font-medium"></p>
        <div class="flex justify-between items-center mt-4 border-t border-slate-100 pt-4">
            <span id="tour-step-counter" class="text-xs font-bold text-slate-400 bg-slate-100 px-2 py-1 rounded"></span>
            <div class="flex gap-2">
                <button type="button" onclick="endTour()" class="px-4 py-2 text-xs font-bold text-slate-500">Quitter</button>
                <button type="button" onclick="nextTourStep()" id="tour-next-btn" class="px-5 py-2 bg-blue-600 text-white text-xs font-black rounded-lg">Suivant</button>
            </div>
        </div>
    </div>

    <!-- Modale : liste des validations -->
    <div id="validated-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:680px">
            <div class="modal-head">
                <div>
                    <span class="modal-title"><i class="fa-solid fa-circle-check text-emerald-500 mr-2"></i>Registre des Validations Opérateurs</span>
                    <div id="validated-counter" class="text-[10px] font-bold text-slate-400 mt-1"></div>
                </div>
                <button class="modal-close" onclick="closeModal('validated-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body p-0"><div id="validated-list" class="divide-y divide-slate-100 max-h-[60vh] overflow-y-auto"></div></div>
            <div class="modal-foot"><button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('validated-modal')">Fermer</button></div>
        </div>
    </div>

    <!-- Modale : actions sur une qualification (clic carte) -->
    <div id="card-modal" class="modal-backdrop">
        <div class="modal-panel">
            <div class="modal-head">
                <div>
                    <span class="modal-title" id="card-modal-title">QUALIFICATION</span>
                    <div id="card-modal-sub" class="text-[10px] font-bold text-slate-400 mt-1"></div>
                </div>
                <button class="modal-close" onclick="closeModal('card-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-4">
                <div>
                    <label class="form-label">Statut de la qualification</label>
                    <div class="flex flex-wrap gap-2" id="card-state-buttons">
                        <button type="button" data-state="normal" onclick="setCardState('normal')" class="state-btn">Normal</button>
                        <button type="button" data-state="validated" onclick="setCardState('validated')" class="state-btn">✔ Validée</button>
                        <button type="button" data-state="priority" onclick="setCardState('priority')" class="state-btn">Priorité</button>
                        <button type="button" data-state="standby" onclick="setCardState('standby')" class="state-btn">Standby</button>
                        <button type="button" data-state="disabled" onclick="setCardState('disabled')" class="state-btn">Pas capable</button>
                    </div>
                </div>
                <div><label class="form-label">Date d'échéance</label>
                    <div class="flex gap-2">
                        <input type="date" id="card-date" class="form-input" style="flex-grow">
                        <button type="button" onclick="quickDate('card-date', 1)" class="px-3 rounded-lg text-[10px] font-black bg-slate-100 hover:bg-blue-100 text-slate-600 border border-slate-200 whitespace-nowrap" title="Reporter d'un an">+1 an</button>
                        <button type="button" onclick="quickDate('card-date', 2)" class="px-3 rounded-lg text-[10px] font-black bg-slate-100 hover:bg-blue-100 text-slate-600 border border-slate-200 whitespace-nowrap" title="Reporter de deux ans">+2 ans</button>
                    </div>
                </div>
                <div><label class="form-label">Validateur / QLS</label><select id="card-validator" class="form-input"><option value="">—</option></select></div>
                <div><label class="form-label">Note</label><textarea id="card-note" rows="3" class="form-input" placeholder="Remarque, blocage, contre-observation..."></textarea></div>
                <div class="text-[10px] text-slate-400 font-bold"><i class="fa-solid fa-circle-info mr-1"></i>Une qualification passée en « Validée » alimente le compteur du bandeau et l'onglet KPI.</div>
            </div>
            <div class="modal-foot justify-between">
                <button onclick="deleteQualif()" class="px-4 py-2 rounded-lg text-xs font-black bg-red-50 text-red-600 hover:bg-red-100"><i class="fa-solid fa-trash mr-1"></i>Supprimer</button>
                <div class="flex gap-2">
                    <button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('card-modal')">Annuler</button>
                    <button onclick="saveCardModal()" class="px-5 py-2 rounded-lg text-xs font-black bg-blue-600 text-white hover:bg-blue-500 shadow-md">Enregistrer</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modale : ajouter une qualification à un opérateur -->
    <div id="addqualif-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:480px">
            <div class="modal-head">
                <span class="modal-title"><i class="fa-solid fa-plus text-blue-500 mr-2"></i>Ajouter une qualification</span>
                <button class="modal-close" onclick="closeModal('addqualif-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-4">
                <div id="addqualif-op" class="text-xs font-black uppercase text-slate-700 bg-slate-100 rounded-lg p-3 border border-slate-200"></div>
                <div><label class="form-label">Code - Intitulé</label><input id="aq-code" list="qualifs-codes" class="form-input mono" placeholder="BSC0S00-Serrage Meca"></div>
                <div class="grid grid-cols-2 gap-3">
                    <div><label class="form-label">Type</label><select id="aq-type" class="form-input"><option value="N">Prorogation (PRO)</option><option value="O">Initiale (INI)</option></select></div>
                    <div><label class="form-label">Échéance</label><input type="date" id="aq-date" class="form-input"></div>
                </div>
            </div>
            <div class="modal-foot justify-between">
                <span class="text-[10px] font-bold text-slate-400 self-center">Sans échéance = « À QUALIFIER »</span>
                <div class="flex gap-2">
                    <button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('addqualif-modal')">Annuler</button>
                    <button onclick="saveAddQualif()" class="px-5 py-2 rounded-lg text-xs font-black bg-blue-600 text-white hover:bg-blue-500 shadow-md">Ajouter</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modale : gestion opérateurs + historique -->
    <div id="manage-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:720px">
            <div class="modal-head">
                <span class="modal-title"><i class="fa-solid fa-users-gear text-slate-500 mr-2"></i>Gestion des opérateurs & historique</span>
                <button class="modal-close" onclick="closeModal('manage-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-5">
                <div>
                    <label class="form-label">Ajouter un opérateur</label>
                    <div class="flex gap-2">
                        <input id="op-new-name" class="form-input" placeholder="NOM Prénom" style="flex-grow">
                        <select id="op-new-team" class="form-input" style="width:140px"></select>
                        <button onclick="addOperator()" class="px-4 rounded-lg text-xs font-black bg-blue-600 text-white hover:bg-blue-500"><i class="fa-solid fa-plus mr-1"></i>Ajouter</button>
                    </div>
                </div>
                <div>
                    <label class="form-label">Opérateurs (renommer / changer d'équipe / supprimer)</label>
                    <div id="manage-op-list" class="flex flex-col gap-2 max-h-[36vh] overflow-y-auto pr-1"></div>
                </div>
                <div>
                    <label class="form-label">Historique des sauvegardes automatiques</label>
                    <div id="manage-history" class="flex flex-col gap-1 max-h-[16vh] overflow-y-auto pr-1"></div>
                </div>
                <div>
                    <label class="form-label">Corbeille (opérateurs supprimés)</label>
                    <div id="manage-trash" class="flex flex-col gap-1 max-h-[14vh] overflow-y-auto pr-1"></div>
                </div>
                <div class="bg-blue-50 border border-blue-200 rounded-xl p-3">
                    <label class="form-label text-blue-700"><i class="fa-solid fa-floppy-disk mr-1"></i>Sauvegarde & Restauration</label>
                    <p class="text-[10px] font-bold text-blue-700/80 mb-2">Les données vivent sur CE poste uniquement. Exporte un fichier .json régulièrement (clef USB, mail) et pour transférer vers un autre PC.</p>
                    <div class="flex gap-2 flex-wrap">
                        <button onclick="exportBackupJSON()" class="bg-emerald-600 hover:bg-emerald-500 text-white px-3 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-download"></i> Exporter (.json)</button>
                        <button onclick="document.getElementById('import-file').click()" class="bg-slate-800 hover:bg-slate-700 text-white px-3 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-upload"></i> Importer (.json)</button>
                        <input type="file" id="import-file" accept=".json,application/json" class="hidden" onchange="importBackupJSON(this)">
                    </div>
                </div>
            </div>
            <div class="modal-foot"><button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('manage-modal')">Fermer</button></div>
        </div>
    </div>

    <!-- Modale : code PIN -->
    <div id="pin-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:360px">
            <div class="modal-head">
                <span class="modal-title" id="pin-title">Code de verrouillage</span>
                <button class="modal-close" onclick="closeModal('pin-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-3">
                <p id="pin-help" class="text-xs text-slate-500 font-medium leading-relaxed"></p>
                <div id="pin-set-block" class="flex flex-col gap-3">
                    <div><label class="form-label">Nouveau code (4 caractères min.)</label><input type="password" id="pin-new" class="form-input mono" autocomplete="new-password"></div>
                    <div><label class="form-label">Confirmer le code</label><input type="password" id="pin-new2" class="form-input mono" autocomplete="new-password"></div>
                </div>
                <div id="pin-check-block" class="flex flex-col gap-3 hidden">
                    <div><label class="form-label">Code PIN</label><input type="password" id="pin-enter" class="form-input mono" autocomplete="current-password" onkeydown="if(event.key==='Enter')submitPin()"></div>
                </div>
                <button onclick="removePin()" id="pin-remove-btn" class="hidden text-[11px] font-bold text-red-500 text-left hover:underline"><i class="fa-solid fa-lock-open mr-1"></i>Supprimer le code PIN (ouvrir les modifications à tous)</button>
            </div>
            <div class="modal-foot justify-between">
                <button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('pin-modal')">Annuler</button>
                <button onclick="pinPrimaryAction()" id="pin-primary" class="px-5 py-2 rounded-lg text-xs font-black bg-slate-900 text-white hover:bg-slate-700">Valider</button>
            </div>
        </div>
    </div>

    <!-- Modale : ajout manuel au registre KPI -->
    <div id="manual-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:560px">
            <div class="modal-head">
                <span class="modal-title"><i class="fa-solid fa-pen-to-square text-blue-500 mr-2"></i>Ajout manuel d'une validation</span>
                <button class="modal-close" onclick="closeModal('manual-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body grid grid-cols-2 gap-3">
                <div><label class="form-label">Poste</label><select id="ml-poste" class="form-input"><option>P40</option><option>P50</option></select></div>
                <div><label class="form-label">Station</label><input id="ml-station" class="form-input" placeholder="P40A"></div>
                <div class="col-span-2"><label class="form-label">Nom de la QA</label><input id="ml-qualif" list="qualifs-codes" class="form-input mono" placeholder="BSC0S00 Serrage au couple Meca"></div>
                <div class="col-span-2"><label class="form-label">Nom du Compagnon</label><input id="ml-compagnon" list="operators-names" class="form-input"></div>
                <div><label class="form-label">Type</label><select id="ml-type" class="form-input"><option>Initiale</option><option>Prorogation</option></select></div>
                <div><label class="form-label">QLS</label><select id="ml-qls" class="form-input"><option value="">—</option><option>QLS1</option><option>QLS2</option></select></div>
                <div><label class="form-label">Validée par</label><select id="ml-validateur" class="form-input"></select></div>
                <div><label class="form-label">Date de validation</label><input type="date" id="ml-date" class="form-input"></div>
                <div><label class="form-label">QCM / Commentaire</label><input id="ml-qcm" class="form-input" placeholder="Oui / Non / En attente"></div>
                <div><label class="form-label">Calendrier (CW)</label><input type="number" id="ml-cw" class="form-input"></div>
            </div>
            <div class="modal-foot justify-between">
                <span class="text-[10px] font-bold text-slate-400 self-center">Alimente le registre, les graphiques et le tableau validateur.</span>
                <div class="flex gap-2">
                    <button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('manual-modal')">Annuler</button>
                    <button onclick="saveManualLog()" class="px-5 py-2 rounded-lg text-xs font-black bg-emerald-600 text-white hover:bg-emerald-500 shadow-md">Enregistrer</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ===== V10 — MODALE BROUILLON (note + photo) ===== -->
    <div id="brouillon-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:520px">
            <div class="modal-head">
                <span class="modal-title" id="br-modal-title"><i class="fa-solid fa-pen-to-square text-rose-500 mr-2"></i>Nouvelle note</span>
                <button class="modal-close" onclick="closeModal('brouillon-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-3">
                <div><label class="form-label">Titre</label><input id="br-title" maxlength="80" placeholder="Ex : extrait procédure, consigne atelier…" class="form-input"></div>
                <div><label class="form-label">Note</label><textarea id="br-text" rows="5" maxlength="5000" placeholder="Ce que tu veux te rappeler…" class="form-input"></textarea></div>
                <div class="flex items-center gap-2 flex-wrap">
                    <button onclick="document.getElementById('br-file').click()" class="px-3 py-2 rounded-lg text-xs font-black bg-slate-100 text-slate-600 hover:bg-slate-200 border border-slate-200"><i class="fa-solid fa-camera mr-1"></i> Joindre une photo</button>
                    <button id="br-photo-del" onclick="removeBrouillonPhoto()" class="px-3 py-2 rounded-lg text-xs font-bold text-red-500 hover:bg-red-50 border border-red-100 hidden"><i class="fa-solid fa-xmark mr-1"></i> Retirer</button>
                    <span id="br-photo-name" class="text-[10px] font-bold text-slate-400"></span>
                    <input type="file" id="br-file" accept="image/*" class="hidden" onchange="addBrouillonPhoto(this)">
                </div>
                <img id="br-photo-preview" class="hidden" alt="Aperçu" style="max-width:100%; max-height:220px; border-radius:10px; border:1px solid #e2e8f0; object-fit:contain;">
                <div id="br-photo-err" class="hidden text-[11px] font-bold text-red-500"></div>
            </div>
            <div class="modal-foot justify-between">
                <button id="br-delete" onclick="deleteBrouillon()" class="px-4 py-2 rounded-lg text-xs font-black bg-red-50 text-red-600 hover:bg-red-100 hidden"><i class="fa-solid fa-trash mr-1"></i>Supprimer</button>
                <div class="flex gap-2">
                    <button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('brouillon-modal')">Annuler</button>
                    <button onclick="saveBrouillon()" class="px-5 py-2 rounded-lg text-xs font-black bg-blue-600 text-white hover:bg-blue-500 shadow-md">Enregistrer</button>
                </div>
            </div>
        </div>
    </div>

    <!-- ===== V10 — ÉCRAN DE VERROUILLAGE (code d'accès) =====
         Visible par défaut ; masqué dès le parse si la session de l'onglet
         est déjà ouverte → aucun flash au rechargement. -->
    <div id="access-lock" style="position:fixed; inset:0; z-index:10010; background:rgba(15,23,42,.72); display:flex; align-items:center; justify-content:center; padding:16px; backdrop-filter:blur(2px);">
        <div style="background:#fff; border-radius:16px; box-shadow:0 25px 60px rgba(15,23,42,.35); width:100%; max-width:360px; padding:28px 24px; text-align:center;">
            <i class="fa-solid fa-lock" style="font-size:34px; color:#2563eb;"></i>
            <div style="font-weight:900; font-size:17px; color:#0f172a; margin-top:10px;">Application verrouillée</div>
            <div style="font-size:12px; color:#64748b; font-weight:700; margin-top:4px;">Entre ton code d'accès pour continuer</div>
            <input id="access-code" type="password" inputmode="numeric" autocomplete="off" maxlength="4" placeholder="••••"
                   style="margin-top:18px; width:100%; font-size:26px; letter-spacing:14px; text-align:center; font-weight:900; padding:8px 4px; border:2px solid #cbd5e1; border-radius:10px; outline:none; font-family:'JetBrains Mono',Consolas,monospace; box-sizing:border-box;">
            <div id="access-msg" style="display:none; color:#dc2626; font-size:12px; font-weight:900; margin-top:8px;">Code incorrect — réessaie.</div>
            <button id="access-btn" style="margin-top:16px; width:100%; padding:13px; background:#2563eb; color:#fff; font-weight:900; border:none; border-radius:10px; font-size:14px; cursor:pointer;">Entrer</button>
            <div style="font-size:10px; color:#94a3b8; font-weight:700; margin-top:12px;">Verrouillage automatique à la fermeture de l'onglet.</div>
        </div>
    </div>
    <script>
        // Masquage immédiat (au parse) si session déjà ouverte ; essai de la saisie sinon.
        (function () {
            // V10 — les DEUX seules références du verrou, déclarées ICI (bloc le plus
            // tôt du fichier) : l'anti-flash s'exécute avant le script principal.
            var ACCESS_CODE = '2704';
            var ACCESS_SESSION_KEY = 'cockpit_qa_access_ok';
            function lockEl() { return document.getElementById('access-lock'); }
            try {
                if (sessionStorage.getItem(ACCESS_SESSION_KEY) === '1') { var l0 = lockEl(); if (l0) l0.style.display = 'none'; }
            } catch (e) { /* sessionStorage indisponible : l'écran reste, on peut saisir le code */ }
            function essayer() {
                var champ = document.getElementById('access-code');
                var msg = document.getElementById('access-msg');
                if (!champ) return;
                if (champ.value === ACCESS_CODE) {
                    try { sessionStorage.setItem(ACCESS_SESSION_KEY, '1'); } catch (e) {}
                    var l = lockEl(); if (l) l.style.display = 'none';
                    champ.value = '';
                    // Rappels différés du onload (guide première visite / sauvegarde)
                    if (typeof window.__apresAcces === 'function') { var f = window.__apresAcces; window.__apresAcces = null; f(); }
                } else {
                    if (msg) msg.style.display = 'block';
                    champ.value = ''; champ.focus();
                }
            }
            document.addEventListener('DOMContentLoaded', function () {
                var btn = document.getElementById('access-btn');
                var champ = document.getElementById('access-code');
                if (btn) btn.addEventListener('click', essayer);
                if (champ) {
                    champ.addEventListener('keydown', function (e) { if (e.key === 'Enter') { e.preventDefault(); essayer(); } });
                    champ.addEventListener('input', function () { var m = document.getElementById('access-msg'); if (m) m.style.display = 'none'; });
                    setTimeout(function () { try { champ.focus(); } catch (e) {} }, 60);
                }
            });
            window.__verrouActif = function () { var l = lockEl(); return !!l && l.style.display !== 'none'; };
        })();
    </script>

    <div id="toast-box" class="toast-box"></div>

    <!-- F5 : retour en haut -->
    <button id="back-to-top" onclick="window.scrollTo({top:0,behavior:'smooth'})" title="Retour en haut"><i class="fa-solid fa-arrow-up"></i></button>

    <!-- F2 : fiche opérateur imprimable (enfant direct du body → impression isolée) -->
    <div id="fiche-print">
        <div class="fiche-sheet" id="fiche-sheet"></div>
    </div>

    <!-- V8-3 : liste des échéances imprimable (enfant direct du body → impression isolée) -->
    <div id="ech-print"></div>

    <!-- F3 : aide des raccourcis clavier -->
    <div id="shortcuts-modal" class="modal-backdrop">
        <div class="modal-panel" style="max-width:460px">
            <div class="modal-head">
                <span class="modal-title"><i class="fa-solid fa-keyboard text-blue-500 mr-2"></i>Raccourcis Clavier</span>
                <button class="modal-close" onclick="closeModal('shortcuts-modal')" title="Fermer"><i class="fa-solid fa-xmark"></i></button>
            </div>
            <div class="modal-body flex flex-col gap-2">
                <div class="flex justify-between items-center bg-slate-50 rounded-lg px-3 py-2 border border-slate-200"><span class="text-xs font-bold text-slate-600">Aller aux onglets</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">1</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">2</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">3</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">4</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">5</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">6</span></div>
                <div class="flex justify-between items-center bg-slate-50 rounded-lg px-3 py-2 border border-slate-200"><span class="text-xs font-bold text-slate-600">Recherche instantanée</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">/</span></div>
                <div class="flex justify-between items-center bg-slate-50 rounded-lg px-3 py-2 border border-slate-200"><span class="text-xs font-bold text-slate-600">Cette aide</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">?</span></div>
                <div class="flex justify-between items-center bg-slate-50 rounded-lg px-3 py-2 border border-slate-200"><span class="text-xs font-bold text-slate-600">Fermer / quitter</span><span class="mono text-[11px] font-black bg-slate-800 text-white px-2 py-1 rounded">Échap</span></div>
                <div class="flex justify-between items-center bg-slate-50 rounded-lg px-3 py-2 border border-slate-200"><span class="text-xs font-bold text-slate-600">Ailleurs : clic sur une carte = actions, clic sur un compteur = filtre</span></div>
            </div>
            <div class="modal-foot"><button class="px-4 py-2 text-xs font-bold text-slate-500" onclick="closeModal('shortcuts-modal')">Fermer</button></div>
        </div>
    </div>

    <datalist id="qualifs-codes"></datalist>
    <datalist id="operators-names"></datalist>

    <!-- V7 : canvas confettis (sous les modales, non interactif) -->
    <canvas id="confetti-canvas" aria-hidden="true"></canvas>
    <!-- V7 : tampon d'état (au-dessus des modales, non interactif) -->
    <div id="state-stamp" class="state-stamp" aria-hidden="true"></div>

    <!-- Drag & drop : import d'une sauvegarde .json déposée n'importe où -->
    <div id="drop-overlay">
        <div class="drop-card">
            <i class="fa-solid fa-cloud-arrow-down text-4xl text-blue-500 mb-3"></i>
            <div class="text-lg font-black text-slate-800 uppercase">Dépose ta sauvegarde</div>
            <div class="text-xs font-bold text-slate-500 mt-1">Fichier <span class="mono">.json</span> exporté depuis Gestion ⚙️ (PIN requis à l'import)</div>
        </div>
    </div>

    <!-- ===== SCRIPT COMPLET ===== -->
    <script>
        var STORAGE_KEY = 'cockpit_qa_master_data_v45';
        var KPI_LOG_KEY = 'cockpit_boss_log_master_v45';
        var HISTORY_KEY = 'cockpit_qa_history_master';
        var CORBEILLE_KEY = 'cockpit_qa_corbeille_master';
        var PIN_KEY = 'cockpit_qa_pin_hash_v1';
        var ZOOM_KEY = 'cockpit_qa_zoom_v1';
        var UNLOCK_SESSION_KEY = 'cockpit_qa_unlock_session';
        // V10 — Brouillons (cahier de texte) : clé DÉDIÉE, jamais mélangée aux clés v45
        var BROUILLONS_KEY = 'cockpit_qa_brouillons_v1';
        // V10 — Verrou d'entrée : le code et sa clé de session sont déclarés dans le
        // script inline du verrou (bloc antérieur à celui-ci) — un seul endroit à changer.

        /* ---------- Utilitaires ---------- */
        function cleanName(text) { return text ? text.replace(/\s*\(.*?\)\s*/g, '').trim() : "QUALIFICATION"; }
        function sanitize(str) { if (!str) return ''; var t = document.createElement('div'); t.textContent = str; return t.innerHTML.replace(/"/g, '&quot;').replace(/'/g, '&#39;'); }
        // Teinte pastille déterministe (même couleur dans le tableau et sur la fiche imprimable)
        function opHue(nom) { var hues = ['bg-blue-500', 'bg-indigo-500', 'bg-emerald-500', 'bg-amber-500', 'bg-rose-500', 'bg-cyan-600', 'bg-violet-500']; return hues[(nom.charCodeAt(0) + nom.length) % hues.length]; }

        function getWeekNumber(d) {
            var date = new Date(Date.UTC(d.getFullYear(), d.getMonth(), d.getDate()));
            date.setUTCDate(date.getUTCDate() + 4 - (date.getUTCDay() || 7));
            var yearStart = new Date(Date.UTC(date.getUTCFullYear(), 0, 1));
            return Math.ceil((((date - yearStart) / 86400000) + 1) / 7);
        }

        function getQAWeekStartTimestamp() {
            var d = new Date();
            var day = d.getDay();
            var diff = (day <= 3) ? (7 - 3 + day) : (day - 3);
            d.setDate(d.getDate() - diff);
            d.setHours(23, 59, 59, 999);
            return d.getTime();
        }

        function getSafeStorageWithMigration(primaryKey, fallbackKeys, defaultVal) {
            var data = null;
            try { data = localStorage.getItem(primaryKey); } catch (e) { return defaultVal; }
            if (data) {
                try { return JSON.parse(data); } catch (e) { /* clé primaire corrompue : on tente les clés legacy */ }
            }
            for (var i = 0; i < fallbackKeys.length; i++) {
                try { data = localStorage.getItem(fallbackKeys[i]); } catch (e) { return defaultVal; }
                if (data) {
                    try { var parsed = JSON.parse(data); localStorage.setItem(primaryKey, data); return parsed; } catch (e) { /* legacy corrompu aussi */ }
                }
            }
            return defaultVal;
        }

        function getSafeStorage(key, defaultVal) {
            try { var item = localStorage.getItem(key); return item ? JSON.parse(item) : defaultVal; } catch (e) { return defaultVal; }
        }

        function openModal(id) { var m = document.getElementById(id); if (m) m.classList.add('open'); }
        function closeModal(id) { var m = document.getElementById(id); if (m) m.classList.remove('open'); }
        function closeAllModals() { document.querySelectorAll('.modal-backdrop.open').forEach(function (m) { m.classList.remove('open'); }); }

        function toast(msg, isErr, ms) {
            var box = document.getElementById('toast-box');
            if (!box) return null;
            var t = document.createElement('div');
            t.className = 'toast' + (isErr ? ' err' : '');
            t.innerHTML = msg;
            box.appendChild(t);
            var delay = ms || 2600;
            setTimeout(function () { t.style.opacity = '0'; t.style.transition = 'opacity 0.3s'; setTimeout(function () { t.remove(); }, 320); }, delay);
            return t;
        }

        /* ---------- I2 : validation en 1 clic depuis une ligne Échéances ---------- */
        function quickValidate(oi, qi, btn) {
            if (!requireUnlock()) return;
            var op = database[oi];
            if (!op) return;
            var raw = (op.qualifs || '').split(',');
            if (!raw[qi] || !raw[qi].trim()) { toast('Qualification introuvable.', true); return; }
            var before = raw.slice();                    // instantané pour l'annulation
            var q = splitQualif(raw[qi].trim(), qi);
            if (q.state === 'validated') { toast('Déjà validée.'); return; }
            var stAvant = computeOpStats(op);   // V8-2 : état AVANT écriture (transition 100 %)
            q.state = 'validated';
            if (!q.date || q.date === 'À QUALIFIER') q.date = new Date().toLocaleDateString('fr-FR');
            raw[qi] = joinQualif(q);
            op.qualifs = raw.join(',');
            persistData();
            renderTable();
            renderEcheances();
            renderTodayBanner();
            // DA : même retour que la modale — tampon + verrouillage de la carte
            // V8-2 : si cette validation ferme le dernier trou → tampon COMPLET (un seul à l'écran)
            var stApres = computeOpStats(op);
            var completNow = stAvant.total > 0 && stApres.valides === stApres.total && stAvant.valides < stApres.valides;
            showStamp(completNow ? 'complete' : 'validated');
            flashCard(oi, qi);
            var pos = btn && btn.getBoundingClientRect ? btn.getBoundingClientRect() : null;
            fireConfetti(pos ? pos.left + pos.width / 2 : window.innerWidth / 2, pos ? pos.top : window.innerHeight / 2);
            if (!q.validator) toast('<i class="fa-solid fa-lightbulb mr-1"></i>Conseil : ouvre la qualification pour tracer le validateur.', false, 3800);
            // Jeton d'annulation : deux validations rapprochées ne doivent pas restaurer la mauvaise capture
            var token = Date.now() + '|' + oi + '|' + qi;
            window.__undoToken = token;
            var t = toast('<i class="fa-solid fa-check mr-1"></i>' + sanitize(q.code) + ' validée pour ' + sanitize(op.nom) + ' <button class="ml-2 underline font-black text-blue-600 hover:text-blue-800" onclick="__undoQuick(this)" data-undo-token="' + token + '">Annuler</button>', false, 6000);
            window.__undoQuick = function (btnEl) {
                // si ce bouton n'est plus le dernier (toast périmé), on n'annule que ce toast
                var mine = !btnEl || !btnEl.getAttribute || btnEl.getAttribute('data-undo-token') === window.__undoToken;
                if (!mine) { toast('<i class="fa-solid fa-circle-info mr-1"></i>Une validation plus récente t attend : ce bouton est désactivé.', false, 3600); return; }
                if (t) t.remove();
                window.__undoToken = null;
                // V9 : après un rechargement depuis un autre onglet (listener storage),
                // `op` pointe vers un OBJET ORPHELIN de l'ancienne base. Écrire dessus
                // afficherait « Validation annulée » sans rien annuler. On refuse.
                if (database[oi] !== op) { toast('<i class="fa-solid fa-triangle-exclamation mr-1"></i>Données rechargées : annulation impossible, la base a changé.', true, 4200); return; }
                op.qualifs = before.join(',');
                persistData();
                renderTable();
                renderEcheances();
                renderTodayBanner();
                flashCard(oi, qi);   // DA : halo pour repérer la carte remise à son état antérieur
                toast('<i class="fa-solid fa-rotate-left mr-1"></i>Validation annulée.');
            };
        }

        function toInputDate(ddmmyyyy) {
            if (!ddmmyyyy) return '';
            var p = ddmmyyyy.split('/');
            if (p.length !== 3) return '';
            return p[2] + '-' + ('0' + p[1]).slice(-2) + '-' + ('0' + p[0]).slice(-2);
        }
        function fromInputDate(iso) {
            if (!iso) return '';
            var p = iso.split('-');
            if (p.length !== 3) return '';
            return p[2] + '/' + p[1] + '/' + p[0];
        }

        /* ---------- Données de référence ---------- */
        var HISTORICAL_KPI = {
            'P40': { 2:{init:12,pro:0}, 3:{init:6,pro:1}, 4:{init:0,pro:3}, 5:{init:1,pro:6}, 6:{init:6,pro:12}, 7:{init:5,pro:13}, 8:{init:6,pro:2}, 9:{init:0,pro:7}, 10:{init:3,pro:15}, 11:{init:7,pro:13}, 12:{init:5,pro:10}, 13:{init:2,pro:7} },
            'P50': { 4:{init:14,pro:10}, 5:{init:14,pro:8}, 6:{init:10,pro:12}, 7:{init:17,pro:6}, 8:{init:14,pro:6}, 9:{init:1,pro:13}, 10:{init:3,pro:3}, 11:{init:17,pro:5}, 12:{init:10,pro:19}, 13:{init:3,pro:5} }
        };

        /* V9.4 — Seul validateur restant : Sliman (les 5 autres personnes ont été retirées à sa demande). */
        var VALIDATORS_LIST = [
            { name: 'Sliman OUERTANI', alias: 'Sliman' }
        ];

        var QUALIFS_LIST = [ "ET0O45-Certification étanchage", "B40TE31-Install harness+torquage", "BCO0E30-Collage Support Electrique" ];

        var TEAM_LIST = ['P40A-A', 'P40B-A', 'P40C-A', 'P50A-A', 'P50B-A', 'P50C-A', 'P28A-A', 'P28B-A', 'P28C-A'];

        var database = [];
        var bossKpiLog = [];
        var currentZone = 'P40', currentSecteur = 'A', currentTeam = 'A', currentTeamFilter = 'P40A-A', currentKpiView = 'Tout';
        var currentProgramme = 'A350';   // V6 : A350 (P40/P50) | A330 (P28) — dérivé de op.equipe, jamais stocké
        var statusFilter = null;      // null | 'expired' | 'soon' | 'aqual' | 'validated'  (D1/D3)
        var echanceFilter = 'all';    // 'all' | 'expired' | '7' | '30' | '90'            (F1)
        var echViewMode = 'list';     // V1 : 'list' | 'timeline'                          (V1)
        var echWindowMonths = 3;      // V1 : fenêtre glissante 3 | 6 | 12 mois            (V1)
        var currentZoom = 100;

        window.onload = function () {
            try {
                initializeDatabase();
                currentZoom = parseInt(localStorage.getItem(ZOOM_KEY) || '100', 10);
                if (isNaN(currentZoom)) currentZoom = 100;
                applyZoom();
                fillCommonLists();
                updateFilters();
            } catch (e) {
                if (window.console) console.error('Init:', e);
                toast('<i class="fa-solid fa-triangle-exclamation mr-1"></i>Erreur d\'initialisation : ' + sanitize(e.message), true);
            }
            try { performWeeklyPurge(); } catch (e) { if (window.console) console.error('Purge:', e); }
            document.addEventListener('keydown', function (e) {
                if (e.key === 'Escape') { closeAllModals(); endTour(); hideSearchResults(); closeFiche(); return; }
                if (e.ctrlKey || e.metaKey || e.altKey) return;
                var tag = (e.target && e.target.tagName) ? e.target.tagName.toLowerCase() : '';
                var typing = tag === 'input' || tag === 'textarea' || tag === 'select';
                if (typing) return;
                var modalOpen = document.querySelector('.modal-backdrop.open');
                var tourEl = document.getElementById('tour-overlay');
                var tourActive = tourEl && tourEl.style.display !== 'none' && tourEl.style.display !== '';
                if (modalOpen || tourActive) return;
                // V10 : aucun raccourci 1-6 pendant l'écran de verrouillage
                if (typeof window.__verrouActif === 'function' && window.__verrouActif()) return;
                // F3 : 1-6 = onglets
                var tabKeys = { '1': 'operators', '2': 'reporting', '3': 'hebdo', '4': 'echances', '5': 'brouillons', '6': 'tuto' };
                if (tabKeys[e.key]) { e.preventDefault(); switchTab(tabKeys[e.key]); if (tabKeys[e.key] === 'brouillons') renderBrouillons(); return; }
                // F3 : "?" = aide des raccourcis
                if (e.key === '?') { e.preventDefault(); openModal('shortcuts-modal'); return; }
                // Raccourci "/" : focus recherche
                if (e.key === '/') {
                    e.preventDefault();
                    var si = document.getElementById('searchInput');
                    if (si) { si.focus(); si.select(); }
                }
            });
            // D5 : bouton retour en haut
            window.addEventListener('scroll', function () {
                var b = document.getElementById('back-to-top');
                if (b) b.classList.toggle('show', window.scrollY > 600);
            });
            // Première visite + rappel sauvegarde : différés derrière le verrou
            // (sinon ils partent sous l'écran de verrouillage à chaque nouvel
            // onglet et le guide ne s'affiche jamais). Le flag de déclenchement
            // est window.__apresAcces (nulé après usage → zéro double toast).
            function rappelsApresAcces() {
                var seenTour = null;
                try { seenTour = localStorage.getItem('cockpit_qa_tour_seen'); } catch (e) {}
                if (!seenTour) {
                    setTimeout(function () {
                        var t = toast('<i class="fa-solid fa-lightbulb mr-1"></i>Première visite ? Clique ici pour le guide en 6 étapes.', false);
                        if (t) {
                            t.style.cursor = 'pointer';
                            t.title = 'Démarrer le guide';
                            t.onclick = function () { startTour(); t.remove(); };
                        }
                        try { localStorage.setItem('cockpit_qa_tour_seen', Date.now().toString()); } catch (e) {}
                    }, 1400);
                }
                // Rappel de sauvegarde hebdomadaire
                var lastExport = null;
                try { lastExport = parseInt(localStorage.getItem('cockpit_qa_last_export') || '0', 10); } catch (e) {}
                if (!lastExport || (Date.now() - lastExport) > 7 * 86400000) {
                    setTimeout(function () {
                        toast('<i class="fa-solid fa-floppy-disk mr-1"></i>Pense à exporter ta sauvegarde (.json) — Gestion des opérateurs.', false);
                    }, 4000);
                }
            }
            if (typeof window.__verrouActif === 'function' && window.__verrouActif()) window.__apresAcces = rappelsApresAcces;
            else rappelsApresAcces();

            // ===================== V9 — REMISE EN QUESTION =====================
            // 1) « L'app ne ment plus dans le temps » : la page peut rester ouverte
            //    des jours sur le PC atelier. On compare (chaque minute, au retour
            //    visible, au focus) la chaîne-du-jour : AUCUN rendu tant que le jour
            //    n'a pas changé. Au changement, on ne fait que rappeler le rendu
            //    standard de l'écran visible — mêmes fonctions que switchTab, aucun
            //    code des onglets protégés modifié.
            window.__jourAffiche = new Date().toDateString();
            window.rafraichitSiNouveauJour = function () {
                try {
                    var jour = new Date().toDateString();
                    if (jour === window.__jourAffiche) return;
                    window.__jourAffiche = jour;  // AVANT le rendu : sinon toast en boucle à chaque tick
                    // La visibilité se joue sur la classe « hidden » des #view-*
                    // (mécanisme exact de switchTab, helpers partagés ci-dessous) :
                    // on trouve l'écran actif, puis on ne fait que rappeler SON rendu.
                    var visible = vueActiveId();
                    var rendu = false;
                    if (visible === 'operators') { renderTable(); rendu = true; }
                    else if (visible === 'reporting') { renderTable(); renderReporting(); rendu = true; }
                    else if (visible === 'hebdo') { renderTable(); renderHebdoStats(); rendu = true; }
                    else if (visible === 'echances') { renderTable(); renderEcheances(); rendu = true; }
                    // On ne promet « indicateurs rafraîchis » que si on a VRAIMENT
                    // rendu un écran (l'onglet Procédures n'a rien à rafraîchir).
                    if (rendu) toast('<i class="fa-solid fa-calendar-day mr-1"></i>Nouvelle journée : indicateurs rafraîchis.', false, 3800);
                } catch (err) { /* on garde l'affichage en place plutôt que de planter */ }
            };
            setInterval(window.rafraichitSiNouveauJour, 60000);
            document.addEventListener('visibilitychange', function () { if (!document.hidden) window.rafraichitSiNouveauJour(); });
            window.addEventListener('focus', window.rafraichitSiNouveauJour);

            // 2) « Deux onglets ne s'écrasent plus silencieusement » : le navigateur
            //    notifie l'onglet PERDANT de toute écriture d'un autre onglet. On
            //    recharge la mémoire (lecture seule, zéro écriture ici → pas de
            //    boucle), on ferme les modales dont les contextes (indices) sont
            //    périmés, puis on resynchronise avec un toast d'explication.
            window.addEventListener('storage', function (e) {
                // V10 : les brouillons ont LEUR clé dédiée — branche AVANT toute
                // logique de rechargement des clés v45 (sinon les notes
                // écraseraient bossKpiLog en mémoire puis le corrompt au prochain
                // persistData). Aucune écriture ici : juste le rendu si visible.
                if (e.key === BROUILLONS_KEY) {
                    if (vueActiveId() === 'brouillons') { try { renderBrouillons(); } catch (err) {} }
                    return;
                }
                if (e.key !== STORAGE_KEY && e.key !== KPI_LOG_KEY) return;
                var donnees = [];
                var efface = !e.newValue;   // effacement externe (réinit. faite dans l'autre onglet)
                if (!efface) {
                    try { donnees = JSON.parse(e.newValue); }
                    catch (err) { return; }    // écriture partielle en cours : on ignore
                    if (!Array.isArray(donnees)) return;
                }
                // Effacement OU remplacement : dans les deux cas on reflète la réalité.
                // Ignorer l'effacement laisserait un fantôme que la prochaine écriture
                // ferait ressusciter sans prévenir.
                if (e.key === STORAGE_KEY) database = donnees; else bossKpiLog = donnees;
                // persistData écrit les DEUX clés : un seul enregistrement croisé
                // déclenche donc 2 événements. On regroupe (même motif que le
                // débounce des échéances) : UN seul ressynchronisme + UN seul
                // toast pour la rafale entière.
                window.__resyncEfface = window.__resyncEfface || efface;
                if (window.__resyncStockage) clearTimeout(window.__resyncStockage);
                window.__resyncStockage = setTimeout(function () { // laisse passer les retours d'événements en cours
                    window.__resyncStockage = null;
                    var eff = window.__resyncEfface; window.__resyncEfface = false;
                    try {
                        // Les modales ouvertes tiennent des indices dans l'ancienne
                        // base (cardCtx) : elles pointeraient vers d'autres lignes.
                        if (isUnlocked()) closeAllModals();
                        renderTable();               // opérateurs, compteurs, bandeau, échéances
                        var v = vueActiveId();       // l'écran visible aussi : le toast ne ment pas
                        if (v === 'reporting') renderReporting();
                        else if (v === 'hebdo') renderHebdoStats();
                        fillCommonLists();
                        if (eff) toast('<i class="fa-solid fa-trash-can mr-1"></i>Données effacées dans un autre onglet — affichage remis à zéro.', true, 4200);
                        else toast('<i class="fa-solid fa-rotate mr-1"></i>Données modifiées dans un autre onglet — affichage rechargé.', false, 3800);
                    } catch (err) { /* l'affichage actuel est conservé */ }
                }, 400);
            });
        };

        /* ---------- Persistance ---------- */
        function initializeDatabase() {
            var legacyKeys = ['cockpit_qa_master_data_v44', 'cockpit_qa_master_data_v43', 'cockpit_qa_master_data_v42'];
            var rawInitial = null;
            try { rawInitial = localStorage.getItem(STORAGE_KEY); } catch (e) {}
            var primaryParses = false;
            if (rawInitial) { try { JSON.parse(rawInitial); primaryParses = true; } catch (e) {} }
            var data = getSafeStorageWithMigration(STORAGE_KEY, legacyKeys, null);
            if (rawInitial && !primaryParses) {
                // JSON présent mais illisible : on le met de côté avant tout écrasement
                try { localStorage.setItem('cockpit_qa_corrupt_backup_' + Date.now(), rawInitial); } catch (e) {}
            }
            var looksValid = Array.isArray(data) && (data.length === 0 ? rawInitial !== null : data.every(function (o) { return o && typeof o.nom === 'string'; }));
            if (!looksValid && Array.isArray(data) && data.length) {
                // Forme inattendue : backup puis réinitialisation
                try { localStorage.setItem('cockpit_qa_shape_backup_' + Date.now(), JSON.stringify(data)); } catch (e) {}
                data = null;
            }
            if (looksValid) { database = data; }
            else {
                database = [
                    { nom: "ATTARD THEO", equipe: "P40A-A", qualifs: "BSC0E30-Serrage Elec|15/07/2026|N, BTS0S00-Alodine|3/10/2026|N" },
                    { nom: "CROUZERY NICOLAS", equipe: "P40A-A", qualifs: "PSIVXBTS0S00-Application Alodine|À QUALIFIER|O" },
                    { nom: "DAPREMONT MAXIME", equipe: "P40A-A", qualifs: "BCO0S34-Collage résine|À QUALIFIER|O, BET0O45-Etanchage|À QUALIFIER|O, BPV4S21-Visserie A350|À QUALIFIER|O, BSC0S00-Serrage Meca|À QUALIFIER|O, BPV3S21-Visserie composite|À QUALIFIER|O, BPV0S00-Visserie structurale|À QUALIFIER|O, BOP1E31-Fibre Optic|À QUALIFIER|O, BP40S21-Assemb Composite|À QUALIFIER|O" },
                    { nom: "DARAN ALEXANDRE", equipe: "P40A-A", qualifs: "BP40S03-Carburant|31/01/2026|N, BP40S20-Assemb Struct|13/02/2026|N, BPV0S00-Visserie structurale|17/07/2026|N, BP40S37-Ajusteur photogramétrie|03/02/2026|N" },
                    { nom: "DI STASI THOMAS", equipe: "P40A-A", qualifs: "BET0O45-Etanchage|05/06/2026|N" },
                    { nom: "FAGES CLEMENT", equipe: "P40A-A", qualifs: "BP40S03-Carburant|18/03/2026|N, BP40S05-Circuit Eaux|03/02/2026|N, BTS0S00-Alodine|13/02/2026|N" },
                    { nom: "GIMENEZ JULIEN", equipe: "P40A-A", qualifs: "" },
                    { nom: "GIRARDINI VINCENT", equipe: "P40A-A", qualifs: "BP40S01-Mont Méca Réglage|À QUALIFIER|O, BP40S05-Circuit Eaux|À QUALIFIER|O, BP40S10-Commande de Vol|À QUALIFIER|O, BP40S23-Mettre en RéfGrandePiece|À QUALIFIER|O" },
                    { nom: "GONGORA BORIS", equipe: "P40A-A", qualifs: "BSC0S02-Serrage hydraulique|05/06/2026|N, BSE9S02-Permaswage|05/05/2026|N, BSC0E30-Serrage Elec|16/09/2026|N, BP40P01-Peintre Basic|À QUALIFIER|O, BP40P02-Peinture Finition|À QUALIFIER|O" },
                    { nom: "KURTH LUC", equipe: "P40A-A", qualifs: "BP40S05-Circuit Eaux|À QUALIFIER|O, BP40E30-Elec Core Compet|À QUALIFIER|O" },
                    { nom: "MARIA NICOLAS", equipe: "P40A-A", qualifs: "" },
                    { nom: "MARTIN KÉVIN", equipe: "P40A-A", qualifs: "BP40E30-Elec Core Compet|06/02/2026|N, BSC0S00-Serrage Meca|15/07/2026|N, BPV3S21-Pose visserie composit|15/07/2026|N, BP40S20-Assemb Struct|À QUALIFIER|O" },
                    { nom: "MICHEL FREDERIC", equipe: "P40A-A", qualifs: "BTS0S00-Alodine|À QUALIFIER|O" },
                    { nom: "MORELLATO WILLIAM", equipe: "P40A-A", qualifs: "BP40S10-Commande de Vol|À QUALIFIER|O, BME0E31-Métallisation|24/03/2026|N" },
                    { nom: "RIVIERE ENZO", equipe: "P40A-A", qualifs: "BRC0C19-Retou sans moy chauf|À QUALIFIER|O, BSC0S00-Serrage Meca|02/06/2026|N, BP40S01-Mont Méca Réglage|05/05/2026|N, BPV3S21-Pose visserie composit|02/06/2026|N, BPV0S00-Visserie structurale|17/07/2026|N" },
                    { nom: "SANCE ALLAN", equipe: "P40A-A", qualifs: "BMT0S03-Tuyauterie carbu|À QUALIFIER|O" },
                    { nom: "SEGUE MAIRONE", equipe: "P40A-A", qualifs: "BME0S00-Métallisation|À QUALIFIER|O" },
                    { nom: "SCALI GUILLAUME", equipe: "P40B-A", qualifs: "BTS0S00-Application Alodine|25/03/2026|N" },
                    { nom: "WHITE ETHAN", equipe: "P40B-A", qualifs: "BTS0S00-Application Alodine|À QUALIFIER|O, BME0E31-Mesure métallisation élec|À QUALIFIER|O, BP40S20-Assemb/Ajust Elmt Struct|À QUALIFIER|O, BP40P01-Compétence Basic Peintre|À QUALIFIER|O, BP40P02-Appliq Peinture Finition|À QUALIFIER|O" },
                    { nom: "CHEVREL ANTHONY", equipe: "P40B-A", qualifs: "" },
                    { nom: "EL GARAH MOHAMED", equipe: "P40B-A", qualifs: "BME0E31-Mesure métallisation élec|À QUALIFIER|O, BP40S02-Hydraulique|À QUALIFIER|O, BP40A05-Essai Recherche de Fuite|À QUALIFIER|O" },
                    { nom: "MARQUES JEREMY", equipe: "P40B-A", qualifs: "BP40L07-Mouler/Démouler Avion|À QUALIFIER|O, BP40S21-Assemb/Ajuster Composite|06/01/2026|N, BP40E30-Elec Install Core Compet|24/02/2026|N, BPV3S21-Pose visserie dans composit|10/03/2026|N" },
                    { nom: "MARSAULT VINCENT", equipe: "P40B-A", qualifs: "BP40S05-Circuit Eaux|À QUALIFIER|O" },
                    { nom: "MEKARBECH ZAKARIA", equipe: "P40B-A", qualifs: "BP40P02-Appliq Peinture Finition|À QUALIFIER|O, BP40P01-Compétence Basic Peintre|À QUALIFIER|O, BP40S20-Assemb/Ajust Elmt Struct|À QUALIFIER|O, BTS0S00-Application Alodine|À QUALIFIER|O, BET0O45-Etanchage|À QUALIFIER|O" },
                    { nom: "PEZET GABRIEL", equipe: "P40B-A", qualifs: "BP40A05-Essai Recherche de Fuite|À QUALIFIER|O, BP40S42-Installer matelas isolants|À QUALIFIER|O, BP40E32-Install Elec. Equipment|25/02/2026|N, BP40S27-Mont et Régler Empennage|31/01/2026|N, BMT0S03-Mtge joint tuyauterie carbu|31/01/2026|N, BPV4S21-Pose visserie A350 P40|31/01/2026|N" }
                ];
            }

            // Normalisation : types + vire les entrées vides pour que les index restent stables
            database.forEach(function (op) {
                if (typeof op.equipe !== 'string' || !op.equipe) op.equipe = 'P40A-A';
                op.qualifs = (typeof op.qualifs === 'string' ? op.qualifs : '').split(',').map(function (s) { return s.trim(); }).filter(Boolean).join(',');
            });

            var legacyKpiKeys = ['cockpit_boss_log_master_v44', 'cockpit_boss_log_master_v43', 'cockpit_boss_log_master_v42', 'cockpit_boss_log_master_v41', 'cockpit_boss_log_master_v40', 'cockpit_boss_log_master_v39'];
            bossKpiLog = getSafeStorageWithMigration(KPI_LOG_KEY, legacyKpiKeys, null);
            if (!bossKpiLog) {
                var past = new Date().getTime() - (86400000 * 7);
                bossKpiLog = [
                    { poste: 'P50', station: 'P50B', qualif: 'XXXX (qualif de démo)', compagnon: 'XXX', type: 'Initiale', qls: 'QLS2', validateur: 'Sliman OUERTANI', date: '19/03/2026', qcm: 'Oui', cw: 13, timestamp: past },
                    { poste: 'P40', station: 'P40C', qualif: 'Basic Metier Assemblage 1040JS00', compagnon: 'Fihol clement TO124145', type: 'Prorogation', qls: '', validateur: 'Sliman OUERTANI', date: '19/03/2026', qcm: '', cw: 13, timestamp: past },
                    { poste: 'P40', station: 'P40C', qualif: 'BSC0E30 Serrage au couple Elec', compagnon: 'ESPARSEIL CYRIL', type: 'Prorogation', qls: '', validateur: 'Sliman OUERTANI', date: '23/03/2026', qcm: 'Non Attente reponse QCM', cw: 13, timestamp: past },
                    { poste: 'P40', station: 'P40B', qualif: 'PSIVXBSC0S00-Serrage au couple Meca', compagnon: 'ESTERINI ENZO', type: 'Prorogation', qls: '', validateur: 'Sliman OUERTANI', date: '23/03/2026', qcm: 'En attente QCM', cw: 13, timestamp: past },
                    { poste: 'P40', station: 'P40B', qualif: 'PSIVXBTS0S00', compagnon: 'SCALI Guillaume', type: 'Prorogation', qls: '', validateur: 'Sliman OUERTANI', date: '25/03/2026', qcm: 'Oui', cw: 13, timestamp: past },
                    { poste: 'P50', station: 'P50A', qualif: 'PSIVXBP50S21-Assemb/Ajuster Composite', compagnon: 'PARIS PIERRE', type: 'Prorogation', qls: 'QLS1', validateur: 'Sliman OUERTANI', date: '26/03/2026', qcm: 'Oui', cw: 14, timestamp: past }
                ];
            }
            persistData();
        }

        function persistData() {
            try {
                localStorage.setItem(STORAGE_KEY, JSON.stringify(database));
                localStorage.setItem(KPI_LOG_KEY, JSON.stringify(bossKpiLog));
            } catch (e) { toast('Stockage plein : exporte un CSV au plus vite !', true); }
            saveToHistory();
        }

        var lastHistorySave = 0;
        function saveToHistory() {
            var now = Date.now();
            if (now - lastHistorySave < 120000) return; // 1 snapshot max toutes les 2 min
            lastHistorySave = now;
            var history = getSafeStorageWithMigration(HISTORY_KEY, [], []);
            var d = new Date();
            history.unshift({ id: d.getTime(), time: d.toLocaleDateString('fr-FR') + ' à ' + d.toLocaleTimeString('fr-FR'), data: JSON.parse(JSON.stringify(database)) });
            if (history.length > 30) history = history.slice(0, 30);
            try { localStorage.setItem(HISTORY_KEY, JSON.stringify(history)); } catch (e) { /* quota plein : l'historique saute, la base reste sauvegardée */ }
        }

        function performWeeklyPurge() {
            var now = new Date();
            var lastPurge = localStorage.getItem('cockpit_purge_master_v13');
            var lastWed = new Date();
            lastWed.setDate(now.getDate() - ((now.getDay() + 4) % 7));
            lastWed.setHours(0, 0, 0, 0);
            if (!lastPurge || parseInt(lastPurge) < lastWed.getTime()) {
                var purged = 0;
                database.forEach(function (op) {
                    if (!op.qualifs) return;
                    var parts = op.qualifs.split(',').filter(function (q) { return q.trim(); });
                    var kept = parts.filter(function (q) { return !q.includes('|validated'); });
                    purged += parts.length - kept.length;
                    op.qualifs = kept.join(',');
                });
                localStorage.setItem('cockpit_purge_master_v13', now.getTime().toString());
                persistData();
                renderTable();
                if (purged > 0) toast('<i class="fa-solid fa-broom mr-1"></i>Purge hebdo : ' + purged + ' validation(s) de la semaine passée purgée(s).');
            }
        }

        /* ---------- Parsing des qualifications ---------- */
        function analyzeDate(dateStr, isInitial) {
            if (isInitial || dateStr === "À QUALIFIER" || !dateStr) return { status: 'ok', days: null };
            try {
                var parts = dateStr.split('/');
                // V9 : contrôle strict + round-trip. « 31/02 » roule silencieusement
                // au 03/03, un format US (03/31/2026) fabrique une année lointaine et
                // une lettre dans les chiffres donne NaN (badge « J-NaN », tri instable,
                // CSV pollué) : on refuse tout et on traite comme une date absente —
                // aucun J-x n'est jamais inventé sur du texte invalide.
                if (parts.length !== 3 || !/^\d{1,2}$/.test(parts[0]) || !/^\d{1,2}$/.test(parts[1]) || !/^(?:\d{2}|\d{4})$/.test(parts[2])) return { status: 'ok', days: null };
                var jj = parseInt(parts[0], 10), mm = parseInt(parts[1], 10), aaaa = parseInt(parts[2], 10);
                if (parts[2].length === 2) aaaa = 2000 + aaaa;   // héritage : « 26 » = 2026 (sinon l'échéance disparaît de la feuille)
                var expDate = new Date(aaaa, mm - 1, jj);
                if (expDate.getDate() !== jj || expDate.getMonth() !== mm - 1 || expDate.getFullYear() !== aaaa) return { status: 'ok', days: null };
                var today = new Date(); today.setHours(0, 0, 0, 0);
                var diffDays = Math.ceil((expDate - today) / (1000 * 60 * 60 * 24));
                if (isNaN(diffDays)) return { status: 'ok', days: null };
                var status = 'ok';
                if (diffDays <= 0) status = 'expired';
                else if (diffDays <= 5) status = 'critical';
                else if (diffDays <= 15) status = 'warning';
                return { status: status, days: diffDays };
            } catch (e) { return { status: 'ok', days: null }; }
        }

        function splitQualif(raw, idx) {
            var p = (raw || '').split('|');
            var codeFull = p[0] || '';
            var dash = codeFull.indexOf('-');
            var code = dash >= 0 ? codeFull.slice(0, dash) : codeFull;
            var name = dash >= 0 ? cleanName(codeFull.slice(dash + 1)) : 'QUALIFICATION';
            var a = analyzeDate(p[1], p[2] === 'O');
            return {
                idx: idx, code: code, name: name || 'QUALIFICATION',
                date: p[1] || '-', isIni: p[2] === 'O',
                state: p[3] || 'normal', note: p[4] || '', validator: p[5] || '',
                status: a.status, days: a.days
            };
        }

        function joinQualif(q) {
            var clean = function (s) { return (s || '').replace(/[|,]/g, ' ;'); };
            return clean(q.code) + '-' + clean(q.name) + '|' + q.date + '|' + (q.isIni ? 'O' : 'N') + '|' + (q.state || 'normal') + '|' + clean(q.note) + '|' + (q.validator || '');
        }

        function getQualifs(op) {
            return (op.qualifs || '').split(',').map(function (s, i) { return s.trim() ? splitQualif(s.trim(), i) : null; }).filter(Boolean);
        }
        /* ---------- Filtres & onglets ---------- */
        // V6 : programme dérivé de la zone (op.equipe reste la seule source de vérité, zéro migration)
        function programmeDeZone(z) { return z === 'P28' ? 'A330' : 'A350'; }
        var ZONES_BY_PROG = { 'A350': ['P40', 'P50'], 'A330': ['P28'] };
        function setProgramme(p) {
            if (!ZONES_BY_PROG[p]) p = 'A350';
            currentProgramme = p;
            if (ZONES_BY_PROG[p].indexOf(currentZone) < 0) currentZone = ZONES_BY_PROG[p][0];
            updateFilters();
        }
        function setZone(z) { currentZone = z; updateFilters(); }
        function setSecteur(s) { currentSecteur = s; updateFilters(); }
        function setTeam(t) { currentTeam = t; updateFilters(); }

        function setBtnActive(el, active) {
            if (!el) return;
            el.classList.toggle('bg-blue-600', active);
            el.classList.toggle('text-white', active);
            el.classList.toggle('shadow-sm', active);
            el.classList.toggle('font-black', active);
            el.classList.toggle('font-bold', !active);
            el.classList.toggle('text-slate-500', !active);
            el.classList.toggle('hover:bg-slate-200', !active);
        }

        function updateFilters() {
            // V6 : le programme pilote les sous-sections — currentZone est dérivé, jamais libre
            if (currentProgramme === 'A330') currentZone = 'P28';
            else if (currentZone === 'P28') currentZone = 'P40';
            ['A350', 'A330'].forEach(function (p) { setBtnActive(document.getElementById('btn-prog-' + p), p === currentProgramme); });
            ['P40', 'P50'].forEach(function (z) { setBtnActive(document.getElementById('btn-zone-' + z), z === currentZone); });
            var b28 = document.getElementById('btn-zone-P28');
            if (b28) b28.classList.toggle('hidden', currentProgramme !== 'A330');
            var b40 = document.getElementById('btn-zone-P40'), b50 = document.getElementById('btn-zone-P50');
            var showA350 = currentProgramme === 'A350';
            if (b40) b40.classList.toggle('hidden', !showA350);
            if (b50) b50.classList.toggle('hidden', !showA350);
            ['A', 'B', 'C'].forEach(function (s) { setBtnActive(document.getElementById('btn-secteur-' + s), s === currentSecteur); });
            ['A', 'B'].forEach(function (t) { setBtnActive(document.getElementById('btn-team-' + t), t === currentTeam); });
            currentTeamFilter = currentZone + currentSecteur + '-' + currentTeam;
            renderTable();
        }

        var TABS = ['operators', 'reporting', 'hebdo', 'echances', 'brouillons', 'tuto'];
        function vueActiveId() {
            var trouve = null;
            TABS.forEach(function (id) {
                var v = document.getElementById('view-' + id);
                if (v && !v.classList.contains('hidden')) trouve = id;
            });
            return trouve;
        }

        function switchTab(tabId) {
            // Garde-fou : un identifiant inconnu ne doit jamais masquer toutes les vues (écran vide)
            if (TABS.indexOf(tabId) < 0) tabId = 'operators';
            TABS.forEach(function (id) {
                var v = document.getElementById('view-' + id);
                var t = document.getElementById('tab-' + id);
                if (v) v.classList.add('hidden');
                if (t) {
                    t.classList.remove('bg-blue-600', 'text-white', 'shadow-md');
                    t.classList.add('bg-white', 'text-slate-600', 'border', 'border-slate-200');
                }
            });
            var av = document.getElementById('view-' + tabId);
            var at = document.getElementById('tab-' + tabId);
            if (av) {
                av.classList.remove('hidden');
                if (tabId === 'reporting') av.classList.add('flex');
                // D5 : léger fondu à chaque entrée de vue
                av.classList.remove('view-in'); void av.offsetWidth; av.classList.add('view-in');
            }
            if (at) {
                at.classList.remove('bg-white', 'text-slate-600', 'border', 'border-slate-200');
                at.classList.add('bg-blue-600', 'text-white', 'shadow-md');
            }
            if (tabId === 'reporting') { renderReporting(); }
            if (tabId === 'hebdo') { renderHebdoStats(); }
            if (tabId === 'echances') { renderEcheances(); }
        }

        /* ---------- Tableau opérateurs ---------- */
        function computeOpStats(op) {
            var s = { total: 0, valides: 0, echues: 0, warn: 0, aqual: 0 };
            getQualifs(op).forEach(function (q) {
                s.total++;
                if (q.state === 'validated') s.valides++;
                else {
                    if (q.status === 'expired') s.echues++;
                    else if (q.status === 'critical' || q.status === 'warning') s.warn++;
                    if (q.state === 'normal' && q.date === 'À QUALIFIER') s.aqual++;
                }
            });
            return s;
        }

        /* ---------- D1/D3 : statuts globaux, filtres et bandeau du jour ---------- */
        // Source unique : mêmes règles pour les compteurs, le filtre et le bandeau (seuil d'urgence = 7 jours)
        function matchesStatusFilter(q, st) {
            if (!st) return true;
            if (st === 'validated') return q.state === 'validated';
            if (q.state === 'validated') return false;
            if (st === 'expired') return q.status === 'expired';
            if (st === 'aqual') return q.date === 'À QUALIFIER' && q.state === 'normal';
            if (st === 'soon') return q.status !== 'expired' && q.days !== null && q.days <= 7;
            return true;
        }

        function computeStatusCounts() {
            var c = { expired: 0, soon: 0, aqual: 0, validated: 0 };
            database.forEach(function (op) {
                getQualifs(op).forEach(function (q) {
                    if (q.state === 'validated') { c.validated++; return; }
                    if (q.status === 'expired') { c.expired++; return; }
                    if (q.date === 'À QUALIFIER' && q.state === 'normal') { c.aqual++; return; }
                    if (q.days !== null && q.days <= 7) c.soon++;
                });
            });
            return c;
        }

        function renderStatusCounters(c) {
            ['expired', 'soon', 'aqual', 'validated'].forEach(function (k) {
                var n = document.getElementById('cnt-' + k + '-n');
                if (n) n.innerText = c[k];
                var b = document.getElementById('cnt-' + k);
                if (b) {
                    b.classList.toggle('cnt-active', statusFilter === k);
                    b.classList.toggle('cnt-zero', !c[k]);
                }
            });
            var reset = document.getElementById('cnt-reset');
            if (reset) reset.classList.toggle('hidden', !statusFilter);
        }

        function setStatusFilter(s) {
            statusFilter = (statusFilter === s) ? null : s; // re-clic = on retire le filtre
            if (document.getElementById('view-operators').classList.contains('hidden')) switchTab('operators');
            renderTable();
            if (statusFilter) {
                var labels = { expired: 'Échues', soon: 'expirent sous 7 jours', aqual: 'à qualifier', validated: 'Validées' };
                toast('<i class="fa-solid fa-filter mr-1"></i>Filtre « ' + labels[statusFilter] + ' » — re-clique sur le compteur ou « Réinitialiser » pour le lever.');
            }
        }

        function resetAllFilters() {
            statusFilter = null;
            currentProgramme = 'A350';
            currentZone = 'P40'; currentSecteur = 'A'; currentTeam = 'A';
            clearSearch();
            updateFilters();
            toast('<i class="fa-solid fa-rotate-left mr-1"></i>Filtres réinitialisés (A350 · P40 · Ligne A · Équipe A).');
        }

        function renderTodayBanner() {
            var el = document.getElementById('today-banner');
            if (!el) return;
            var urgent = [];
            database.forEach(function (op, oi) {
                getQualifs(op).forEach(function (q) {
                    if (q.state === 'validated') return;
                    if (q.status === 'expired' || (q.days !== null && q.days <= 7)) urgent.push({ oi: oi, qi: q.idx, op: op, q: q });
                });
            });
            urgent.sort(function (a, b) { return a.q.days - b.q.days; });
            el.classList.remove('hidden');
            if (!urgent.length) {
                el.className = 'rounded-xl border px-4 py-3 flex flex-col gap-2 bg-emerald-50 border-emerald-200';
                el.innerHTML = '<div class="text-xs font-black text-emerald-700"><i class="fa-solid fa-circle-check mr-1"></i>Rien d\'urgent : aucune qualification échue ni expirant dans les 7 prochains jours.</div>';
                return;
            }
            el.className = 'rounded-xl border px-4 py-3 flex flex-col gap-2 bg-amber-50 border-amber-200';
            var chips = urgent.slice(0, 5).map(function (u) {
                var isExp = u.q.status === 'expired';
                var cls = isExp ? 'bg-red-100 text-red-700 border-red-300' : 'bg-white text-amber-800 border-amber-300';
                return '<button onclick="openCardModal(' + u.oi + ',' + u.qi + ')" class="rounded-lg border px-2.5 py-1.5 text-[11px] font-black hover:shadow-md transition-shadow ' + cls + '" title="Ouvrir la qualification">' +
                    sanitize(u.op.nom) + ' · <span class="mono">' + sanitize(u.q.code) + '</span> · ' + (isExp ? 'ÉCHUE' : 'J-' + u.q.days) + '</button>';
            }).join('');
            el.innerHTML = '<div class="text-xs font-black text-amber-800 uppercase tracking-wide"><i class="fa-solid fa-bell mr-1"></i>Aujourd\'hui — ' + urgent.length + ' échéance(s) déjà échue(s) ou sous 7 jours <span class="normal-case font-bold text-amber-700/80">(toutes équipes confondues)</span></div>' +
                '<div class="flex flex-wrap gap-2 items-center">' + chips +
                (urgent.length > 5 ? '<span class="text-[11px] font-black text-amber-700">+' + (urgent.length - 5) + '…</span>' : '') +
                '<button onclick="setStatusFilter(\'expired\')" class="rounded-lg border border-amber-300 bg-amber-100 text-amber-800 px-2.5 py-1.5 text-[11px] font-black hover:bg-amber-200 no-print">Voir les échues</button>' +
                '</div>';
        }

        /* ---------- V8-1 : tri des cartes par urgence (affichage seul) ---------- */
        // Rang d'affichage : MÊME logique que la cascade de rendu des cartes
        // (l'état prime sur l'échéance : une carte priorité/pas capable/standby
        // n'affiche jamais « échue », même datée passée). Échue d'abord : en
        // atelier, une qualification échue est un risque opérationnel réel.
        function qualifRank(q) {
            if (q.state === 'validated') return 7;   // validée : fin de marche
            if (q.state === 'priority') return 1;
            if (q.state === 'standby') return 5;
            if (q.state === 'disabled') return 6;
            if (q.status === 'expired') return 0;    // échue (jour J compris)
            if (q.status === 'critical') return 2;   // ≤ 5 j
            if (q.status === 'warning') return 3;    // ≤ 15 j
            return 4;                                 // à qualifier / normal sans échéance
        }
        function sortQualifsForDisplay(qualifs) {
            // getQualifs retourne déjà un NOUVEAU tableau à chaque appel → le tri
            // ne peut toucher ni op.qualifs (contrat de données) ni database[].
            return qualifs.slice().sort(function (a, b) {
                var ra = qualifRank(a), rb = qualifRank(b);
                if (ra !== rb) return ra - rb;
                var da = (a.days === null || a.days === undefined) ? Infinity : a.days;
                var db = (b.days === null || b.days === undefined) ? Infinity : b.days;
                if (da !== db) return da - db;
                return a.idx - b.idx;  // ordre source explicite (tri stable garanti)
            });
        }

        function renderTable() {
            var tbody = document.getElementById('tableBody');
            if (!tbody) return;
            tbody.innerHTML = '';

            var globVal = 0;
            database.forEach(function (op) {
                getQualifs(op).forEach(function (q) { if (q.state === 'validated') globVal++; });
            });
            var c = document.getElementById('global-counter'); if (c) c.innerText = globVal;

            // D1/D3 : recomput global des statuts + bandeau (indépendants des filtres d'équipe)
            renderStatusCounters(computeStatusCounts());
            renderTodayBanner();

            // Tri alphabétique À L'AFFICHAGE uniquement (database[] n'est jamais réordonné → index stables)
            var order = database.map(function (op, i) { return i; }).sort(function (a, b) {
                var cmp = database[a].nom.localeCompare(database[b].nom, 'fr');
                return cmp !== 0 ? cmp : (database[a].equipe || '').localeCompare(database[b].equipe || '');
            });

            order.forEach(function (oi) {
                var op = database[oi];
                if (op.equipe !== currentTeamFilter) return;

                var qualifs = getQualifs(op);
                if (statusFilter && !qualifs.some(function (q) { return matchesStatusFilter(q, statusFilter); })) return;
                // V8-1 : urgence d'abord (tri local sur copie, data-qi/oi intacts)
                var cards = sortQualifsForDisplay(qualifs).map(function (q) {
                    var cls = q.isIni ? "card-ini" : "card-pro";
                    var icon = ""; var banner = ""; var noteHtml = "";
                    if (q.state === 'validated') { cls += ' state-validated'; icon = '<i class="fa-solid fa-circle-check text-emerald-500 q-icon"></i>'; }
                    else if (q.state === 'priority') { cls += ' state-priority'; banner = '<div class="q-banner priority-sky text-blue-600 bg-blue-100"><div class="plane-wrapper"><i class="fa-solid fa-plane-up plane-icon text-blue-500"></i><div class="plane-cable"></div><div class="plane-banner-content"><i class="fa-solid fa-bolt"></i> PRIORITÉ</div></div></div>'; }
                    else if (q.state === 'disabled') { cls += ' state-disabled'; banner = '<div class="q-banner">PAS CAPABLE</div>'; }
                    else if (q.state === 'standby') { cls += ' state-standby'; banner = '<div class="q-banner">STANDBY</div>'; }
                    else if (q.status !== 'ok') { cls += ' status-' + q.status; if (q.status === 'expired') { icon = '<i class="fa-solid fa-triangle-exclamation q-icon"></i>'; banner = '<div class="q-banner">ÉCHU</div>'; } }
                    else if (q.date === 'À QUALIFIER') { cls += ' status-aqual'; }   /* DA : ruban d'attente */
                    if (q.note) noteHtml = '<div class="q-note"><i class="fa-solid fa-comment-dots mr-1"></i>' + sanitize(q.note) + '</div>';

                    var validatorHtml = q.validator ? '<span class="text-[9px] font-black text-slate-400"><i class="fa-solid fa-user-check mr-1"></i>' + sanitize(q.validator) + '</span>' : '';
                    var timerHtml = '';
                    if (q.state === 'normal' && (q.status === 'critical' || q.status === 'warning') && q.days !== null) {
                        timerHtml = '<span class="timer-badge ' + (q.status === 'critical' ? 'timer-expired' : 'timer-soon') + '" title="Expire dans ' + q.days + ' jour(s)">' + q.days + ' j</span>';
                    }

                    return '<div class="q-card ' + cls + '" data-qi="' + q.idx + '" onclick="openCardModal(' + oi + ',' + q.idx + ')" title="Cliquer pour agir sur cette qualification">' +
                        banner +
                        '<div class="q-header"><span class="q-code">' + sanitize(q.code) + '</span><div class="flex items-center"><span class="badge-type ' + (q.isIni ? 'type-ini' : 'type-pro') + '">' + (q.isIni ? 'INI' : 'PRO') + '</span></div></div>' +
                        '<div class="q-body"><div class="q-title-row">' + icon + '<span class="q-title">' + sanitize(q.name) + '</span></div>' + noteHtml + '</div>' +
                        '<div class="q-footer"><span class="q-date">' + sanitize(q.date) + '</span><span class="flex items-center gap-2">' + timerHtml + validatorHtml + '</span></div>' +
                        '</div>';
                }).join('');

                var st = computeOpStats(op);
                var indColor = st.echues > 0 ? 'text-red-600' : (st.warn > 0 ? 'text-amber-600' : (st.total > 0 && st.valides === st.total ? 'text-emerald-600' : 'text-slate-700'));
                var pct = st.total ? Math.round(st.valides * 100 / st.total) : 0;
                var barColor = st.echues > 0 ? '#DC2626' : (st.warn > 0 ? '#D97706' : (st.total > 0 && st.valides === st.total ? '#059669' : '#2563EB'));
                var complet = st.total > 0 && st.valides === st.total;   // V8-2 : tout est validé
                var completChip = complet ? '<div class="op-complet" title="Toutes les qualifications de cet opérateur sont validées"><i class="fa-solid fa-circle-check"></i> COMPLET</div>' : '';
                var indHtml = '<td class="px-4 py-6 border-l-2 border-slate-200 text-center align-top">' +
                    '<div class="mono font-black text-lg ' + indColor + '" title="Qualifications validées / total">' + st.valides + '/' + st.total + '</div>' +
                    '<div class="op-progress mx-auto w-16" title="' + pct + '% validé"><i style="width:' + pct + '%;background:' + barColor + '"></i></div>' +
                    completChip +
                    (st.echues ? '<div class="text-[10px] font-black text-red-600 mt-1"><i class="fa-solid fa-triangle-exclamation"></i> ' + st.echues + ' échue(s)</div>' : '') +
                    (st.warn ? '<div class="text-[10px] font-black text-amber-600 mt-1"><i class="fa-solid fa-clock"></i> ' + st.warn + ' bientôt</div>' : '') +
                    (st.aqual ? '<div class="text-[10px] font-black text-sky-600 mt-1"><i class="fa-solid fa-hourglass-half"></i> ' + st.aqual + ' à qualifier</div>' : '') +
                    '</td>';

                // D2 : pastille d'initiales colorée (déterministe à partir du nom)
                var ini = op.nom.split(/\s+/).map(function (w) { return w.charAt(0); }).join('').slice(0, 2).toUpperCase();
                var hue = opHue(op.nom);

                var tr = document.createElement('tr');
                tr.className = "bg-white border-b border-slate-200";
                tr.setAttribute('data-op', op.nom);
                tr.innerHTML =
                    '<td class="px-6 py-6 border-r-2 border-slate-200 align-top w-48">' +
                        '<div class="flex items-start justify-between gap-2">' +
                            '<div class="flex items-center gap-3 min-w-0">' +
                                '<span class="op-pastille ' + hue + '" title="' + sanitize(op.nom) + '">' + sanitize(ini) + '</span>' +
                                '<div class="min-w-0"><div class="font-black text-slate-800 uppercase leading-tight">' + sanitize(op.nom) + '</div>' +
                                '<div class="text-[10px] font-bold text-slate-400 mt-1">' + sanitize(op.equipe) + '</div></div>' +
                            '</div>' +
                            '<div class="flex flex-col gap-1 flex-shrink-0">' +
                                '<button onclick="event.stopPropagation(); openAddQualifModal(' + oi + ')" title="Ajouter une qualification" class="w-7 h-7 rounded-lg bg-slate-100 hover:bg-blue-600 hover:text-white text-slate-500 flex items-center justify-center"><i class="fa-solid fa-plus text-xs"></i></button>' +
                                '<button onclick="event.stopPropagation(); openFiche(' + oi + ')" title="Fiche opérateur imprimable" class="w-7 h-7 rounded-lg bg-slate-100 hover:bg-slate-800 hover:text-white text-slate-500 flex items-center justify-center"><i class="fa-solid fa-print text-xs"></i></button>' +
                                '<button onclick="event.stopPropagation(); toggleTeam(' + oi + ')" title="Déplacer dans l\'autre équipe (A / B)" class="w-7 h-7 rounded-lg bg-slate-100 hover:bg-emerald-600 hover:text-white text-slate-500 flex items-center justify-center"><i class="fa-solid fa-right-left text-xs"></i></button>' +
                            '</div>' +
                        '</div>' +
                    '</td>' +
                    '<td class="px-6 py-4 flex flex-wrap gap-2">' + (cards || '<span class="text-xs font-bold text-slate-400 py-4 block">Aucune qualification enregistrée — cliquez sur + pour en ajouter une.</span>') + '</td>' +
                    indHtml;
                tbody.appendChild(tr);
            });

            if (!tbody.children.length) {
                if (statusFilter) {
                    var sLabel = { expired: 'des qualifications ÉCHUES', soon: 'de qualification expirant sous 7 jours', aqual: 'de qualification à qualifier', validated: 'de qualification Validée' }[statusFilter];
                    tbody.innerHTML = '<tr class="bg-white"><td colspan="3" class="px-6 py-10 text-center"><div class="text-sm font-black text-slate-500"><i class="fa-solid fa-filter mr-2 text-slate-300"></i>Aucun opérateur avec ' + sLabel + ' dans ' + sanitize(currentTeamFilter) + '</div><button onclick="setStatusFilter(null)" class="mt-3 px-4 py-2 rounded-lg text-xs font-black bg-blue-600 text-white shadow-md hover:bg-blue-500 no-print">Retirer ce filtre</button></td></tr>';
                } else {
                    tbody.innerHTML = '<tr class="bg-white"><td colspan="3" class="px-6 py-10 text-center"><div class="text-sm font-black text-slate-500"><i class="fa-solid fa-user-slash mr-2 text-slate-300"></i>Aucun opérateur dans ' + sanitize(currentTeamFilter) + '</div><div class="text-xs font-bold text-slate-400 mt-2">Ajoute-en un via le bouton Gestion (icône engrenage, en haut à droite).</div></td></tr>';
                }
            }

            // DA : garde perf — au-delà de 40 cartes affichées, les animations
            // d'état infinies passent en statique doux (body.motion-soft)
            document.body.classList.toggle('motion-soft', tbody.querySelectorAll('.q-card').length > 40);

            // V9 : la feuille des échéances se resynchronise d'elle-même. Tous les
            // chemins de modification passent par renderTable() (purge hebdo,
            // suppression, ajout, import, restauration, revert…) : UN seul point
            // d'attache = plus jamais de liste périmée pointant vers de mauvaises
            // lignes. Le regroupement anti-rafale est assuré par le débounce de
            // renderEcheances lui-même.
            renderEcheances();
        }

        /* ---------- Modale carte (actions qualification) ---------- */
        var cardCtx = { oi: -1, qi: -1 };
        var cardState = 'normal';

        function openCardModal(oi, qi) {
            if (!requireUnlock()) return;
            var op = database[oi];
            // V9 : plus jamais de clic silencieux sur une ligne périmée (liste
            // rechargée par un autre onglet, suppression entre-temps…) : on dit
            // pourquoi et on resynchronise l'affichage.
            if (!op) { toast('Cette ligne a changé — affichage resynchronisé.', true); renderTable(); return; }
            var raw = (op.qualifs || '').split(',');
            if (!raw[qi] || !raw[qi].trim()) { toast('Cette qualification a changé — affichage resynchronisé.', true); renderTable(); return; }
            cardCtx = { oi: oi, qi: qi };
            var q = splitQualif(raw[qi].trim(), qi);
            cardState = q.state;

            document.getElementById('card-modal-title').innerText = q.code + ' — ' + q.name;
            document.getElementById('card-modal-sub').innerText = op.nom + ' · ' + op.equipe + ' · ' + (q.isIni ? 'Initiale' : 'Prorogation');
            document.querySelectorAll('#card-state-buttons .state-btn').forEach(function (b) {
                b.classList.toggle('active', b.getAttribute('data-state') === cardState);
            });
            var dateInput = document.getElementById('card-date');
            dateInput.value = (q.date && q.date !== 'À QUALIFIER' && q.date !== '-') ? toInputDate(q.date) : '';
            var sel = document.getElementById('card-validator');
            sel.innerHTML = '<option value="">—</option>' + VALIDATORS_LIST.map(function (v) { return '<option value="' + sanitize(v.name) + '"' + (v.name === q.validator ? ' selected' : '') + '>' + sanitize(v.name) + '</option>'; }).join('');
            document.getElementById('card-note').value = q.note || '';
            openModal('card-modal');
        }

        function setCardState(s) {
            cardState = s;
            document.querySelectorAll('#card-state-buttons .state-btn').forEach(function (b) {
                b.classList.toggle('active', b.getAttribute('data-state') === s);
            });
        }

        /* ---------- V7 : confettis canvas maison (zéro dépendance, reduced-motion respecté) ---------- */
        var _confettiRAF = null;
        function fireConfetti(x, y) {
            if (window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches) return;
            var cv = document.getElementById('confetti-canvas');
            if (!cv || !cv.getContext) return;
            var ctx = cv.getContext('2d');
            if (!ctx) return;   // canvas 2d indisponible (poste verrouillé) : pas de confettis, pas d'erreur
            var dpr = window.devicePixelRatio || 1;
            cv.width = window.innerWidth * dpr; cv.height = window.innerHeight * dpr;
            cv.style.width = window.innerWidth + 'px'; cv.style.height = window.innerHeight + 'px';
            ctx.setTransform(dpr, 0, 0, dpr, 0, 0);
            var colors = ['#059669', '#10B981', '#34D399', '#2563EB', '#F59E0B', '#F87171', '#A78BFA'];
            var parts = [];
            for (var i = 0; i < 120; i++) {
                var a = Math.random() * Math.PI * 2, sp = 3 + Math.random() * 7;
                parts.push({
                    x: x, y: y,
                    vx: Math.cos(a) * sp, vy: Math.sin(a) * sp - 3,
                    w: 5 + Math.random() * 6, h: 8 + Math.random() * 8,
                    rot: Math.random() * Math.PI, vr: (Math.random() - 0.5) * 0.4,
                    c: colors[(Math.random() * colors.length) | 0], life: 1
                });
            }
            if (_confettiRAF) cancelAnimationFrame(_confettiRAF);
            var start = null;
            function step(ts) {
                if (!start) start = ts;
                var el = ts - start;
                ctx.clearRect(0, 0, window.innerWidth, window.innerHeight);
                var alive = 0;
                parts.forEach(function (p) {
                    p.vy += 0.22; p.x += p.vx; p.y += p.vy; p.vx *= 0.99; p.rot += p.vr;
                    if (el > 1400) p.life -= 0.02;
                    if (p.life > 0 && p.y < window.innerHeight + 40) {
                        alive++;
                        ctx.save();
                        ctx.globalAlpha = Math.max(0, p.life);
                        ctx.translate(p.x, p.y); ctx.rotate(p.rot);
                        ctx.fillStyle = p.c;
                        ctx.fillRect(-p.w / 2, -p.h / 2, p.w, p.h);
                        ctx.restore();
                    }
                });
                if (alive > 0) _confettiRAF = requestAnimationFrame(step);
                else { ctx.clearRect(0, 0, window.innerWidth, window.innerHeight); _confettiRAF = null; }
            }
            _confettiRAF = requestAnimationFrame(step);
        }

        /* ---------- V7 : tampon d'état qui claque ---------- */
        var _stampTimer = null;
        var STAMP_META = {
            validated: ['VALIDÉE', 'stamp-validated'],
            priority: ['PRIORITÉ', 'stamp-priority'],
            standby: ['STANDBY', 'stamp-standby'],
            disabled: ['PAS CAPABLE', 'stamp-disabled'],
            complete: ['OPÉRATEUR COMPLET', 'stamp-complete']
        };
        function showStamp(state) {
            var s = document.getElementById('state-stamp');
            if (!s) return;
            var meta = STAMP_META[state];
            if (!meta) return;
            var reduced = window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches;
            s.textContent = meta[0];
            s.className = 'state-stamp ' + meta[1] + (reduced ? ' play-noanim' : ' play');
            if (reduced) { s.style.opacity = '0.9'; }
            clearTimeout(_stampTimer);
            _stampTimer = setTimeout(function () { s.classList.remove('play', 'play-noanim'); s.style.opacity = ''; s.textContent = ''; }, reduced ? 900 : 1300);
        }

        function flashCard(oi, qi) {
            setTimeout(function () {
                var op = database[oi];
                if (!op) return;
                var row = document.querySelector('#tableBody tr[data-op="' + (window.CSS && CSS.escape ? CSS.escape(op.nom) : op.nom.replace(/"/g, '\\"')) + '"]');
                if (!row) return;
                row.classList.add('op-flash');
                setTimeout(function () { row.classList.remove('op-flash'); }, 2100);
                if (qi >= 0) {
                    // DA : .card-just-changed déclenche l'animation one-shot du NOUVEL état
                    var card = row.querySelector('.q-card[data-qi="' + qi + '"]');
                    if (card) { card.classList.add('op-flash', 'card-just-changed'); setTimeout(function () { card.classList.remove('op-flash'); card.classList.remove('card-just-changed'); }, 2100); }
                }
            }, 60);
        }

        function saveCardModal() {
            if (!requireUnlock()) return;
            var op = database[cardCtx.oi];
            if (!op) return;
            var raw = (op.qualifs || '').split(',');
            if (!raw[cardCtx.qi] || !raw[cardCtx.qi].trim()) { toast('Qualification introuvable (données modifiées entre-temps).', true); renderTable(); closeModal('card-modal'); return; }
            var q = splitQualif(raw[cardCtx.qi].trim(), cardCtx.qi);
            var prevState = q.state;   // V7 : mémorise l'état avant écrasement
            q.state = cardState;
            q.note = document.getElementById('card-note').value.trim();
            q.validator = document.getElementById('card-validator').value;
            var newDate = fromInputDate(document.getElementById('card-date').value);
            q.date = newDate || 'À QUALIFIER';
            if (q.state === 'validated' && !q.validator) {
                toast('Conseil : précise un validateur pour tracer la validation.', true);
            }
            var stAvant = computeOpStats(op);   // V8-2 : état AVANT écriture (transition 100 %)
            raw[cardCtx.qi] = joinQualif(q);
            op.qualifs = raw.join(',');
            persistData();
            renderTable();
            renderEcheances();
            renderTodayBanner();
            closeModal('card-modal');
            toast('<i class="fa-solid fa-check mr-1"></i>' + sanitize(q.code) + ' mise à jour.');
            // V7 : plaisir du changement d'état — tampon + confettis (validation) + flash de la carte
            if (cardState !== prevState) {
                // V8-2 : si cette validation ferme le dernier trou → tampon COMPLET (un seul à l'écran)
                var stApres = computeOpStats(op);
                var completNow = stAvant.total > 0 && stApres.valides === stApres.total && stAvant.valides < stApres.valides;
                showStamp(completNow ? 'complete' : cardState);
                if (cardState === 'validated') fireConfetti(window.innerWidth / 2, window.innerHeight / 2);
                flashCard(cardCtx.oi, cardCtx.qi);
            }
        }

        function deleteQualif() {
            if (!requireUnlock()) return;
            var op = database[cardCtx.oi];
            if (!op) return;
            var raw = (op.qualifs || '').split(',');
            if (!raw[cardCtx.qi] || !raw[cardCtx.qi].trim()) { toast('Qualification introuvable.', true); renderTable(); closeModal('card-modal'); return; }
            var q = splitQualif(raw[cardCtx.qi].trim(), cardCtx.qi);
            if (!confirm('Supprimer la qualification « ' + q.code + ' - ' + q.name + ' » de ' + op.nom + ' ?')) return;
            raw.splice(cardCtx.qi, 1);
            op.qualifs = raw.join(',').replace(/^,|,$/g, '');
            persistData();
            renderTable();
            closeModal('card-modal');
            toast('Qualification supprimée.');
        }

        /* ---------- Ajouter une qualification ---------- */
        var addQualifCtx = { oi: -1 };

        function openAddQualifModal(oi) {
            if (!requireUnlock()) return;
            var op = database[oi];
            if (!op) return;
            addQualifCtx = { oi: oi };
            document.getElementById('addqualif-op').innerHTML = '<i class="fa-solid fa-user mr-2 text-blue-500"></i>' + sanitize(op.nom) + ' <span class="text-slate-400">· ' + sanitize(op.equipe) + '</span>';
            document.getElementById('aq-code').value = '';
            document.getElementById('aq-type').value = 'N';
            document.getElementById('aq-date').value = '';
            openModal('addqualif-modal');
            setTimeout(function () { document.getElementById('aq-code').focus(); }, 80);
        }

        function saveAddQualif() {
            if (!requireUnlock()) return;
            var op = database[addQualifCtx.oi];
            if (!op) return;
            var full = document.getElementById('aq-code').value.trim().replace(/[|,]/g, ' ;');
            if (!full) { toast('Saisis un code qualification (ex : BSC0S00-Serrage Meca).', true); return; }
            var dash = full.indexOf('-');
            var code = dash >= 0 ? full.slice(0, dash) : full;
            var name = dash >= 0 ? full.slice(dash + 1) : 'QUALIFICATION';
            var isIni = document.getElementById('aq-type').value === 'O';
            var date = fromInputDate(document.getElementById('aq-date').value) || 'À QUALIFIER';
            var newQualif = joinQualif({ code: code, name: name, date: date, isIni: isIni, state: 'normal', note: '', validator: '' });
            op.qualifs = op.qualifs ? (op.qualifs + ',' + newQualif) : newQualif;
            persistData();
            renderTable();
            closeModal('addqualif-modal');
            toast('<i class="fa-solid fa-plus mr-1"></i>' + sanitize(code) + ' ajoutée à ' + sanitize(op.nom) + '.');
        }

        /* ---------- Modale liste des validations ---------- */
        function openValidatedModal() {
            refreshValidatedList();
            openModal('validated-modal');
        }

        function refreshValidatedList() {
            var items = [];
            database.forEach(function (op, oi) {
                getQualifs(op).forEach(function (q) {
                    if (q.state === 'validated') items.push({ oi: oi, qi: q.idx, op: op.nom, code: q.code, name: q.name, date: q.date, validator: q.validator });
                });
            });
            var counter = document.getElementById('validated-counter');
            if (counter) counter.innerText = items.length + ' qualification(s) validée(s) en cours';
            var list = document.getElementById('validated-list');
            if (!list) return;
            if (!items.length) {
                list.innerHTML = '<div class="px-4 py-8 text-center text-xs font-bold text-slate-400">Aucune validation en cours.<br>Ouvre une carte qualification et passe-la en « ✔ Validée ».</div>';
                return;
            }
            list.innerHTML = items.map(function (it) {
                return '<div class="px-4 py-3 flex items-center justify-between gap-3 hover:bg-slate-50">' +
                    '<div class="min-w-0">' +
                        '<div class="text-[12px] font-black text-slate-800 truncate"><span class="mono text-blue-600">' + sanitize(it.code) + '</span> — ' + sanitize(it.name) + '</div>' +
                        '<div class="text-[10px] font-bold text-slate-400 mt-0.5">' + sanitize(it.op) + (it.validator ? ' · validé par ' + sanitize(it.validator) : '') + (it.date && it.date !== '-' ? ' · échéance ' + sanitize(it.date) : '') + '</div>' +
                    '</div>' +
                    '<button onclick="revertValidation(' + it.oi + ',' + it.qi + ')" title="Annuler la validation" class="px-3 py-1.5 rounded-lg text-[10px] font-black bg-red-50 text-red-600 hover:bg-red-100 flex-shrink-0"><i class="fa-solid fa-rotate-left mr-1"></i>Annuler</button>' +
                '</div>';
            }).join('');
        }

        function revertValidation(oi, qi) {
            if (!requireUnlock()) return;
            var op = database[oi];
            if (!op) return;
            var raw = (op.qualifs || '').split(',');
            if (!raw[qi] || !raw[qi].trim()) { toast('Qualification introuvable.', true); renderTable(); refreshValidatedList(); return; }
            var q = splitQualif(raw[qi].trim(), qi);
            q.state = 'normal';
            raw[qi] = joinQualif(q);
            op.qualifs = raw.join(',');
            persistData();
            renderTable();
            refreshValidatedList();
            flashCard(oi, qi);   // DA : halo d'encre pour repérer la carte remise en état
            toast('Validation annulée : ' + sanitize(q.code) + '.');
        }
        /* ---------- Gestion opérateurs ---------- */
        function openManageModal() {
            renderManageModal();
            openModal('manage-modal');
        }

        function teamOptions(selected) {
            // V6 : sélecteur d'équipe groupé par programme (A350 → P40/P50, A330 → P28)
            var groups = [['A350', ['P40A-A', 'P40B-A', 'P40C-A', 'P50A-A', 'P50B-A', 'P50C-A']], ['A330', ['P28A-A', 'P28B-A', 'P28C-A']]];
            var html = groups.map(function (g) {
                return '<optgroup label="' + g[0] + '">' + g[1].map(function (t) {
                    return '<option value="' + t + '"' + (t === selected ? ' selected' : '') + '>' + t + '</option>';
                }).join('') + '</optgroup>';
            }).join('');
            // équipe existante hors liste (données plus anciennes) : option de secours pour ne rien perdre
            if (selected && ['P40A-A', 'P40B-A', 'P40C-A', 'P50A-A', 'P50B-A', 'P50C-A', 'P28A-A', 'P28B-A', 'P28C-A'].indexOf(selected) < 0) {
                html += '<option value="' + sanitize(selected) + '" selected>' + sanitize(selected) + '</option>';
            }
            return html;
        }

        function renderManageModal() {
            var teamSel = document.getElementById('op-new-team');
            if (teamSel) teamSel.innerHTML = teamOptions(null);

            var list = document.getElementById('manage-op-list');
            if (list) {
                list.innerHTML = database.map(function (op, i) {
                    return '<div class="flex items-center gap-2 bg-slate-50 rounded-lg p-2 border border-slate-200">' +
                        '<input value="' + sanitize(op.nom) + '" onchange="renameOp(' + i + ', this.value)" class="form-input" style="flex-grow" title="Renommer">' +
                        '<select onchange="moveOp(' + i + ', this.value)" class="form-input" style="width:120px" title="Changer d\'équipe">' +
                            teamOptions(op.equipe) +
                        '</select>' +
                        '<button onclick="deleteOperator(' + i + ')" title="Supprimer" class="w-8 h-8 rounded-lg bg-white border border-slate-200 text-red-400 hover:text-red-600 hover:bg-red-50 flex items-center justify-center flex-shrink-0"><i class="fa-solid fa-trash text-xs"></i></button>' +
                    '</div>';
                }).join('') || '<div class="text-xs font-bold text-slate-400">Aucun opérateur.</div>';
            }
            renderHistoryRows();
            renderCorbeilleList();
        }

        function addOperator() {
            if (!requireUnlock()) return;
            var nameEl = document.getElementById('op-new-name');
            var name = nameEl.value.trim();
            if (!name) { toast('Saisis un nom d\'opérateur.', true); return; }
            if (database.some(function (o) { return o.nom.toUpperCase() === name.toUpperCase(); })) { toast('Cet opérateur existe déjà.', true); return; }
            database.push({ nom: name, equipe: document.getElementById('op-new-team').value, qualifs: '' });
            database.sort(function (a, b) { return a.nom.localeCompare(b.nom); });
            nameEl.value = '';
            persistData();
            renderTable();
            renderManageModal();
            fillCommonLists();
            toast('<i class="fa-solid fa-user-plus mr-1"></i>' + sanitize(name) + ' ajouté.');
        }

        function renameOp(i, v) {
            if (!requireUnlock()) { renderManageModal(); return; }
            v = v.trim();
            if (!v) { renderManageModal(); return; }
            // V9 : un homonyme créerait deux lignes data-op identiques — repérage et
            // flashing viseraient toujours la première. Même garde que addOperator.
            if (database.some(function (o, j) { return j !== i && o.nom.toUpperCase() === v.toUpperCase(); })) { toast('Cet opérateur existe déjà.', true); renderManageModal(); return; }
            database[i].nom = v;
            persistData();
            renderTable();
            fillCommonLists();
            toast('Opérateur renommé.');
        }

        function moveOp(i, v) {
            if (!requireUnlock()) { renderManageModal(); return; }
            database[i].equipe = v;
            persistData();
            renderTable();
            toast('Opérateur déplacé vers ' + v + '.');
        }
        // V10 — Bascule A↔B en un clic depuis la ligne du tableau (même
        // chemin que moveOp : PIN, persistance, rendu). Garde-fou : seule
        // une équipe se terminant par A ou B est basculable (sinon nom
        // corrompu possible via import libre) — sinon no-op expliqué.
        function toggleTeam(i) {
            var op = database[i];
            if (!op) { toast('Cette ligne a changé — affichage resynchronisé.', true); renderTable(); return; }
            var eq = typeof op.equipe === 'string' ? op.equipe : '';
            if (!/[AB]$/.test(eq)) {
                toast('Équipe « ' + (eq || 'inconnue') + ' » non reconnue : passez par Gestion des opérateurs.', true, 4200);
                return;
            }
            var cible = eq.slice(0, -1) + (eq.slice(-1) === 'A' ? 'B' : 'A');
            moveOp(i, cible);
        }

        /* ================= V10 — BROUILLONS (cahier de texte) =================
           Lecture directe à chaque rendu (aucun cache en mémoire → pas de
           désynchronisation entre onglets), clé DÉDIÉE (jamais persistData),
           photos compressées pour rester sous le quota du navigateur. */
        var brouillonCtx = { id: null, photo: null, photoNom: '' };

        function getBrouillons() {
            var v = getSafeStorage(BROUILLONS_KEY, []);
            return Array.isArray(v) ? v.filter(function (b) { return b && typeof b === 'object'; }) : [];
        }
        function setBrouillons(list) {
            try { localStorage.setItem(BROUILLONS_KEY, JSON.stringify(list)); return true; }
            catch (e) {
                toast('<i class="fa-solid fa-database mr-1"></i>Espace plein : la note n\'a pas été enregistrée. Supprime une vieille photo.', true, 5200);
                return false;
            }
        }
        function brouillonDate(d) {
            d = d || new Date();
            function p(n) { return ('0' + n).slice(-2); }
            return p(d.getDate()) + '/' + p(d.getMonth() + 1) + '/' + d.getFullYear() + ' ' + p(d.getHours()) + 'h' + p(d.getMinutes());
        }
        function escapeAttr(s) { return String(s || '').replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;').replace(/"/g, '&quot;').replace(/'/g, '&#39;'); }
        // V10 — l'id d'une note part dans un attribut onclick="…'id'…" : on retire tout
        // caractère capable de fermer la chaîne JS (' et \) ou l'attribut HTML (" < >).
        // (Nécessaire surtout pour les ids venus d'un .json importé.)
        function safeNoteId(s) { return String(s || '').replace(/['"\\<>]/g, '').slice(0, 40); }

        function renderBrouillons() {
            var zone = document.getElementById('brouillons-list');
            if (!zone) return;
            var liste = getBrouillons();
            var q = ((document.getElementById('br-search') || {}).value || '').trim().toLowerCase();
            if (q) {
                liste = liste.filter(function (b) {
                    return String(b.titre || '').toLowerCase().indexOf(q) >= 0 || String(b.texte || '').toLowerCase().indexOf(q) >= 0;
                });
            }
            liste.sort(function (a, b) { return (b.ts || 0) - (a.ts || 0); });
            if (!liste.length) {
                zone.innerHTML = '<div class="text-center py-8 text-slate-400 text-xs font-bold">' +
                    (q ? 'Aucune note ne correspond à « ' + sanitize(q) + ' ».' : 'Aucun brouillon pour l\'instant — clique sur « Nouvelle note » pour ouvrir ton cahier de texte.') + '</div>';
                return;
            }
            zone.innerHTML = liste.map(function (b) {
                var thumb = (typeof b.photo === 'string' && b.photo.indexOf('data:image/') === 0)
                    ? '<img src="' + escapeAttr(b.photo) + '" alt="" style="width:44px;height:44px;object-fit:cover;border-radius:8px;border:1px solid #e2e8f0;flex-shrink:0;">'
                    : '';
                return '<div class="flex items-start gap-3 bg-slate-50 border border-slate-200 rounded-xl p-3">' +
                    '<div class="flex flex-col items-center gap-1 flex-shrink-0" style="width:44px">' + thumb + '</div>' +
                    '<div class="min-w-0 flex-grow" onclick="openBrouillon(\'' + safeNoteId(b.id) + '\')" style="cursor:pointer">' +
                        '<div class="flex items-center gap-2 flex-wrap"><span class="font-black text-slate-800 text-sm truncate">' + sanitize(b.titre || '(sans titre)') + '</span>' +
                        '<span class="text-[10px] font-bold text-slate-400">' + sanitize(b.date || '') + '</span></div>' +
                        (b.texte ? '<div class="text-xs text-slate-600 mt-1 whitespace-pre-wrap break-words" style="max-height:60px;overflow:hidden;">' + sanitize(b.texte) + '</div>' : '') +
                    '</div>' +
                    '<button onclick="openBrouillon(\'' + safeNoteId(b.id) + '\')" title="Modifier" class="w-8 h-8 rounded-lg bg-white border border-slate-200 text-slate-400 hover:text-blue-600 hover:border-blue-300 flex items-center justify-center flex-shrink-0"><i class="fa-solid fa-pen text-xs"></i></button>' +
                    '<button onclick="deleteBrouillonDirect(\'' + safeNoteId(b.id) + '\')" title="Supprimer" class="w-8 h-8 rounded-lg bg-white border border-slate-200 text-slate-400 hover:text-red-600 hover:border-red-300 flex items-center justify-center flex-shrink-0"><i class="fa-solid fa-trash text-xs"></i></button>' +
                '</div>';
            }).join('');
        }

        function newBrouillon() {
            brouillonCtx = { id: null, photo: null, photoNom: '' };
            document.getElementById('br-modal-title').innerHTML = '<i class="fa-solid fa-pen-to-square text-rose-500 mr-2"></i>Nouvelle note';
            document.getElementById('br-title').value = '';
            document.getElementById('br-text').value = '';
            refreshBrouillonPhotoUI();
            document.getElementById('br-delete').classList.add('hidden');
            openModal('brouillon-modal');
            setTimeout(function () { var t = document.getElementById('br-title'); if (t) t.focus(); }, 80);
        }
        function openBrouillon(id) {
            var b = getBrouillons().filter(function (x) { return String(x.id) === String(id); })[0];
            if (!b) { toast('Cette note a changé — liste resynchronisée.', true); renderBrouillons(); return; }
            brouillonCtx = { id: b.id, photo: (typeof b.photo === 'string' && b.photo.indexOf('data:image/') === 0) ? b.photo : null, photoNom: b.photoNom || 'photo' };
            document.getElementById('br-modal-title').innerHTML = '<i class="fa-solid fa-pen-to-square text-rose-500 mr-2"></i>Modifier la note';
            document.getElementById('br-title').value = b.titre || '';
            document.getElementById('br-text').value = b.texte || '';
            refreshBrouillonPhotoUI();
            document.getElementById('br-delete').classList.remove('hidden');
            openModal('brouillon-modal');
        }
        function refreshBrouillonPhotoUI() {
            var pv = document.getElementById('br-photo-preview');
            var del = document.getElementById('br-photo-del');
            var nm = document.getElementById('br-photo-name');
            if (brouillonCtx.photo) { pv.src = brouillonCtx.photo; pv.classList.remove('hidden'); del.classList.remove('hidden'); nm.textContent = brouillonCtx.photoNom || ''; }
            else { pv.removeAttribute('src'); pv.classList.add('hidden'); del.classList.add('hidden'); nm.textContent = ''; }
        }
        function addBrouillonPhoto(inputEl) {
            var file = inputEl && inputEl.files && inputEl.files[0];
            var err = document.getElementById('br-photo-err');
            err.classList.add('hidden');
            if (!file) return;
            if (file.type.indexOf('image/') !== 0) { err.textContent = 'Seules les images sont acceptées.'; err.classList.remove('hidden'); inputEl.value = ''; return; }
            var reader = new FileReader();
            reader.onload = function () {
                var img = new Image();
                img.onload = function () {
                    try {
                        var MAX = 1280;
                        var w = img.width, h = img.height;
                        if (w > MAX || h > MAX) { if (w >= h) { h = Math.round(h * MAX / w); w = MAX; } else { w = Math.round(w * MAX / h); h = MAX; } }
                        var cv = document.createElement('canvas');
                        cv.width = w; cv.height = h;
                        cv.getContext('2d').drawImage(img, 0, 0, w, h);
                        var dataUrl = cv.toDataURL('image/jpeg', 0.7);
                        if (dataUrl.length > 1500000) { err.textContent = 'Photo trop lourde même après compression — prends une image plus petite.'; err.classList.remove('hidden'); inputEl.value = ''; return; }
                        brouillonCtx.photo = dataUrl;
                        brouillonCtx.photoNom = file.name || 'photo';
                        refreshBrouillonPhotoUI();
                    } catch (e) { err.textContent = 'Traitement de l\'image impossible.'; err.classList.remove('hidden'); }
                    inputEl.value = '';
                };
                img.onerror = function () { err.textContent = 'Image illisible.'; err.classList.remove('hidden'); inputEl.value = ''; };
                img.src = reader.result;
            };
            reader.readAsDataURL(file);
        }
        function removeBrouillonPhoto() {
            brouillonCtx.photo = null; brouillonCtx.photoNom = '';
            refreshBrouillonPhotoUI();
        }
        function saveBrouillon() {
            var titre = (document.getElementById('br-title').value || '').trim();
            var texte = (document.getElementById('br-text').value || '').trim();
            if (!titre && !texte) { toast('Écris au moins un titre ou une note.', true); return; }
            var list = getBrouillons();
            var now = Date.now();
            if (brouillonCtx.id) {
                var trouve = false;
                list = list.map(function (b) {
                    if (String(b.id) !== String(brouillonCtx.id)) return b;
                    trouve = true;
                    return { id: b.id, titre: titre, texte: texte, date: b.date || brouillonDate(new Date(b.ts || now)), maj: brouillonDate(), ts: b.ts || now, photo: brouillonCtx.photo, photoNom: brouillonCtx.photoNom };
                });
                if (!trouve) { toast('Cette note a changé — annulation.', true); closeModal('brouillon-modal'); renderBrouillons(); return; }
            } else {
                list.push({ id: 'br' + now + Math.floor(Math.random() * 1000), titre: titre, texte: texte, date: brouillonDate(), maj: brouillonDate(), ts: now, photo: brouillonCtx.photo, photoNom: brouillonCtx.photoNom });
            }
            if (!setBrouillons(list)) return;   // quota : la modale reste ouverte, rien n'est perdu
            closeModal('brouillon-modal');
            renderBrouillons();
            toast('<i class="fa-solid fa-check mr-1"></i>Note enregistrée.');
        }
        function deleteBrouillon() {
            if (!brouillonCtx.id) return;
            deleteBrouillonDirect(brouillonCtx.id, true);
        }
        function deleteBrouillonDirect(id, fermer) {
            if (!confirm('Supprimer cette note définitivement ?')) return;
            var list = getBrouillons().filter(function (b) { return String(b.id) !== String(id); });
            if (!setBrouillons(list)) return;
            if (fermer) closeModal('brouillon-modal');
            renderBrouillons();
            toast('<i class="fa-solid fa-trash mr-1"></i>Note supprimée.');
        }

        function deleteOperator(i) {
            if (!requireUnlock()) return;
            var op = database[i];
            if (!confirm('Supprimer l\'opérateur « ' + op.nom + ' » ? (il sera mis en corbeille)')) return;
            var corbeille = getSafeStorage(CORBEILLE_KEY, []);
            corbeille.unshift({ op: op, idx: i, deletedAt: new Date().toLocaleString('fr-FR') });
            // V9 : si la corbeille ne peut pas être écrite (stockage plein), on
            // REFUSE la suppression plutôt que de perdre la copie de secours sans
            // prévenir (l'utilisateur croirait que rien ne s'est passé).
            try { localStorage.setItem(CORBEILLE_KEY, JSON.stringify(corbeille.slice(0, 50))); }
            catch (err) { toast('Corbeille locale pleine : suppression annulée.', true); return; }
            database.splice(i, 1);
            persistData();
            renderTable();
            renderManageModal();
            fillCommonLists();
            toast('Opérateur supprimé (récupérable dans la corbeille locale).');
        }

        function renderHistoryRows() {
            var el = document.getElementById('manage-history');
            if (!el) return;
            var history = getSafeStorage(HISTORY_KEY, []);
            if (!history.length) { el.innerHTML = '<div class="text-xs font-bold text-slate-400">Aucun historique pour l\'instant.</div>'; return; }
            el.innerHTML = history.slice(0, 10).map(function (h, i) {
                return '<div class="flex items-center justify-between bg-slate-50 rounded-lg px-3 py-2 border border-slate-200">' +
                    '<span class="text-[11px] font-bold text-slate-600"><i class="fa-solid fa-clock-rotate-left mr-2 text-slate-400"></i>' + sanitize(h.time) + '</span>' +
                    '<button onclick="restoreHistory(' + i + ')" class="px-3 py-1 rounded-lg text-[10px] font-black bg-blue-50 text-blue-600 hover:bg-blue-100">Restaurer</button>' +
                '</div>';
            }).join('');
        }

        function restoreHistory(idx) {
            if (!requireUnlock()) return;
            var history = getSafeStorage(HISTORY_KEY, []);
            if (!history[idx]) return;
            if (!confirm('Restaurer la base du ' + history[idx].time + ' ?\nLes modifications plus récentes seront perdues (un nouvel historique est créé avant la restauration).')) return;
            lastHistorySave = 0;
            saveToHistory(); // snapshot forcé avant d'écraser
            database = JSON.parse(JSON.stringify(history[idx].data));
            try { localStorage.setItem(STORAGE_KEY, JSON.stringify(database)); } catch (e) {}
            renderTable();
            renderManageModal();
            fillCommonLists();
            toast('Base restaurée.');
        }

        /* ---------- Sauvegarde / Restauration complète (fichier .json) ---------- */
        function exportBackupJSON() {
            var backup = {
                format: 'cockpit_qa_backup',
                version: 1,
                dateExport: new Date().toLocaleString('fr-FR'),
                database: database,
                bossKpiLog: bossKpiLog,
                history: getSafeStorage(HISTORY_KEY, []),
                corbeille: getSafeStorage(CORBEILLE_KEY, []),
                brouillons: getBrouillons(),
                zoom: currentZoom,
                purgeMarker: (function () { try { return localStorage.getItem('cockpit_purge_master_v13') || ''; } catch (e) { return ''; } })()
            };
            var blob = new Blob([JSON.stringify(backup, null, 1)], { type: 'application/json' });
            var a = document.createElement('a');
            a.href = URL.createObjectURL(blob);
            a.download = 'sauvegarde_planing_qa_' + new Date().toISOString().slice(0, 10) + '.json';
            document.body.appendChild(a);
            a.click();
            setTimeout(function () { URL.revokeObjectURL(a.href); a.remove(); }, 300);
            try { localStorage.setItem('cockpit_qa_last_export', Date.now().toString()); } catch (e) {}
            toast('<i class="fa-solid fa-download mr-1"></i>Sauvegarde exportée (' + database.length + ' opérateurs).');
        }

        function importBackupJSON(inputEl) {
            if (!requireUnlock()) { if (inputEl) inputEl.value = ''; return; }
            var file = inputEl && inputEl.files && inputEl.files[0];
            if (!file) return;
            var reader = new FileReader();
            reader.onload = function () {
                var obj = null;
                try { obj = JSON.parse(reader.result); } catch (e) { toast('Fichier illisible : ce n\'est pas un JSON valide.', true); inputEl.value = ''; return; }
                // --- Validation stricte avant toute écriture ---
                if (!obj || typeof obj !== 'object' || Array.isArray(obj)) { toast('Structure inattendue : objet avec "database" attendu.', true); inputEl.value = ''; return; }
                if (!Array.isArray(obj.database)) { toast('Le fichier ne contient pas de liste d\'opérateurs ("database").', true); inputEl.value = ''; return; }
                if (obj.database.length > 5000) { toast('Fichier suspect : ' + obj.database.length + ' opérateurs.', true); inputEl.value = ''; return; }
                var bad = obj.database.some(function (o) { return !o || typeof o.nom !== 'string' || !o.nom.trim(); });
                if (bad) { toast('Opérateur sans nom valide dans le fichier — import annulé.', true); inputEl.value = ''; return; }
                var logs = Array.isArray(obj.bossKpiLog) ? obj.bossKpiLog.filter(function (l) { return l && typeof l === 'object' && typeof l.poste === 'string'; }).slice(0, 20000) : [];
                // Normalisation (mêmes règles que l'init) + round-trip défensif sur chaque qualification
                var imported = obj.database.map(function (o) {
                    var quals = (typeof o.qualifs === 'string' ? o.qualifs : '').split(',').map(function (s) { return s.trim(); }).filter(Boolean).map(function (seg) {
                        try { return joinQualif(splitQualif(seg, 0)); } catch (e) { return null; }
                    }).filter(Boolean).join(',');
                    return { nom: o.nom.trim(), equipe: (typeof o.equipe === 'string' && o.equipe) ? o.equipe : 'P40A-A', qualifs: quals };
                });
                var preview = imported.slice(0, 8).map(function (o) { return ' · ' + o.nom; }).join('\n');
                if (!confirm('Importer cette sauvegarde (' + file.name + ') ?\n\n' + imported.length + ' opérateurs (actuellement ' + database.length + '), ' + logs.length + ' entrées de registre.\n\nÀ remplacer :\n' + preview + (imported.length > 8 ? '\n · ...' : '') + '\n\nUn instantané de l\'état actuel sera conservé dans l\'historique.')) {
                    inputEl.value = ''; return;
                }
                // --- Écriture : snapshot forcé, purge neutralisée, puis persistance ---
                lastHistorySave = 0; saveToHistory();
                // Ne garde qu'UN snapshot pré-import (évite de gonfler le stockage)
                try {
                    var oldKeys = [];
                    for (var k = 0; k < localStorage.length; k++) { var key = localStorage.key(k); if (key && key.indexOf('cockpit_qa_preimport_') === 0) oldKeys.push(key); }
                    oldKeys.forEach(function (key) { localStorage.removeItem(key); });
                    localStorage.setItem('cockpit_qa_preimport_' + Date.now(), JSON.stringify({ database: database, bossKpiLog: bossKpiLog }));
                } catch (e) {}
                try { localStorage.setItem('cockpit_purge_master_v13', new Date().getTime().toString()); } catch (e) {}
                database = imported;
                bossKpiLog = logs;
                var goodHistory = Array.isArray(obj.history) ? obj.history.filter(function (h) { return h && Array.isArray(h.data); }).slice(0, 30) : [];
                if (goodHistory.length) { try { localStorage.setItem(HISTORY_KEY, JSON.stringify(goodHistory)); } catch (e) {} }
                var goodTrash = Array.isArray(obj.corbeille) ? obj.corbeille.filter(function (c) { return c && c.op && typeof c.op.nom === 'string'; }).slice(0, 50) : [];
                if (goodTrash.length) { try { localStorage.setItem(CORBEILLE_KEY, JSON.stringify(goodTrash)); } catch (e) {} }
                // V10 : brouillons — clé optionnelle (ancien fichier = conservés tels quels)
                if (Array.isArray(obj.brouillons)) {
                    var goodBr = obj.brouillons.filter(function (b) { return b && typeof b === 'object' && (typeof b.titre === 'string' || typeof b.texte === 'string'); }).slice(0, 500);
                    // Photo importée : uniquement data:image, plafonné (anti quota / anti injection)
                    goodBr = goodBr.map(function (b) {
                        var ph = (typeof b.photo === 'string' && b.photo.indexOf('data:image/') === 0 && b.photo.length < 1500000) ? b.photo : null;
                        var nid = safeNoteId((typeof b.id === 'string' && b.id) ? b.id : '');
                        return { id: nid || ('br' + Date.now() + Math.floor(Math.random() * 1000)),
                                 titre: String(b.titre || '').slice(0, 80), texte: String(b.texte || '').slice(0, 5000),
                                 date: String(b.date || '').slice(0, 30), maj: String(b.maj || '').slice(0, 30),
                                 ts: typeof b.ts === 'number' ? b.ts : Date.now(), photo: ph, photoNom: String(b.photoNom || '').slice(0, 60) };
                    });
                    try { localStorage.setItem(BROUILLONS_KEY, JSON.stringify(goodBr)); } catch (e) {}
                }
                if (typeof obj.zoom === 'number' && obj.zoom >= 70 && obj.zoom <= 140) { currentZoom = obj.zoom; applyZoom(); }
                persistData();
                renderTable();
                fillCommonLists();
                renderManageModal();
                if (document.getElementById('view-reporting') && !document.getElementById('view-reporting').classList.contains('hidden')) renderReporting();
                if (vueActiveId() === 'brouillons') { try { renderBrouillons(); } catch (e) {} }
                toast('<i class="fa-solid fa-check mr-1"></i>Sauvegarde importée : ' + imported.length + ' opérateurs.');
            };
            reader.onerror = function () { toast('Lecture du fichier impossible.', true); inputEl.value = ''; };
            reader.readAsText(file);
            inputEl.value = '';
        }

        /* ---------- Corbeille : restauration ---------- */
        function renderCorbeilleList() {
            var el = document.getElementById('manage-trash');
            if (!el) return;
            var corbeille = getSafeStorage(CORBEILLE_KEY, []);
            if (!corbeille.length) { el.innerHTML = '<div class="text-xs font-bold text-slate-400 italic">Corbeille vide.</div>'; return; }
            el.innerHTML = corbeille.slice(0, 20).map(function (c, i) {
                return '<div class="flex items-center justify-between bg-slate-50 rounded-lg px-3 py-2 border border-slate-200">' +
                    '<span class="text-[11px] font-bold text-slate-600 truncate"><i class="fa-solid fa-user-slash mr-2 text-slate-400"></i>' + sanitize(c.op && c.op.nom ? c.op.nom : '?') + ' <span class="text-slate-400">(' + sanitize(c.op && c.op.equipe ? c.op.equipe : '') + ')</span></span>' +
                    '<button onclick="restoreOperator(' + i + ')" class="px-3 py-1 rounded-lg text-[10px] font-black bg-emerald-50 text-emerald-600 hover:bg-emerald-100 flex-shrink-0 ml-2">Restaurer</button>' +
                '</div>';
            }).join('');
        }

        function restoreOperator(i) {
            if (!requireUnlock()) return;
            var corbeille = getSafeStorage(CORBEILLE_KEY, []);
            var entry = corbeille[i];
            if (!entry || !entry.op) return;
            var op = JSON.parse(JSON.stringify(entry.op));
            op.qualifs = (typeof op.qualifs === 'string' ? op.qualifs : '').split(',').map(function (s) { return s.trim(); }).filter(Boolean).join(',');
            if (typeof op.equipe !== 'string' || !op.equipe) op.equipe = 'P40A-A';
            var at = (typeof entry.idx === 'number' && entry.idx >= 0 && entry.idx <= database.length) ? entry.idx : database.length;
            database.splice(at, 0, op);
            corbeille.splice(i, 1);
            try { localStorage.setItem(CORBEILLE_KEY, JSON.stringify(corbeille)); } catch (e) {}
            persistData();
            renderTable();
            renderManageModal();
            fillCommonLists();
            toast('<i class="fa-solid fa-rotate-left mr-1"></i>' + sanitize(op.nom) + ' restauré.');
        }

        /* ---------- Code PIN ---------- */
        var pinMode = 'set'; // 'set' | 'check'

        function isUnlocked() {
            return !localStorage.getItem(PIN_KEY) || sessionStorage.getItem(UNLOCK_SESSION_KEY) === '1';
        }

        function requireUnlock() {
            if (isUnlocked()) return true;
            openPinModal();
            toast('<i class="fa-solid fa-lock mr-1"></i>Verrouillé : saisis le code PIN pour modifier.', true);
            return false;
        }

        function djb2(p) {
            var h = 5381;
            for (var i = 0; i < p.length; i++) { h = ((h << 5) + h + p.charCodeAt(i)) >>> 0; }
            return 'x' + h.toString(16);
        }

        async function hashPin(p) {
            var stored = null;
            try { stored = localStorage.getItem(PIN_KEY); } catch (e) {}
            // Pin posé en mode fallback : on vérifie aussi en fallback (évite le soft-lock cross-navigateur)
            if (stored && stored.indexOf('x') === 0) return djb2(p);
            try {
                if (window.crypto && crypto.subtle && window.TextEncoder) {
                    var buf = await crypto.subtle.digest('SHA-256', new TextEncoder().encode('qa_sliman_' + p));
                    return Array.from(new Uint8Array(buf)).map(function (b) { return b.toString(16).padStart(2, '0'); }).join('');
                }
            } catch (e) { /* fallback ci-dessous */ }
            return djb2(p);
        }

        function openPinModal() {
            var hasPin = !!localStorage.getItem(PIN_KEY);
            pinMode = hasPin ? 'check' : 'set';
            document.getElementById('pin-set-block').classList.toggle('hidden', hasPin);
            document.getElementById('pin-check-block').classList.toggle('hidden', !hasPin);
            document.getElementById('pin-remove-btn').classList.toggle('hidden', !hasPin);
            document.getElementById('pin-title').innerText = hasPin ? 'Déverrouillage' : 'Définir un code PIN';
            document.getElementById('pin-help').innerText = hasPin
                ? 'Le PIN protège les modifications (validation, ajout/suppression, import de sauvegarde, export CSV). L\'export de secours .json reste libre. Valable jusqu\'à la fermeture de l\'onglet.'
                : 'Définis un code pour protéger les modifications (validations, suppressions, ajout manuel). Laisse vide et ferme pour ne pas en mettre.';
            document.getElementById('pin-new').value = '';
            document.getElementById('pin-new2').value = '';
            document.getElementById('pin-enter').value = '';
            openModal('pin-modal');
        }

        async function pinPrimaryAction() {
            if (pinMode === 'set') await saveNewPin(); else await submitPin();
        }

        async function saveNewPin() {
            var p1 = document.getElementById('pin-new').value;
            var p2 = document.getElementById('pin-new2').value;
            if (p1.length < 4) { toast('Le code doit faire au moins 4 caractères.', true); return; }
            if (p1 !== p2) { toast('Les deux codes ne correspondent pas.', true); return; }
            var h = await hashPin(p1);
            localStorage.setItem(PIN_KEY, h);
            sessionStorage.setItem(UNLOCK_SESSION_KEY, '1');
            closeModal('pin-modal');
            toast('Code PIN défini. Les modifications restent ouvertes pour cette session.');
        }

        async function submitPin() {
            var p = document.getElementById('pin-enter').value;
            var h = await hashPin(p);
            if (h === localStorage.getItem(PIN_KEY)) {
                sessionStorage.setItem(UNLOCK_SESSION_KEY, '1');
                closeModal('pin-modal');
                toast('<i class="fa-solid fa-lock-open mr-1"></i>Déverrouillé pour cette session.');
            } else {
                toast('Code incorrect.', true);
            }
        }

        function removePin() {
            var p = document.getElementById('pin-enter').value;
            if (!p) { toast('Saisis le code PIN actuel dans le champ pour pouvoir le supprimer.', true); return; }
            var stored = null;
            try { stored = localStorage.getItem(PIN_KEY); } catch (e) {}
            hashPin(p).then(function (h) {
                var ok = (h === stored);
                var canCheck = (stored && stored.indexOf('x') === 0) || (window.crypto && crypto.subtle);
                if (!ok && !canCheck) {
                    // PIN créé dans un navigateur avec SHA-256, vérification impossible ici
                    if (confirm('Vérification impossible dans ce navigateur (le code a été créé ailleurs).\nSupprimer le code PIN quand même ?')) {
                        try { localStorage.removeItem(PIN_KEY); } catch (e) {}
                        sessionStorage.removeItem(UNLOCK_SESSION_KEY);
                        closeModal('pin-modal');
                        toast('Code PIN supprimé.');
                    }
                    return;
                }
                if (!ok) { toast('Code incorrect.', true); return; }
                if (!confirm('Supprimer le code PIN ? Toutes les modifications seront ouvertes à tous.')) return;
                try { localStorage.removeItem(PIN_KEY); } catch (e) {}
                sessionStorage.removeItem(UNLOCK_SESSION_KEY);
                closeModal('pin-modal');
                toast('Code PIN supprimé.');
            });
        }

        /* ---------- Ajout manuel au registre KPI ---------- */
        function openManualLogModal() {
            if (!requireUnlock()) return;
            var vSel = document.getElementById('ml-validateur');
            vSel.innerHTML = VALIDATORS_LIST.map(function (v) { return '<option value="' + sanitize(v.name) + '">' + sanitize(v.name) + '</option>'; }).join('');
            document.getElementById('ml-station').value = '';
            document.getElementById('ml-qualif').value = '';
            document.getElementById('ml-compagnon').value = '';
            document.getElementById('ml-type').value = 'Initiale';
            document.getElementById('ml-qls').value = '';
            var d = new Date();
            document.getElementById('ml-date').value = d.getFullYear() + '-' + ('0' + (d.getMonth() + 1)).slice(-2) + '-' + ('0' + d.getDate()).slice(-2);
            document.getElementById('ml-qcm').value = '';
            document.getElementById('ml-cw').value = getWeekNumber(d);
            openModal('manual-modal');
        }

        function saveManualLog() {
            if (!requireUnlock()) return;
            var qualif = document.getElementById('ml-qualif').value.trim();
            var compagnon = document.getElementById('ml-compagnon').value.trim();
            if (!qualif || !compagnon) { toast('QA et Compagnon sont obligatoires.', true); return; }
            var date = fromInputDate(document.getElementById('ml-date').value);
            bossKpiLog.push({
                poste: document.getElementById('ml-poste').value,
                station: document.getElementById('ml-station').value.trim(),
                qualif: qualif,
                compagnon: compagnon,
                type: document.getElementById('ml-type').value,
                qls: document.getElementById('ml-qls').value,
                validateur: document.getElementById('ml-validateur').value,
                date: date,
                qcm: document.getElementById('ml-qcm').value.trim(),
                cw: parseInt(document.getElementById('ml-cw').value, 10) || getWeekNumber(new Date()),
                timestamp: Date.now()
            });
            persistData();
            closeModal('manual-modal');
            toast('<i class="fa-solid fa-table-list mr-1"></i>Validation ajoutée au registre.');
            if (document.getElementById('view-reporting') && !document.getElementById('view-reporting').classList.contains('hidden')) renderReporting();
        }

        /* ---------- Export CSV ---------- */
        function exportBossCSV() {
            if (!requireUnlock()) return;
            var rows = [['Poste', 'Station', 'Nom de la QA', 'Nom du Compagnon', 'Init/Proro', 'QLS1/QLS2', 'Validée Par', 'Date Val. QA', 'QCM/Com.', 'CW']];
            bossKpiLog.forEach(function (l) {
                rows.push([l.poste, l.station, l.qualif, l.compagnon, l.type, l.qls, l.validateur, l.date, l.qcm, 'CW' + l.cw]);
            });
            var csv = rows.map(function (r) {
                return r.map(function (cell) { var c = (cell == null ? '' : String(cell)); return '"' + c.replace(/"/g, '""') + '"'; }).join(';');
            }).join('\r\n');
            var blob = new Blob(['\uFEFF' + csv], { type: 'text/csv;charset=utf-8;' });
            var a = document.createElement('a');
            a.href = URL.createObjectURL(blob);
            a.download = 'registre_validations_' + new Date().toISOString().slice(0, 10) + '.csv';
            document.body.appendChild(a);
            a.click();
            setTimeout(function () { URL.revokeObjectURL(a.href); a.remove(); }, 300);
            toast('<i class="fa-solid fa-file-excel mr-1"></i>CSV exporté (' + (rows.length - 1) + ' lignes).');
        }

        /* ---------- Recherche ---------- */
        var searchTimer = null;

        function debouncedSearch() {
            var input = document.getElementById('searchInput');
            var clearBtn = document.getElementById('clearSearchBtn');
            if (clearBtn) clearBtn.classList.toggle('hidden', !input.value);
            clearTimeout(searchTimer);
            searchTimer = setTimeout(runSearch, 220);
        }

        function runSearch() {
            var input = document.getElementById('searchInput');
            var box = document.getElementById('searchResults');
            if (!input || !box) return;
            var q = input.value.trim().toLowerCase();
            if (q.length < 2) { box.classList.add('hidden'); return; }
            var hits = [];
            database.forEach(function (op, oi) {
                if (op.nom.toLowerCase().indexOf(q) >= 0 || op.equipe.toLowerCase().indexOf(q) >= 0) {
                    hits.push({ oi: oi, qi: -1, label: op.nom, sub: 'Opérateur · ' + op.equipe });
                }
                getQualifs(op).forEach(function (kf) {
                    var hay = (kf.code + ' ' + kf.name).toLowerCase();
                    if (hay.indexOf(q) >= 0) {
                        hits.push({ oi: oi, qi: kf.idx, label: kf.code + ' — ' + kf.name, sub: op.nom + ' · ' + op.equipe });
                    }
                });
            });
            box.innerHTML = hits.length
                ? hits.slice(0, 25).map(function (h) {
                    return '<li onclick="jumpTo(' + h.oi + ',' + h.qi + ')" class="px-4 py-3 hover:bg-blue-50 cursor-pointer flex justify-between items-center gap-2">' +
                        '<div class="min-w-0"><div class="text-[12px] font-black truncate">' + sanitize(h.label) + '</div>' +
                        '<div class="text-[10px] font-bold text-slate-400 uppercase truncate">' + sanitize(h.sub) + '</div></div>' +
                        '<i class="fa-solid fa-arrow-right text-slate-300"></i></li>';
                }).join('')
                : '<li class="px-4 py-3 text-xs font-bold text-slate-400">Aucun résultat pour « ' + sanitize(input.value) + ' »</li>';
            box.classList.remove('hidden');
        }

        function clearSearch() {
            var input = document.getElementById('searchInput');
            if (input) input.value = '';
            debouncedSearch();
            hideSearchResults();
        }

        function hideSearchResults() {
            var box = document.getElementById('searchResults');
            if (box) box.classList.add('hidden');
        }

        function jumpTo(oi, qi) {
            var op = database[oi];
            if (!op) return;
            var eq = op.equipe || 'P40A-A';
            currentZone = eq.substring(0, 3); currentSecteur = eq.charAt(3); currentTeam = eq.charAt(5) || 'A';
            currentProgramme = programmeDeZone(currentZone); // V6 : P28 → A330, sinon A350
            statusFilter = null; // le résultat de la recherche doit être visible : on lève le filtre de statut
            if (document.getElementById('view-operators').classList.contains('hidden')) switchTab('operators');
            updateFilters();
            hideSearchResults();
            setTimeout(function () {
                var row = document.querySelector('#tableBody tr[data-op="' + (window.CSS && CSS.escape ? CSS.escape(op.nom) : op.nom.replace(/"/g, '\\"')) + '"]');
                if (!row) return;
                row.scrollIntoView({ behavior: 'smooth', block: 'center' });
                row.classList.add('op-flash');
                setTimeout(function () { row.classList.remove('op-flash'); }, 2100);
                if (qi >= 0) {
                    var card = row.querySelector('.q-card[data-qi="' + qi + '"]');
                    if (card) { card.classList.add('op-flash'); setTimeout(function () { card.classList.remove('op-flash'); }, 2100); }
                }
            }, 90);
        }

        /* ---------- Filtre registre + dates rapides ---------- */
        var regSearchTimer = null;
        function debouncedRegSearch() {
            clearTimeout(regSearchTimer);
            regSearchTimer = setTimeout(function () { renderReporting(); }, 250);
        }

        function quickDate(inputId, years) {
            var el = document.getElementById(inputId);
            if (!el) return;
            var base = el.value ? new Date(el.value) : new Date();
            if (isNaN(base.getTime())) base = new Date();
            base.setFullYear(base.getFullYear() + years);
            el.value = base.getFullYear() + '-' + ('0' + (base.getMonth() + 1)).slice(-2) + '-' + ('0' + base.getDate()).slice(-2);
        }

        /* ---------- F1 : onglet Échéances ---------- */
        function setEchanceFilter(f) {
            echanceFilter = f;
            var map = { all: 'btn-ech-all', expired: 'btn-ech-expired', '7': 'btn-ech-7', '30': 'btn-ech-30', '90': 'btn-ech-90' };
            Object.keys(map).forEach(function (k) {
                var b = document.getElementById(map[k]);
                if (!b) return;
                var on = (k === f);
                b.classList.toggle('bg-blue-600', on);
                b.classList.toggle('text-white', on);
                b.classList.toggle('shadow-sm', on);
                b.classList.toggle('font-black', on);
                b.classList.toggle('font-bold', !on);
                b.classList.toggle('text-slate-500', !on);
                b.classList.toggle('hover:bg-slate-200', !on);
            });
            renderEcheances();
        }

        function collectEcheances(ignoreFilter) {
            var rows = [];
            database.forEach(function (op, oi) {
                getQualifs(op).forEach(function (q) {
                    if (q.days === null) return; // initiales & à qualifier : pas d'échéance datée
                    rows.push({ oi: oi, qi: q.idx, op: op, q: q });
                });
            });
            rows.sort(function (a, b) { return a.q.days - b.q.days; }); // les plus proches d'abord (échues en tête)
            if (ignoreFilter) return rows; // V1 : la timeline/heatmap travaille sur TOUTES les échéances
            if (echanceFilter === 'expired') rows = rows.filter(function (r) { return r.q.status === 'expired'; });   // V8 : jour J compris, comme les cartes et la feuille imprimée
            else if (echanceFilter !== 'all') {
                var lim = parseInt(echanceFilter, 10);
                rows = rows.filter(function (r) { return r.q.days >= 0 && r.q.days <= lim; });
            }
            return rows;
        }

        /* ---------- V1 : bascule Liste/Timeline + fenêtre glissante ---------- */
        function setEchViewMode(m) {
            echViewMode = (m === 'timeline') ? 'timeline' : 'list';
            var map = { list: 'btn-echm-list', timeline: 'btn-echm-timeline' };
            Object.keys(map).forEach(function (k) {
                var b = document.getElementById(map[k]);
                if (!b) return;
                var on = (k === echViewMode);
                b.classList.toggle('bg-blue-600', on);
                b.classList.toggle('text-white', on);
                b.classList.toggle('shadow-sm', on);
                b.classList.toggle('font-black', on);
                b.classList.toggle('font-bold', !on);
                b.classList.toggle('text-slate-500', !on);
                b.classList.toggle('hover:bg-slate-200', !on);
            });
            // en mode Timeline : les filtres Tout/Échues/≤7j… ne s'appliquent qu'à la liste → on les masque, on montre la fenêtre
            var f = document.getElementById('ech-filters'), w = document.getElementById('ech-windows');
            if (f) f.classList.toggle('hidden', echViewMode === 'timeline');
            if (w) w.classList.toggle('hidden', echViewMode !== 'timeline');
            renderEcheances();
        }

        function setEchWindow(m) {
            echWindowMonths = (m === 6) ? 6 : (m === 12) ? 12 : 3;
            ['3', '6', '12'].forEach(function (k) {
                var b = document.getElementById('btn-echw-' + k);
                if (!b) return;
                var on = (parseInt(k, 10) === echWindowMonths);
                b.classList.toggle('bg-blue-600', on);
                b.classList.toggle('text-white', on);
                b.classList.toggle('shadow-sm', on);
                b.classList.toggle('font-black', on);
                b.classList.toggle('font-bold', !on);
                b.classList.toggle('text-slate-500', !on);
                b.classList.toggle('hover:bg-slate-200', !on);
            });
            renderEcheances();
        }

        // V9 : un seul regroupement de rendu — un enchaînement de modifications
        // (renderTable appelé plusieurs fois de suite : purge + import + restauration…)
        // ne reconstruit la liste qu'une seule fois, 60 ms après la dernière, et
        // JAMAIS zéro (le prochain appel relance un timer à la place).
        var echanceRenderTimer = null;
        function renderEcheances() {
            if (echanceRenderTimer) return;
            echanceRenderTimer = setTimeout(function () { echanceRenderTimer = null; renderEcheancesCore(); }, 60);
        }

        function renderEcheancesCore() {
            var el = document.getElementById('echances-list');
            var tl = document.getElementById('ech-timeline');
            if (!el) return;
            // V1 : dispatch Liste / Timeline
            if (echViewMode === 'timeline') {
                el.classList.add('hidden');
                if (tl) { tl.classList.remove('hidden'); renderTimeline(tl); }
                return;
            }
            el.classList.remove('hidden');
            if (tl) { tl.classList.add('hidden'); tl.innerHTML = ''; }
            var rows = collectEcheances();
            if (!rows.length) {
                el.innerHTML = '<div class="bg-white border border-slate-200 rounded-xl px-5 py-10 text-center"><div class="text-sm font-black text-slate-500"><i class="fa-solid fa-calendar-check mr-2 text-emerald-400"></i>Aucune échéance sur ce filtre.</div><div class="text-xs font-bold text-slate-400 mt-1">Change de fenêtre (≤ 30 j, ≤ 90 j) ou choisis « Tout ».</div></div>';
                return;
            }
            el.innerHTML = rows.map(function (r) {
                var d = r.q.days;
                var badge, cls;
                if (r.q.status === 'expired' && r.q.state === 'validated') { badge = 'J+' + Math.abs(d); cls = 'bg-slate-100 text-slate-500 border-slate-200'; }
                else if (r.q.status === 'expired') { badge = 'ÉCHUE J+' + Math.abs(d); cls = 'bg-red-100 text-red-700 border-red-300'; }   // V8 : jour J compris, comme les cartes
                else if (d <= 7) { badge = 'J-' + d; cls = 'bg-amber-100 text-amber-800 border-amber-300'; }
                else if (d <= 30) { badge = 'J-' + d; cls = 'bg-orange-50 text-orange-700 border-orange-200'; }
                else { badge = 'J-' + d; cls = 'bg-slate-100 text-slate-600 border-slate-200'; }
                var pill = '';
                if (r.q.state === 'validated') pill = '<span class="bg-emerald-100 text-emerald-700 border border-emerald-200 px-2 py-0.5 rounded-full text-[9px] font-black whitespace-nowrap">VALIDÉE</span>';
                else if (r.q.state === 'priority') pill = '<span class="bg-blue-100 text-blue-700 border border-blue-200 px-2 py-0.5 rounded-full text-[9px] font-black whitespace-nowrap">PRIORITÉ</span>';
                else if (r.q.state === 'standby') pill = '<span class="bg-slate-200 text-slate-600 border border-slate-300 px-2 py-0.5 rounded-full text-[9px] font-black whitespace-nowrap">STANDBY</span>';
                else if (r.q.state === 'disabled') pill = '<span class="bg-red-50 text-red-500 border border-red-200 px-2 py-0.5 rounded-full text-[9px] font-black whitespace-nowrap">PAS CAPABLE</span>';
                return '<div class="ech-row bg-white border border-slate-200 rounded-xl px-4 py-3 flex flex-wrap items-center gap-3 shadow-sm" onclick="openCardModal(' + r.oi + ',' + r.qi + ')" title="Ouvrir la qualification">' +
                    '<span class="mono text-[11px] font-black px-2.5 py-1.5 rounded-lg border ' + cls + ' min-w-[76px] text-center whitespace-nowrap">' + badge + '</span>' +
                    '<div class="min-w-0 flex-grow">' +
                        '<div class="text-[13px] font-black text-slate-800 uppercase truncate">' + sanitize(r.op.nom) + ' <span class="text-slate-400 font-bold">· ' + sanitize(r.op.equipe) + '</span></div>' +
                        '<div class="text-[11px] font-bold text-slate-500 truncate"><span class="mono text-blue-600">' + sanitize(r.q.code) + '</span> — ' + sanitize(r.q.name) + '</div>' +
                    '</div>' +
                    '<span class="badge-type ' + (r.q.isIni ? 'type-ini' : 'type-pro') + '">' + (r.q.isIni ? 'INI' : 'PRO') + '</span>' +
                    '<span class="mono text-[11px] font-bold text-slate-500 whitespace-nowrap">' + sanitize(r.q.date) + '</span>' +
                    pill +
                    (r.q.validator ? '<span class="text-[10px] font-bold text-slate-400 whitespace-nowrap hidden sm:inline"><i class="fa-solid fa-user-check mr-1"></i>' + sanitize(r.q.validator) + '</span>' : '') +
                    (r.q.state !== 'validated' ? '<button class="ech-fast" onclick="event.stopPropagation(); quickValidate(' + r.oi + ',' + r.qi + ', this)" title="Valider en 1 clic (bouton Annuler dans le message)"><i class="fa-solid fa-check text-[10px]"></i></button>' : '') +
                    '<i class="fa-solid fa-chevron-right text-slate-300 ml-auto"></i>' +
                '</div>';
            }).join('') +
            '<div class="text-[10px] font-bold text-slate-400 text-center mt-1">' + rows.length + ' qualification(s) datée(s) — cliquer une ligne ouvre le panneau d\'actions</div>';
        }

        /* ---------- V1 : timeline Gantt (CSS pur, offline-safe) ---------- */
        function renderTimeline(container) {
            var rows = collectEcheances(true);   // toutes les échéances, non filtrées
            var today = new Date(); today.setHours(0, 0, 0, 0);
            var winDays = Math.round(echWindowMonths * 30.44);
            var horizon = new Date(today.getTime() + winDays * 86400000);
            var MLbl = ['JAN', 'FEV', 'MARS', 'AVR', 'MAI', 'JUIN', 'JUIL', 'AOUT', 'SEPT', 'OCT', 'NOV', 'DEC'];
            // mois de la fenêtre (1er du mois EN COURS inclus — une échéance de ce mois-ci doit apparaître)
            var months = [];
            var m = new Date(today.getFullYear(), today.getMonth(), 1);
            while (m <= horizon && months.length < 24) { months.push(new Date(m)); m = new Date(m.getFullYear(), m.getMonth() + 1, 1); }
            function pct(ms) { return Math.max(0, Math.min(100, (ms - today.getTime()) / (winDays * 86400000) * 100)); }
            var gridlines = months.map(function (mo) { return '<div class="tl-grid month-start" style="left:' + pct(mo.getTime()).toFixed(2) + '%"></div>'; }).join('');
            var monthLbls = months.map(function (mo) { return '<span class="tl-month-lbl" style="left:' + pct(mo.getTime()).toFixed(2) + '%">' + MLbl[mo.getMonth()] + '</span>'; }).join('');

            // groupement par opérateur (tri alphabétique), échues + à venir mélangées
            var byOp = {};
            rows.forEach(function (r) {
                if (!byOp[r.oi]) byOp[r.oi] = { op: r.op, exp: [], fut: [] };
                if (r.q.days < 0) byOp[r.oi].exp.push(r); else if (r.q.days <= winDays) byOp[r.oi].fut.push(r);
            });
            var ois = Object.keys(byOp).filter(function (oi) { return byOp[oi].exp.length || byOp[oi].fut.length; });
            ois.sort(function (a, b) { return byOp[a].op.nom.localeCompare(byOp[b].op.nom, 'fr'); });
            var totalExp = ois.reduce(function (s, oi) { return s + byOp[oi].exp.length; }, 0);

            if (!ois.length) {
                container.innerHTML = '<div class="bg-white border border-slate-200 rounded-xl px-5 py-10 text-center"><div class="text-sm font-black text-slate-500"><i class="fa-solid fa-plane mr-2 text-blue-300"></i>Aucune échéance sur ' + echWindowMonths + ' mois.</div></div>';
                return;
            }

            var body = ois.map(function (oi) {
                var grp = byOp[oi];
                var expBars = grp.exp.map(function (r, k) {
                    return '<div class="tl-bar bar-exp" style="left:0%;min-width:12px;z-index:' + (3 - Math.min(k, 2)) + '" title="' + sanitize(grp.op.nom) + ' · ' + sanitize(r.q.code) + ' — ÉCHUE depuis ' + Math.abs(r.q.days) + ' j" onclick="event.stopPropagation();openCardModal(' + r.oi + ',' + r.qi + ')">⚠ ' + sanitize(r.q.code) + '</div>';
                }).join('');
                var futBars = grp.fut.map(function (r) {
                    var d = r.q.days;
                    var cls = d <= 30 ? 'bar-30' : d <= 90 ? 'bar-90' : 'bar-far';
                    var left = Math.min(96, (d / winDays) * 100);
                    return '<div class="tl-bar ' + cls + '" style="left:' + left.toFixed(2) + '%;min-width:12px" title="' + sanitize(grp.op.nom) + ' · ' + sanitize(r.q.code) + ' · ' + sanitize(r.q.date) + ' (J-' + d + ')" onclick="event.stopPropagation();openCardModal(' + r.oi + ',' + r.qi + ')">' + sanitize(r.q.code) + '</div>';
                }).join('');
                return '<div class="tl-row"><div class="tl-name" title="' + sanitize(grp.op.nom) + ' · ' + sanitize(grp.op.equipe) + '">' + sanitize(grp.op.nom) + '</div><div class="tl-track">' + gridlines + '<div class="tl-today" style="left:0%"></div>' + expBars + futBars + '</div></div>';
            }).join('');

            var chip = totalExp ? '<span class="bg-red-100 text-red-700 border border-red-200 px-2.5 py-1 rounded-full text-[10px] font-black whitespace-nowrap"><i class="fa-solid fa-triangle-exclamation mr-1"></i>' + totalExp + ' échue(s) — barre ⚠ à gauche</span>' : '';
            var html = '<div class="bg-white border border-slate-200 rounded-2xl p-4 flex flex-col gap-3">' +
                '<div class="flex flex-wrap items-center gap-2 text-xs font-black text-slate-700 uppercase"><i class="fa-solid fa-chart-gantt text-blue-500 mr-1"></i>Timeline ' + echWindowMonths + ' mois · ' + ois.length + ' opérateur(s) · ' + (rows.length - totalExp) + ' échéance(s) à venir ' + chip + '</div>' +
                '<div class="flex items-center"><div class="tl-name" style="position:static;background:transparent">Opérateur</div><div style="position:relative;flex-grow:1;height:18px">' + monthLbls + '</div></div>' +
                '<div class="tl-scroll">' + body + '</div>' +
                '<div class="flex flex-wrap gap-3 text-[10px] font-bold text-slate-500 border-t border-slate-100 pt-2">' +
                    '<span><i class="fa-solid fa-square inline-block" style="color:#DC2626"></i> Échue</span>' +
                    '<span><i class="fa-solid fa-square inline-block" style="color:#EA580C"></i> ≤ 30 j</span>' +
                    '<span><i class="fa-solid fa-square inline-block" style="color:#D97706"></i> ≤ 90 j</span>' +
                    '<span><i class="fa-solid fa-square inline-block" style="color:#2563EB"></i> Au-delà</span>' +
                    '<span class="text-slate-400"><i class="fa-solid fa-hand-pointer mr-1"></i>Clique une barre = agir sur la qualification</span>' +
                '</div>' +
            '</div>';
            container.innerHTML = html + renderHeatmap(rows, months, today);
        }

        /* ---------- V2 : heatmap prévisionnel opérateurs × mois ---------- */
        function renderHeatmap(rows, months, today) {
            var MLbl = ['JANVIER', 'FEVRIER', 'MARS', 'AVRIL', 'MAI', 'JUIN', 'JUILLET', 'AOUT', 'SEPTEMBRE', 'OCTOBRE', 'NOVEMBRE', 'DECEMBRE'];
            var mkeys = months.map(function (mo) { return mo.getFullYear() * 12 + mo.getMonth(); });
            var counts = {}, colTot = {}, ois = [];
            rows.forEach(function (r) {
                if (r.q.days === null || r.q.days < 0) return;   // échues : hors heatmap (déjà dans la timeline ⚠)
                var dt = new Date(today.getTime() + r.q.days * 86400000);
                var mk = dt.getFullYear() * 12 + dt.getMonth();
                var ci = mkeys.indexOf(mk);
                if (ci < 0) return;   // hors fenêtre : ne pas créer de ligne vide
                if (ois.indexOf(r.oi) < 0) ois.push(r.oi);
                if (!counts[r.oi]) counts[r.oi] = {};
                counts[r.oi][ci] = (counts[r.oi][ci] || 0) + 1;
                colTot[ci] = (colTot[ci] || 0) + 1;
            });
            ois.sort(function (a, b) {
                var na = (database[a] && database[a].nom) || '', nb = (database[b] && database[b].nom) || '';
                return na.localeCompare(nb, 'fr');
            });
            if (!ois.length) return '';
            var critCi = -1, critN = 0;
            Object.keys(colTot).forEach(function (k) { if (colTot[k] > critN) { critN = colTot[k]; critCi = parseInt(k, 10); } });

            var cols = 'display:grid;grid-template-columns:140px repeat(' + months.length + ',1fr);gap:2px;align-items:center;';
            var head = '<div style="' + cols + 'margin-bottom:3px"><div></div>' + months.map(function (mo, ci) {
                return '<div class="text-center text-[9px] font-black ' + (ci === critCi ? 'text-red-600' : 'text-slate-400') + '">' + MLbl[mo.getMonth()].slice(0, 3) + '<br><span class="text-[8px] text-slate-300 font-bold">' + String(mo.getFullYear()).slice(2) + '</span></div>';
            }).join('') + '</div>';
            var body = ois.map(function (oi) {
                var op = database[oi] || { nom: '?' };
                var cells = months.map(function (mo, ci) {
                    var n = (counts[oi] && counts[oi][ci]) || 0;
                    var lvl = n === 0 ? '' : n === 1 ? ' lvl-1' : n === 2 ? ' lvl-2' : n === 3 ? ' lvl-3' : ' lvl-4';
                    var crit = (n > 0 && ci === critCi) ? ' crit' : '';
                    return '<div class="hm-cell' + lvl + crit + '" title="' + sanitize(op.nom) + ' · ' + MLbl[mo.getMonth()] + ' ' + mo.getFullYear() + ' · ' + n + ' échéance(s)">' + (n || '') + '</div>';
                }).join('');
                return '<div style="' + cols + '"><div class="text-[10px] font-black text-slate-600 uppercase truncate pr-2" title="' + sanitize(op.nom) + '">' + sanitize(op.nom) + '</div>' + cells + '</div>';
            }).join('');
            return '<div class="bg-white border border-slate-200 rounded-2xl p-4">' +
                '<div class="text-xs font-black text-slate-700 uppercase mb-1"><i class="fa-solid fa-table-cells text-amber-500 mr-2"></i>Heatmap prévisionnel — opérateurs × mois</div>' +
                '<div class="text-[10px] font-bold text-slate-400 mb-3">Rouge foncé = mois chargé en échéances. Case cerclée = mois le plus tendu de la fenêtre.</div>' +
                head + body +
            '</div>';
        }

        function exportEcheancesCSV() {
            if (!requireUnlock()) return;
            var rows = collectEcheances();
            if (!rows.length) { toast('Aucune échéance à exporter sur ce filtre.', true); return; }
            var lines = [['Opérateur', 'Équipe', 'Code', 'Qualification', 'Type', 'Échéance', 'Jours', 'Statut', 'Validateur']];
            rows.forEach(function (r) {
                var statut = r.q.state === 'validated' ? 'Validée' : (r.q.days < 0 ? 'Échue' : (r.q.days <= 7 ? 'Urgent (<=7j)' : 'À venir'));
                lines.push([r.op.nom, r.op.equipe, r.q.code, r.q.name, r.q.isIni ? 'Initiale' : 'Prorogation', r.q.date, r.q.days, statut, r.q.validator || '']);
            });
            var csv = lines.map(function (row) {
                return row.map(function (cell) { return '"' + String(cell).replace(/"/g, '""') + '"'; }).join(';');
            }).join('\r\n');
            var blob = new Blob(['\uFEFF' + csv], { type: 'text/csv;charset=utf-8;' });
            var a = document.createElement('a');
            a.href = URL.createObjectURL(blob);
            a.download = 'echances_' + new Date().toISOString().slice(0, 10) + '.csv';
            document.body.appendChild(a);
            a.click();
            setTimeout(function () { URL.revokeObjectURL(a.href); a.remove(); }, 300);
            toast('<i class="fa-solid fa-file-csv mr-1"></i>' + rows.length + ' échéance(s) exportée(s) (CSV Excel).');
        }

        /* ---------- F2 : fiche opérateur imprimable ---------- */
        function openFiche(oi) {
            var op = database[oi];
            if (!op) return;
            var qualifs = getQualifs(op);
            var st = computeOpStats(op);
            var today = new Date().toLocaleDateString('fr-FR');
            var qrows = qualifs.map(function (q) {
                var badge;
                if (q.state === 'validated') badge = '<b style="color:#059669">Validée</b>';
                else if (q.state === 'disabled') badge = '<b style="color:#DC2626">Pas capable</b>';
                else if (q.state === 'standby') badge = '<b style="color:#64748B">Standby</b>';
                else if (q.status === 'expired') badge = '<b style="color:#DC2626">Échue</b>';
                else if (q.date === 'À QUALIFIER') badge = '<b style="color:#0284C7">À qualifier</b>';
                else if (q.days !== null && q.days <= 15) badge = '<b style="color:#D97706">Expire dans ' + q.days + ' j</b>';
                else badge = '<b style="color:#475569">Valide</b>';
                return '<tr>' +
                    '<td class="mono">' + sanitize(q.code) + '</td>' +
                    '<td>' + sanitize(q.name) + '</td>' +
                    '<td style="text-align:center">' + (q.isIni ? 'Initiale' : 'Prorogation') + '</td>' +
                    '<td class="mono" style="text-align:center">' + sanitize(q.date) + '</td>' +
                    '<td style="text-align:center">' + badge + '</td>' +
                    '<td>' + sanitize(q.validator) + '</td>' +
                    '<td>' + sanitize(q.note) + '</td>' +
                '</tr>';
            }).join('');
            var sheet = document.getElementById('fiche-sheet');
            if (!sheet) return;
            sheet.innerHTML =
                '<div class="no-print flex justify-end gap-2 mb-3">' +
                    '<button onclick="printFiche()" class="bg-blue-600 hover:bg-blue-500 text-white px-4 py-2 rounded-lg text-xs font-black uppercase shadow-md flex items-center gap-2"><i class="fa-solid fa-print"></i> Imprimer la fiche</button>' +
                    '<button onclick="closeFiche()" class="bg-slate-200 hover:bg-slate-300 text-slate-700 px-4 py-2 rounded-lg text-xs font-black uppercase flex items-center gap-2"><i class="fa-solid fa-xmark"></i> Fermer</button>' +
                '</div>' +
                '<div style="border-bottom:3px solid #0F172A;padding-bottom:10px;margin-bottom:16px;display:flex;justify-content:space-between;align-items:flex-end;gap:12px">' +
                    '<div><div style="font-weight:900;text-transform:uppercase;font-size:17px;letter-spacing:-.02em">Fiche Opérateur QA</div>' +
                    '<div style="font-size:11px;font-weight:800;color:#64748B;text-transform:uppercase;letter-spacing:.08em">Planing QA Sliman — document de travail atelier</div></div>' +
                    '<div style="font-size:11px;font-weight:800;color:#64748B">Éditée le ' + today + '</div>' +
                '</div>' +
                '<div style="display:flex;flex-wrap:wrap;gap:14px;align-items:center;margin-bottom:16px">' +
                    '<span class="op-pastille ' + opHue(op.nom) + '" style="width:44px;height:44px;font-size:14px">' + sanitize(op.nom.split(/\s+/).map(function (w) { return w.charAt(0); }).join('').slice(0, 2).toUpperCase()) + '</span>' +
                    '<div><div style="font-size:19px;font-weight:900;text-transform:uppercase">' + sanitize(op.nom) + '</div>' +
                    '<div style="font-size:12px;font-weight:800;color:#64748B">Équipe ' + sanitize(op.equipe) + '</div></div>' +
                    '<div style="margin-left:auto;display:flex;gap:8px;flex-wrap:wrap">' +
                        '<span style="background:#ECFDF5;border:1px solid #A7F3D0;color:#065F46;padding:5px 10px;border-radius:999px;font-size:11px;font-weight:900">' + st.valides + '/' + st.total + ' validées</span>' +
                        (st.echues ? '<span style="background:#FEF2F2;border:1px solid #FECACA;color:#B91C1C;padding:5px 10px;border-radius:999px;font-size:11px;font-weight:900">' + st.echues + ' échue(s)</span>' : '') +
                        (st.warn ? '<span style="background:#FFFBEB;border:1px solid #FDE68A;color:#92400E;padding:5px 10px;border-radius:999px;font-size:11px;font-weight:900">' + st.warn + ' à risque</span>' : '') +
                        (st.aqual ? '<span style="background:#F0F9FF;border:1px solid #BAE6FD;color:#075985;padding:5px 10px;border-radius:999px;font-size:11px;font-weight:900">' + st.aqual + ' à qualifier</span>' : '') +
                    '</div>' +
                '</div>' +
                (qualifs.length
                    ? '<table><thead><tr><th>Code</th><th>Qualification</th><th style="text-align:center">Type</th><th style="text-align:center">Échéance</th><th style="text-align:center">Statut</th><th>Validateur</th><th>Note</th></tr></thead><tbody>' + qrows + '</tbody></table>'
                    : '<div style="padding:18px;text-align:center;color:#64748B;font-weight:700;font-size:13px">Aucune qualification enregistrée pour cet opérateur.</div>') +
                '<div style="margin-top:16px;font-size:10px;font-weight:700;color:#94A3B8;text-align:right">Document généré localement — aucune donnée envoyée sur le réseau.</div>';
            document.getElementById('fiche-print').classList.add('fiche-open');
        }

        function printFiche() {
            var fp = document.getElementById('fiche-print');
            if (!fp || !fp.classList.contains('fiche-open')) return; // garde : rien à imprimer
            document.body.classList.remove('print-ech');   // V8-3 : les deux flux d'impression sont exclusifs
            document.body.classList.add('print-fiche');
            var cleanup = function () {
                document.body.classList.remove('print-fiche');
                if (window.onafterprint === cleanup) window.onafterprint = null;   // V8-3 : ne pas écraser le flux suivant
            };
            window.onafterprint = cleanup;
            window.print();
            // file:// Edge : onafterprint n'est pas garanti → filet de sécurité (un seul actif à la fois)
            clearTimeout(window.__printTimer);
            window.__printTimer = setTimeout(cleanup, 2500);
        }

        /* ---------- V8-3 : impression de la liste des Échéances (feuille atelier) ---------- */
        function printEcheancesListe() {
            // En mode Timeline, la fenêtre 3/6/12 mois ne s'applique qu'à la timeline :
            // on bascule d'abord en Liste pour que la feuille reflète bien l'écran.
            if (echViewMode === 'timeline') setEchViewMode('list');
            var rows = collectEcheances();   // respecte le filtre actif (Tout/Échues/≤7 j…)
            if (!rows.length) { toast('Aucune échéance à imprimer sur ce filtre.', true); return; }
            var fLabel = { all: 'Toutes les échéances', expired: 'Échues uniquement', '7': 'Échéant sous 7 jours', '30': 'Échéant sous 30 jours', '90': 'Échéant sous 90 jours' }[echanceFilter] || 'Toutes les échéances';
            var today = new Date().toLocaleDateString('fr-FR');
            var echues = rows.filter(function (r) { return r.q.status === 'expired'; }).length;   // MÊME cascade que les cartes : le jour J compte échu
            var body = rows.map(function (r) {
                // même priorité d'affichage que les cartes : l'état (validée/priorité…) prime
                var etat, etatCls;
                if (r.q.state === 'validated') { etat = 'VALIDÉE'; etatCls = 'etat-valide'; }
                else if (r.q.state === 'priority') { etat = 'PRIORITÉ'; etatCls = ''; }
                else if (r.q.state === 'standby') { etat = 'STANDBY'; etatCls = ''; }
                else if (r.q.state === 'disabled') { etat = 'PAS CAPABLE'; etatCls = ''; }
                else if (r.q.status === 'expired') { etat = 'ÉCHUE'; etatCls = 'etat-echue'; }   // jour J compris, comme les cartes
                else if (r.q.days <= 7) { etat = 'URGENT (J-' + r.q.days + ')'; etatCls = ''; }
                else if (r.q.days <= 15) { etat = 'BIENTÔT (J-' + r.q.days + ')'; etatCls = ''; }
                else { etat = 'À SUIVRE (J-' + r.q.days + ')'; etatCls = ''; }
                var reste = r.q.status === 'expired' ? 'J+' + Math.abs(r.q.days) : 'J-' + r.q.days;
                return '<tr>' +
                    '<td>' + sanitize(r.op.nom) + '</td>' +
                    '<td>' + sanitize(r.op.equipe) + '</td>' +
                    '<td>' + sanitize(r.q.code) + ' — ' + sanitize(r.q.name) + '</td>' +
                    '<td class="c">' + sanitize(r.q.date) + '</td>' +
                    '<td class="c">' + reste + '</td>' +
                    '<td class="c ' + etatCls + '">' + etat + '</td>' +
                    '</tr>';
            }).join('');
            document.getElementById('ech-print').innerHTML =
                '<div class="ep-head">' +
                    '<div><div class="ep-title">Liste des Échéances QA</div>' +
                    '<div class="ep-sub">Planing QA Sliman — document de travail atelier</div></div>' +
                    '<div class="ep-meta">Éditée le ' + today + '<br>Filtre : ' + fLabel + '<br>' + rows.length + ' ligne(s) — dont ' + echues + ' échue(s)</div>' +
                '</div>' +
                '<table class="ep-table"><thead><tr><th>Opérateur</th><th>Équipe</th><th>Qualification</th><th class="c">Échéance</th><th class="c">Reste</th><th class="c">État</th></tr></thead><tbody>' + body + '</tbody></table>' +
                '<div class="ep-foot">Document généré localement — aucune donnée envoyée sur le réseau.</div>';
            document.body.classList.remove('print-fiche');   // XOR : jamais les deux flux
            document.body.classList.add('print-ech');
            var cleanup = function () {
                document.body.classList.remove('print-ech');
                if (window.onafterprint === cleanup) window.onafterprint = null;   // V8-3 : ne pas écraser le flux suivant
            };
            window.onafterprint = cleanup;
            window.print();
            // file:// Edge : onafterprint n'est pas garanti → filet de sécurité (un seul actif à la fois)
            clearTimeout(window.__printTimer);
            window.__printTimer = setTimeout(cleanup, 2500);
        }

        function closeFiche() {
            var f = document.getElementById('fiche-print');
            if (f) f.classList.remove('fiche-open');
        }

        /* ---------- Zoom ---------- */
        function applyZoom() {
            document.body.style.zoom = (currentZoom / 100);
            var zl = document.getElementById('zoom-level');
            if (zl) zl.innerText = currentZoom + '%';
            try { localStorage.setItem(ZOOM_KEY, currentZoom); } catch (e) {}
        }
        function zoomIn() { currentZoom = Math.min(140, currentZoom + 10); applyZoom(); }
        function zoomOut() { currentZoom = Math.max(70, currentZoom - 10); applyZoom(); }

        /* ---------- Tour guidé ---------- */
        var tourSteps = [
            { sel: '#search-container', title: 'La Recherche', text: 'Tape un nom d\'opérateur ou un code qualification : les résultats apparaissent en direct. Un clic resulte l\'opérateur et surligne la carte concernée.' },
            { sel: '#filters-container', title: 'Les Filtres', text: 'Zone (P40/P50), Ligne (A/B/C) et Équipe (A/B) pilotent le tableau ci-dessous. L\'équipe se déduit automatiquement (ex : P40 + A + Équipe A = P40A-A).' },
            { sel: '#tableBody tr', title: 'Les Cartes Qualifications', text: 'Chaque carte = une qualification. Le bandeau coloré gauche indique le type (bleu = Initiale, orange = Prorogation). Un CLIC sur une carte ouvre le panneau d\'actions : statut, échéance, validateur, note, suppression.' },
            { sel: '#btn-validated-modal', title: 'Le Compteur de Validations', text: 'Ce compteur agrège toutes les qualifications passées en « Validée ». Un clic ouvre la liste complète avec possibilité d\'annuler chaque validation.' },
            { sel: '#tab-reporting', title: 'KPI & Direction', text: 'Onglet réservé à la direction : graphiques P40/P50, performance par validateur (tableau QLS), registre officiel avec ajout manuel et export CSV Excel.' },
            { sel: '#tab-hebdo', title: 'Le Résumé Hebdo', text: 'Synthèse de la semaine (mercredi → mercredi) : prorogations échues, initiales et prorogations validées, par secteur. Bouton « Copier le résumé » pour le coller dans ton mail ou chat.' }
        ];
        var tourIdx = 0;

        function startTour() {
            tourIdx = 0;
            document.getElementById('tour-overlay').style.display = 'block';
            document.getElementById('tour-dialog').style.display = 'block';
            showTourStep();
        }

        function showTourStep() {
            var s = tourSteps[tourIdx];
            var el = document.querySelector(s.sel);
            if (el) el.scrollIntoView({ block: 'center' });
            document.getElementById('tour-title').innerText = s.title;
            document.getElementById('tour-text').innerText = s.text;
            document.getElementById('tour-step-counter').innerText = (tourIdx + 1) + ' / ' + tourSteps.length;
            setTimeout(positionTourBox, 150);
        }

        function positionTourBox() {
            var s = tourSteps[tourIdx];
            var el = document.querySelector(s.sel);
            var box = document.getElementById('tour-focus-box');
            if (!el || !box) return;
            var r = el.getBoundingClientRect();
            box.style.top = (r.top - 6) + 'px';
            box.style.left = (r.left - 6) + 'px';
            box.style.width = (r.width + 12) + 'px';
            box.style.height = (r.height + 12) + 'px';
            box.classList.add('active');
        }

        function nextTourStep() {
            tourIdx++;
            if (tourIdx >= tourSteps.length) { endTour(); toast('Tour terminé — bonne utilisation !'); }
            else showTourStep();
        }

        function endTour() {
            var ov = document.getElementById('tour-overlay');
            var dlg = document.getElementById('tour-dialog');
            var box = document.getElementById('tour-focus-box');
            if (ov) ov.style.display = 'none';
            if (dlg) dlg.style.display = 'none';
            if (box) box.classList.remove('active');
        }

        window.addEventListener('resize', function () {
            var ov = document.getElementById('tour-overlay');
            if (ov && ov.style.display === 'block') positionTourBox();
        });
        /* ---------- Onglet KPI & Direction ---------- */
        function changeKpiView(view) { currentKpiView = view; renderReporting(); }

        function renderReporting() {
            var activeCls = "flex-1 px-5 py-2 rounded-md text-xs font-black bg-blue-600 text-white shadow-sm";
            var inactiveCls = "flex-1 px-5 py-2 rounded-md text-xs font-bold text-slate-500 hover:bg-slate-200";

            var btnTout = document.getElementById('btn-kpi-Tout'); if (btnTout) btnTout.className = (currentKpiView === 'Tout') ? activeCls : inactiveCls;
            var btnP40 = document.getElementById('btn-kpi-P40'); if (btnP40) btnP40.className = (currentKpiView === 'P40') ? activeCls : inactiveCls;
            var btnP50 = document.getElementById('btn-kpi-P50'); if (btnP50) btnP50.className = (currentKpiView === 'P50') ? activeCls : inactiveCls;

            var p40Container = document.getElementById('kpi-section-p40');
            var p50Container = document.getElementById('kpi-section-p50');
            if (p40Container) p40Container.style.display = (currentKpiView === 'Tout' || currentKpiView === 'P40') ? 'flex' : 'none';
            if (p50Container) p50Container.style.display = (currentKpiView === 'Tout' || currentKpiView === 'P50') ? 'flex' : 'none';

            var tbody = document.getElementById('boss-registry-tbody');
            if (tbody) {
                var vSel = document.getElementById('reg-validator-filter');
                if (vSel && vSel.options.length <= 1) {
                    vSel.innerHTML = '<option value="">Tous</option>' + VALIDATORS_LIST.map(function (v) { return '<option value="' + sanitize(v.name) + '">' + sanitize(v.name) + '</option>'; }).join('');
                }
                var vFilt = vSel ? vSel.value : '';
                var sEl = document.getElementById('reg-search-filter');
                var sFilt = sEl ? sEl.value.trim().toLowerCase() : '';
                var logs = currentKpiView === 'Tout' ? bossKpiLog : bossKpiLog.filter(function (l) { return l.poste === currentKpiView; });
                if (vFilt) logs = logs.filter(function (l) { return (l.validateur || '') === vFilt; });
                if (sFilt) logs = logs.filter(function (l) { return [l.qualif, l.compagnon, l.station, l.qcm, l.type].join(' ').toLowerCase().indexOf(sFilt) >= 0; });
                var countEl = document.getElementById('reg-count');
                if (countEl) countEl.innerText = logs.length + ' ligne(s)' + ((vFilt || sFilt) ? ' (filtré sur ' + bossKpiLog.length + ')' : '');
                if (!logs.length) {
                    tbody.innerHTML = '<tr><td colspan="10" class="px-4 py-6 text-center text-xs font-bold text-slate-400">Aucune validation enregistrée pour ce filtre.</td></tr>';
                } else {
                    tbody.innerHTML = logs.slice().reverse().map(function (log) {
                        return '<tr class="hover:bg-blue-50 transition-colors border-b border-slate-50">' +
                            '<td class="font-bold">' + sanitize(log.poste) + '</td><td>' + sanitize(log.station) + '</td><td class="font-mono text-blue-600">' + sanitize(log.qualif) + '</td>' +
                            '<td class="font-bold">' + sanitize(log.compagnon) + '</td>' +
                            '<td><span class="px-2 py-0.5 rounded-full text-[9px] font-black border ' + (log.type === 'Initiale' ? 'bg-sky-100 text-sky-800 border-sky-200' : 'bg-orange-100 text-orange-800 border-orange-200') + '">' + sanitize(log.type) + '</span></td>' +
                            '<td class="text-center">' + (sanitize(log.qls) || '-') + '</td><td class="font-bold text-emerald-600">' + sanitize(log.validateur) + '</td>' +
                            '<td class="mono text-center">' + sanitize(log.date) + '</td><td class="font-black text-center">' + sanitize(log.qcm) + '</td><td class="text-center font-bold">CW' + log.cw + '</td>' +
                        '</tr>';
                    }).join('');
                }
            }

            if (window.Chart) {
                updateChart('P40', 'bossKpiChartP40');
                updateChart('P50', 'bossKpiChartP50');
            }
            drawQlsTable();
        }

        function drawQlsTable() {
            var container = document.getElementById('qls-table-container');
            if (!container) return;

            var weeks = new Set();
            var currentWeek = getWeekNumber(new Date());
            weeks.add(currentWeek);

            // Fenêtre glissante : 8 dernières semaines (modulo 53 = passage d'année en janvier)
            function inWeekWindow(cw) {
                var diff = currentWeek - cw;
                if (diff < 0) diff += 53;
                return diff >= 1 && diff <= 7;
            }
            bossKpiLog.forEach(function (log) {
                var cw = parseInt(log.cw);
                if (!isNaN(cw) && inWeekWindow(cw)) weeks.add(cw);
            });

            var sortedWeeks = Array.from(weeks).sort(function (a, b) { return a - b; });

            var stats = {};
            var weekTotals = {};

            VALIDATORS_LIST.forEach(function (v) {
                stats[v.alias] = {};
                sortedWeeks.forEach(function (cw) { stats[v.alias][cw] = { init: 0, proro: 0, tot: 0 }; });
            });
            sortedWeeks.forEach(function (cw) { weekTotals[cw] = 0; });

            bossKpiLog.forEach(function (log) {
                var cw = parseInt(log.cw);
                if (!sortedWeeks.includes(cw)) return;
                var valName = log.validateur;
                if (!valName) return;
                var valObj = VALIDATORS_LIST.find(function (v) { return valName.indexOf(v.alias) >= 0 || valName === v.name; });
                if (valObj) {
                    if (log.type === 'Initiale') stats[valObj.alias][cw].init++;
                    else stats[valObj.alias][cw].proro++;
                    stats[valObj.alias][cw].tot++;
                    weekTotals[cw]++;
                }
            });

            var getBg = function (val) {
                if (val === 0) return 'bg-[#E6A5A5]';
                if (val <= 4) return 'bg-[#FDE047]';
                return 'bg-[#A7F3D0]';
            };
            var getTotBg = function (val) {
                if (val === 0) return 'bg-slate-300 text-slate-800';
                if (val <= 2) return 'bg-[#FCA5A5]';
                if (val <= 4) return 'bg-[#FDE047]';
                return 'bg-[#A7F3D0]';
            };

            var html = '<div class="flex justify-center overflow-x-auto w-full pb-2"><table class="w-full sm:w-auto mx-auto text-[10px] text-center border-collapse border border-slate-400 qls-table">';
            html += '<thead><tr><th class="w-20 bg-slate-200 border border-slate-400"></th><th class="w-12 bg-slate-200 border border-slate-400"></th>';
            sortedWeeks.forEach(function (cw) { html += '<th class="bg-slate-200 border border-slate-400 font-bold min-w-[60px]">Sem. ' + cw + '</th><th class="bg-slate-300 border border-slate-400 font-bold min-w-[60px]">Total CW' + cw + '</th>'; });
            html += '</tr></thead><tbody class="bg-white">';

            VALIDATORS_LIST.forEach(function (v) {
                var row1 = '<tr><td rowspan="2" class="font-bold text-slate-800 bg-slate-100 border border-slate-400 align-middle">' + v.alias + '</td><td class="text-slate-800 bg-slate-100 border border-slate-400 p-1">Prorog</td>';
                var row2 = '<tr><td class="text-slate-800 bg-slate-100 border border-slate-400 p-1">Init</td>';
                sortedWeeks.forEach(function (cw) {
                    var s = stats[v.alias][cw];
                    row1 += '<td class="' + getBg(s.proro) + ' border border-slate-400 font-mono">' + s.proro + '</td><td rowspan="2" class="align-middle ' + getTotBg(s.tot) + ' border border-slate-400 font-mono font-bold text-sm">' + s.tot + '</td>';
                    row2 += '<td class="' + getBg(s.init) + ' border border-slate-400 font-mono">' + s.init + '</td>';
                });
                row1 += '</tr>'; row2 += '</tr>';
                html += row1 + row2;
            });

            html += '<tr class="bg-slate-800 text-white font-black"><td colspan="2" class="uppercase tracking-widest text-left pl-4 border border-slate-400">Total</td>';
            sortedWeeks.forEach(function (cw) { html += '<td class="border border-slate-400"></td><td class="font-mono text-sm border border-slate-400 bg-slate-700">' + weekTotals[cw] + '</td>'; });
            html += '</tr></tbody></table></div>';
            html += '<div class="flex flex-wrap justify-center items-center gap-4 mt-2 text-[10px] font-bold text-slate-500">' +
                '<span><span class="inline-block w-3 h-3 align-middle bg-[#E6A5A5] border border-slate-400 mr-1"></span>0</span>' +
                '<span><span class="inline-block w-3 h-3 align-middle bg-[#FDE047] border border-slate-400 mr-1"></span>1 à 4</span>' +
                '<span><span class="inline-block w-3 h-3 align-middle bg-[#A7F3D0] border border-slate-400 mr-1"></span>5 et +</span>' +
                '<span class="text-slate-400"><i class="fa-solid fa-circle-info mr-1"></i>Fenêtre : 8 dernières semaines</span>' +
                '</div>';
            container.innerHTML = html;
        }

        function updateChart(poste, canvasId) {
            var canvas = document.getElementById(canvasId);
            if (!canvas) return;
            var ctx = canvas.getContext('2d');

            var init = 0, pro = 0;
            if (HISTORICAL_KPI[poste]) { Object.values(HISTORICAL_KPI[poste]).forEach(function (w) { init += w.init; pro += w.pro; }); }
            bossKpiLog.forEach(function (log) {
                if (log.poste === poste && log.cw >= 14) { if (log.type === 'Initiale') init++; else pro++; }
            });

            var totalEl = document.getElementById('kpi-' + poste.toLowerCase() + '-total');
            if (totalEl) totalEl.innerText = init + pro;

            // F4 : tendance sur les deux DERNIÈRES SEMAINES COMPLÈTES (S-1 vs S-2, jamais la semaine en cours à moitié remplie)
            var trendEl = document.getElementById('kpi-' + poste.toLowerCase() + '-trend');
            if (trendEl) {
                var cwNow = getWeekNumber(new Date());
                var cw1 = cwNow - 1; if (cw1 < 1) cw1 = 53;
                var cw2 = cwNow - 2; if (cw2 < 1) cw2 += 53;
                var n1 = 0, n2 = 0;
                bossKpiLog.forEach(function (l) {
                    if (l.poste !== poste) return;
                    var cwl = parseInt(l.cw, 10);
                    if (cwl === cw1) n1++; else if (cwl === cw2) n2++;
                });
                if (n2 > 0) {
                    var arrow = n1 > n2
                        ? '<span style="color:#059669;font-weight:900">▲ ' + (n1 - n2) + '</span>'
                        : (n1 < n2
                            ? '<span style="color:#DC2626;font-weight:900">▼ ' + (n2 - n1) + '</span>'
                            : '<span style="color:#94A3B8;font-weight:900">→ stable</span>');
                    trendEl.innerHTML = 'S-1 : ' + n1 + ' ' + arrow;
                    trendEl.title = 'Semaine dernière : ' + n1 + ' validation(s) · avant-dernière : ' + n2 + ' (2 semaines complètes)';
                } else {
                    trendEl.innerText = 'S-1 : ' + n1;
                    trendEl.title = 'Validations enregistrées la semaine dernière (aucune donnée sur S-2 pour comparer)';
                }
            }

            var weeksData = {};
            for (var w in HISTORICAL_KPI[poste]) {
                weeksData[w] = { i: HISTORICAL_KPI[poste][w].init, p: HISTORICAL_KPI[poste][w].pro, t: HISTORICAL_KPI[poste][w].init + HISTORICAL_KPI[poste][w].pro };
            }
            bossKpiLog.forEach(function (log) {
                if (log.poste === poste && log.cw >= 14) {
                    if (!weeksData[log.cw]) weeksData[log.cw] = { i: 0, p: 0, t: 0 };
                    if (log.type === 'Initiale') weeksData[log.cw].i++; else weeksData[log.cw].p++;
                    weeksData[log.cw].t++;
                }
            });

            var sortedKeys = Object.keys(weeksData).sort(function (a, b) { return a - b; });
            var labels = sortedKeys.map(function (w) { return 'CW' + w; });
            var dataI = sortedKeys.map(function (w) { return weeksData[w].i; });
            var dataP = sortedKeys.map(function (w) { return weeksData[w].p; });
            var dataT = sortedKeys.map(function (w) { return weeksData[w].t; });

            if (poste === 'P40' && window.bossKpiChartInstanceP40) window.bossKpiChartInstanceP40.destroy();
            if (poste === 'P50' && window.bossKpiChartInstanceP50) window.bossKpiChartInstanceP50.destroy();

            var chart = new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: labels,
                    datasets: [
                        { type: 'line', label: 'Total', data: dataT, borderColor: '#1E293B', borderWidth: 2, tension: 0.3, pointRadius: 2 },
                        { label: 'Initiales', data: dataI, backgroundColor: '#0EA5E9', stack: 'A' },
                        { label: 'Prorogations', data: dataP, backgroundColor: '#F97316', stack: 'A' }
                    ]
                },
                options: { responsive: true, maintainAspectRatio: false, plugins: { legend: { display: false } }, scales: { x: { stacked: true }, y: { stacked: true, beginAtZero: true } } }
            });

            if (poste === 'P40') window.bossKpiChartInstanceP40 = chart; else window.bossKpiChartInstanceP50 = chart;
        }

        /* ---------- Onglet Résumé Hebdo (P40 + P50 + listes) ---------- */
        function renderHebdoStats() {
            var hc = document.getElementById('hebdo-container');
            if (!hc) return;

            var stats = {
                P40: { proExp: 0, iniVal: 0, proVal: 0, listProExp: [], listIniVal: [], listProVal: [] },
                P50: { proExp: 0, iniVal: 0, proVal: 0, listProExp: [], listIniVal: [], listProVal: [] }
            };

            var lastWed = new Date(getQAWeekStartTimestamp());
            var nextWed = new Date(lastWed.getTime() + 7 * 24 * 60 * 60 * 1000);

            database.forEach(function (op) {
                var poste = (op.equipe && op.equipe.indexOf('P50') === 0) ? 'P50' : 'P40';
                var s = stats[poste];

                getQualifs(op).forEach(function (q) {
                    if (q.state === 'validated') {
                        if (q.isIni) { s.iniVal++; s.listIniVal.push({ op: op.nom, q: q.name, validator: q.validator }); }
                        else { s.proVal++; s.listProVal.push({ op: op.nom, q: q.name, validator: q.validator }); }
                    }
                    if (!q.isIni && q.state !== 'validated' && q.state !== 'standby' && q.state !== 'disabled') {
                        if (q.date && q.date !== 'À QUALIFIER' && q.date !== '-') {
                            var dParts = q.date.split('/');
                            if (dParts.length === 3) {
                                var expDate = new Date(dParts[2], dParts[1] - 1, dParts[0]);
                                expDate.setHours(12, 0, 0, 0);
                                if (expDate > lastWed && expDate <= nextWed) {
                                    s.proExp++;
                                    s.listProExp.push({ op: op.nom, q: q.name, date: q.date });
                                }
                            }
                        }
                    }
                });
            });

            var period = 'Semaine CW' + getWeekNumber(new Date()) + ' : du ' + lastWed.toLocaleDateString('fr-FR') + ' au ' + new Date(nextWed.getTime() - 86400000).toLocaleDateString('fr-FR');
            hc.innerHTML = hebdoBlock('Secteur P40', stats.P40, 'blue', period) + hebdoBlock('Secteur P50', stats.P50, 'indigo', period);
        }

        function hebdoList(items, emptyTxt, fmt) {
            if (!items.length) return '<div class="text-[11px] font-bold text-slate-400 italic p-2 bg-white rounded-lg border border-dashed border-slate-200">' + emptyTxt + '</div>';
            return '<ul class="flex flex-col gap-1">' + items.map(function (it) {
                return '<li class="text-[11px] font-bold text-slate-700 bg-white rounded-lg border border-slate-200 px-3 py-2"><i class="fa-solid fa-caret-right mr-2 text-slate-300"></i>' + fmt(it) + '</li>';
            }).join('') + '</ul>';
        }

        function hebdoBlock(title, s, color, period) {
            return '<div class="bg-slate-50 border border-slate-200 rounded-xl p-4 sm:p-5 overflow-hidden">' +
                '<div class="flex flex-wrap justify-between items-center gap-2 mb-4">' +
                    '<h3 class="font-black text-base text-slate-800 uppercase tracking-widest"><i class="fa-solid fa-industry text-' + color + '-500 mr-2"></i>' + title + '</h3>' +
                    '<span class="text-[10px] font-bold text-slate-400">' + period + '</span>' +
                '</div>' +
                '<div class="grid grid-cols-3 gap-4 mb-5 text-center">' +
                    '<div class="bg-white border border-red-200 p-4 rounded-xl"><span class="block text-[10px] text-red-500 font-bold uppercase">Pro. Échues</span><span class="text-2xl font-black text-red-600">' + s.proExp + '</span></div>' +
                    '<div class="bg-white border border-sky-200 p-4 rounded-xl"><span class="block text-[10px] text-sky-500 font-bold uppercase">Ini. Val</span><span class="text-2xl font-black text-sky-600">' + s.iniVal + '</span></div>' +
                    '<div class="bg-white border border-orange-200 p-4 rounded-xl"><span class="block text-[10px] text-orange-500 font-bold uppercase">Pro. Val</span><span class="text-2xl font-black text-orange-600">' + s.proVal + '</span></div>' +
                '</div>' +
                '<div class="grid grid-cols-1 md:grid-cols-3 gap-4">' +
                    '<div><div class="text-[10px] font-black uppercase text-red-500 mb-2"><i class="fa-solid fa-triangle-exclamation mr-1"></i>Prorogations échues cette semaine</div>' +
                        hebdoList(s.listProExp, 'Aucune prorogation échue cette semaine.', function (it) { return '<b>' + sanitize(it.op) + '</b> — ' + sanitize(it.q) + ' <span class="mono text-red-500">' + sanitize(it.date) + '</span>'; }) + '</div>' +
                    '<div><div class="text-[10px] font-black uppercase text-sky-500 mb-2"><i class="fa-solid fa-circle-check mr-1"></i>Initiales validées</div>' +
                        hebdoList(s.listIniVal, 'Aucune initiale validée cette semaine.', function (it) { return '<b>' + sanitize(it.op) + '</b> — ' + sanitize(it.q) + (it.validator ? ' <span class="text-slate-400">(' + sanitize(it.validator) + ')</span>' : ''); }) + '</div>' +
                    '<div><div class="text-[10px] font-black uppercase text-orange-500 mb-2"><i class="fa-solid fa-rotate mr-1"></i>Prorogations validées</div>' +
                        hebdoList(s.listProVal, 'Aucune prorogation validée cette semaine.', function (it) { return '<b>' + sanitize(it.op) + '</b> — ' + sanitize(it.q) + (it.validator ? ' <span class="text-slate-400">(' + sanitize(it.validator) + ')</span>' : ''); }) + '</div>' +
                '</div>' +
            '</div>';
        }

        function buildHebdoText() {
            var lines = [];
            var lastWed = new Date(getQAWeekStartTimestamp());
            var nextWed = new Date(lastWed.getTime() + 7 * 24 * 60 * 60 * 1000);
            lines.push('RÉSUMÉ HEBDO QA — CW' + getWeekNumber(new Date()));
            lines.push('Période : du ' + lastWed.toLocaleDateString('fr-FR') + ' au ' + new Date(nextWed.getTime() - 86400000).toLocaleDateString('fr-FR'));
            lines.push('');
            ['P40', 'P50'].forEach(function (poste) {
                var exp = [], ini = [], pro = [];
                database.forEach(function (op) {
                    var p = (op.equipe && op.equipe.indexOf(poste) === 0) ? poste : null;
                    if (p !== poste) return;
                    getQualifs(op).forEach(function (q) {
                        if (q.state === 'validated') {
                            if (q.isIni) ini.push(op.nom + ' — ' + q.name + (q.validator ? ' (' + q.validator + ')' : ''));
                            else pro.push(op.nom + ' — ' + q.name + (q.validator ? ' (' + q.validator + ')' : ''));
                        } else if (!q.isIni && q.state !== 'standby' && q.state !== 'disabled' && q.date && q.date !== 'À QUALIFIER' && q.date !== '-') {
                            var dParts = q.date.split('/');
                            if (dParts.length === 3) {
                                var expDate = new Date(dParts[2], dParts[1] - 1, dParts[0]);
                                expDate.setHours(12, 0, 0, 0);
                                if (expDate > lastWed && expDate <= nextWed) exp.push(op.nom + ' — ' + q.name + ' (' + q.date + ')');
                            }
                        }
                    });
                });
                lines.push('== ' + poste + ' ==');
                lines.push('Prorogations échues (' + exp.length + ')' + (exp.length ? ' :\n- ' + exp.join('\n- ') : ''));
                lines.push('Initiales validées (' + ini.length + ')' + (ini.length ? ' :\n- ' + ini.join('\n- ') : ''));
                lines.push('Prorogations validées (' + pro.length + ')' + (pro.length ? ' :\n- ' + pro.join('\n- ') : ''));
                lines.push('');
            });
            return lines.join('\n');
        }

        function copyHebdo() {
            var text = buildHebdoText();
            if (navigator.clipboard && navigator.clipboard.writeText) {
                navigator.clipboard.writeText(text).then(function () {
                    toast('<i class="fa-solid fa-copy mr-1"></i>Résumé copié dans le presse-papier.');
                }).catch(function () { fallbackCopy(text); });
            } else { fallbackCopy(text); }
        }

        function fallbackCopy(text) {
            var ta = document.createElement('textarea');
            ta.value = text;
            ta.style.position = 'fixed'; ta.style.opacity = '0';
            document.body.appendChild(ta);
            ta.select();
            var ok = false;
            try { ok = document.execCommand('copy'); } catch (e) {}
            ta.remove();
            toast(ok ? 'Résumé copié.' : 'Copie impossible — utilise Imprimer.', !ok);
        }

        /* ---------- Listes déroulantes communes ---------- */
        function fillCommonLists() {
            var qDatalist = document.getElementById('qualifs-codes');
            if (qDatalist) qDatalist.innerHTML = QUALIFS_LIST.map(function (q) { return '<option value="' + sanitize(q) + '"></option>'; }).join('');
            var nDatalist = document.getElementById('operators-names');
            if (nDatalist) nDatalist.innerHTML = database.map(function (op) { return '<option value="' + sanitize(op.nom) + '"></option>'; }).join('');
        }

        /* ---------- Drag & drop : import d'une sauvegarde .json déposée n'importe où ---------- */
        (function () {
            var dragDepth = 0;
            function overlay() { return document.getElementById('drop-overlay'); }
            function hasFiles(e) {
                var dt = e.dataTransfer;
                if (!dt) return false;
                var types = dt.types;
                if (!types) return false;
                for (var i = 0; i < types.length; i++) { if (types[i] === 'Files') return true; }
                return false;
            }
            window.addEventListener('dragenter', function (e) {
                if (!hasFiles(e)) return;               // glisser une sélection de texte = ignoré
                e.preventDefault();
                dragDepth++;
                var o = overlay(); if (o) o.classList.add('show');
            });
            window.addEventListener('dragover', function (e) { if (hasFiles(e)) e.preventDefault(); });
            window.addEventListener('dragleave', function (e) {
                if (!hasFiles(e)) return;
                dragDepth = Math.max(0, dragDepth - 1);
                if (!dragDepth) { var o = overlay(); if (o) o.classList.remove('show'); }
            });
            window.addEventListener('drop', function (e) {
                if (!hasFiles(e)) return;
                e.preventDefault();
                dragDepth = 0;
                var o = overlay(); if (o) o.classList.remove('show');
                var f = e.dataTransfer.files && e.dataTransfer.files[0];
                if (!f) return;
                if (!/\.json$/i.test(f.name)) {
                    toast('<i class="fa-solid fa-triangle-exclamation mr-1"></i>Dépose un fichier <b>.json</b> de sauvegarde (crée-le via Gestion ⚙️ → Exporter).', true, 4200);
                    return;
                }
                // On alimente un input éphémère pour réutiliser importBackupJSON (PIN + validation + confirmation)
                try {
                    var dt = new DataTransfer();
                    dt.items.add(f);
                    var tmp = document.createElement('input');
                    tmp.type = 'file';
                    tmp.files = dt.files;
                    importBackupJSON(tmp);
                } catch (err) {
                    toast('Import impossible : utilise Gestion ⚙️ → Importer.', true);
                }
            });
        })();
    </script>
</body>
</html>
