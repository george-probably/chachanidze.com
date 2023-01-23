---
Title: Page Template
Type: Template
---

<!DOCTYPE html>
<html lang="en">
<head>
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-1BGSZG6MG3"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-1BGSZG6MG3');
</script>
<title>{post-title}{separator}{weblog-title}</title>
<meta charset="utf-8">
<link rel="icon" type="image/x-icon" href="https://raw.githubusercontent.com/george-probably/chachanidze.com/main/Images/favicon.png">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#288cf0">
<meta name="apple-mobile-web-app-status-bar-style" content="#288cf0">
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans');

:root {
    --foreground: #eee;
    --background: #288cf0;
    --link: #eee;
    --unimportant: #ebebeb;
    --articleBG: #1c62a8;
    --articleBorder: #083e73;
}

table th:first-of-type {
    width: 30%;
}
table th:nth-of-type(2) {
    width: 40%;
}
table th:nth-of-type(3) {
    width: 30%;
}


@media (prefers-color-scheme: dark){
    :root {
    --foreground: #eee;
    --background: #083e73;
    --link: #eee;
    --unimportant: #ebebeb;
    --articleBG: #1c62a8;
    --articleBorder: #288cf0;
    }
}

* {
    box-sizing: border-box;
}

body {
    font-family: 'Open Sans', sans-serif;
    font-size: 120%;
    color: var(--foreground);
    background: var(--background);
}

img {
    width: 100%;
    border-radius: 30px;
}

h1, h2, h3, h4, h5, h6 {
    font-family: 'VC Honey Deck', serif;
    margin: 1rem 0;
}

p, li {
    line-height: inherit;
}

nav {
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: var(--articleBG);
    border-radius: 30px;
    border: 5px solid var(--articleBorder);
    font-family: 'VC Honey Deck';
    line-height: 100%;
}

nav li {
    list-style-type: none;
}

nav ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    padding: 0;
    margin: 10px 15px 10px 15px;
    align-content: center;
}

box ul {
    line-height: 150%;
    padding-inline-start: 20px;
}

header, main, footer {
    max-width: 40em;
    margin: 1em auto;
    padding: 0 1em;
}

footer p {
    font-size: 90%;
    text-align: center;
}

a:link { color: var(--link); text-decoration: none; border-bottom: 1px dotted var(--link); }
a:visited { color: var(--link); text-decoration: none; border-bottom: 1px dotted var(--link) }
a:hover { color: var(--link); text-decoration: none; border-bottom: 1px solid var(--link) }
a:active { color: var(--link); text-decoration: none; border-bottom: 1px solid var(--link) }

.post-info, .post-tags {
    font-size: 85%;
    color: var(--unimportant);
    text-align: center;
}

.post-info i:nth-child(2) {
    margin-left: .75em;
}

.tag {
    font-family: 'VC Honey Deck';
    color: var(--foreground) !important;
    padding: 0em .4em;
    border-radius: 25px;
    display: inline-block;
}

.tag:before {
    font-family: "Font Awesome 6 Free";
    font-weight: bold;
    content: '\f02b';
    padding-right: 0.25em;
}
hr {
    border: 0;
    height: 1px;
    background: var(--articleBorder);
    margin: 1em 0;
}

.video-container {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
}

.video-container-square {
    position: relative;
    width: 100%;
    padding-bottom: 100%;
}

.video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 30px;
    
}

.caption {
    font-size: 90%;
    font-style: italic;
    text-align: center;
    margin-top: -18px;
}

article{
    padding: 5px 25px 5px 25px;
    border-radius: 30px;
    background: var(--articleBG);
    border: 5px solid var(--articleBorder);
}

box{
    padding: 0px 25px 0px 25px;
    border-radius: 30px;
    background: var(--articleBG);
    border: 5px solid var(--articleBorder);
    display: block;

}

aside {
    border-radius: 100px;
    background: var(--articleBorder);
    padding: 10px;
}

blockquote {
    background: var(--articleBorder);
    border-radius: 20px;
    padding: inherit;
    font-style: italic;
    margin: 20px 0 20px 0;
}

code {
    background: black;
    color: #00ff00;
}

</style>
</head>

<body>

<header>
	<h1 class="weblog-title"><a style="text-decoration:none; border-bottom:0px" href="{base-path}">{weblog-title}</a></h1>
	{navigation}
</header>
<main>
<hr>
<article>
	{body}
</article>
<hr>
<box>
<h2><i class="fa-solid fa-clock-rotate-left"></i> Recent Posts</h2>
{recent-posts}
</box>
<hr>
</main>
<footer>
<p>Made with <a href="https://weblog.lol">weblog.lol</a>. </br>kindness binds us</p>
</footer>
</body>
</html>