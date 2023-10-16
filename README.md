# Lab4Web
Nama : Anggita Risqi Nur Clarita

NIM : 312210450

Kelas : TI.22.A.4

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Modul Praktikum 4|[Click Here](https://drive.google.com/file/d/1rBPhEkkg5SBwTc119zkqYyBGwA3d_9Yr/view)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Box Element|[Click Here](#box-element)|
|4|Layout Sederhana|[Click Here](#layout-sederhana)|
|5|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Praktikum
> ### Instruksi Praktikum
> 1. Persiapkan text editor misalnya **VSCode**.
>
> 2. Buat folder baru dengan nama **Lab4Web**.
>
> 3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.

## Box Element
1. ### Membuat Box Element
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Box Element</title>
    </head>
    <body>
        <header>
            <h1>Box Element</h1>
        </header>
    </body>
    </html>
    ```

    **Keterangan** : Disini diperintahkan untuk membuat file dengan nama `lab4_box.html`, kemudian menambahkan script yang telah tersedia.

    Kemudian tambahkan kode untuk membuat box element dengan tag div, seperti berikut:

    ```html
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
    ```

    Selanjutnya tambahkan deklarasi CSS pada `head` untuk membuat float element, seperti berikut:

    ```css
    <style>
        div {
            float:left;
            padding: 10px;
        }
        .div1 {
            background: red;
        }
        .div2 {
            background: yellow;
        }
        .div3 {
            background: green;
        }
    </style>
    ```

    **Output**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/1.png)
     **Keterangan** : Script HTML tersebut digunakan untuk membuat **Box Element Float**

2. ### Mengatur Clearfix Element
    ```html
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
    </section>
    ```

    Setelah itu tambahkan element div4 lainnya seteleah div3 seperti diatas, Kemudian atur property clear pada CSS, seperti berikut:

    ```css
    .div4 {
        background-color: blue;
        clear: left;
        float: none;
    }
    ```

    **Output**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/2.png)
    **Keterangan** : **_Clearfix_** digunakan untuk mengatur element setelah float element. Dan property clear digunakan untuk mengaturnya.


## Layout Sederhana
1. ### Membuat Layout Sederhana
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div id="container">
        
        </div>
    </body>
    </html>
    ```

    Pada Praktikum kali ini diperintahkan untuk membuat folder baru dengan nama **lab4_layout**, kemudian membuat file baru di dalamnya dengan nama `home.html`, dan file css dengan nama `style.css`, pada file `home.html` ditambahkan script diatas.

    Kemudian tambahkan script, seperti berikut:

    ```html
    <header>
        <h1>Layout Sederhana</h1>
    </header>
    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="contact.html">Kontak</a>
    </nav>
    <section id="hero"></section>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>
    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/3.png)
    **Keterangan** : Script HTML tersebut digunakan untuk membuat tampilan kerangka layout.

    Kemudian tambahkan kode CSS untuk membuat layout-nya, seperti berikut:

    ```css
    /* import google font */
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

    /* Reset CSS */
    * {
        margin: 0;
        padding: 0;
    }

    body {
        line-height:1;
        font-size:100%;
        font-family:'Open Sans', sans-serif;
        color:#5a5a5a;
    }

    #container {
        width: 980px;
        margin: 0 auto;
        box-shadow: 0 0 1em #cccccc;
    }

    /* header */
    header {
        padding: 20px;
    }

    header h1 {
        margin: 20px 10px;
        color: #b5b5b5;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/4.png)
    **Keterangan** : Script CSS tersebut digunakan untuk membuat tampilan header layout.


2. ### Membuat Navigasi
    ```css
    /* navigasi */
    nav {
        display: block;
        background-color: #1f5faa;
    }

    nav a {
        padding: 15px 30px;
        display: inline-block;
        color: #ffffff;
        font-size: 14px;
        text-decoration: none;
        font-weight: bold;
    }

    nav a.active,
    nav a:hover {
        background-color: #2b83ea;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/5.png)
    **Keterangan** : Script CSS tersebut digunakan untuk mengatur tampilan navigasi.


3. ### Membuat Hero Panel
    ```html
    <section id="hero">
        <h1>Hello World!</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
        <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>
    ```

    Selanjutnya untuk membuat **hero panel** maka tambahkan kode script CSS, seperti berikut:

    ```css
    /* Hero Panel */
    #hero {
        background-color: #e4e4e5;
        padding: 50px 20px;
        margin-bottom: 20px;
    }

    #hero h1 {
        margin-bottom: 20px;
        font-size: 35px;
    }

    #hero p {
        margin-bottom: 20px;
        font-size: 18px;
        line-height: 25px;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/6.png)
    **Keterangan** : Script diatas digunakan untuk membuat tampilan hero panel.


4. ### Mengatur Layout Main dan Sidebar
    ```css
    /* main content */
    #wrapper {
        margin: 0;
    }

    #main {
        float: left;
        width: 640px;
        padding: 20px;
    }

    /* sidebar area */
    #sidebar {
        float: left;
        width: 260px;
        padding: 20px;
    }
    ```

5. ### Membuat Sidebar Widget
    ```html
    <aside id="sidebar">
        <div class="widget-box">
            <h3 class="title">Widget Header</h3>
            <ul>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
            </ul>
        </div>
        <div class="widget-box">
            <h3 class="title">Widget Text</h3>
            <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
        </div>
    </aside>
    ```

    Kemudian tambahkan kode CSS untuk membuat tampilan **sidebar widget**, seperti berikut:

    ```css
    /* widget */
    .widget-box {
        border:1px solid #eee;
        margin-bottom:20px;
    }

    .widget-box .title {
        padding:10px 16px;
        background-color:#428bca;
        color:#fff;
    }

    .widget-box ul {
        list-style-type:none;
    }

    .widget-box li {
        border-bottom:1px solid #eee;
    }

    .widget-box li a {
        padding:10px 16px;
        color:#333;
        display:block;
        text-decoration:none;
    }

    .widget-box li:hover a {
        background-color:#eee;
    }

    .widget-box p {
        padding:15px;
        line-height:25px;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/7.png)
    **Keterangan** : Script diatas digunakan untuk membuat tampilan sidebar widget.


6. ### Mengatur Footer
    ```css
    /* footer */
    footer {
        clear:both;
        background-color:#1d1d1d;
        padding:20px;
        color:#eee;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/8.png)
    **Keterangan** : Script diatas digunakan untuk megatur tampilan footer.

7. ### Menambahkan Elemen lainnya pada Main Content
    ```html
    <section id="main">
        <div class="row">
            <div class="box">
                <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
            </div>
            <div class="box">
                <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
            </div>
            <div class="box">
                <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
            </div>
        </div>
    </section>    
    ```

    Kemudian tambahkan script CSS, seperti berikut:

    ```css
    /* box */
    .box {
        display:block;
        float:left;
        width:33.333333%;
        box-sizing:border-box;
        -moz-box-sizing:border-box;
        -webkit-box-sizing:border-box;
        padding:0 10px;
        text-align:center;
    }

    .box h3 {
        margin: 15px 0;
    }

    .box p {
        line-height: 20px;
        font-size: 14px;
        margin-bottom: 15px;
    }

    .box img {
        border: 0;
        vertical-align: middle;
    }

    .image-circle {
        border-radius: 50%;
    }

    .row {
        margin: 0 -10px;
        box-sizing: border-box;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
    }

    .row:after, .row:before,
    .entry:after, .entry:before {
        content:'';
        display:table;
    }

    .row:after,
    .entry:after {
        clear:both;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/9.png)
    **Keterangan** : Script diatas digunakan untuk megatur tampilan content.

8. ### Menambahkan Content Artikel
    ```html
    <hr class="divider" />
    <article class="entry">
        <h2>First featurette heading.</h2>
        <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
    </article>
    <hr class="divider" />
    <article class="entry">
        <h2>First featurette heading.</h2>
        <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
    </article>
    ```

    Kemudian tambahkan script CSS, seperti berikut:

    ```css
    .divider {
        border:0;
        border-top:1px solid #eeeeee;
        margin:40px 0;
    }

    /* entry */    
    .entry {
        margin: 15px 0;
    }

    .entry h2 {
        margin-bottom: 20px;
    }

    .entry p {
        line-height: 25px;
    }
        
    .entry img {
        float: left;
        border-radius: 5px;
        margin-right: 15px;
    }
        
    .entry .right-img {
        float: right;
    }
    ```

    **Output**

    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/10.png)
    **Keterangan** : Script diatas digunakan untuk membuat content artikel pada main content.

9. ### Tampilan Website Secara Keseluruhan
    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/home.png)

## Pertanyaan dan Tugas

1. **Tambahkan Layout untuk menu About (buat single layout yang berisi deskripsi, portfolio, dll)**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/about.png)
    **Keterangan** : Disini saya menambahkan layout untuk menu About seperti berikut dan tampilan websitenya seperti ini, untuk script-nya dapat dilihat langsung pada file [about.html](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/lab4_layout/about.html) dan [about.css](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/lab4_layout/about.css)

2. **Tambahkan layout untuk menu Contact (yang berisi form isian: nama, email, message, dll)**
    
    ![image](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/screenshot/contact.png)
    **Keterangan** : Disini saya menambahkan layout untuk menu Contact seperti berikut dan tampilan websitenya seperti ini, untuk script-nya dapat dilihat langsung pada file [contact.html](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/lab4_layout/contact.html) dan [contact.css](https://github.com/AnggitaRisqiNC/Lab4Web/blob/main/lab4_layout/contact.css)

## Finish