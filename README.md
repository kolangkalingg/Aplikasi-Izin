<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Bootstrap demo</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9"
      crossorigin="anonymous"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container">
        <a class="navbar-brand" href="#">Navbar</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse ms-auto" id="navbarNavDropdown">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Features</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Pricing</a>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Dropdown link
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li>
                  <a class="dropdown-item" href="#">Something else here</a>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <h2 class="my-5">APLIKASI IZIN KELAS XI RPL</h2>
    <div class="alert alert-success alert-dismissible fade show" role="alert">
      <strong>Terima Kasih!</strong> data ijin telah kami terima
      <button
        type="button"
        class="btn-close"
        data-bs-dismiss="alert"
        aria-label="Close"
      ></button>
    </div>
    <div class="container mt-4">
      <form class="row" name="proses-ijin">
        <div class="col-md-4">
          <label for="kelas" class="form-label">Kelas</label>
          <select class="form-select" name="kelas">
            <option selected>- PILIH KELAS-</option>
            <option value="XI RPL">XI RPL</option>
          </select>
        </div>
        <div class="col-md-4 mb-4">
          <label for="nama" class="form-label">Nama Siswa</label>
          <select class="form-select" name="nama">
            <option selected>- NAMA SISWA -</option>
            <option value="ANDI NAUVAL ZACKY">ZACKY</option>
            <option value="RENDY">RENDY</option>
            <option value="MARITZKA">MARITZKA</option>
            <option value="AHYAN">AHYAN</option>
          </select>
        </div>

        <div class="col-md-4 mb-4">
          <label for="nama" class="form-label">Nis</label>
          <select class="form-select" name="nis">
            <option selected>- PILIH NIS -</option>
            <option value="123212">1233212</option>
            <option value="456654">456654</option>
            <option value="999999">999999</option>
            <option value="888888">888888</option>
          </select>
        </div>

        <div class="col-md-4 mb-4">
          <label for="tgl" class="form-label mb-3">Tanggal</label>
          <input type="date" id="tgl" class="form-control" name="tanggal" />
        </div>

        <!-- form radio button untuk pilih keterangan tidak masuk -->
        <label for="keterangan" class="form-label mb-3">Keterangan Ijin</label>
        <div
          class="btn-group mb-4"
          role="group"
          aria-label="Basic radio toggle button group"
        >
          <input
            type="radio"
            class="btn-check"
            name="keterangan"
            id="btnradio1"
            autocomplete="off"
            value="KEPERLUAN KELUARGA"
            checked
          />
          <label class="btn btn-outline-primary" for="btnradio1"
            >KEPERLUAN KELUARGA</label
          >

          <input
            type="radio"
            class="btn-check"
            name="keterangan"
            id="btnradio2"
            autocomplete="off"
            value="SAKIT"
          />
          <label class="btn btn-outline-primary" for="btnradio2">SAKIT</label>

          <input
            type="radio"
            class="btn-check"
            name="keterangan"
            id="btnradio3"
            autocomplete="off"
            value="TERLAMBAT"
          />
          <label class="btn btn-outline-primary" for="btnradio3"
            >TERLAMBAT</label
          >
        </div>

        <div class="col-8 mt-6">
          <label for="alasan" class="form-label-lg mb-3"
            >Alasan tidak masuk/ijin/terlambat</label
          >
          <input
            type="text"
            class="form-control"
            id="alasan"
            name="alasan"
            autocomplete="off"
          />
        </div>
        <div class="col-12 mt-4">
          <button type="submit" class="btn btn-outline-primary btn-kirim">
            Kirim Data
          </button>
          <button
            class="btn btn-primary btn-loading d-none"
            type="button"
            disabled
          >
            <span
              class="spinner-grow spinner-grow-sm"
              aria-hidden="true"
            ></span>
            <span role="status">Loading...</span>
          </button>
        </div>
      </form>
    </div>
    <script
      src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js"
      integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm"
      crossorigin="anonymous"
    ></script>
    <script>
      const scriptURL =
        "https://script.google.com/macros/s/AKfycbxHMxStA9DH1UyKJpZb-n4EHwwWe1aA4B-HhWw63-nxN_3TT_8JRJSkUbYPFg9Jx8fg/exec";
      const form = document.forms["proses-ijin"];
      const btnKirim = document.querySelector(".btn-kirim");
      const btnLoading = document.querySelector(".btn-loading");
      const myAlert = document.querySelector(".my-Alert");

      form.addEventListener("submit", (e) => {
        e.preventDefault();

        btnLoading.classList.toggle("d-none");
        btnKirim.classList.toggle("d-none");

        fetch(scriptURL, { method: "POST", body: new FormData(form) })
          .then((response) => {
            btnLoading.classList.toggle("d-none");
            btnKirim.classList.toggle("d-none");

            myAlert.classList.toggle("d-none");
            form.reset();

            console.log("Success!", response);
          })

          .catch((error) => console.error("Error!", error.message));
      });
    </script>
  </body>
</html>
