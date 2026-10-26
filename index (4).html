<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>IDH de mi estado</title>
<style>
  :root {
    --verde-oscuro: #1b4d3e;
    --verde: #2e7d4f;
    --verde-claro: #e8f5e9;
    --tierra: #8d6e3f;
    --cielo: #e3f2fd;
    --texto: #1f2d24;
  }
  * { box-sizing: border-box; }
  body {
    margin: 0;
    min-height: 100vh;
    font-family: system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    color: var(--texto);
    background: linear-gradient(180deg, var(--cielo) 0%, var(--verde-claro) 100%);
    display: flex;
    justify-content: center;
    padding: 16px;
  }
  main {
    width: 100%;
    max-width: 640px;
    background: #fff;
    border-radius: 16px;
    border-top: 8px solid var(--verde);
    box-shadow: 0 6px 24px rgba(27, 77, 62, 0.15);
    padding: 24px 20px;
    align-self: flex-start;
    margin-top: 12px;
  }
  h1 { margin: 0 0 8px; color: var(--verde-oscuro); font-size: 1.8rem; }
  p.intro { line-height: 1.55; margin: 0 0 20px; }
  label { display: block; font-weight: 600; margin-bottom: 6px; color: var(--verde-oscuro); }
  select, button {
    width: 100%;
    font-size: 1rem;
    padding: 12px;
    border-radius: 10px;
  }
  select { border: 2px solid var(--verde); background: #fff; color: var(--texto); }
  button {
    margin-top: 12px;
    border: none;
    background: var(--verde);
    color: #fff;
    font-weight: 700;
    cursor: pointer;
    transition: background 0.2s;
  }
  button:hover:not(:disabled) { background: var(--verde-oscuro); }
  button:disabled { background: #9bb7a6; cursor: not-allowed; }
  #estado { margin-top: 16px; font-weight: 600; color: var(--tierra); min-height: 1.4em; }
  #resultado {
    display: none;
    margin-top: 8px;
    padding: 16px;
    background: var(--verde-claro);
    border-left: 6px solid var(--verde);
    border-radius: 10px;
    white-space: pre-line;
    line-height: 1.55;
    overflow-wrap: anywhere;
  }
  #resultado.error { background: #fdecea; border-left-color: #c62828; color: #7f1d1d; }
  @media (min-width: 600px) {
    main { padding: 32px; }
    h1 { font-size: 2.2rem; }
    button { width: auto; padding: 12px 32px; }
  }
</style>
</head>
<body>
<main>
  <h1>IDH de mi estado</h1>
  <p class="intro">
    El Índice de Desarrollo Humano (IDH) es una medida que resume el bienestar de una población
    en tres dimensiones: salud (esperanza de vida), educación (años de escolaridad) e ingreso
    (nivel de vida digno). Va de 0 a 1; mientras más cercano a 1, mayor es el desarrollo humano.
  </p>

  <label for="entidad">Elige tu entidad federativa</label>
  <select id="entidad">
    <option value="" selected disabled>Selecciona una entidad…</option>
    <option>Aguascalientes</option>
    <option>Baja California</option>
    <option>Baja California Sur</option>
    <option>Campeche</option>
    <option>Chiapas</option>
    <option>Chihuahua</option>
    <option>Ciudad de México</option>
    <option>Coahuila</option>
    <option>Colima</option>
    <option>Durango</option>
    <option>Estado de México</option>
    <option>Guanajuato</option>
    <option>Guerrero</option>
    <option>Hidalgo</option>
    <option>Jalisco</option>
    <option>Michoacán</option>
    <option>Morelos</option>
    <option>Nayarit</option>
    <option>Nuevo León</option>
    <option>Oaxaca</option>
    <option>Puebla</option>
    <option>Querétaro</option>
    <option>Quintana Roo</option>
    <option>San Luis Potosí</option>
    <option>Sinaloa</option>
    <option>Sonora</option>
    <option>Tabasco</option>
    <option>Tamaulipas</option>
    <option>Tlaxcala</option>
    <option>Veracruz</option>
    <option>Yucatán</option>
    <option>Zacatecas</option>
  </select>

  <button id="consultar" type="button">Consultar</button>

  <div id="estado" aria-live="polite"></div>
  <div id="resultado" aria-live="polite"></div>
</main>

<script>
  // Pega aquí la URL del webhook de Make (entre las comillas).
  const WEBHOOK_URL = "PEGA_AQUI_TU_URL_DE_MAKE";

  const select = document.getElementById("entidad");
  const boton = document.getElementById("consultar");
  const estado = document.getElementById("estado");
  const resultado = document.getElementById("resultado");

  boton.addEventListener("click", async () => {
    const entidad = select.value;
    if (!entidad) {
      estado.textContent = "Primero selecciona una entidad.";
      resultado.style.display = "none";
      return;
    }

    estado.textContent = "Consultando...";
    resultado.style.display = "none";
    resultado.classList.remove("error");
    boton.disabled = true;

    try {
      const respuesta = await fetch(WEBHOOK_URL, {
        method: "POST",
        body: new URLSearchParams({ entidad: entidad })
      });
      if (!respuesta.ok) throw new Error("HTTP " + respuesta.status);
      const texto = await respuesta.text();
      resultado.textContent = texto;
      resultado.style.display = "block";
      estado.textContent = "";
    } catch (e) {
      estado.textContent = "";
      resultado.textContent = "No se pudo obtener la información, intenta de nuevo.";
      resultado.classList.add("error");
      resultado.style.display = "block";
    } finally {
      boton.disabled = false;
    }
  });
</script>
</body>
</html>
