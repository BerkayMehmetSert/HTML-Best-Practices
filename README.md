<div align="center">
<h1>HTML'de Örnek Yöntemler</h1>
<a target="_blank" href="https://www.linkedin.com/in/berkaymsert/">
   <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin" />
</a>
<a target="_blank" href="https://www.instagram.com/berkaysert.h">
   <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" />
</a>
<a target="_blank" href="https://www.buymeacoffee.com/BerkayMSert">
   <img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me A Coffee" />
</a>
<a target="_blank" href="https://www.patreon.com/BerkayMSert">
   <img src="https://img.shields.io/badge/Patreon-F96854?style=for-the-badge&logo=patreon&logoColor=white" alt="Patreon" />
</a>

<sub>Yazar:
<a href="https://www.linkedin.com/in/berkaymsert/" target="_blank">Berkay M. Sert</a>
</sub>

</div>  

# ✨ Genel

### DOCTYPE ile başlamak

DOCTYPE standart modu etkinleştirmek için gereklidir.

⛔ Yanlış:

```html
<html>
...
</html>
```

✅ Doğru:

```html
<!DOCTYPE html>
<html>
...
</html>
```

### Eskimiş ya da geçersiz DOCTYPE kullanmayın

Güncel bir DOCTYPE kullanmak gerekir.

⛔ Yanlış:
  
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

✅ Doğru:

```html
<!DOCTYPE html>
```

### XML etiketi kullanmayın

⛔ Yanlış:

```html
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
    <!DOCTYPE html>
```

✅ Doğru:

```html
<!DOCTYPE html>
```

### Karakter referanslarını mümkün olduğunca kullanmayın

UTF-8 ile bir HTML belgesi oluşturulurken, hemen hemen tüm karakterler (emojiler dahil) doğrudan kullanılabilir.

⛔ Yanlış:
  
```html
<p><small>Copyright &copy; 2022 W3C<sup>&reg;</sup></small></p>
```

✅ Doğru:

```html
<p><small>Copyright © 2022 W3C<sup>®</sup></small></p>
```

### `&`, `<`, `>` , `"`, ve `'` karakter referanslarını olduğu gibi kullanmaktan kaçının

Hatasız bir HTML belgesi oluşturmak için bu karakterlerden kaçınılmalıdır.

⛔ Yanlış:
  
```html
<h1>The "&" character</h1>
```

✅ Doğru:

```html
<h1>The &quot;&amp;&quot; character</h1>
```

### Kontrol veya görünmeyen karakterler için sayısal karakter referanslarını kullanın.

Bu karakterler başka bir karakter ile kolayca karıştırılabilir.

⛔ Yanlış:
  
```html
<p>This book can read in 1 hour.</p>
```

✅ Doğru:

```html
<p>This book can read in 1&#xA0;hour.</p>
```

### Yorum içeriğinin etrafına boşluk karakteri yerleştirirn

⛔ Yanlış:
  
```html
<!--This is a comment-->
```

✅ Doğru:

```html
<!-- This is a comment -->
```

### Kapanış etiketini unutmatyın

⛔ Yanlış:
  
```html
<html>
  <body>
    ...
```

✅ Doğru:

```html
<html>
  <body>
    ...
  </body>
</html>
```

### Boş eleman formatını karıştırmayın

⛔ Yanlış:
  
```html
<img alt="HTML Best Practices" src="/img/logo.png">
  <hr />
```

✅ Doğru:

```html
<img alt="HTML Best Practices" src="/img/logo.png">
    <hr>
```

### Etiketlerin ve özelliklerin değerlerinin etrafına boşluk karakteri koymayın

⛔ Yanlış:
  
```html
<h1 class=" title " >HTML Best Practices</h1>
```

✅ Doğru:

```html
<h1 class="title">HTML Best Practices</h1>
```

### Büyük küçük karakterleri aynı anda kullanmayın

⛔ Yanlış:
  
```html
<a HREF="http://www.w3.org/">W3C</a>
```

✅ Doğru:

```html
<a href="http://www.w3.org/">W3C</a>
<!-- ya da -->
<A HREF = "http://www.w3.org/" > W3C </A>
```

### Tırnak işaretlerini karıştırmayın

⛔ Yanlış:
  
```html
 <img alt="HTML Best Practices" src='/img/logo.jpg'>
```

✅ Doğru:

```html
 <img alt="HTML Best Practices" src="/img/logo.jpg">
```

### Özellikleri iki veya daha fazla boşluk ile ayırmayın

⛔ Yanlış:
  
```html
<input  type="text"    name="name" value="John Doe">
```

✅ Doğru:

```html
<input type="text" name="name" value="John Doe">
```

### Boolean özellik değerini yazmayın

⛔ Yanlış:
  
```html
<audio autoplay="autoplay" src="/audio/theme.mp3">
```

✅ Doğru:

```html
<audio autoplay src="/audio/theme.mp3">
```

### Ad alanlarını kullanmayın

⛔ Yanlış:
  
```html
<svg xmlns="http://www.w3.org/2000/svg">
  ...
</svg>
```

✅ Doğru:

```html
<svg>
  ...
</svg>
```

### XML özelliklerini kullanmayın

⛔ Yanlış:
  
```html
<span lang="ja" xml:lang="ja">...</span>
```

✅ Doğru:

```html
<span lang="ja">...</span>
```

### Varsayılan örtülü ARIA gramerini tercih edin

⛔ Yanlış:

```html
<nav role="navigation">
  <ul>
    <li>...</li>
  </ul>
</nav>
```

✅ Doğru:

```html
<nav>
  <ul>
    <li>...</li>
  </ul>
</nav>
```

## Kök elemanı

### `lang` özelliği ekleyin

⛔ Yanlış:
    
```html
<html>
</html>
```

✅ Doğru:

```html
<html lang="en">
</html>
```

### `lang` değerini mümkün olduğunca kısa tutun

⛔ Yanlış:
      
```html
<html lang="ja-JP">
</html>
```

✅ Doğru:

```html
<html lang="ja">
</html>
```

### Mümkün olduğunca `data-*` kullanmayın

⛔ Yanlış:

```html
<span data-language="french">chemises</span>
    ...
<strong data-type="warning">Do not wash!</strong>
```

✅ Doğru:

```html
<span title="French"><span lang="fr">chemises</span></span>
    ...
<strong class="warning">Do not wash!</strong>
```

## Metadata'yı belgeleyin

### `title` elemanı ekleyin

⛔ Yanlış:

```html
<head>
<meta charset="utf-8">
</head>
```

✅ Doğru:

```html
<head>
  <meta charset="utf-8">
  <title>HTML Best Practices</title>
</head>

### `base` elemanı kullanmayın

⛔ Yanlış:

```html
<head>
  <meta charset="utf-8">
  <title>HTML Best Practices</title>
  <base href="http://www.w3.org/">
</head>
```

✅ Doğru:

```html
<head>
  <meta charset="utf-8">
  <title>HTML Best Practices</title>
</head>
```

### Bağlantılı kaynakların MIME türünü belirtin

⛔ Yanlış:

```html
<link rel="stylesheet" href="/css/style.css">
```

✅ Doğru:

```html
<link rel="stylesheet" href="/css/style.css" type="text/css">
```

### `favicon.ico`'ya link vermeyin

⛔ Yanlış:

```html
<link rel="icon" href="/favicon.ico" type="image/vnd.microsoft.icon">
```

✅ Doğru:

```html
 <!-- Place `favicon.ico` in the root directory. -->
```

### `apple-touch-icon` ekleyin

⛔ Yanlış:

```html
<!-- Hey Apple! Please download `/apple-touch-icon.png`! -->
```

✅ Doğru:

```html
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
```

### Alternatif stil sayfalarına `title` ekleyin

⛔ Yanlış:

```html
<link href="/css/screen.css" rel="stylesheet">
<link href="/css/high-contrast.css" rel="alternate stylesheet">
```

✅ Doğru:

```html
<link href="/css/screen.css" rel="stylesheet">
<link href="/css/high-contrast.css" rel="alternate stylesheet" title="High Contrast">
```

### URL için `link` kullanın

⛔ Yanlış:

```html
<section itemscope itemtype="http://schema.org/BlogPosting">
  <meta content="https://example.com/blog/hello" itemprop="url">
    ...
</section>
```

✅ Doğru:

```html
<section itemscope itemtype="http://schema.org/BlogPosting">
  <link href="/blog/hello" itemprop="url">
    ...
</section>
```

### Belge karakter kodunu belirtin

⛔ Yanlış:

```html
<head>
  <title>HTML Best Practices</title>
</head>
```

✅ Doğru:

```html
<head>
  <meta charset="utf-8">
  <title>HTML Best Practices</title>
</head>
```

### Eski karakter kodlama formatını kullanmayın

⛔ Yanlış:

```html
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
```

✅ Doğru:

```html
<meta charset="utf-8">
```

### İlk önce karakter kodlamasını belirtin  

⛔ Yanlış:

```html
<head>
  <meta content="width=device-width" name="viewport">
  <meta charset="utf-8">
</head>
```

✅ Doğru:

```html
<head>
  <meta charset="utf-8">
  <meta content="width=device-width" name="viewport">
</head>
```

### CSS için `type` kullanmayın

⛔ Yanlış:

```html
<style type="text/css">
  ...
</style>
```

✅ Doğru:

```html
<style>
  ...
</style>
```

### CSS ve JavaScript etiketlerini karıştırmayın

⛔ Yanlış:

```html
<script src="/js/jquery.min.js"></script>
<link href="/css/screen.css" rel="stylesheet">
<script src="/js/main.js"></script>
```

✅ Doğru:

```html
<script src="/js/jquery.min.js"></script>
<script src="/js/main.js"></script>
<link href="/css/screen.css" rel="stylesheet">
```

## Bölümler

### `body` etiketi ekleyin

⛔ Yanlış:

```html
<html>
  <head>
    ...
  </head>
    ...
</html>
```

✅ Doğru:

```html
<html>
  <head>
    ...
  </head>
  <body>
    ...
  </body>
</html>
```

### `hgroup` etiketini unutun

⛔ Yanlış:

```html
<hgroup>
  <h1>HTML Best Practices</h1>
  <h2>HTML Best Practices</h2>
  <h3>HTML Best Practices</h3>
  <h4>HTML Best Practices</h4>
  <h5>HTML Best Practices</h5>
  <h6>HTML Best Practices</h6>
</hgroup>
```

✅ Doğru:

```html
<h1>HTML Best Practices</h1>
<h2>HTML Best Practices</h2>
<h3>HTML Best Practices</h3>
<h4>HTML Best Practices</h4>
<h5>HTML Best Practices</h5>
<h6>HTML Best Practices</h6>
```

### `address` etiketini yalnızca iletişim bilgileri için kullanın

⛔ Yanlış:

```html
<address>No rights reserved.</address>
```

✅ Doğru:

```html
<address>Contact: <a href="https://twitter.com">Account</a></address>
```

## İçeriği gruplama

### `pre` elemandaki satır başı ile başlamayın

⛔ Yanlış:
  
```html
<pre>
    &lt;!DOCTYPE html&gt;
</pre
```

✅ Doğru:

```html
<pre>&lt;!DOCTYPE html&gt;
</pre>
```

### `blockquote` içinde uygun etiket kullanın

⛔ Yanlış:

```html
<blockquote>For writing maintainable and scalable HTML documents.</blockquote>
```

✅ Doğru:

```html
<blockquote>
  <p>For writing maintainable and scalable HTML documents.</p>
</blockquote>
```

### Satır başına bir liste öğesi yaz

⛔ Yanlış:

```html
<ul>
<li>List item 1</li><li>List item 2</li><li>List item 3</li>
</ul>
```

✅ Doğru:

```html
<ul>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ul>
```

### `ol` etiketi için `type` özelliğini kullanın

⛔ Yanlış:

```html
<ol>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ol>
```

✅ Doğru:

```html
<ol type="1">
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ol>
```

### Diyalog için `dl` kullanmayın

⛔ Yanlış:

```html
<dl>
  <dt>Costello</dt>
  <dd>Look, you gotta first baseman?</dd>
  <dt>Abbott</dt>
  <dd>Certainly.</dd>
  <dt>Costello</dt>
  <dd>Who’s playing first?</dd>
  <dt>Abbott</dt>
  <dd>That’s right.</dd>
  <dt>Costello becomes exasperated.</dd>
  <dt>Costello</dt>
  <dd>When you pay off the first baseman every month, who gets the money?</dd>
  <dt>Abbott</dt>
  <dd>Every dollar of it.</dd>
</dl>
```

✅ Doğru:

```html
<p>Costello: Look, you gotta first baseman?</p>
<p>Abbott: Certainly.</p>
<p>Costello: Who’s playing first?</p>
<p>Abbott: That’s right.</p>
<p>Costello becomes exasperated.</p>
<p>Costello: When you pay off the first baseman every month, who gets the money?</p>
<p>Abbott: Every dollar of it.</p>
```

### `main` etiketini kullanın

⛔ Yanlış:

```html
<div id="main">
  <h1>HTML Best Practices</h1>
  <p>HTML Best Practices is a book about best practices for writing HTML.</p>
</div>
```

✅ Doğru:

```html
<main>
  <h1>HTML Best Practices</h1>
  <p>HTML Best Practices is a book about best practices for writing HTML.</p>
</main>
```

### İndirilebilir kaynağı belirtmek için `download` özelliğini kullanın

⛔ Yanlış:

```html
<a href="https://html.com/">HTML</a>
```

✅ Doğru:

```html
<a href="https://html.com/" download>HTML</a>
```

### `s` , `i` , `b` ve `u` etiketlerinden mümkün olduğunca kaçının

⛔ Yanlış:

```html
<i class="icon-search"></i>
```

✅ Doğru:

```html
<span class="icon-search" aria-hidden="true"></span>
```

### `br` etiketinden sonra satır sonu yapın

⛔ Yanlış:

```html
<p>
  <a href="https://html.com/">HTML</a><br><a href="https://css.com/">CSS</a>
</p>
```

✅ Doğru:

```html
<p>
  <a href="https://html.com/">HTML</a><br>
  <a href="https://css.com/">CSS</a>
</p>
```

### Gerekirse `img` öğesine `alt` özelliği ekleyin

⛔ Yanlış:

```html
<img src="https://html.com/">
```

✅ Doğru:

```html
<img src="https://html.com/" alt="HTML">
```

## Tablo verileri

### Her satıra bir hücre yazın

⛔ Yanlış:

```html
<tr>
  <td>General</td><td>The root Element</td><td>Sections</td>
</tr>
```

✅ Doğru:

```html
<tr>
  <td>General</td>
  <td>The root Element</td>
  <td>Sections</td>
</tr>
```

## Formlar

### `label` etiketini ile form kontrolünü sağlayın

⛔ Yanlış:

```html
<p>Query: <input name="q" type="text"></p>
```

✅ Doğru:

```html
<p><label>Query: <input name="q" type="text"></label></p>
```

### `input` etiketi için uygun `type` özelliğini kullanın

⛔ Yanlış:

```html
<label>Search keyword: <input name="q" type="text"></label>
```

✅ Doğru:

```html
<label>Search keyword: <input name="q" type="search"></label>
```

## Script ekleme

### JavaScript için `type` özelliğini kullanmayın

⛔ Yanlış:

```html
<script type="text/javascript">
  ...
</script>
```

✅ Doğru:

```html
<script>
  ...
</script>
```

### Tutarlı girintiler kullanın

⛔ Yanlış:

```html
<html>
    <head>
        ...
</head>
<body>
    <p>
        <input type="text" name="q" value="HTML">
    </p>
</body>
</html>
```

✅ Doğru:

```html
<html>
  <head>
    ...
  </head>
  <body>
      <p>
        <input type="text" name="q" value="HTML">
      </p>
  </body>
</html>
```

### Harici kaynaklar için protokole bağlı URL kullanmayın

⛔ Yanlış:

```html
<script src="//example.com/js/library.js"></script>
```

✅ Doğru:

```html
<script src="https://example.com/js/library.js"></script>
```