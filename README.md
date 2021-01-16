# Google Drive Index

Menggabungkan [Cloudflare Workers](https://workers.cloudflare.com/) dan [Google Drive](https://www.google.com/drive/) akan memungkinkan Anda untuk mengindeks file google drive anda di browser.

[Script](https://github.com/kuro-creator/Google-Drive-Index/blob/main/worker/worker-beta.js) ini adalah hasil redesain saya dari [ParveenBhadooOfficial](https://github.com/ParveenBhadooOfficial/Google-Drive-Index).

## Situs Demo

* [Light Mode Demo](https://light.floral.workers.dev/0:/)
* [Dark Mode Demo](https://dark.floral.workers.dev/0:/)
* [Password Demo](https://pass.floral.workers.dev/0:/) id dan passwordnya adalah `admin` and `admin`

## Pembaharuan
* Tambah menu list project
* Background keren

## Cara Deploy
Buka link di bawah ini :

- https://indexgenerator.floral.workers.dev/

Auth dan dapatkan kode
    
Setelah itu, deploy kode tsb ke Cloudflare Workers

Untuk lebih detailnya bisa tonton video ini [Watch Video](https://www.youtube.com/watch?v=8WMddzVX1Dw&feature=youtu.be)

## Contoh pengisian Config dasar

	"siteName": "Kuro Creator Drive Index", // Website name
	"client_id": "58094879805-4654k2k5nqdid5bavft7fvea5u9po0t1.apps.googleusercontent.com",
	"client_secret": "ZNPZ-vS6N9Zjsyb_sNMZmXHL",
	"refresh_token": "sNMZmXHLsNMZmXHLsNMZmXHLsNMZmXHLsNMZmXHLsNMZmXHL", // Authorize token

````
"roots": [
{
	"id": "0BO_4Z3921k36Uk2PVA", // shared drive id or folder id
	"name": "Index 1", // nama drive
	"user": "admin", // username
	"pass": "admin", // password
	"protect_file_link": true }, // protects the direct links when true.
{
   "id": "1jxK5rZxsov72dBGHB9h-R723_VWt8yc3",
   "name": "Index 2"
}
],
````

## Kustomisasi Brand

* Dalam rilisan ini, kamu dapat mengcustom indeks sesuai kebutuhanmu.
* Di line ke 57. kamu dapat mengubah tema jadi dark mode atau light mode,di mana false adalah dark mode, dan true adalah light mode
* Lihat kode berikut untuk mengerti kustomisasinya.
````
const uiConfig = {
	"theme": "kuro_bootstrap", // Change doesn't works
	"dark_mode": true, // Please select above theme before selecting here true or false
	"version": "2.0", // don't touch this one. get latest code using generator at https://github.com/kuro-creator/Google-Drive-Index
	"logo_image": false, // Site Logo Name, can also be replaced with Image using <img border="0" alt="Alternative Name" src="logo-url" height="30px">
	"logo_link_name": "Light Demo", // if logo is true then link otherwise just text for name
	"contact_link": "https://github.com/kuro-creator/Google-Drive-Index", //Link to Contact Button on Menu
	"copyright_year": "2020", // year of copyright, can be anything like 2015 - 2020 or just 2020
	"company_name": "Search Google Web", // Name next to copyright
	"company_link": "https://www.google.com", // link of copyright name
	"credit": true, // Set this to true to give us credit
  	"project1_name": "Project 1",
  	"project1_link": "https://",
  	"project2_name": "Project 2",
  	"project2_link": "https://",
  	"project3_name": "Proect 3",
  	"project3_link": "https://",
  	"project4_name": "Project 4",
  	"project4_link": "https://",
  	"project5_name": "Project 5",
  	"project5_link": "https://",
  	"project6_name": "Project 6",
  	"project6_link": "https://",
  	"project7_name": "Project 7",
  	"project7_link": "https://",
};
````

## Credits

* Source: [maple3142](https://github.com/maple3142/GDIndex)
* Source: [yanzai](https://github.com/yanzai/goindex)
* Source: [ParveenBhadooOfficial](https://github.com/ParveenBhadooOfficial/Google-Drive-Index)
* New Design: [Bootstrap](https://getbootstrap.com)
* Cloudflare: Workers
