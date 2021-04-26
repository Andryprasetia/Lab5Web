# Pemograman Web
~~~
Nama  : Andry Prasetia Perdana
NIM   : 311910284
Kelas : TI19C1
~~~
# Langkah Praktikut
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
~~~
<!DOCTYPE  html>
<html  lang="en">
<head>
<title>Mengenal  JavaScript</title>
</head>
<body>
<h1>Pengenalan  JavaScript</h1>
<h3>Contoh  document.write  dan  console.log</h3>
<script>
document.write("Hello  World"); console.log("Hello  World");
</script>
</body>
</html>
~~~
![Screenshot (89)](https://user-images.githubusercontent.com/81818989/116067816-b9b5fa80-a6b3-11eb-838c-c05bd3a0f140.png)
# Javascrip Dasar
Pemakaian Alert sebagai property window.
~~~
<!DOCTYPE  html>
<html>
<head>
<title>alert box</title>
</head>
<body>
<script language = "javascript">
<!--
    window.alert("ini merupakan pesan untuk anda");
    //-->
</script>
</body>
</html>
~~~
![Screenshot (90)](https://user-images.githubusercontent.com/81818989/116067943-dce0aa00-a6b3-11eb-86aa-304a3d2b7d42.png)
Pemakaian method dalam objek
~~~
<!DOCTYPE  html>
<html>
<head>
<title>skrip javascript</title>
</head>
<body>
Percobaan Memakai Javascript<br> 
<script language = "javascript">
<!--
    document.write("selamat mencoba javasript<br>");
    document.write("semoga sukses!");
    //-->
</script>
</body>
</html>
~~~
![Screenshot (91)](https://user-images.githubusercontent.com/81818989/116068649-a9eae600-a6b4-11eb-825c-6d8de7147c48.png)
Pemakaian Prompt
~~~
<!DOCTYPE  html>
<html>
<head>
<title>pemasukan data</title>
</head>
<body>
<script language = "javascript">
<!--
    var nama = prompt("siapa nama anda?","Andry Prasetia");
    document.write("hai ","Andry Prasetia");
    //-->
</script>
</body>
</html>
~~~
![Screenshot (92)](https://user-images.githubusercontent.com/81818989/116069721-eb2fc580-a6b5-11eb-82d5-22b643e5d383.png)
![Screenshot (93)](https://user-images.githubusercontent.com/81818989/116069807-06023a00-a6b6-11eb-9303-f21cf35f2672.png)
Pembuatan fungsi dan cara pemanggilannya
~~~
<!DOCTYPE  html>
<html>
<head>
    <title>Contoh program javascript</title>
    <script language = "javascript">
    function pesan(){alert ("Memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
~~~
![Screenshot (94)](https://user-images.githubusercontent.com/81818989/116070676-1cf55c00-a6b7-11eb-98bb-e4dbec2b771a.png)
# Dasar Pemrograman Di Javascript
Operasi dasar aritmatika
~~~
<html>
<head>
    <title>Contoh program javascript</title>

    <script language = "javascript">
    function test (val1,val2)
    {   
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="aritmatika" onclick=test(9,4)>
</body>
</html>
~~~
![Screenshot (95)](https://user-images.githubusercontent.com/81818989/116073863-2da7d100-a6bb-11eb-8507-2a088e93041e.png)
![Screenshot (96)](https://user-images.githubusercontent.com/81818989/116073884-326c8500-a6bb-11eb-96fe-276c9b845a8e.png)
Seleksi kondisi (if..else)
~~~
<html>
<head>
    <title>Contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
    var nilai = prompt("nilai (0-10): ", 0);
    var hasil = "";
    if (nilai >=60)
    hasil = "lulus";
    else
    hasil = "tidak lulus";
    document.write("hasil: " + hasil);
    //-->    
    </script>
</body>
</html>
~~~
![Screenshot (97)](https://user-images.githubusercontent.com/81818989/116075003-a3f90300-a6bc-11eb-9b1d-5ef23514bc16.png)
![Screenshot (98)](https://user-images.githubusercontent.com/81818989/116075068-b2471f00-a6bc-11eb-8557-092b8109ad02.png)
Penggunaan operator switch untuk seleksi kondisi
~~~
<html>
<head>
    <title>Contoh program javascript</title>

    <script language = "javascript">
    function test ()
    {
        vall=window.prompt("input nilai (1-5):")
        switch (vall)
        {
            case "1" :
                document.write("bilangan satu")
                break
            case "2" :
                document.write("bilangan dua")
                break
            case "3" :
                document.write("bilangan tiga")
                break
            case "4" :
                document.write("bilangan empat")
                break            
            case "5" :
                document.write("bilangan lima")
                break
            default :
                document.write("bilangan lainnya")
        }
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
~~~
![Screenshot (100)](https://user-images.githubusercontent.com/81818989/116081851-f4745e80-a6c4-11eb-8c5c-da3c19fcca14.png)
![Screenshot (101)](https://user-images.githubusercontent.com/81818989/116081870-f8a07c00-a6c4-11eb-9dc4-cbeba4ccba4c.png)
# Pembuatan Form
Form Input
~~~
<html>
<head>
    <title>Contoh program javascript</title>

    <script language = "javascript">
    function test ()
    {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
~~~
![Screenshot (102)](https://user-images.githubusercontent.com/81818989/116083390-c1cb6580-a6c6-11eb-8349-02290500e302.png)
Form Button
~~~
<html>
<head>
    <title>Contoh program javascript</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }   
        -->
    </script>
    <h1>Tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onClick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onClick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onClick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onClick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
     document.write("Dimodifikasi terakhidr pada" +
     document.lastModified);
    //-->
    </script>
</body>
</html>
~~~
Background Hijau dengan text kuning
![Screenshot (103)](https://user-images.githubusercontent.com/81818989/116085221-cbee6380-a6c8-11eb-8361-4f3915018ddd.png)
Bacground putih dengan text biru
![Screenshot (104)](https://user-images.githubusercontent.com/81818989/116085255-d6a8f880-a6c8-11eb-9cf0-764f880a689f.png)
# HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis
~~~
 <!--
File: daftar_menu.html
//-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            }
            else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
<h1>Daftar Menu Makanan</h1>
<label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp.5000 </label><br />
<label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp.500 </label><br />
<label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp.2500 </label><hr />
<strong>Total Bayar : Rp. <input id="total" type="text" /></strong>
</body>
</html>
~~~
Ceklis beberapa menu makanan, lalu akan muncul total dari makanan yang di ceklis
![Screenshot (105)](https://user-images.githubusercontent.com/81818989/116093284-be3cdc00-a6d0-11eb-834c-f81c3e9bd9fe.png)
# Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.
~~~
<html>
<head>
	<title>login</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<center><h2>Pendaftaran</h2></center>
	<div class="login">
		<form action="#" method="POST" onSubmit="validasi()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
<script type="text/javascript">
	function validasi() {
		var nama = document.getElementById("nama").value;
		var email = document.getElementById("email").value;
		var alamat = document.getElementById("alamat").value;
		if (nama != "" && email!="" && alamat !="") {
			return true;
		}else{
			alert('Anda harus mengisi data dengan lengkap !');
		}
	}
</script>
</html>
~~~
Jika nama, enail dan alaat terisi atau tidak kosong maka akan dikembalikan ke nilai true
pada form agar dapat diteruskan
![Screenshot (108)](https://user-images.githubusercontent.com/81818989/116099474-36f26700-a6d6-11eb-8cd1-d7b243ab4772.png)
Jika masih ada yang kosong makan akan muncul alert "Anda harus mengisi data dengan lengkap"
![Screenshot (109)](https://user-images.githubusercontent.com/81818989/116099644-5f7a6100-a6d6-11eb-960f-0b7671bcdb9f.png)
