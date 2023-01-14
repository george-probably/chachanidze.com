Title: Page Template
Type: Template
---

<!DOCTYPE html>
<html lang="en">
<head>
<title>{post-title}{separator}{weblog-title}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#288cf0">
<meta name="apple-mobile-web-app-status-bar-style" content="#288cf0">
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');

:root {
    --foreground: #eee;
    --background: #288cf0;
    --link: #eee;
    --unimportant: #ebebeb;
    --articleBG: #68aef4 ;
    --articleBorder: #1c62a8 ;
}

@media (prefers-color-scheme: dark) {
    :root {
    --foreground: #eee;
    --background: #288cf0;
    --link: #eee;
    --unimportant: #ebebeb;
    --articleBG: #1c62a8;
    --articleBorder: #68aef4  ;
    }
}

* {
    box-sizing: border-box;
}

body {
    font-family: 'Lato', sans-serif;
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

a:link { color: var(--link); }
a:visited { color: var(--link); }
a:hover { color: var(--link); }
a:active { color: var(--link); }

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

</style>
</head>

<body>

<header>
	<h1 class="weblog-title"><a style="text-decoration:none" href="{base-path}">{weblog-title}</a></h1>
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
<!-- <hr>
<box>
<h2><i class="fa-solid fa-box-archive"></i> Looking for something older?</h2>
<p><a href="/archive">Take a look in the Archive</a></p>
</box> -->
<hr>
</main>
<footer>
<p>Made with <a href="https://weblog.lol">weblog.lol</a>. </br>kindness binds us</p>
</footer>
</body>
</html>