<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Movie Hub</title><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Movie Hub</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Arial,sans-serif}

body{
background:#111;
color:white;
}

header{
background:#e50914;
padding:20px;
text-align:center;
font-size:32px;
font-weight:bold;
}

.search{
width:90%;
max-width:500px;
display:block;
margin:20px auto;
padding:12px;
border:none;
border-radius:25px;
font-size:16px;
}

.movies{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
padding:20px;
}

.movie{
background:#1d1d1d;
border-radius:12px;
overflow:hidden;
transition:.3s;
}

.movie:hover{
transform:scale(1.03);
}

.movie img{
width:100%;
height:350px;
object-fit:cover;
}

.movie-info{
padding:15px;
}

.movie-info h3{
margin-bottom:10px;
}

.rating{
color:gold;
font-weight:bold;
}

footer{
text-align:center;
padding:20px;
background:#1a1a1a;
}
</style>
</head>

<body>

<header>🎬 Movie Hub</header>

<input
type="text"
class="search"
id="search"
placeholder="ابحث عن فيلم..."
>

<div class="movies" id="movies">

<div class="movie">
<img src="https://images.unsplash.com/photo-1489599849927-2ee91cede3ba?w=800">
<div class="movie-info">
<h3>Action Movie</h3>
<p class="rating">⭐ 8.8</p>
</div>
</div>

<div class="movie">
<img src="https://images.unsplash.com/photo-1440404653325-ab127d49abc1?w=800">
<div class="movie-info">
<h3>Adventure Movie</h3>
<p class="rating">⭐ 8.5</p>
</div>
</div>

<div class="movie">
<img src="https://images.unsplash.com/photo-1517604931442-7e0c8ed2963c?w=800">
<div class="movie-info">
<h3>Sci-Fi Movie</h3>
<p class="rating">⭐ 9.1</p>
</div>
</div>

<div class="movie">
<img src="https://images.unsplash.com/photo-1478720568477-152d9b164e26?w=800">
<div class="movie-info">
<h3>Drama Movie</h3>
<p class="rating">⭐ 8.3</p>
</div>
</div>

</div>

<footer>
Movie Hub © 2026
</footer>

<script>
document.getElementById("search").addEventListener("keyup", function(){

let value=this.value.toLowerCase();

document.querySelectorAll(".movie").forEach(movie=>{

movie.style.display=
movie.innerText.toLowerCase().includes(value)
? "block"
: "none";

});

});
</script>

</body>
</html><div class="movie">
<img src="https://upload.wikimedia.org/wikipedia/en/8/8a/Dark_Knight.jpg">
<div class="movie-info">
<h3>The Dark Knight</h3>
<p class="rating">⭐ 9.0</p>
<p>باتمان يواجه الجوكر في واحدة من أشهر أفلام الأبطال الخارقين.</p>
</div>
</div>

<div class="movie">
<img src="https://upload.wikimedia.org/wikipedia/en/7/7f/Inception_ver3.jpg">
<div class="movie-info">
<h3>Inception</h3>
<p class="rating">⭐ 8.8</p>
<p>فيلم خيال علمي عن الأحلام والواقع.</p>
</div>
</div>

<div class="movie">
<img src="https://upload.wikimedia.org/wikipedia/en/b/bc/Interstellar_film_poster.jpg">
<div class="movie-info">
<h3>Interstellar</h3>
<p class="rating">⭐ 8.7</p>
<p>رحلة عبر الفضاء لإنقاذ البشرية.</p>
</div>
</div>
