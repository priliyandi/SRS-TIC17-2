<p align="center"><font size="5"><b>Software Requirements Specifications</b></font><br>
"Sistem Informasi Absensi dan Penggajian Kafka Konveksi"</p>

<p align="center"><img src="Gambar/POLINDRA.png" width="250" height="250"></p>

<br>

<p align="center">
    <b><font size="4">Kelompok 2:</font></b><br>
    1. Priliyandi (1703073) <br>
    2. Riyanwar Setiadi (1703087)<br>
    3. Setyo Abiansyah (1703071)<br>
    4. Uum Khumaeroh (1703084)
</p>
<center><font size="3"><p align="center">Kelas D3TI2C</p></font></center>

<br>

<br>

<p align="center"><b><font size="5">D3 TEKNIK INFORMATIKA</font></b><br>
<b><font size="3">POLITEKNIK NEGERI INDRAMAYU</font></b><br>
<b><font size="3">2019</font></b></p>

**1.** **Pendahuluan** <br>
	**1.1**	**Tujuan** <br>
<ol>Dokumen ini akan menyajikan deskripsi rinci tentang Sistem Informasi Absensi dan Penggajian di Kafka Konveksi yang akan dikembangkan. Dokumen akan menjelaskan mengenai spesifikasi pada Sistem Informasi Absensi dan Penggajian di Perusahaan Kafka seperti fitur sistem, antarmuka sistem, sistem apa yang akan dilakukan, apa saja kendala pada saat aplikasi beroperasi, dan bagaimana system akan bereaksi pada saat sedang digunakan oleh pemakai atau user.</ol> <br>

**1.2**	**Lingkup Masalah** <br>
<ol>Dokumen ini menyediakan acuan untuk pengendalian tentang Sistem Informasi Absensi dan Penggajian di Kafka Konveksi. Adapun ruang lingkup pembuatan aplikasi ini adalah berbasis website dan mobile yang memilih beberapa fasilitas yang ada yaitu :<br>

1.	Admin untuk mengelola data CRUD (Create, Read, Update, Delete) yang ada pada fitur- fitur Sistem Informasi Absensi dan Penggajian di Kafka Konveksi seperti input gaji hasil dari pekerjaan karyawan dan jenis pekerjaan, menambahkan data karyawan, mendaftarkan akun karyawan, serta memonitoring laporan rekap gaji.<br>
2.	Karyawan sebagai tempat melayani keinginan konsumen maupun dalam mendesain gambar.<br>
3.	Pemilik sebagai pemilik distro yang biasanya sudah memiliki konveksi sendiri untuk membuat berbagai produk-produk yang dipasarkan di distro tersebut.</ol><br>
 <br>

**1.3**	**Definisi, akronim, singkatan** <br>
		Adapun definisi dari dokumen tersebut adalah :<br>
		<table>
			<tr>
				<td> No </td>
				<td> Akronim </td>
				<td> Singkatan </td>
			</tr>
			<tr>
				<td> 1. </td>
				<td> SPMP </td>
				<td> Software Project Management Plan </td>
			</tr>
			<tr>
				<td> 2. </td>
				<td> SRS </td>
				<td> Software Requirements Specifications </td>
			</tr>
			<tr>
				<td> 3. </td>
				<td> SDD </td>
				<td> Software Design Document </td>
			</tr>
			<tr>
				<td> 4. </td>
				<td> DFD </td>
				<td> Data Flow Diagram </td>
			</tr>
			<tr>
				<td> 5. </td>
				<td> IEEE </td>
				<td> International Institute of Electronic and Electrical Engineers </td>
			</tr>
			<tr>
				<td> 6. </td>
				<td> CRUD </td>
				<td> Create, Read, Update, dan Delete </td>
			</tr>
			<tr>
				<td> 7. </td>
				<td> SIAPKK </td>
				<td> Sistem Informasi Absensi dan Penggajian di Kafka Konveksi </td>
			</tr>
		</table>
	**1.4**	**Referensi** <br>
IEEE. IEEE Std 830-1998 IEEE Recommended Practice for Software Requirements Specifications.<br>
	**1.5**	**Overview** <br>
<ol>Penulisan dokumen SRS ini dibagi menjadi beberapa bab sebagai berikut:<br>

**BAB I** berisi pendahuluan, menjelaskan mengenai tujuan pembuatan dokumen SRS, lingkup, definisi (akronim, atau singkatan), referensi, dan Overview.<br>

**BAB II** menjelaskan keseluruhan deskripsi dari Sistem Informasi Absensi dan Penggajian di Kafka Konveksi. Deskripsi umum tersebut memberikan gambaran lengkap mengenai semua fungsi yang akan dilakukan oleh sistem.<br>

**BAB III** berisi penjelasan detail dari  masing-masing kebutuhan lain yang spesifik.<br>

**BAB IV** berisikan tentang uraian mengenai informasi pendukung dalam pembuatan proyek Sistem Informasi Absensi dan Penggajian di Kafka Konveksi.<br></ol>

**2.** **Gambaran Umum**<br>
<ol>Kafka merupakan sebuah perusahaan konvenksi dengan karyawan yang cukup banyak. Oleh karena itu, sistem absen dan penggajian merupakan hal yang sangat pokok pada kegiatan financial sebuah perusahaan karena hal tersebut sangat berpengaruh kepada kinerja para pegawai yang setiap hari melakukan aktifitas. Sistem penggajian menyajikan cara-cara penggajian pegawai secara akurat, menghasilkan laporan-laporan yang diperlukan dan menyajikan kebutuhan informasi kepada manajemen. Adapun kendala yang dihadapi di Kafka konveksi yaitu absensi dan penggajian yang masih dilakukan secara manual masih berbentuk arsip sehingga memperlambat dalam proses pencarian, penghitungan dan proses pembuatan laporan penggajian. oleh karena itu, akan dirancang sebuah sistem informasi absensi dan  penggajian. Antara lain meliputi sistem absensi karyawan, sistem penghitungan gaji dan berbagai attributnya seperti lembur, cuti, potongan dan sebagainya secara terotomatisasi. Selain itu sistem juga mampu membuat berbagai laporan baik yang ditujukan untuk karyawan seperti slip gaji dan laporan yang ditujukan untuk direktur seperti laporan data karyawan, laporan absensi karyawan, dan laporan gaji karyawan secara terotomatisasi dimana system informasi tersebut dibuat dengan Framework Laravel dan Android.<br></ol>

**2.1** **Perspektif produk**<br>
<ol>Sistem Informasi Absensi dan Penggajian Karyawan di Kafka Konveksi adalah aplikasi yang digunakan untuk melakukan absensi dan cetak struk gaji melalui mobile yang sebelumnya menggunakan metode manual dengan menulis struk gajinya. Kemudian Sistem Informasi Absensi dan Penggajian Karyawan di Kafka Konveksi juga dapat melakukan perhitungan gaji karyawan<br></ol>

**2.1.1** **Antarmuka Sistem**<br>
**2.1.1.1**	**Use Cases Pemilik**<br>
<center><img src="Gambar/usecase_pemilik.png" width="250" height="250"></center>
**2.1.1.2** **Use Cases Karyawan**<br>
<center><img src="Gambar/usecase_karyawan.png" width="250" height="250"></center>

**2.1.1.3**	**Use Cases Admin**<br>
<center><img src="Gambar/usecase_admin.png" width="250" height="250"></center>

**2.1.2** **Antarmuka pengguna**<br>
<ol>Sistem Informasi Absensi dan Penggajian Karyawan di Kafka Konveksi menggunakan antarmuka berbasis mobile dan website. Dimana antarmuka mobile digunakan untuk karyawan sedangkan antarmuka website digunakan oleh admin.<br></ol>

**2.1.3** **Antarmuka perangkat keras**<br>
•	Laptop<br>
•	Processor Core i3 or higher<br>
•	Penyimpanan(Hardisk) Minimal 4 GB free space<br>
•	Smartphone minimal android Jelly Bean or higher<br>
•	Monitor resolusi 1240 x 768 colors 5<br>
•	Keyboard dan mouse compatible with windows<br>

**2.1.4** **Antarmuka perangkat lunak**<br>
<ol>Perangkat lunak yang dibutuhkan untuk aplikasi ini yaitu :<br></ol>
•	Windows 7 or higher<br>
•	Android Studio<br>
•	Corel Draw X7<br>
•	Database Mysql<br>
•	Balsamiq Mockups 3<br>
•	Sublime Text 3<br><br>

**2.1.5** **Antarmuka komunikasi**<br> 
•	Paket Data<br>
•	Wifi<br>
•	Modem<br>
•	Smartphone<br>

2.1.6** **Batasan-batasan memori**<br>
•	RAM yang kami gunakan adalah minimal 4 gb.<br>
•	Memori yang dibutuhkan aplikasi minimal 50 mb.<br>

**2.1.7** **Operasi-operasi**<br>
•	Input data karyawan<br>
•	Input data absensi<br>
•	Input data gaji karyawan<br>
•	Input data pekerjaan<br>
•	Update data admin<br>
•	Update data karyawan<br>
•	Update data absensi<br>
•	Update data gaji karyawan<br>
•	Tampilan informasi karyawan<br>
•	Tampilan struk gaji karyawan<br>
•	Laporan Absensi<br>
•	Laporan rekap gaji<br>

**2.1.8** **Kebutuhan-kebutuhan dalam tahapan adaptasi**<br>

<ol>
Kebutuhan adaptasi yang diperlukan pada saat pengembangan aplikasi dengan menggunakan fungsi update data agar memudahkan admin dalam mengkoreksi pengetikan yang salah.
</ol>

**2.2** **Fungsi-fungsi produk**<br>

<ol>
•	Memudahkan proses absensi karyawan.<br>
•	Memudahkan dalam pembuatan laporan absensi, laporan struk gaji, dan laporan rekap gaji karyawan<br>
•	Memberi tahu karyawan tentang informasi data karyawan dan informasi gaji karyawan.<br>
•	Menambah data karyawan, data absensi, dan data gaji karyawan.<br>
•	Memudahkan pemilik kafka konveksi dalam melihat laporan rekap gaji, laporan absensi, dan laporan data karyawan.<br>
</ol>

**2.3** **Karakteristik pengguna**<br>

<ol>
•	Pengguna mampu membaca dan menulis.<br>
•	Pengguna mengerti cara menggunakan smartphone dengan sistem operasi android.<br>
•	Pengguna mengerti cara menggunakan PC dengan sistem operasi setidaknya windows.<br>
•	Mengerti cara menggunakan browser pada PC.<br>
</ol>

**2.4** **Batasan-batasan**<br>

<ol>
•	Berjalan pada platform android dan website<br>
•	Sementara ini aplikasi ini hanya untuk Kafka Konveksi<br>
•	Aplikasi ini tidak untuk layanan pemesanan<br>
</ol>


**2.5** **Asumsi-asumsi dan ketergantungan / keterkaitan**<br>
<ol>Sistem Informasi Absensi dan Penggajian Karyawan di Kafka Konveksi ini dapat dikembangkan lagi dengan menambah banyak perusahaan konveksi, dan penambahan super admin untuk konfirmasi perusahaan konveksi mana saja yang boleh menggunakan aplikasi ini. Sehingga aplikasi ini dapat digunakan oleh banyak perusahaan konveksi yang ingin menggunakan aplikasi ini.
</ol>

**2.6** **Kebutuhan-kebutuhan penyeimbang**<br>
	•	Customer Requirements <br>
<ol>Customer Requirements adalah analisis yang dilakukan terhadap pelanggan agar dapat mengetahui apa saja kebutuhan pelanggan sehingga pengembang dapat membuat sistem yang sesuai dengan kebutuhan pelanggan.<br></ol>
•	Detil Requirements<br>
<ol>Detil Requirements adalah suatu analisis yang terdiri dari properti dan fungsionalitas spesifik yang diekspresikan dalam bentuk yang detail<br></ol>

**3.** **Kebutuhan lain yang spesifik**<br>
	
**3.1** **Performa**<br>
•	Berjalan pada system operasi minimal android lollipop. <br>
•	Respon program kurang 30 detik. <br>
•	Berjalan pada browser apapun.<br></ol>

**3.2** **Keamanan Aplikasi** <br>
<ol>Validasi username dan password harus sesuai dengan yang didaftarkan sehingga tidak terjadi kesalahan login pada Sistem Informasi Absensi dan Penggajian Karyawan di Kafka Konveksi.
</ol>

**4.** **Informasi Pendukung**<br>
<ol>
		1. Informasi permasalahan yang sedang di alami<br>
		2. Informasi Perusahaan<br>
		3. Informasi sistem yang ada di perusahaan yang terkait dengan permasalahan yang diambil<br>
	</ol>