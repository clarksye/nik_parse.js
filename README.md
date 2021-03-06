# nik_parse.js
Parse & Validasi Nomor Induk Kependudukan (NIK) KTP Menggunakan Javascript.

# rumus
<img src="kodenik.jpg"/>

Sample
------
```html
<script type="text/javascript" src="js/nik_parse.js"></script>
<script>

	const nik = "3204110609970001";

	nikParse(nik, function(result) {
	
		// object
		console.log(result);
	
	});
	
</script>
```

Result
------
```json
{
  "status": "success",
  "pesan": "NIK valid",
  "data": {
    "nik": "3204110609970001",
    "kelamin": "LAKI-LAKI",
    "lahir": "06/09/1997",
    "provinsi": "JAWA BARAT",
    "kotakab": "KAB. BANDUNG",
    "kecamatan": "KATAPANG",
    "uniqcode": "0001",
    "tambahan": {
      "kodepos": "40921",
      "pasaran": "Sabtu Pahing, 6 September 1997",
      "usia": "23 Tahun 1 Bulan 27 Hari",
      "ultah": "10 Bulan 8 Hari Lagi",
      "zodiak": "Virgo"
    }
  }
}
```

```json
{
  "status": "error",
  "pesan": "NIK tidak valid"
}
```

<h2><a target="_BLANK" href="http://bachors.com/code/validasi-nik-ktp-menggunakan-javascript-nik_parsejs?embed">DEMO</a></h2>

# nik_parser.ts
NIK Parser in TypeScript by <a target="_BLANK" href="https://github.com/mul14/nik_parser.ts?fbclid=IwAR0yu4Vadmdi13Z9rVNyiSIuZuybq2bD1THGNTQqZMQNanYvjsCVN9HldR0">mul14</a>.

# note
Data yang dihasilkan hanya hasil menterjemahkan tiap digit NIK sehingga data yang dihasilkan adalah tempat pertamakali NIK dibuat/tempat lahir (bukan tempat domisili pemilik NIK secara uptodate).
