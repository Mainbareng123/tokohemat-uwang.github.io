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

body{
    background-image: url(gambar/background.jpg);
    width: 500px;
    height: 300px;
    margin: 10 auto;
    opacity: 0.9;
    border: #00868b;
    margin-top: -20px;
    box-sizing: 50px;
   }
   .konten{
    background:#3d9f046f;
    border: #00868b;
    width: 360px;
    margin: 30px auto 0;
    border-radius: 16px;
    overflow: hidden;
   }
   .kepala{
    background: #0414c0b8;
    padding: 7px 7px;
    height: 40px;
   }
   .lock{
    display: inline-block;
    width: 20px;
    height: 10px;
    margin-top: 10px;
    float: center;
    margin-right: 40px;
    border: #00868b;
   }
   .judul{
    color: #ffffff;
    font-weight: 20px;
    line-height: 10px;
    display: inline-block;
   }
   .artikel{
    padding:10px 15px;
    color: #ffffff;
    border-radius: 7px;
   }
   .grup{
    margin: 7px 0;
   }
   .grup label,
   .grup input,
   .grup button{
    display: block;
   }
   .grup label{
    display: inline-block;
    font-size: 15px;
    text-align: center;
    margin: 0 0.2em;
    margin-bottom: 7px;
   }
   .grup input[type="text"],
   .grup input[type="tel"],
   .grup input[type="email"],
   .grup input[type="password"]{
    width: 300px;
    height: 30px;
    padding: 0 10px;
    background: #cccccc;
    border: #000000;
    font-size: 13px;
    color: #1a1a1a;
   }
   .grup input[type="textarea"]{
    width: 187px;
    height: 50px;
    background: #cccccc;
    border: #000000;
    font-size: 13px;
    color: #1a1a1a;
    float: right;
    margin-right: 60px;
    margin-bottom: 10px;
    text-align: center ;
   }
   .grup button[type="radio"]{
    margin: 80px;
    margin-right: 7px;
    float: left;
   }
   .grup button[type="submit"],
   .grup button[type="reset"] hover{
    background: #00868b;
    border: 2px solid #00e5ee;
    float: left;
    border-radius: 7px;
    color: #ffffff;
    cursor: pointer;
   }
   .required{
    color: red;
    font-weight: normal;
   }
   .footer{
    padding: 3px;
    color: #ffffff;
    height: 30px;
    margin-left: 30px;
    margin-bottom: :-40px;
    margin-top: -20px;
   }
   .btn {
    cursor: pointer;
    margin-left: 5em;
    color: white;
    background-color:rgb(54, 0, 249) ;
   }
