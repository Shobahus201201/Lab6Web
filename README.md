| Nama      | Shobahus Solichin |
| ----------- | ----------- |
| NIM     | 312010076       |
| Kelas   | TI.20.A.1        |

## Langkah langkah praktikum 6

## 1. Buat folder baru dengan nama lab6_css_framework, Buat file baru dokumen html

![Foto](Foto/foto1.png)

## 2. Buatlah layout web sederhana menggunakan css frameword (Twitter Bootsrtap)

### 1. Quick start
Buka web https://getbootstrap.com Disini saya memakai Bootstrap 4. Copy atau download CSS & JS Bootstrap, Saya memilih copy

```HTML <br>
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>lab6_css_framework</title>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css" integrity="sha384-zCbKRCUGaJDkqS1kPbPd7TveP5iyJE0EjAuZQTgFLD2ylzuqKfdKlfG/eSrtxUkn" crossorigin="anonymous">
</head>
<body>

<script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-fQybjgWLrvvRgtW6bFlB7jaZrFsaBXjsOMm/tB9LTS58ONXgqbR9W8oWht/amnpF" crossorigin="anonymous"></script>
</body>
</html>
```

### 2. Navbar
Buat komponen website yang berupa menu. yang biasanya diletakkan pada header website.

Untuk mencari component klik menu documentation pada web bootstrap

```html <br>
<!--NAVBAR-->
<div class="jumbotron jumbotron-fluid bg-light pb-2 mb-1">
  <div class="container">
    <h1 class="display-4">Layout Sederhana</h1>
  </div>
</div>

<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Artikel</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">About</a>
      </li>
      <li class="nav-item">
        <a class="nav-link">Kontak</a>
      </li>
    </ul>
  </div>
</nav>
```

![Foto](Foto/foto2.png)

### 3. Jumbotron
Selanjutnya buat jumbotron atau area besar pada Bootstrap, umumnya digunakan untuk menampilkan sebuah infromasi penting.

```html <br>
<!--JUMBOTRON-->
<div class="jumbotron">
  <h1 class="display-4">Hello, world!</h1>
  <p class="lead">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
  quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
  consequat.</p>
  <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
</div>
</div>
```

![Foto](Foto/foto3.png)

### 4. Cards
Untuk membuat body konten, saya menggunakan cards. 

pertama saya akan membagi kolom menggunakan display flex agar dapat memuat 2 kolom yang nanti akan di isi oleh menu List Group

```html <br>
<!--CARDS-->
    <div class="row" >
    <div class="col">
    <div class="card pt-3">
      <img src="120px.png" class="card-img-top rounded-circle" alt="...">
      <div class="card-body">
        <h5 class="card-title text-center">Heading</h5>
        <p class="card-text text-center">Some quick example text to build on the card title and make up the bulk of the card's content.
        <a href="#" class="btn btn-secondary mt-3">View Detail</a></p>
      </div>
    </div>
    </div>
    <div class="col">
    <div class="card pt-3">
      <img src="120px.png" class="card-img-top rounded-circle" alt="...">
      <div class="card-body">
        <h5 class="card-title text-center">Heading</h5>
        <p class="card-text text-center">Some quick example text to build on the card title and make up the bulk of the card's content.
        <a href="#" class="btn btn-secondary mt-3">View Detail</a></p>
      </div>
    </div>
    </div>
    <div class="col">
    <div class="card pt-3">
      <img src="120px.png" class="card-img-top rounded-circle" alt="...">
      <div class="card-body">
        <h5 class="card-title text-center">Heading</h5>
        <p class="card-text text-center">Some quick example text to build on the card title and make up the bulk of the card's content.
        <a href="#" class="btn btn-secondary mt-3">View Detail</a></p>
      </div>
    </div>
    <div class="col-md-3">
          <img src="150.jpeg" alt="...">
        </div>
      </div>
    </div>

  </div>

  <div class="p-2">
```

Penjelasan :

`col` memberi style sebuah table berdasarkan kolom tertentu 

`img-rounded-circle` untuk membuat border pada gambar menjadi bulat

`pt-3` padding top = 3

`mt-3` margin top = 3

saya menambah style untuk mengatur ukuran dan posisi pada gambar

```html <br>
.card-img-top{
	width: 120px;
	align-self: center;
}
```

refresh browser

![Foto](Foto/foto4.png)

### 5. List Group
lalu tambahkan widget disamping kanan cards

```html <br>
<!--LIST GROUP-->
    <div class="col">
    <div class="list-group">
      <a href="#" class="list-group-item list-group-item-action active" aria-current="true">
        Widget Header
      </a>
      <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
      <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
      <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
      <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
      <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
    </div>
    <div class="list-group mt-3">
      <a href="#" class="list-group-item list-group-item-action active" aria-current="true">
        Widget Text
      </a>
      <span class="list-group-item list-group-item-action">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
      tempor incididunt ut.</span>
    </div>
  </div>  
  </div>
</div>
```
![Foto](Foto/foto5.png)

### 6. Cards 2
Buat body konten untuk yg kedua, dan masih menggunakan card

```html <br>
<!--CARDS 2-->
    <div class="mt-3 mb-5">
      <h2>First Featurette Heading</h2>
      <div class="row no-gutters">
        <div class="col-md-3">
          <img src="150.jpeg" alt="...">
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
          </div>
        </div>
      </div>
    </div>
<hr>
    <div class="mt-5">
      <h2>First Featurette Heading</h2>
      <div class="row">
        <div class="col-md-8">
          <div class="card-body">
            <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
          </div>
        </div>
        <div class="col-md-3">
          <img src="150.jpeg" alt="...">
        </div>
      </div>
    </div>

  </div>
```

![Foto](Foto/foto6.png)

### 7. Footer 
bagian akhir tambahkan footer.

```html <br>
<footer>
  <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
</div>
```

![Foto](Foto/foto7.png)

## Tampilan full

![Foto](Foto/foto8.png)
![Foto](Foto/foto9.png)