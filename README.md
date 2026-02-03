<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>VYKORA Digital</title>
  <style>
    /* Acessibilidade: link de pular para conteúdo, foco visível, contraste e layout responsivo */
    :root{
      --bg: #0f0f14;
      --card-bg: #1a1a22;
      --primary: #6a00ff; /* revise se precisar ajustar contraste */
      --muted: #cfcfcf;
      --footer: #111;
      --focus: 3px solid #ffb86b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, Helvetica, sans-serif; }
    html,body { height: 100%; }
    body { background: var(--bg); color: #f2f2f2; line-height:1.4; -webkit-font-smoothing:antialiased; }

    /* Skip link (visível ao focar) */
    .skip-link {
      position: absolute;
      left: -999px;
      top: auto;
      width: 1px;
      height: 1px;
      overflow: hidden;
    }
    .skip-link:focus {
      left: 1rem;
      top: 1rem;
      width: auto;
      height: auto;
      padding: 0.5rem 1rem;
      background: #fff;
      color: var(--bg);
      border-radius: 4px;
      z-index: 1000;
      box-shadow: 0 2px 8px rgba(0,0,0,0.4);
    }

    header { padding: 40px 20px; text-align: center; background: linear-gradient(135deg, var(--primary), #000); }
    header h1 { font-size: 2.5rem; letter-spacing: 2px; }
    header p { margin-top: 10px; color: var(--muted); }

    nav { display: flex; justify-content: center; padding: 15px; background: var(--footer); }
    nav ul { list-style: none; display:flex; gap:20px; align-items:center; }
    nav a { color: #fff; text-decoration: none; font-weight: bold; padding: 6px 8px; border-radius:4px; }
    nav a:focus, nav a:hover { color: var(--primary); outline: none; box-shadow: var(--focus); }
    nav a[aria-current="page"] { text-decoration: underline; }

    main { padding: 60px 20px; max-width: 1000px; margin: auto; }

    section h2* 

