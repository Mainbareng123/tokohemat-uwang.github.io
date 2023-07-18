<html>
<head>
    <title>FORM PENDAFTARAN AKUN</title>
    <link rel="stylesheet" type="text/css" href="daftar.css">
<script type="text/javascript">
    function validasi (form) {
        if (form.password.value.length <6){
            alert("Password harus lebih dari 6 karakter");
            return false;
        }

        if (form.password.value !== form.rtp.value){
            alert("Password yang anda masukkan tidak cocok!");
            return false;
        }
        return true;
    }
</script>
</head>

<body>

<div class="konten">
    <div class="kepala">
        <div class="lock"></div>
        <h2 class="judul">Buat Akun Baru</h2>
        </div>
    <br>
    <br>

    <div class="artikel">
        <form class="horizontal" action="daftar.html" method="post" onsubmit="return validasi(this);">
        <fieldset><legend>Data Login</legend>
        <div class="grup">
            <label for="username">Username/ID<span class="required" >*</span></label>
            <input type="text" name="username" required placeholder="Masukkan Username Anda">
        </div>
        <div class="grup">
            <label for="password">Password<span class="required">*</span></label>
            <input type="password" name="password" required placeholder="Masukkan password Anda">
        </div>
        <div class="grup">
            <label for="rtp">Re-Type Password<span class="required">*</span></label>
            <input type="password" name="rtp" required placeholder="Masukkan kembali password Anda">
        </div>
        </fieldset>

        <fieldset><legend>Data Pribadi</legend>
        <div class="grup">
            <label for="nama">Nama Lengkap<span class="required">*</span></label>
            <input type="text" name="Nama" required placeholder="Masukkan Nama Lengkap Anda">
        </div>

        <div class="grup">
            <label for="email">Alamat E-mail<span class="required">*</span></label>
            <input type="email" name="email" required placeholder="Masukkan Alamat Email Anda">
        </div>

        <div class="grup">
            <label for="no.telp">No Handphone<span class="required">*</span></label>
            <input type="tel" name="No.Hp" pattern="\d\d\d\d\d\d\d\d\d\d\d\d" required placeholder=" Masukkan No.Hp 08xxxxxxxxxx">
        </div>

        <div class="grup-offset">
            <label for="JK">Jenis Kelamin<span class="required">*</span><br></label>
            <input type="radio" name="JK" value="Laki-Laki" required>Laki-laki
            <input type="radio" name="JK" value="Perempuan" required>Perempuan
        </div>

        <div class="grup">
            <label for="birth">Tanggal Lahir<span class="required">*</span></label>
            <input type="date"  id="birth" name="birth">
        </div>
        <br>
        <br>
        <div class="grup-offset">
        <button type="submit" value="Sign In">Submit</button>
        <button type="reset" value="Reset">Reset</button>
        </div>
        </fieldset>
        </div>
        </form>
        <div class="akun">
            <p>Sudah Punya Akun?</p>
            <a target="_self" href="login.html"><button class="btn btn-danger">Login</button></a>
            </div>
          <br>
          <br>

</div>
</body>
</html>
