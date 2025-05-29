
✅ Bootstrap 5 Gyorstalpaló

🔹 Mi az a Bootstrap?
A Bootstrap egy népszerű front-end keretrendszer, amellyel gyorsan lehet reszponzív (mobilbarát) weboldalakat fejleszteni HTML, CSS és JavaScript segítségével.

📦 1. Bootstrap használata
👉 CDN-es beillesztés (ajánlott gyors kezdéshez):
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

🧱 2. Alap layout: Container, Row, Column
<div class="container">
  <div class="row">
    <div class="col">1. oszlop</div>
    <div class="col">2. oszlop</div>
  </div>
</div>

- container: rögzített szélességű középre igazított tartalom
- row: sor, amelybe oszlopokat helyezünk
- col: automatikusan elosztja a szélességet (vagy col-6, col-md-4, stb.)

🎨 3. Színek és háttérszínek
<div class="text-primary">Kék szöveg</div>
<div class="bg-warning text-dark">Sárga háttér, sötét szöveg</div>
Használható osztályok: primary, secondary, success, danger, warning, info, light, dark

🔘 4. Gombok
<button class="btn btn-primary">Elsődleges gomb</button>
Típusok: btn-primary, btn-secondary, btn-outline-danger, stb.

📝 5. Form elemek
<form>
  <div class="mb-3">
    <label for="email" class="form-label">Email cím</label>
    <input type="email" class="form-control" id="email">
  </div>
  <button type="submit" class="btn btn-success">Küldés</button>
</form>

📱 6. Reszponzív szöveg és elemek
- d-none d-md-block: kis képernyőn elrejt, közepestől látható
- text-center, text-md-start: szöveg igazítása méret szerint

🎁 7. Komponensek

📌 Navbar (navigációs sáv)
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Weboldal</a>
    <button class="navbar-toggler" ... ></button>
    <div class="collapse navbar-collapse">
      <ul class="navbar-nav">
        <li class="nav-item"><a class="nav-link active" href="#">Főoldal</a></li>
      </ul>
    </div>
  </div>
</nav>

📌 Kártya (Card)
<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Cím</h5>
    <p class="card-text">Leírás...</p>
    <a href="#" class="btn btn-primary">Gomb</a>
  </div>
</div>

📌 Modal (felugró ablak)
<button data-bs-toggle="modal" data-bs-target="#myModal">Megnyitás</button>
<div class="modal fade" id="myModal" tabindex="-1">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header"><h5>Modal Cím</h5></div>
      <div class="modal-body">Tartalom</div>
      <div class="modal-footer">
        <button class="btn btn-secondary" data-bs-dismiss="modal">Bezár</button>
      </div>
    </div>
  </div>
</div>

📚 8. Hasznos linkek
- Bootstrap 5 Dokumentáció: https://getbootstrap.com/docs/5.3/getting-started/introduction/
- W3Schools Bootstrap Tutorial: https://www.w3schools.com/bootstrap5/


📏 9. Grid rendszer és méretek

A Bootstrap egy 12 oszlopos rácsrendszert (grid system) használ. Ez azt jelenti, hogy egy sor (row) legfeljebb 12 oszlopnyi (col) szélességet tartalmazhat.

Például, ha két nagyobb és egy kisebb kártyát szeretnél egymás mellé tenni, akkor így oszthatod el:
- Az első kártya 5 oszlop szélességű (`col-5`)
- A második kártya is 5 oszlop szélességű (`col-5`)
- A harmadik kártya kisebb, 2 oszlop szélességű (`col-2`)

Ez összesen: 5 + 5 + 2 = 12

📌 Példa:
<div class="container">
  <div class="row">
    <div class="col-5">
      <div class="card">
        <div class="card-body">Nagyobb kártya 1</div>
      </div>
    </div>
    <div class="col-5">
      <div class="card">
        <div class="card-body">Nagyobb kártya 2</div>
      </div>
    </div>
    <div class="col-2">
      <div class="card">
        <div class="card-body">Kisebb kártya</div>
      </div>
    </div>
  </div>
</div>

Ha az oszlopok méreteinek összege több mint 12, akkor a felesleges elemek automatikusan a következő sorba kerülnek.

