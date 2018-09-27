Modifikasi aplikasi dari jurnal untuk memasukan data baru dengan checkbox berupa 
Genre film yang disukai (horror, action, anime, thriller dan animasi)*
Tempat wisata tujuan travelling (Bali, Raja Ampat, Pulau Derawan, Bangka Belitung, Labuan Bajo)*

Ketentuan :
*Sebelum menambahkan geren film dan tempat wisata tujuan. Pengguna harus login terlebih dahulu
*Data pengguna, genre film, tempat wisata tujuan harus masuk ke array

jawwb

formawal.php

<form method="post" action="proses.php">
<br><b>Username :</b><input name="Username" type="text" size="30" maxlength="100">
<br><b>Password :</b><input name="password" type="password" size="30" maxlength="100">
<br><input type="submit" name="login" value="Login">
</form>


proses.php

Genre Film Yang disukai?<br />
<form action="#" method="POST">
	<input type="checkbox" name="Film[]" value="Action">Action<br />
	<input type="checkbox" name="Film[]" value="Horror">Horror<br />
	<input type="checkbox" name="Film[]" value="Anime">Anime<br />
	<input type="checkbox" name="Film[]" value="Thriller">Thriller<br />
	<input type="checkbox" name="Film[]" value="Animasi">Animasi<br />
<br>

Tempat wisata tujuan travelling?<br />
	<input type="checkbox" name="Tempat[]" value="Bali">Bali<br />
	<input type="checkbox" name="Tempat[]" value="Raja Ampat">Raja ampat<br />
	<input type="checkbox" name="Tempat[]" value="Pulau Derawan ">Pulau Derawan<br />
	<input type="checkbox" name="Tempat[]" value="Bangka Belitung">Bangka Belitung<br />
	<input type="checkbox" name="Tempat[]" value="Labuan Bajo">Labuan Bajo<br />
	<input type="submit" value="Kirim">
</form><br>

<p align="center">EDIT DATA
<?php
	if(isset($_POST['Pilihan'])){
		$pilihan		= $_POST['pilihan'];

	}
	else{
	$Film= '';
	$Tempat = '';
	}
?>
