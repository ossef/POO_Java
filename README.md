<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="generator" content="Asciidoctor 2.0.10">
<meta name="author" content="Stéphane Lopes">
<title>Programmation orientée-objet</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,300italic,400,400italic,600,600italic%7CNoto+Serif:400,400italic,700,700italic%7CDroid+Sans+Mono:400,700">
<style>
/* Asciidoctor default stylesheet | MIT License | https://asciidoctor.org */
/* Uncomment @import statement to use as custom stylesheet */
/*@import "https://fonts.googleapis.com/css?family=Open+Sans:300,300italic,400,400italic,600,600italic%7CNoto+Serif:400,400italic,700,700italic%7CDroid+Sans+Mono:400,700";*/
article,aside,details,figcaption,figure,footer,header,hgroup,main,nav,section{display:block}
audio,video{display:inline-block}
audio:not([controls]){display:none;height:0}
html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}
a{background:none}
a:focus{outline:thin dotted}
a:active,a:hover{outline:0}
h1{font-size:2em;margin:.67em 0}
abbr[title]{border-bottom:1px dotted}
b,strong{font-weight:bold}
dfn{font-style:italic}
hr{-moz-box-sizing:content-box;box-sizing:content-box;height:0}
mark{background:#ff0;color:#000}
code,kbd,pre,samp{font-family:monospace;font-size:1em}
pre{white-space:pre-wrap}
q{quotes:"\201C" "\201D" "\2018" "\2019"}
small{font-size:80%}
sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}
sup{top:-.5em}
sub{bottom:-.25em}
img{border:0}
svg:not(:root){overflow:hidden}
figure{margin:0}
fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}
legend{border:0;padding:0}
button,input,select,textarea{font-family:inherit;font-size:100%;margin:0}
button,input{line-height:normal}
button,select{text-transform:none}
button,html input[type="button"],input[type="reset"],input[type="submit"]{-webkit-appearance:button;cursor:pointer}
button[disabled],html input[disabled]{cursor:default}
input[type="checkbox"],input[type="radio"]{box-sizing:border-box;padding:0}
button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}
textarea{overflow:auto;vertical-align:top}
table{border-collapse:collapse;border-spacing:0}
*,*::before,*::after{-moz-box-sizing:border-box;-webkit-box-sizing:border-box;box-sizing:border-box}
html,body{font-size:100%}
body{background:#fff;color:rgba(0,0,0,.8);padding:0;margin:0;font-family:"Noto Serif","DejaVu Serif",serif;font-weight:400;font-style:normal;line-height:1;position:relative;cursor:auto;tab-size:4;-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased}
a:hover{cursor:pointer}
img,object,embed{max-width:100%;height:auto}
object,embed{height:100%}
img{-ms-interpolation-mode:bicubic}
.left{float:left!important}
.right{float:right!important}
.text-left{text-align:left!important}
.text-right{text-align:right!important}
.text-center{text-align:center!important}
.text-justify{text-align:justify!important}
.hide{display:none}
img,object,svg{display:inline-block;vertical-align:middle}
textarea{height:auto;min-height:50px}
select{width:100%}
.center{margin-left:auto;margin-right:auto}
.stretch{width:100%}
.subheader,.admonitionblock td.content>.title,.audioblock>.title,.exampleblock>.title,.imageblock>.title,.listingblock>.title,.literalblock>.title,.stemblock>.title,.openblock>.title,.paragraph>.title,.quoteblock>.title,table.tableblock>.title,.verseblock>.title,.videoblock>.title,.dlist>.title,.olist>.title,.ulist>.title,.qlist>.title,.hdlist>.title{line-height:1.45;color:#7a2518;font-weight:400;margin-top:0;margin-bottom:.25em}
div,dl,dt,dd,ul,ol,li,h1,h2,h3,#toctitle,.sidebarblock>.content>.title,h4,h5,h6,pre,form,p,blockquote,th,td{margin:0;padding:0;direction:ltr}
a{color:#2156a5;text-decoration:underline;line-height:inherit}
a:hover,a:focus{color:#1d4b8f}
a img{border:0}
p{font-family:inherit;font-weight:400;font-size:1em;line-height:1.6;margin-bottom:1.25em;text-rendering:optimizeLegibility}
p aside{font-size:.875em;line-height:1.35;font-style:italic}
h1,h2,h3,#toctitle,.sidebarblock>.content>.title,h4,h5,h6{font-family:"Open Sans","DejaVu Sans",sans-serif;font-weight:300;font-style:normal;color:#ba3925;text-rendering:optimizeLegibility;margin-top:1em;margin-bottom:.5em;line-height:1.0125em}
h1 small,h2 small,h3 small,#toctitle small,.sidebarblock>.content>.title small,h4 small,h5 small,h6 small{font-size:60%;color:#e99b8f;line-height:0}
h1{font-size:2.125em}
h2{font-size:1.6875em}
h3,#toctitle,.sidebarblock>.content>.title{font-size:1.375em}
h4,h5{font-size:1.125em}
h6{font-size:1em}
hr{border:solid #dddddf;border-width:1px 0 0;clear:both;margin:1.25em 0 1.1875em;height:0}
em,i{font-style:italic;line-height:inherit}
strong,b{font-weight:bold;line-height:inherit}
small{font-size:60%;line-height:inherit}
code{font-family:"Droid Sans Mono","DejaVu Sans Mono",monospace;font-weight:400;color:rgba(0,0,0,.9)}
ul,ol,dl{font-size:1em;line-height:1.6;margin-bottom:1.25em;list-style-position:outside;font-family:inherit}
ul,ol{margin-left:1.5em}
ul li ul,ul li ol{margin-left:1.25em;margin-bottom:0;font-size:1em}
ul.square li ul,ul.circle li ul,ul.disc li ul{list-style:inherit}
ul.square{list-style-type:square}
ul.circle{list-style-type:circle}
ul.disc{list-style-type:disc}
ol li ul,ol li ol{margin-left:1.25em;margin-bottom:0}
dl dt{margin-bottom:.3125em;font-weight:bold}
dl dd{margin-bottom:1.25em}
abbr,acronym{text-transform:uppercase;font-size:90%;color:rgba(0,0,0,.8);border-bottom:1px dotted #ddd;cursor:help}
abbr{text-transform:none}
blockquote{margin:0 0 1.25em;padding:.5625em 1.25em 0 1.1875em;border-left:1px solid #ddd}
blockquote cite{display:block;font-size:.9375em;color:rgba(0,0,0,.6)}
blockquote cite::before{content:"\2014 \0020"}
blockquote cite a,blockquote cite a:visited{color:rgba(0,0,0,.6)}
blockquote,blockquote p{line-height:1.6;color:rgba(0,0,0,.85)}
@media screen and (min-width:768px){h1,h2,h3,#toctitle,.sidebarblock>.content>.title,h4,h5,h6{line-height:1.2}
h1{font-size:2.75em}
h2{font-size:2.3125em}
h3,#toctitle,.sidebarblock>.content>.title{font-size:1.6875em}
h4{font-size:1.4375em}}
table{background:#fff;margin-bottom:1.25em;border:solid 1px #dedede}
table thead,table tfoot{background:#f7f8f7}
table thead tr th,table thead tr td,table tfoot tr th,table tfoot tr td{padding:.5em .625em .625em;font-size:inherit;color:rgba(0,0,0,.8);text-align:left}
table tr th,table tr td{padding:.5625em .625em;font-size:inherit;color:rgba(0,0,0,.8)}
table tr.even,table tr.alt{background:#f8f8f7}
table thead tr th,table tfoot tr th,table tbody tr td,table tr td,table tfoot tr td{display:table-cell;line-height:1.6}
h1,h2,h3,#toctitle,.sidebarblock>.content>.title,h4,h5,h6{line-height:1.2;word-spacing:-.05em}
h1 strong,h2 strong,h3 strong,#toctitle strong,.sidebarblock>.content>.title strong,h4 strong,h5 strong,h6 strong{font-weight:400}
.clearfix::before,.clearfix::after,.float-group::before,.float-group::after{content:" ";display:table}
.clearfix::after,.float-group::after{clear:both}
:not(pre):not([class^=L])>code{font-size:.9375em;font-style:normal!important;letter-spacing:0;padding:.1em .5ex;word-spacing:-.15em;background:#f7f7f8;-webkit-border-radius:4px;border-radius:4px;line-height:1.45;text-rendering:optimizeSpeed;word-wrap:break-word}
:not(pre)>code.nobreak{word-wrap:normal}
:not(pre)>code.nowrap{white-space:nowrap}
pre{color:rgba(0,0,0,.9);font-family:"Droid Sans Mono","DejaVu Sans Mono",monospace;line-height:1.45;text-rendering:optimizeSpeed}
pre code,pre pre{color:inherit;font-size:inherit;line-height:inherit}
pre>code{display:block}
pre.nowrap,pre.nowrap pre{white-space:pre;word-wrap:normal}
em em{font-style:normal}
strong strong{font-weight:400}
.keyseq{color:rgba(51,51,51,.8)}
kbd{font-family:"Droid Sans Mono","DejaVu Sans Mono",monospace;display:inline-block;color:rgba(0,0,0,.8);font-size:.65em;line-height:1.45;background:#f7f7f7;border:1px solid #ccc;-webkit-border-radius:3px;border-radius:3px;-webkit-box-shadow:0 1px 0 rgba(0,0,0,.2),0 0 0 .1em white inset;box-shadow:0 1px 0 rgba(0,0,0,.2),0 0 0 .1em #fff inset;margin:0 .15em;padding:.2em .5em;vertical-align:middle;position:relative;top:-.1em;white-space:nowrap}
.keyseq kbd:first-child{margin-left:0}
.keyseq kbd:last-child{margin-right:0}
.menuseq,.menuref{color:#000}
.menuseq b:not(.caret),.menuref{font-weight:inherit}
.menuseq{word-spacing:-.02em}
.menuseq b.caret{font-size:1.25em;line-height:.8}
.menuseq i.caret{font-weight:bold;text-align:center;width:.45em}
b.button::before,b.button::after{position:relative;top:-1px;font-weight:400}
b.button::before{content:"[";padding:0 3px 0 2px}
b.button::after{content:"]";padding:0 2px 0 3px}
p a>code:hover{color:rgba(0,0,0,.9)}
#header,#content,#footnotes,#footer{width:100%;margin-left:auto;margin-right:auto;margin-top:0;margin-bottom:0;max-width:62.5em;*zoom:1;position:relative;padding-left:.9375em;padding-right:.9375em}
#header::before,#header::after,#content::before,#content::after,#footnotes::before,#footnotes::after,#footer::before,#footer::after{content:" ";display:table}
#header::after,#content::after,#footnotes::after,#footer::after{clear:both}
#content{margin-top:1.25em}
#content::before{content:none}
#header>h1:first-child{color:rgba(0,0,0,.85);margin-top:2.25rem;margin-bottom:0}
#header>h1:first-child+#toc{margin-top:8px;border-top:1px solid #dddddf}
#header>h1:only-child,body.toc2 #header>h1:nth-last-child(2){border-bottom:1px solid #dddddf;padding-bottom:8px}
#header .details{border-bottom:1px solid #dddddf;line-height:1.45;padding-top:.25em;padding-bottom:.25em;padding-left:.25em;color:rgba(0,0,0,.6);display:-ms-flexbox;display:-webkit-flex;display:flex;-ms-flex-flow:row wrap;-webkit-flex-flow:row wrap;flex-flow:row wrap}
#header .details span:first-child{margin-left:-.125em}
#header .details span.email a{color:rgba(0,0,0,.85)}
#header .details br{display:none}
#header .details br+span::before{content:"\00a0\2013\00a0"}
#header .details br+span.author::before{content:"\00a0\22c5\00a0";color:rgba(0,0,0,.85)}
#header .details br+span#revremark::before{content:"\00a0|\00a0"}
#header #revnumber{text-transform:capitalize}
#header #revnumber::after{content:"\00a0"}
#content>h1:first-child:not([class]){color:rgba(0,0,0,.85);border-bottom:1px solid #dddddf;padding-bottom:8px;margin-top:0;padding-top:1rem;margin-bottom:1.25rem}
#toc{border-bottom:1px solid #e7e7e9;padding-bottom:.5em}
#toc>ul{margin-left:.125em}
#toc ul.sectlevel0>li>a{font-style:italic}
#toc ul.sectlevel0 ul.sectlevel1{margin:.5em 0}
#toc ul{font-family:"Open Sans","DejaVu Sans",sans-serif;list-style-type:none}
#toc li{line-height:1.3334;margin-top:.3334em}
#toc a{text-decoration:none}
#toc a:active{text-decoration:underline}
#toctitle{color:#7a2518;font-size:1.2em}
@media screen and (min-width:768px){#toctitle{font-size:1.375em}
body.toc2{padding-left:15em;padding-right:0}
#toc.toc2{margin-top:0!important;background:#f8f8f7;position:fixed;width:15em;left:0;top:0;border-right:1px solid #e7e7e9;border-top-width:0!important;border-bottom-width:0!important;z-index:1000;padding:1.25em 1em;height:100%;overflow:auto}
#toc.toc2 #toctitle{margin-top:0;margin-bottom:.8rem;font-size:1.2em}
#toc.toc2>ul{font-size:.9em;margin-bottom:0}
#toc.toc2 ul ul{margin-left:0;padding-left:1em}
#toc.toc2 ul.sectlevel0 ul.sectlevel1{padding-left:0;margin-top:.5em;margin-bottom:.5em}
body.toc2.toc-right{padding-left:0;padding-right:15em}
body.toc2.toc-right #toc.toc2{border-right-width:0;border-left:1px solid #e7e7e9;left:auto;right:0}}
@media screen and (min-width:1280px){body.toc2{padding-left:20em;padding-right:0}
#toc.toc2{width:20em}
#toc.toc2 #toctitle{font-size:1.375em}
#toc.toc2>ul{font-size:.95em}
#toc.toc2 ul ul{padding-left:1.25em}
body.toc2.toc-right{padding-left:0;padding-right:20em}}
#content #toc{border-style:solid;border-width:1px;border-color:#e0e0dc;margin-bottom:1.25em;padding:1.25em;background:#f8f8f7;-webkit-border-radius:4px;border-radius:4px}
#content #toc>:first-child{margin-top:0}
#content #toc>:last-child{margin-bottom:0}
#footer{max-width:100%;background:rgba(0,0,0,.8);padding:1.25em}
#footer-text{color:rgba(255,255,255,.8);line-height:1.44}
#content{margin-bottom:.625em}
.sect1{padding-bottom:.625em}
@media screen and (min-width:768px){#content{margin-bottom:1.25em}
.sect1{padding-bottom:1.25em}}
.sect1:last-child{padding-bottom:0}
.sect1+.sect1{border-top:1px solid #e7e7e9}
#content h1>a.anchor,h2>a.anchor,h3>a.anchor,#toctitle>a.anchor,.sidebarblock>.content>.title>a.anchor,h4>a.anchor,h5>a.anchor,h6>a.anchor{position:absolute;z-index:1001;width:1.5ex;margin-left:-1.5ex;display:block;text-decoration:none!important;visibility:hidden;text-align:center;font-weight:400}
#content h1>a.anchor::before,h2>a.anchor::before,h3>a.anchor::before,#toctitle>a.anchor::before,.sidebarblock>.content>.title>a.anchor::before,h4>a.anchor::before,h5>a.anchor::before,h6>a.anchor::before{content:"\00A7";font-size:.85em;display:block;padding-top:.1em}
#content h1:hover>a.anchor,#content h1>a.anchor:hover,h2:hover>a.anchor,h2>a.anchor:hover,h3:hover>a.anchor,#toctitle:hover>a.anchor,.sidebarblock>.content>.title:hover>a.anchor,h3>a.anchor:hover,#toctitle>a.anchor:hover,.sidebarblock>.content>.title>a.anchor:hover,h4:hover>a.anchor,h4>a.anchor:hover,h5:hover>a.anchor,h5>a.anchor:hover,h6:hover>a.anchor,h6>a.anchor:hover{visibility:visible}
#content h1>a.link,h2>a.link,h3>a.link,#toctitle>a.link,.sidebarblock>.content>.title>a.link,h4>a.link,h5>a.link,h6>a.link{color:#ba3925;text-decoration:none}
#content h1>a.link:hover,h2>a.link:hover,h3>a.link:hover,#toctitle>a.link:hover,.sidebarblock>.content>.title>a.link:hover,h4>a.link:hover,h5>a.link:hover,h6>a.link:hover{color:#a53221}
details,.audioblock,.imageblock,.literalblock,.listingblock,.stemblock,.videoblock{margin-bottom:1.25em}
details>summary:first-of-type{cursor:pointer;display:list-item;outline:none;margin-bottom:.75em}
.admonitionblock td.content>.title,.audioblock>.title,.exampleblock>.title,.imageblock>.title,.listingblock>.title,.literalblock>.title,.stemblock>.title,.openblock>.title,.paragraph>.title,.quoteblock>.title,table.tableblock>.title,.verseblock>.title,.videoblock>.title,.dlist>.title,.olist>.title,.ulist>.title,.qlist>.title,.hdlist>.title{text-rendering:optimizeLegibility;text-align:left;font-family:"Noto Serif","DejaVu Serif",serif;font-size:1rem;font-style:italic}
table.tableblock.fit-content>caption.title{white-space:nowrap;width:0}
.paragraph.lead>p,#preamble>.sectionbody>[class="paragraph"]:first-of-type p{font-size:1.21875em;line-height:1.6;color:rgba(0,0,0,.85)}
table.tableblock #preamble>.sectionbody>[class="paragraph"]:first-of-type p{font-size:inherit}
.admonitionblock>table{border-collapse:separate;border:0;background:none;width:100%}
.admonitionblock>table td.icon{text-align:center;width:80px}
.admonitionblock>table td.icon img{max-width:none}
.admonitionblock>table td.icon .title{font-weight:bold;font-family:"Open Sans","DejaVu Sans",sans-serif;text-transform:uppercase}
.admonitionblock>table td.content{padding-left:1.125em;padding-right:1.25em;border-left:1px solid #dddddf;color:rgba(0,0,0,.6)}
.admonitionblock>table td.content>:last-child>:last-child{margin-bottom:0}
.exampleblock>.content{border-style:solid;border-width:1px;border-color:#e6e6e6;margin-bottom:1.25em;padding:1.25em;background:#fff;-webkit-border-radius:4px;border-radius:4px}
.exampleblock>.content>:first-child{margin-top:0}
.exampleblock>.content>:last-child{margin-bottom:0}
.sidebarblock{border-style:solid;border-width:1px;border-color:#dbdbd6;margin-bottom:1.25em;padding:1.25em;background:#f3f3f2;-webkit-border-radius:4px;border-radius:4px}
.sidebarblock>:first-child{margin-top:0}
.sidebarblock>:last-child{margin-bottom:0}
.sidebarblock>.content>.title{color:#7a2518;margin-top:0;text-align:center}
.exampleblock>.content>:last-child>:last-child,.exampleblock>.content .olist>ol>li:last-child>:last-child,.exampleblock>.content .ulist>ul>li:last-child>:last-child,.exampleblock>.content .qlist>ol>li:last-child>:last-child,.sidebarblock>.content>:last-child>:last-child,.sidebarblock>.content .olist>ol>li:last-child>:last-child,.sidebarblock>.content .ulist>ul>li:last-child>:last-child,.sidebarblock>.content .qlist>ol>li:last-child>:last-child{margin-bottom:0}
.literalblock pre,.listingblock>.content>pre{-webkit-border-radius:4px;border-radius:4px;word-wrap:break-word;overflow-x:auto;padding:1em;font-size:.8125em}
@media screen and (min-width:768px){.literalblock pre,.listingblock>.content>pre{font-size:.90625em}}
@media screen and (min-width:1280px){.literalblock pre,.listingblock>.content>pre{font-size:1em}}
.literalblock pre,.listingblock>.content>pre:not(.highlight),.listingblock>.content>pre[class="highlight"],.listingblock>.content>pre[class^="highlight "]{background:#f7f7f8}
.literalblock.output pre{color:#f7f7f8;background:rgba(0,0,0,.9)}
.listingblock>.content{position:relative}
.listingblock code[data-lang]::before{display:none;content:attr(data-lang);position:absolute;font-size:.75em;top:.425rem;right:.5rem;line-height:1;text-transform:uppercase;color:inherit;opacity:.5}
.listingblock:hover code[data-lang]::before{display:block}
.listingblock.terminal pre .command::before{content:attr(data-prompt);padding-right:.5em;color:inherit;opacity:.5}
.listingblock.terminal pre .command:not([data-prompt])::before{content:"$"}
.listingblock pre.highlightjs{padding:0}
.listingblock pre.highlightjs>code{padding:1em;-webkit-border-radius:4px;border-radius:4px}
.listingblock pre.prettyprint{border-width:0}
.prettyprint{background:#f7f7f8}
pre.prettyprint .linenums{line-height:1.45;margin-left:2em}
pre.prettyprint li{background:none;list-style-type:inherit;padding-left:0}
pre.prettyprint li code[data-lang]::before{opacity:1}
pre.prettyprint li:not(:first-child) code[data-lang]::before{display:none}
table.linenotable{border-collapse:separate;border:0;margin-bottom:0;background:none}
table.linenotable td[class]{color:inherit;vertical-align:top;padding:0;line-height:inherit;white-space:normal}
table.linenotable td.code{padding-left:.75em}
table.linenotable td.linenos{border-right:1px solid currentColor;opacity:.35;padding-right:.5em}
pre.pygments .lineno{border-right:1px solid currentColor;opacity:.35;display:inline-block;margin-right:.75em}
pre.pygments .lineno::before{content:"";margin-right:-.125em}
.quoteblock{margin:0 1em 1.25em 1.5em;display:table}
.quoteblock:not(.excerpt)>.title{margin-left:-1.5em;margin-bottom:.75em}
.quoteblock blockquote,.quoteblock p{color:rgba(0,0,0,.85);font-size:1.15rem;line-height:1.75;word-spacing:.1em;letter-spacing:0;font-style:italic;text-align:justify}
.quoteblock blockquote{margin:0;padding:0;border:0}
.quoteblock blockquote::before{content:"\201c";float:left;font-size:2.75em;font-weight:bold;line-height:.6em;margin-left:-.6em;color:#7a2518;text-shadow:0 1px 2px rgba(0,0,0,.1)}
.quoteblock blockquote>.paragraph:last-child p{margin-bottom:0}
.quoteblock .attribution{margin-top:.75em;margin-right:.5ex;text-align:right}
.verseblock{margin:0 1em 1.25em}
.verseblock pre{font-family:"Open Sans","DejaVu Sans",sans;font-size:1.15rem;color:rgba(0,0,0,.85);font-weight:300;text-rendering:optimizeLegibility}
.verseblock pre strong{font-weight:400}
.verseblock .attribution{margin-top:1.25rem;margin-left:.5ex}
.quoteblock .attribution,.verseblock .attribution{font-size:.9375em;line-height:1.45;font-style:italic}
.quoteblock .attribution br,.verseblock .attribution br{display:none}
.quoteblock .attribution cite,.verseblock .attribution cite{display:block;letter-spacing:-.025em;color:rgba(0,0,0,.6)}
.quoteblock.abstract blockquote::before,.quoteblock.excerpt blockquote::before,.quoteblock .quoteblock blockquote::before{display:none}
.quoteblock.abstract blockquote,.quoteblock.abstract p,.quoteblock.excerpt blockquote,.quoteblock.excerpt p,.quoteblock .quoteblock blockquote,.quoteblock .quoteblock p{line-height:1.6;word-spacing:0}
.quoteblock.abstract{margin:0 1em 1.25em;display:block}
.quoteblock.abstract>.title{margin:0 0 .375em;font-size:1.15em;text-align:center}
.quoteblock.excerpt>blockquote,.quoteblock .quoteblock{padding:0 0 .25em 1em;border-left:.25em solid #dddddf}
.quoteblock.excerpt,.quoteblock .quoteblock{margin-left:0}
.quoteblock.excerpt blockquote,.quoteblock.excerpt p,.quoteblock .quoteblock blockquote,.quoteblock .quoteblock p{color:inherit;font-size:1.0625rem}
.quoteblock.excerpt .attribution,.quoteblock .quoteblock .attribution{color:inherit;text-align:left;margin-right:0}
table.tableblock{max-width:100%;border-collapse:separate}
p.tableblock:last-child{margin-bottom:0}
td.tableblock>.content>:last-child{margin-bottom:-1.25em}
td.tableblock>.content>:last-child.sidebarblock{margin-bottom:0}
table.tableblock,th.tableblock,td.tableblock{border:0 solid #dedede}
table.grid-all>thead>tr>.tableblock,table.grid-all>tbody>tr>.tableblock{border-width:0 1px 1px 0}
table.grid-all>tfoot>tr>.tableblock{border-width:1px 1px 0 0}
table.grid-cols>*>tr>.tableblock{border-width:0 1px 0 0}
table.grid-rows>thead>tr>.tableblock,table.grid-rows>tbody>tr>.tableblock{border-width:0 0 1px}
table.grid-rows>tfoot>tr>.tableblock{border-width:1px 0 0}
table.grid-all>*>tr>.tableblock:last-child,table.grid-cols>*>tr>.tableblock:last-child{border-right-width:0}
table.grid-all>tbody>tr:last-child>.tableblock,table.grid-all>thead:last-child>tr>.tableblock,table.grid-rows>tbody>tr:last-child>.tableblock,table.grid-rows>thead:last-child>tr>.tableblock{border-bottom-width:0}
table.frame-all{border-width:1px}
table.frame-sides{border-width:0 1px}
table.frame-topbot,table.frame-ends{border-width:1px 0}
table.stripes-all tr,table.stripes-odd tr:nth-of-type(odd),table.stripes-even tr:nth-of-type(even),table.stripes-hover tr:hover{background:#f8f8f7}
th.halign-left,td.halign-left{text-align:left}
th.halign-right,td.halign-right{text-align:right}
th.halign-center,td.halign-center{text-align:center}
th.valign-top,td.valign-top{vertical-align:top}
th.valign-bottom,td.valign-bottom{vertical-align:bottom}
th.valign-middle,td.valign-middle{vertical-align:middle}
table thead th,table tfoot th{font-weight:bold}
tbody tr th{display:table-cell;line-height:1.6;background:#f7f8f7}
tbody tr th,tbody tr th p,tfoot tr th,tfoot tr th p{color:rgba(0,0,0,.8);font-weight:bold}
p.tableblock>code:only-child{background:none;padding:0}
p.tableblock{font-size:1em}
ol{margin-left:1.75em}
ul li ol{margin-left:1.5em}
dl dd{margin-left:1.125em}
dl dd:last-child,dl dd:last-child>:last-child{margin-bottom:0}
ol>li p,ul>li p,ul dd,ol dd,.olist .olist,.ulist .ulist,.ulist .olist,.olist .ulist{margin-bottom:.625em}
ul.checklist,ul.none,ol.none,ul.no-bullet,ol.no-bullet,ol.unnumbered,ul.unstyled,ol.unstyled{list-style-type:none}
ul.no-bullet,ol.no-bullet,ol.unnumbered{margin-left:.625em}
ul.unstyled,ol.unstyled{margin-left:0}
ul.checklist{margin-left:.625em}
ul.checklist li>p:first-child>.fa-square-o:first-child,ul.checklist li>p:first-child>.fa-check-square-o:first-child{width:1.25em;font-size:.8em;position:relative;bottom:.125em}
ul.checklist li>p:first-child>input[type="checkbox"]:first-child{margin-right:.25em}
ul.inline{display:-ms-flexbox;display:-webkit-box;display:flex;-ms-flex-flow:row wrap;-webkit-flex-flow:row wrap;flex-flow:row wrap;list-style:none;margin:0 0 .625em -1.25em}
ul.inline>li{margin-left:1.25em}
.unstyled dl dt{font-weight:400;font-style:normal}
ol.arabic{list-style-type:decimal}
ol.decimal{list-style-type:decimal-leading-zero}
ol.loweralpha{list-style-type:lower-alpha}
ol.upperalpha{list-style-type:upper-alpha}
ol.lowerroman{list-style-type:lower-roman}
ol.upperroman{list-style-type:upper-roman}
ol.lowergreek{list-style-type:lower-greek}
.hdlist>table,.colist>table{border:0;background:none}
.hdlist>table>tbody>tr,.colist>table>tbody>tr{background:none}
td.hdlist1,td.hdlist2{vertical-align:top;padding:0 .625em}
td.hdlist1{font-weight:bold;padding-bottom:1.25em}
.literalblock+.colist,.listingblock+.colist{margin-top:-.5em}
.colist td:not([class]):first-child{padding:.4em .75em 0;line-height:1;vertical-align:top}
.colist td:not([class]):first-child img{max-width:none}
.colist td:not([class]):last-child{padding:.25em 0}
.thumb,.th{line-height:0;display:inline-block;border:solid 4px #fff;-webkit-box-shadow:0 0 0 1px #ddd;box-shadow:0 0 0 1px #ddd}
.imageblock.left{margin:.25em .625em 1.25em 0}
.imageblock.right{margin:.25em 0 1.25em .625em}
.imageblock>.title{margin-bottom:0}
.imageblock.thumb,.imageblock.th{border-width:6px}
.imageblock.thumb>.title,.imageblock.th>.title{padding:0 .125em}
.image.left,.image.right{margin-top:.25em;margin-bottom:.25em;display:inline-block;line-height:0}
.image.left{margin-right:.625em}
.image.right{margin-left:.625em}
a.image{text-decoration:none;display:inline-block}
a.image object{pointer-events:none}
sup.footnote,sup.footnoteref{font-size:.875em;position:static;vertical-align:super}
sup.footnote a,sup.footnoteref a{text-decoration:none}
sup.footnote a:active,sup.footnoteref a:active{text-decoration:underline}
#footnotes{padding-top:.75em;padding-bottom:.75em;margin-bottom:.625em}
#footnotes hr{width:20%;min-width:6.25em;margin:-.25em 0 .75em;border-width:1px 0 0}
#footnotes .footnote{padding:0 .375em 0 .225em;line-height:1.3334;font-size:.875em;margin-left:1.2em;margin-bottom:.2em}
#footnotes .footnote a:first-of-type{font-weight:bold;text-decoration:none;margin-left:-1.05em}
#footnotes .footnote:last-of-type{margin-bottom:0}
#content #footnotes{margin-top:-.625em;margin-bottom:0;padding:.75em 0}
.gist .file-data>table{border:0;background:#fff;width:100%;margin-bottom:0}
.gist .file-data>table td.line-data{width:99%}
div.unbreakable{page-break-inside:avoid}
.big{font-size:larger}
.small{font-size:smaller}
.underline{text-decoration:underline}
.overline{text-decoration:overline}
.line-through{text-decoration:line-through}
.aqua{color:#00bfbf}
.aqua-background{background:#00fafa}
.black{color:#000}
.black-background{background:#000}
.blue{color:#0000bf}
.blue-background{background:#0000fa}
.fuchsia{color:#bf00bf}
.fuchsia-background{background:#fa00fa}
.gray{color:#606060}
.gray-background{background:#7d7d7d}
.green{color:#006000}
.green-background{background:#007d00}
.lime{color:#00bf00}
.lime-background{background:#00fa00}
.maroon{color:#600000}
.maroon-background{background:#7d0000}
.navy{color:#000060}
.navy-background{background:#00007d}
.olive{color:#606000}
.olive-background{background:#7d7d00}
.purple{color:#600060}
.purple-background{background:#7d007d}
.red{color:#bf0000}
.red-background{background:#fa0000}
.silver{color:#909090}
.silver-background{background:#bcbcbc}
.teal{color:#006060}
.teal-background{background:#007d7d}
.white{color:#bfbfbf}
.white-background{background:#fafafa}
.yellow{color:#bfbf00}
.yellow-background{background:#fafa00}
span.icon>.fa{cursor:default}
a span.icon>.fa{cursor:inherit}
.admonitionblock td.icon [class^="fa icon-"]{font-size:2.5em;text-shadow:1px 1px 2px rgba(0,0,0,.5);cursor:default}
.admonitionblock td.icon .icon-note::before{content:"\f05a";color:#19407c}
.admonitionblock td.icon .icon-tip::before{content:"\f0eb";text-shadow:1px 1px 2px rgba(155,155,0,.8);color:#111}
.admonitionblock td.icon .icon-warning::before{content:"\f071";color:#bf6900}
.admonitionblock td.icon .icon-caution::before{content:"\f06d";color:#bf3400}
.admonitionblock td.icon .icon-important::before{content:"\f06a";color:#bf0000}
.conum[data-value]{display:inline-block;color:#fff!important;background:rgba(0,0,0,.8);-webkit-border-radius:100px;border-radius:100px;text-align:center;font-size:.75em;width:1.67em;height:1.67em;line-height:1.67em;font-family:"Open Sans","DejaVu Sans",sans-serif;font-style:normal;font-weight:bold}
.conum[data-value] *{color:#fff!important}
.conum[data-value]+b{display:none}
.conum[data-value]::after{content:attr(data-value)}
pre .conum[data-value]{position:relative;top:-.125em}
b.conum *{color:inherit!important}
.conum:not([data-value]):empty{display:none}
dt,th.tableblock,td.content,div.footnote{text-rendering:optimizeLegibility}
h1,h2,p,td.content,span.alt{letter-spacing:-.01em}
p strong,td.content strong,div.footnote strong{letter-spacing:-.005em}
p,blockquote,dt,td.content,span.alt{font-size:1.0625rem}
p{margin-bottom:1.25rem}
.sidebarblock p,.sidebarblock dt,.sidebarblock td.content,p.tableblock{font-size:1em}
.exampleblock>.content{background:#fffef7;border-color:#e0e0dc;-webkit-box-shadow:0 1px 4px #e0e0dc;box-shadow:0 1px 4px #e0e0dc}
.print-only{display:none!important}
@page{margin:1.25cm .75cm}
@media print{*{-webkit-box-shadow:none!important;box-shadow:none!important;text-shadow:none!important}
html{font-size:80%}
a{color:inherit!important;text-decoration:underline!important}
a.bare,a[href^="#"],a[href^="mailto:"]{text-decoration:none!important}
a[href^="http:"]:not(.bare)::after,a[href^="https:"]:not(.bare)::after{content:"(" attr(href) ")";display:inline-block;font-size:.875em;padding-left:.25em}
abbr[title]::after{content:" (" attr(title) ")"}
pre,blockquote,tr,img,object,svg{page-break-inside:avoid}
thead{display:table-header-group}
svg{max-width:100%}
p,blockquote,dt,td.content{font-size:1em;orphans:3;widows:3}
h2,h3,#toctitle,.sidebarblock>.content>.title{page-break-after:avoid}
#toc,.sidebarblock,.exampleblock>.content{background:none!important}
#toc{border-bottom:1px solid #dddddf!important;padding-bottom:0!important}
body.book #header{text-align:center}
body.book #header>h1:first-child{border:0!important;margin:2.5em 0 1em}
body.book #header .details{border:0!important;display:block;padding:0!important}
body.book #header .details span:first-child{margin-left:0!important}
body.book #header .details br{display:block}
body.book #header .details br+span::before{content:none!important}
body.book #toc{border:0!important;text-align:left!important;padding:0!important;margin:0!important}
body.book #toc,body.book #preamble,body.book h1.sect0,body.book .sect1>h2{page-break-before:always}
.listingblock code[data-lang]::before{display:block}
#footer{padding:0 .9375em}
.hide-on-print{display:none!important}
.print-only{display:block!important}
.hide-for-print{display:none!important}
.show-for-print{display:inherit!important}}
@media print,amzn-kf8{#header>h1:first-child{margin-top:1.25rem}
.sect1{padding:0!important}
.sect1+.sect1{border:0}
#footer{background:none}
#footer-text{color:rgba(0,0,0,.6);font-size:.9em}}
@media amzn-kf8{#header,#content,#footnotes,#footer{padding:0}}
</style>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body class="book toc2 toc-left">
<div id="header">
<h1>Programmation orientée-objet</h1>
<div class="details">
<span id="author" class="author">Stéphane Lopes - UVSQ</span><br>
</div>
<div class="details">
<span id="author" class="author">Youssef Ait El Mahjoub</span><br>
<span id="email" class="email"><a href="mailto:youssef.ait-el-mahjoub@efrei.fr">youssef.ait-el-mahjoub@efrei.fr</a></span><br>
<span id="revnumber">version 2022-2023</span>
</div>
<div id="toc" class="toc2">
<div id="toctitle">Sommaire</div>
<ul class="sectlevel1">
<li><a href="#_introduction">1. Introduction</a>
<ul class="sectlevel2">
<li><a href="#_caractéristiques_des_langages_de_programmation">1.1. Caractéristiques des langages de programmation</a></li>
<li><a href="#_quelques_langages_de_programmation">1.2. Quelques langages de programmation</a></li>
<li><a href="#_évolution_des_langages_de_programmation_impératifs">1.3. Évolution des langages de programmation impératifs</a></li>
<li><a href="#_le_langage_java">1.4. Le langage Java</a></li>
<li><a href="#_python_refcard">1.5. Python RefCard</a></li>
<li><a href="#_références_poojava">Références (POO/Java)</a></li>
<li><a href="#_exercices_python">1.6. Exercices (Python)</a></li>
</ul>
</li>
<li><a href="#_vue_densemble_des_concepts_objet">2. Vue d&#8217;ensemble des concepts objet</a>
<ul class="sectlevel2">
<li><a href="#_objet_et_message">2.1. Objet et message</a></li>
<li><a href="#_type_et_classe">2.2. Type et classe</a></li>
<li><a href="#_héritage">2.3. Héritage</a></li>
<li><a href="#_relations_entre_classes">2.4. Relations entre classes</a></li>
<li><a href="#_module">2.5. Module</a></li>
<li><a href="#_exercices_python_2">2.6. Exercices (Python)</a></li>
<li><a href="#_exercices_java">2.7. Exercices (Java)</a></li>
</ul>
</li>
<li><a href="#_objets_et_classes">3. Objets et classes</a>
<ul class="sectlevel2">
<li><a href="#_caractéristiques_dun_objet">3.1. Caractéristiques d&#8217;un objet</a></li>
<li><a href="#_les_objets_en_java">3.2. Les objets en Java</a></li>
<li><a href="#_les_chaînes_de_caractères_en_java">3.3. Les chaînes de caractères en Java</a></li>
<li><a href="#_caractéristiques_dune_classe">3.4. Caractéristiques d&#8217;une classe</a></li>
<li><a href="#_les_classes_en_java">3.5. Les classes en Java</a></li>
<li><a href="#_métaclasse_et_membres_de_classe">3.6. Métaclasse et membres de classe</a></li>
<li><a href="#_membres_de_classe_en_java">3.7. Membres de classe en Java</a></li>
<li><a href="#_le_programme_principal_en_java">3.8. Le programme principal en Java</a></li>
<li><a href="#_énumération_en_java">3.9. Énumération en Java</a></li>
<li><a href="#_généricité">3.10. Généricité</a></li>
<li><a href="#_généricité_en_java">3.11. Généricité en Java</a></li>
<li><a href="#_exercices_java_2">3.12. Exercices (Java)</a></li>
</ul>
</li>
<li><a href="#_héritage_3">4. Héritage</a>
<ul class="sectlevel2">
<li><a href="#_héritage_en_java">4.1. Héritage en Java</a></li>
<li><a href="#_polymorphisme_en_java">4.2. Polymorphisme en Java</a></li>
<li><a href="#_la_classe_object">4.3. La classe <code>Object</code></a></li>
<li><a href="#_classe_abstraite_en_java">4.4. Classe abstraite en Java</a></li>
<li><a href="#_la_classe_number">4.5. La classe <code>Number</code></a></li>
<li><a href="#_interface">4.6. Interface</a></li>
<li><a href="#_exercices_java_3">4.7. Exercices (Java)</a></li>
</ul>
</li>
<li><a href="#_module_et_bibliothèques">5. Module et bibliothèques</a>
<ul class="sectlevel2">
<li><a href="#_module_en_java">5.1. Module en Java</a></li>
<li><a href="#_bibliothèques_en_java">5.2. Bibliothèques en Java</a></li>
<li><a href="#_exercices_java_4">5.3. Exercices (Java)</a></li>
</ul>
</li>
<li><a href="#_gestion_derreurs_et_exceptions">6. Gestion d&#8217;erreurs et exceptions</a>
<ul class="sectlevel2">
<li><a href="#_les_erreurs_en_programmation">6.1. Les erreurs en programmation</a></li>
<li><a href="#_gestion_derreurs">6.2. Gestion d&#8217;erreurs</a></li>
<li><a href="#_exceptions">6.3. Exceptions</a></li>
<li><a href="#_exceptions_en_java">6.4. Exceptions en Java</a></li>
<li><a href="#_exercices">6.5. Exercices</a></li>
</ul>
</li>
<li><a href="#_entréessorties_et_persistance">7. Entrées/sorties et persistance</a>
<ul class="sectlevel2">
<li><a href="#_entréessorties_flux_et_persistance">7.1. Entrées/sorties, flux et persistance</a></li>
<li><a href="#_io_en_java">7.2. I/O en Java</a></li>
<li><a href="#_utilisation_des_flux">7.3. Utilisation des flux</a></li>
<li><a href="#_sérialisation_en_java">7.4. Sérialisation en Java</a></li>
<li><a href="#_exercices_2">7.5. Exercices</a></li>
</ul>
</li>
<li><a href="#_gestion_des_collections">8. Gestion des collections</a>
<ul class="sectlevel2">
<li><a href="#_introduction_2">8.1. Introduction</a></li>
<li><a href="#_interfaces">8.2. Interfaces</a></li>
<li><a href="#_implémentations_2">8.3. Implémentations</a></li>
<li><a href="#_algorithmes">8.4. Algorithmes</a></li>
<li><a href="#_mise_en_uvre">8.5. Mise en &oelig;uvre</a></li>
<li><a href="#_exercices_3">8.6. Exercices</a></li>
</ul>
</li>
<li><a href="#_la_bibliothèques_streams_et_la_programmation_fonctionnelle_en_java">9. La bibliothèques <em>streams</em> et la programmation fonctionnelle en Java</a>
<ul class="sectlevel2">
<li><a href="#_introduction_3">9.1. Introduction</a></li>
<li><a href="#_programmation_fonctionnelle_en_java">9.2. Programmation fonctionnelle en Java</a></li>
<li><a href="#_la_bibliothèque_streams">9.3. La bibliothèque streams</a></li>
<li><a href="#_exercices_4">9.4. Exercices</a></li>
</ul>
</li>
<li><a href="#_conclusion">10. Conclusion</a>
<ul class="sectlevel2">
<li><a href="#_bilan">10.1. Bilan</a></li>
<li><a href="#_conception_orientée_objet">10.2. Conception orientée-objet</a></li>
<li><a href="#_pour_aller_plus_loin">10.3. Pour aller plus loin&#8230;&#8203;</a></li>
</ul>
</li>
</ul>
</div>
</div>
<div id="content">
<div class="sect1">
<h2 id="_introduction"><a class="anchor" href="#_introduction"></a><a class="link" href="#_introduction">1. Introduction</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_caractéristiques_des_langages_de_programmation"><a class="anchor" href="#_caractéristiques_des_langages_de_programmation"></a><a class="link" href="#_caractéristiques_des_langages_de_programmation">1.1. Caractéristiques des langages de programmation</a></h3>
<div class="sect3">
<h4 id="_implémentation_des_langages"><a class="anchor" href="#_implémentation_des_langages"></a><a class="link" href="#_implémentation_des_langages">1.1.1. Implémentation des langages</a></h4>
<div class="ulist">
<ul>
<li>
<p>Avec un <a href="https://en.wikipedia.org/wiki/Compiled_language"><em>langage compilé</em></a>, le code source du programme est transformé en <em>code machine</em> par le <em>compilateur</em></p>
</li>
<li>
<p>Dans un <a href="https://en.wikipedia.org/wiki/Interpreted_language"><em>langage interprété</em></a>, le code source du programme est exécuté "à la volée" par l'<em>interpréteur</em></p>
</li>
<li>
<p>Certains langages sont à la fois compilés et interprétés</p>
</li>
<li>
<p>Il existe des approches intermédiaires (compilation <em>Just In Time</em> (JIT))</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_c_est_compilé"><a class="anchor" href="#_c_est_compilé"></a><a class="link" href="#_c_est_compilé">1.1.2. C est compilé</a></h4>
<div class="listingblock">
<div class="title">Compilation séparée (produit <code>util.o</code> et <code>main.o</code>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ gcc -c util.c
$ gcc -c main.c</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Édition de liens (produit <code>monprog</code>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ gcc -o monprog main.o util.o</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title"><code>monprog</code> est exécutable</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ ./monprog</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_php_est_interprété"><a class="anchor" href="#_php_est_interprété"></a><a class="link" href="#_php_est_interprété">1.1.3. PHP est interprété</a></h4>
<div class="listingblock">
<div class="title">Exécution d&#8217;un programme PHP</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ php monprog.php</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_java_est_compilé_puis_interprété_jit"><a class="anchor" href="#_java_est_compilé_puis_interprété_jit"></a><a class="link" href="#_java_est_compilé_puis_interprété_jit">1.1.4. Java est compilé puis interprété (JIT)</a></h4>
<div class="listingblock">
<div class="title">Compilation en <em>bytecode</em> (produit Main.class)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ javac Main.java</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Exécution avec la JVM (<em>Java Virtual Machine</em>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ java Main</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_langage_de_scripts"><a class="anchor" href="#_langage_de_scripts"></a><a class="link" href="#_langage_de_scripts">1.1.5. Langage de scripts</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>script</em> est un programme destiné à automatiser l&#8217;enchaînement de tâches dans un environnement particulier</p>
</li>
<li>
<p>Un <em>langage de scripts</em> est un langage de programmation permettant de développer des scripts</p>
</li>
<li>
<p>Il permet d&#8217;invoquer les primitives du système sous-jacent</p>
</li>
<li>
<p>Il dispose en général d&#8217;un <em>REPL</em> (<em>Read-Eval-Print Loop</em>)</p>
</li>
<li>
<p>Quelques exemples</p>
<div class="ulist">
<ul>
<li>
<p>shells pour les OS : Bash, Zsh, tcsh</p>
</li>
<li>
<p>ECMAScript (Javascript) pour les navigateurs web</p>
</li>
<li>
<p>Lua embarqué dans une application (<em>VLC Media Player</em>, jeu <em>Battle for Wesnoth</em>)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_système_de_typage"><a class="anchor" href="#_système_de_typage"></a><a class="link" href="#_système_de_typage">1.1.6. Système de typage</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>système de typage</em> attribue des types aux éléments du langage</p>
</li>
<li>
<p>Attribuer un type à une expression permet de limiter les erreurs de programmation</p>
<div class="ulist">
<ul>
<li>
<p>en définissant ce qu&#8217;il est possible de faire avec une expression</p>
</li>
<li>
<p>en définissant les règles de compatibilité entre expressions</p>
</li>
<li>
<p>en vérifiant ces contraintes</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_typage_explicite_vs_implicite"><a class="anchor" href="#_typage_explicite_vs_implicite"></a><a class="link" href="#_typage_explicite_vs_implicite">1.1.7. Typage explicite vs. implicite</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le typage est <em>explicite</em> si les annotations de type sont visibles dans le code source</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En C, chaque déclaration de variable précise son type</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="C" class="language-C hljs">int nombre = 1;
double pi = 3.141592;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le typage est <em>implicite</em> si les types ne sont pas précisés dans le code source</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En PHP, la première affectation crée la variable</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="php" class="language-php hljs">$nombre = 1;
$pi = 3.141592;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Des langages à typage explicite peuvent faire appel à l'<em>inférence de types</em> dans certaines situations</p>
<div class="ulist">
<ul>
<li>
<p>permet la déduction automatique des types</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_typage_statique_vs_dynamique"><a class="anchor" href="#_typage_statique_vs_dynamique"></a><a class="link" href="#_typage_statique_vs_dynamique">1.1.8. Typage statique vs. dynamique</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le typage est <em>statique</em> si l&#8217;information de type est associée à l&#8217;identificateur</p>
<div class="ulist">
<ul>
<li>
<p>&#8658; la vérification des types peut être réalisée lors de la compilation</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le typage est <em>dynamique</em> si l&#8217;information de type est portée par l&#8217;objet lui-même</p>
<div class="ulist">
<ul>
<li>
<p>&#8658; la vérification se fait durant l&#8217;exécution</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_typage_statique"><a class="anchor" href="#_typage_statique"></a><a class="link" href="#_typage_statique">1.1.9. Typage statique</a></h4>
<div class="ulist">
<ul>
<li>
<p>Améliore la fiabilité du programme (plus de vérifications plus précoces)</p>
</li>
<li>
<p>Meilleur support des outils (IDE)</p>
</li>
<li>
<p>Meilleures performances</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En C, les erreurs de type sont identifiées par le compilateur</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="C" class="language-C hljs">double a = "une chaine";
// error: incompatible types when initializing type ‘double’ using type ‘char *’</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_typage_dynamique"><a class="anchor" href="#_typage_dynamique"></a><a class="link" href="#_typage_dynamique">1.1.10. Typage dynamique</a></h4>
<div class="ulist">
<ul>
<li>
<p>Offre plus de souplesse dans l&#8217;écriture du code source</p>
<div class="ulist">
<ul>
<li>
<p><em>duck typing</em>, <em>data as code</em>, métaprogrammation</p>
</li>
</ul>
</div>
</li>
<li>
<p>Permet le prototypage rapide</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En PHP, les erreurs de type peuvent passer inaperçues</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="php" class="language-php hljs">$a = 1;
$a = "une chaine";
echo $a + 2; // affiche 2</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_typage_fort_vs_faible"><a class="anchor" href="#_typage_fort_vs_faible"></a><a class="link" href="#_typage_fort_vs_faible">1.1.11. Typage fort vs. faible</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le typage est <em>fort</em> si les manipulations entre données de types différents sont limitées et contrôlées</p>
</li>
<li>
<p>Le typage est <em>faible</em> si les possibilités de transtypage sont nombreuses et implicites</p>
</li>
<li>
<p>Ces notions sont relativement floues</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">Le C est à typage fort mais&#8230;&#8203;</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="C" class="language-C hljs">int a = "une chaine";
printf("%d\n", a); // 443215...</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_support_des_paradigmes_de_programmation"><a class="anchor" href="#_support_des_paradigmes_de_programmation"></a><a class="link" href="#_support_des_paradigmes_de_programmation">1.1.12. Support des paradigmes de programmation</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <strong>paradigme de programmation</strong> représente la façon d&#8217;aborder un problème et d&#8217;en concevoir la solution.</p>
</li>
<li>
<p>Quelques paradigmes</p>
<div class="ulist">
<ul>
<li>
<p>Programmation impérative</p>
<div class="ulist">
<ul>
<li>
<p>Programmation structurée</p>
</li>
<li>
<p>Programmation modulaire</p>
</li>
<li>
<p>Programmation par abstraction de données</p>
</li>
<li>
<p>Programmation objet</p>
</li>
</ul>
</div>
</li>
<li>
<p>Programmation fonctionnelle</p>
</li>
<li>
<p>Programmation logique</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un langage <strong>supporte un paradigme</strong> quand il fournit les fonctionnalités pour utiliser ce style (de façon simple, sécurisée et efficace)</p>
</li>
</ul>
</div>
</div>



<div class="sect3">
<h4 id="_langage_impératif"><a class="anchor" href="#_langage_impératif"></a><a class="link" href="#_langage_impératif">1.1.20. Langage impératif</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>langage impératif</em> représente un programme comme une séquence d&#8217;instructions qui modifient son état au cours de son exécution</p>
</li>
<li>
<p>Un programme décrit <strong>comment</strong> aboutir à la solution du problème</p>
</li>
<li>
<p>Proche de l&#8217;architecture matérielle des ordinateurs (<em>architecture de von Neumann</em>)</p>
</li>
<li>
<p>De nombreux langages populaires sont de ce type (C, Java, Python)</p>
</li>
</ul>
</div>
</div>

<div class="sect3">
<h4 id="_langage_fonctionnel"><a class="anchor" href="#_langage_fonctionnel"></a><a class="link" href="#_langage_fonctionnel">1.1.21. Langage fonctionnel</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>langage fonctionnel</em> repose sur le postulat que "tout est fonction".</p>
</li>
<li>
<p>Un programme consiste en  <strong>des appels successifs de fonctions</strong> pour aboutir à la solution du problème</p>
</li>
<li>
<p> Une fonction peut être vue comme une boite noire : on connait les paramètres et le type de retour</p>
</li>
<li>
<p>A la base, trés utilisé dans les domaines de Mathématiques, Analyse de donnée ...</p>
</li>
<li>
<p>Exemple de langages : Js, Python </p>
</li>
</ul>
</div>
</div>

<div class="sect3">
<h4 id="_langage_déclaratif"><a class="anchor" href="#_langage_déclaratif"></a><a class="link" href="#_langage_déclaratif">1.1.22. Langage déclaratif</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>langage déclaratif</em> permet de décrire ce que le programme doit faire (le <strong>quoi</strong>) et non pas comment il doit le faire (le <strong>comment</strong>)</p>
</li>
<li>
<p>Un programme respectant ce style décrit le problème à traiter</p>
</li>
<li>
<p>Quelques exemples : Prolog, SQL</p>
</li>
<li>
<p>Certains langages impératifs embarquent des constructions déclaratives</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_gestion_de_la_mémoire"><a class="anchor" href="#_gestion_de_la_mémoire"></a><a class="link" href="#_gestion_de_la_mémoire">1.1.23. Gestion de la mémoire</a></h4>
<div class="ulist">
<ul>
<li>
<p>La gestion de la mémoire dans un langage de programmation décrit comment les objets inutilisés sont identifiés et désalloués</p>
<div class="ulist">
<ul>
<li>
<p>nécessaire pour éviter les <em>fuites de mémoire</em> (<em>memory leaks</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>La plupart des langages ont une gestion automatique de la mémoire et s&#8217;appuient sur un <em>ramasse-miettes</em> (<em>garbage collector</em>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En Java, le ramasse-miettes est chargé de libérer la mémoire allouée dynamiquement</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] tableau = new int[10]; // allocation d'un tableau de 10 cases
// la désallocation est automatique</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Les langages C et C++ ont une gestion manuelle de la mémoire</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="C" class="language-C hljs">int[] tableau = malloc(10 * sizeof(int)); // allocation d'un tableau de 10 cases
// ...
free(tableau); // libération de la mémoire</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_caractéristiques_de_quelques_langages"><a class="anchor" href="#_caractéristiques_de_quelques_langages"></a><a class="link" href="#_caractéristiques_de_quelques_langages">1.1.24. Caractéristiques de quelques langages</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.667%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Langage</th>
<th class="tableblock halign-left valign-top">Implémentation</th>
<th class="tableblock halign-left valign-top">Scripts</th>
<th class="tableblock halign-left valign-top">Typage</th>
<th class="tableblock halign-left valign-top">Paradigme</th>
<th class="tableblock halign-left valign-top">Mémoire</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">C</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Compilé</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Non</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">explicite, statique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">procédural</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">manuelle</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Java</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Compilé, interprété</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Non</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">explicite, statique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">OO, fonc., générique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">auto</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">PHP</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Interprété</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Oui</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">implicite, dynamique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">proc., OO</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">auto</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Python</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Compilé, Interprété</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Oui</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">implicite, dynamique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">proc., OO, fonc.</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">auto</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Scala</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Compilé, interprété</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Oui</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">implicite, statique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">OO, fonc., générique</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">auto</p></td>
</tr>
</tbody>
</table>
</div>
</div>
<div class="sect2">
<h3 id="_quelques_langages_de_programmation"><a class="anchor" href="#_quelques_langages_de_programmation"></a><a class="link" href="#_quelques_langages_de_programmation">1.2. Quelques langages de programmation</a></h3>
<div class="sect3">
<h4 id="_les_langages_historiques"><a class="anchor" href="#_les_langages_historiques"></a><a class="link" href="#_les_langages_historiques">1.2.1. Les langages "historiques"</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://fr.wikipedia.org/wiki/Fortran">Fortran</a>, <a href="https://fr.wikipedia.org/wiki/John_Backus">John Backus</a> (1954)</p>
</li>
<li>
<p><a href="https://fr.wikipedia.org/wiki/Lisp">Lisp</a>, <a href="https://fr.wikipedia.org/wiki/John_McCarthy">John McCarthy</a> (1958)</p>
</li>
<li>
<p><a href="https://fr.wikipedia.org/wiki/COBOL">COBOL</a>, <em>Short Range Committee</em> (1959)</p>
</li>
<li>
<p><a href="http://en.wikipedia.org/wiki/Simula">Simula</a>, <a href="http://heim.ifi.uio.no/~olejohan/">Ole-Johan Dahl</a> et <a href="http://heim.ifi.uio.no/~kristen/">Kristen Nygaard</a> (années 1960)</p>
</li>
<li>
<p><a href="http://www.smalltalk.org/">SmallTalk</a>, <a href="http://en.wikipedia.org/wiki/Alan_Kay">Alan Kay</a> et <a href="http://en.wikipedia.org/wiki/Dan_Ingalls">Dan Ingalls</a> (début des années 1970)</p>
</li>
<li>
<p><a href="https://fr.wikipedia.org/wiki/C_(langage)">C</a>, <a href="https://fr.wikipedia.org/wiki/Dennis_Ritchie">Denis Ritchie</a> (1972)</p>
</li>
<li>
<p><a href="http://en.wikipedia.org/wiki/Eiffel_(programming_language)">Eiffel</a>, <a href="http://se.ethz.ch/~meyer/">Bertrand Meyer</a> (1985)</p>
</li>
<li>
<p><a href="http://en.wikipedia.org/wiki/C\%2B\%2B">C++</a>, <a href="http://www.research.att.com/~bs/homepage.html">Bjarne Stroustrup</a> (années 1980, Standard ISO en 1998)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_principaux_langages_actuels_i"><a class="anchor" href="#_les_principaux_langages_actuels_i"></a><a class="link" href="#_les_principaux_langages_actuels_i">1.2.2. Les principaux langages actuels I</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/tiobe2022_prog_comm_index.png" alt="tiobe prog comm index">
</div>
<div class="title">Figure 1. <a href="http://www.tiobe.com/tiobe-index/">TIOBE Index</a> (jan. 2023)</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_principaux_langages_actuels_ii"><a class="anchor" href="#_les_principaux_langages_actuels_ii"></a><a class="link" href="#_les_principaux_langages_actuels_ii">1.2.3. Les principaux langages actuels II</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/pypl2022_index.png" alt="pypl index">
</div>
<div class="title">Figure 2. <a href="http://pypl.github.io/PYPL.html">The PYPL PopularitY of Programming Language Index</a> (jan. 2023)</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_principaux_langages_actuels_iii"><a class="anchor" href="#_les_principaux_langages_actuels_iii"></a><a class="link" href="#_les_principaux_langages_actuels_iii">1.2.4. Les principaux langages actuels III</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/ieee2022_spectrum_index.png" alt="ieee spectrum index">
</div>
<div class="title">Figure 3. <a href="http://spectrum.ieee.org/computing/software/the-2016-top-programming-languages">IEEE Spectrum’s ranking</a> (2023)</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_principaux_langages_actuels_iv"><a class="anchor" href="#_les_principaux_langages_actuels_iv"></a><a class="link" href="#_les_principaux_langages_actuels_iv">1.2.5. Les principaux langages actuels IV</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://www.python.org/">Python</a>, <a href="https://gvanrossum.github.io/">Guido van Rossum</a> (1990)</p>
</li>
<li>
<p><a href="https://php.net/">PHP</a>, <a href="https://toys.lerdorf.com/">Rasmus Lerdorf</a> (1994)</p>
</li>
<li>
<p><a href="http://java.sun.com/">Java</a>, <a href="http://blogs.sun.com/jag/">James Gosling</a> (1995)</p>
</li>
<li>
<p><a href="https://fr.wikipedia.org/wiki/JavaScript">Javascript</a>, <a href="https://fr.wikipedia.org/wiki/Brendan_Eich">Brendan Eich</a> (1995)</p>
</li>
<li>
<p><a href="http://msdn.microsoft.com/fr-fr/vcsharp/default.aspx">C#</a>, <a href="http://en.wikipedia.org/wiki/Anders_Hejlsberg">Anders Hejlsberg</a> (2001)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_langages_tendances"><a class="anchor" href="#_les_langages_tendances"></a><a class="link" href="#_les_langages_tendances">1.2.6. Autres langages</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://golang.org/">Go</a>, Robert Griesemer, Rob Pike, Ken Thompson (2009)</p>
</li>
<li>
<p><a href="http://www.groovy-lang.org/">Groovy</a>, Java Community Process (2003)</p>
</li>
<li>
<p><a href="http://julialang.org/">Julia</a>, Jeff Bezanson, Stefan Karpinski, Viral B. Shah, Alan Edelman (2012)</p>
</li>
<li>
<p><a href="http://kotlinlang.org/">Kotlin</a>, JetBrains (2011)</p>
</li>
<li>
<p><a href="https://www.r-project.org/">R</a>, Ross Ihaka, Robert Gentleman (1993)</p>
</li>
<li>
<p><a href="https://www.rust-lang.org/fr/">Rust</a>, Graydon Hoare (2010)</p>
</li>
<li>
<p><a href="https://www.scala-lang.org/">Scala</a>, <a href="http://lampwww.epfl.ch/~odersky/">Martin Odersky</a> (2003)</p>
</li>
<li>
<p><a href="https://fr.wikipedia.org/wiki/Swift_(langage_d&#8217;Apple)">Swift</a>, Apple (2014)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_critères_de_choix_dun_langage"><a class="anchor" href="#_critères_de_choix_dun_langage"></a><a class="link" href="#_critères_de_choix_dun_langage">1.2.7. Critères de choix d&#8217;un langage</a></h4>
<div class="ulist">
<ul>
<li>
<p>Adéquation aux besoins</p>
<div class="ulist">
<ul>
<li>
<p>domaine d&#8217;application, plateforme cible</p>
</li>
</ul>
</div>
</li>
<li>
<p>Simplicité d&#8217;apprentissage/lisibilité du code source</p>
<div class="ulist">
<ul>
<li>
<p>"<em>Programs must be written for people to read, and only incidentally for machines to execute</em>", Harold Abelson</p>
</li>
<li>
<p>"<em>Any fool can write code that a computer can understand. Good programmers write code that humans can understand.</em>", Martin Fowler</p>
</li>
<li>
<p>"<em>Perl – The only language that looks the same before and after RSA encryption</em>", Keith Bostic</p>
</li>
</ul>
</div>
</li>
<li>
<p>Richesse de la bibliothèque standard</p>
</li>
<li>
<p>Écosystème (bibliothèques tierces, outils)</p>
</li>
<li>
<p>Popularité (support)</p>
</li>
<li>
<p>Employabilité</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_évolution_des_langages_de_programmation_impératifs"><a class="anchor" href="#_évolution_des_langages_de_programmation_impératifs"></a><a class="link" href="#_évolution_des_langages_de_programmation_impératifs">1.3. Évolution des langages de programmation impératifs</a></h3>
<div class="sect3">
<h4 id="_programmation_structurée"><a class="anchor" href="#_programmation_structurée"></a><a class="link" href="#_programmation_structurée">1.3.1. Programmation structurée</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<em>Choisissez les procédures. Utiliser les meilleurs algorithmes que vous pourrez trouver.</em>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;accent est mis sur les <em>traitements</em></p>
</li>
<li>
<p>Approche très utilisée depuis de nombreuses années</p>
</li>
<li>
<p>Approche de haut en bas (<em>top-down</em>)</p>
</li>
<li>
<p>A beaucoup amélioré la qualité du logiciel</p>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
<div class="paragraph">
<p><em>Les données et les traitements restent indépendants.</em></p>
</div>
<div class="ulist">
<ul>
<li>
<p>Les données changent moins que les traitements</p>
</li>
<li>
<p>difficile d&#8217;assurer la cohérence entre les structures de données et les traitements qui les utilisent</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_programmation_modulaire"><a class="anchor" href="#_programmation_modulaire"></a><a class="link" href="#_programmation_modulaire">1.3.2. Programmation modulaire</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<em>Choisissez vos modules. Découpez le programme de telle sorte que les données soient masquées par ces modules.</em>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Un module est un ensemble de procédures connexes avec les données qu&#8217;elles manipulent</p>
</li>
<li>
<p>L&#8217;élément primordial passe de la conception des procédures à l&#8217;organisation des données</p>
</li>
<li>
<p>Principe de <em>masquage de l&#8217;information</em></p>
</li>
<li>
<p>Permet la <em>compilation séparée</em></p>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
<div class="paragraph">
<p><em>Les types ainsi définis diffèrent dans leur utilisation (création, &#8230;&#8203;) des types de base.</em></p>
</div>
<div class="ulist">
<ul>
<li>
<p>l&#8217;initialisation d&#8217;une variable d&#8217;un type défini par l&#8217;utilisateur nécessite l&#8217;appel d&#8217;une fonction particulière du type (laissé à la charge du programmeur)</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_programmation_par_abstraction_de_données"><a class="anchor" href="#_programmation_par_abstraction_de_données"></a><a class="link" href="#_programmation_par_abstraction_de_données">1.3.3. Programmation par abstraction de données</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<em>Choisissez les types dont vous avez besoin. Fournissez un ensemble complet d&#8217;opérations pour chaque type.</em>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Utilise les <em>types abstraits de données</em> (TAD)</p>
</li>
<li>
<p>L'<em>interface</em> d&#8217;un type abstrait isole complètement l&#8217;utilisateur des détails d&#8217;implémentation</p>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
<div class="paragraph">
<p><em>Il est nécessaire de modifier un type pour l&#8217;adapter.</em></p>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_programmation_orientée_objet"><a class="anchor" href="#_programmation_orientée_objet"></a><a class="link" href="#_programmation_orientée_objet">1.3.4. Programmation orientée objet</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<em>Choisissez vos classes. Fournissez un ensemble complet d&#8217;opérations pour chaque classe. Rendez toute similitude explicite à l&#8217;aide de l&#8217;héritage.</em>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Consiste à définir les classes puis à préciser les relations entre elles (notamment l'<em>héritage</em>)</p>
<div class="ulist">
<ul>
<li>
<p>définir des classes = définir des types utilisateurs</p>
</li>
<li>
<p>factoriser des comportements en créant des hiérarchies d&#8217;héritage</p>
</li>
<li>
<p>permet d&#8217;adapter un type existant sans le modifier</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
<div class="paragraph">
<p><em>La conception objet est une tâche difficile.</em></p>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_approche_objet_vs_approche_structurée"><a class="anchor" href="#_approche_objet_vs_approche_structurée"></a><a class="link" href="#_approche_objet_vs_approche_structurée">1.3.5. Approche objet vs. approche structurée</a></h4>
<div class="ulist">
<ul>
<li>
<p><strong>L&#8217;approche objet est moins intuitive</strong></p>
<div class="ulist">
<ul>
<li>
<p>décomposer un problème en une hiérarchie de fonctions atomiques et de données est plus naturel</p>
</li>
</ul>
</div>
</li>
<li>
<p><strong>La modélisation objet est difficile</strong></p>
<div class="ulist">
<ul>
<li>
<p>rien dans les concepts de base de l&#8217;approche objet ne dicte comment modéliser la structure objet d&#8217;un système de manière pertinente.</p>
</li>
<li>
<p>Comment mener une analyse qui respecte les concepts objet ?</p>
</li>
<li>
<p>Sans un cadre méthodologique approprié, la dérive structurée de la conception est inévitable</p>
</li>
</ul>
</div>
</li>
<li>
<p><strong>L&#8217;application des concepts objet nécessite de la rigueur</strong></p>
<div class="ulist">
<ul>
<li>
<p>Le vocabulaire précis est un facteur d&#8217;incompréhensions</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_approche_objet_vs_langage_de_programmation"><a class="anchor" href="#_approche_objet_vs_langage_de_programmation"></a><a class="link" href="#_approche_objet_vs_langage_de_programmation">1.3.6. Approche objet vs. langage de programmation</a></h4>
<div class="ulist">
<ul>
<li>
<p>Certains développeurs ne pensent objet qu&#8217;à travers un langage de programmation</p>
<div class="ulist">
<ul>
<li>
<p>les langages ne sont que des outils implémentant <strong>certains</strong> concepts objet d&#8217;une <strong>certaine</strong> façon</p>
</li>
<li>
<p>les langages ne garantissent en rien l&#8217;utilisation adéquat de ces moyens techniques</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
<div class="paragraph">
<p><em>Programmer en Java, en Python ou en C# n&#8217;est pas concevoir objet !</em></p>
</div>
<div class="ulist">
<ul>
<li>
<p>Seule une analyse objet conduit à une solution objet</p>
<div class="ulist">
<ul>
<li>
<p>i.e. qui respecte les concepts de base de l&#8217;approche objet.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le langage de programmation est un moyen d&#8217;implémentation</p>
<div class="ulist">
<ul>
<li>
<p>il ne garantit pas le respect des concepts objet</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_conception_objet"><a class="anchor" href="#_conception_objet"></a><a class="link" href="#_conception_objet">1.3.7. Conception objet</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
Concevoir objet, c&#8217;est d&#8217;abord concevoir un <em>modèle</em> qui respecte les concepts objet.
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Pour penser et concevoir objet, il faut savoir "prendre de la hauteur", jongler avec des concepts abstraits, indépendants des langages d&#8217;implémentation et des contraintes purement techniques</p>
</li>
<li>
<p>Les langages de programmation ne sont pas un support adéquat pour cela</p>
</li>
<li>
<p>Pour conduire une analyse objet cohérente, il ne faut pas directement penser en terme de pointeurs, d&#8217;attributs et de tableaux, mais en terme d&#8217;association, de propriétés et de cardinalités</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_évolutions_récentes"><a class="anchor" href="#_évolutions_récentes"></a><a class="link" href="#_évolutions_récentes">1.3.8. Évolutions récentes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Concepts OO/modularité :
<a href="https://en.wikipedia.org/wiki/Mixin">Mixin</a>/
<a href="https://en.wikipedia.org/wiki/Trait_%28computer_programming%29">Trait</a>,
<a href="https://en.wikipedia.org/wiki/Delegation_%28object-oriented_programming%29">Délégation</a>,
<a href="https://en.wikipedia.org/wiki/Aspect-oriented_programming">Aspect</a></p>
</li>
<li>
<p>Concepts issus de la <a href="https://en.wikipedia.org/wiki/Functional_programming">programmation fonctionnelle</a> :
fonctions lambda/fermeture (closure),
fonction d&#8217;ordre supérieure,
évaluation parasseuse</p>
</li>
<li>
<p>Programmation parallèle/gestion de la concurrence :
support des processeurs multi-c&oelig;urs</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_le_langage_java"><a class="anchor" href="#_le_langage_java"></a><a class="link" href="#_le_langage_java">1.4. Le langage Java</a></h3>
<div class="sect3">
<h4 id="_les_plateformes_java"><a class="anchor" href="#_les_plateformes_java"></a><a class="link" href="#_les_plateformes_java">1.4.1. Les plateformes Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Java Platform Standard Edition (Java SE)</p>
<div class="ulist">
<ul>
<li>
<p>dédiée aux postes clients et aux stations de travail</p>
</li>
</ul>
</div>
</li>
<li>
<p>Java Platform Enterprise Edition (Jakarta EE ou JEE)</p>
<div class="ulist">
<ul>
<li>
<p>dédiée aux applications d&#8217;entreprises (serveur, postes clients, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Java Embedded</p>
<div class="ulist">
<ul>
<li>
<p>dédiée aux systèmes embarqués (Internet des Objets, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_vue_densemble_de_la_plateforme_java_se"><a class="anchor" href="#_vue_densemble_de_la_plateforme_java_se"></a><a class="link" href="#_vue_densemble_de_la_plateforme_java_se">1.4.2. Vue d&#8217;ensemble de la plateforme Java SE</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/javase_platform.png" alt="javase platform">
</div>
<div class="title">Figure 4. <a href="http://docs.oracle.com/javase/" class="bare">http://docs.oracle.com/javase/</a></div>
</div>
</div>
<div class="sect3">
<h4 id="_java_runtime_environment"><a class="anchor" href="#_java_runtime_environment"></a><a class="link" href="#_java_runtime_environment">1.4.3. Java Runtime Environment</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le <em>Java Runtime Environment</em> (JRE) fournit la <em>machine virtuelle Java</em>, les bibliothèques et d&#8217;autres composants nécessaires pour l&#8217;exécution de programmes Java</p>
</li>
<li>
<p>Déjà installé sur la plupart des systèmes d&#8217;exploitation</p>
</li>
<li>
<p>Le lanceur d&#8217;application (<code>java</code>) est l&#8217;outil ligne de commande permettant l&#8217;exécution de programme Java</p>
</li>
</ul>
</div>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
Plus d&#8217;informations : <a href="http://docs.oracle.com/javase/8/docs/technotes/guides/">Java Platform Overview</a>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_java_development_kit"><a class="anchor" href="#_java_development_kit"></a><a class="link" href="#_java_development_kit">1.4.4. Java Development Kit</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le <em>Java Development Kit</em> (JDK) fournit le JRE ainsi qu&#8217;un ensemble d&#8217;outils pour le développement d&#8217;applications</p>
</li>
<li>
<p><strong>Doit être installé pour développer en Java</strong></p>
</li>
<li>
<p>L&#8217;outil <code>javac</code> est le compilateur en ligne de commande</p>
</li>
</ul>
</div>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
Plus d&#8217;informations : <a href="http://docs.oracle.com/javase/8/docs/technotes/guides/">Java Platform Overview</a>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_caractéristiques_du_langage"><a class="anchor" href="#_caractéristiques_du_langage"></a><a class="link" href="#_caractéristiques_du_langage">1.4.5. Caractéristiques du langage</a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1">Simple</dt>
<dd>
<p>un développeur peut être rapidement opérationnel</p>
</dd>
<dt class="hdlist1">Orienté-objet</dt>
<dd>
<p>bon respect des concepts OO</p>
</dd>
<dt class="hdlist1">Interprété</dt>
<dd>
<p>la compilation génère un code intermédiaire qui est interprété</p>
</dd>
<dt class="hdlist1">Portable</dt>
<dd>
<p>un programme compilé fonctionne sans modification sur différentes plateformes</p>
</dd>
<dt class="hdlist1">Robuste</dt>
<dd>
<p>vérifications à la compilation et à l&#8217;exécution</p>
</dd>
<dt class="hdlist1">Multithread</dt>
<dd>
<p>supporte la programmation concurrente</p>
</dd>
<dt class="hdlist1">Adaptable</dt>
<dd>
<p>supporte le chargement dynamique de code</p>
</dd>
<dt class="hdlist1">Sécurisé</dt>
<dd>
<p>le langage intègre un modèle de sécurité sophistiqué</p>
</dd>
</dl>
</div>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<a href="http://www.oracle.com/technetwork/java/langenv-140151.html">The Java Language Environment: A White Paper</a>, James Gosling, 1996.
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_compilation_et_interprétation"><a class="anchor" href="#_compilation_et_interprétation"></a><a class="link" href="#_compilation_et_interprétation">1.4.6. Compilation et interprétation</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le langage Java est à la fois <em>interprété</em> et <em>compilé</em></p>
</li>
<li>
<p>Un fichier source (<code>.java</code>) est compilé en un langage intermédiaire appelé <em>bytecode</em> (<code>.class</code>)</p>
</li>
<li>
<p>Ce bytecode est ensuite interprété par la <em>machine virtuelle Java</em></p>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/java_compil.png" alt="java compil">
</div>
<div class="title">Figure 5. <a href="http://docs.oracle.com/javase/tutorial/getStarted/intro/definition.html">About the Java Technology</a></div>
</div>
</div>
<div class="sect3">
<h4 id="_compilation_en_ligne_de_commande_jdk"><a class="anchor" href="#_compilation_en_ligne_de_commande_jdk"></a><a class="link" href="#_compilation_en_ligne_de_commande_jdk">1.4.7. Compilation en ligne de commande (JDK)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ javac &lt;options&gt; &lt;fichiers source&gt;</code></pre>
</div>
</div>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>-g</code>|<code>\-g$:$none</code></dt>
<dd>
<p>gère les informations pour le débogage</p>
</dd>
<dt class="hdlist1"><code>-classpath</code>|<code>-cp</code></dt>
<dd>
<p>fixe le chemin de recherche des classes compilées (<em>Classpath</em>)</p>
</dd>
<dt class="hdlist1"><code>-source</code></dt>
<dd>
<p>précise la version des fichiers sources (<code>1.6</code>, &#8230;&#8203;, <code>1.8</code>)</p>
</dd>
<dt class="hdlist1"><code>-sourcepath</code></dt>
<dd>
<p>fixe le chemin de recherche des sources</p>
</dd>
<dt class="hdlist1"><code>-encoding</code></dt>
<dd>
<p>précise l&#8217;encodage des fichiers sources ("UTF-8", &#8230;&#8203;)</p>
</dd>
<dt class="hdlist1"><code>-d</code></dt>
<dd>
<p>fixe le répertoire de destination pour les classes compilées</p>
</dd>
<dt class="hdlist1"><code>-target</code></dt>
<dd>
<p>précise la version de la VM cible</p>
</dd>
</dl>
</div>
<div class="listingblock">
<div class="title">Compilation séparant les sources des fichiers compilés</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ javac -sourcepath src -source 1.7 \
-d classes -classpath classes \
-g src/MonApplication.java</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exécution_en_ligne_de_commande_jre"><a class="anchor" href="#_exécution_en_ligne_de_commande_jre"></a><a class="link" href="#_exécution_en_ligne_de_commande_jre">1.4.8. Exécution en ligne de commande (JRE)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ java [-options] class [args...]
$ java [-options] -jar jarfile [args...]</code></pre>
</div>
</div>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>class</code></dt>
<dd>
<p>est ici le nom de la classe (le <code>.class</code> doit pouvoir être trouvé dans le <em>CLASSPATH</em>)</p>
</dd>
<dt class="hdlist1"><code>-cp|-classpath</code></dt>
<dd>
<p>fixe le chemin de recherche des classes compilées</p>
</dd>
<dt class="hdlist1"><code>-jar</code></dt>
<dd>
<p>exécute un programme encapsulé dans un fichier <code>jar</code></p>
</dd>
</dl>
</div>
<div class="listingblock">
<div class="title">Exécution}</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ java -cp classes MonApplication</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_classpath"><a class="anchor" href="#_classpath"></a><a class="link" href="#_classpath">1.4.9. <em>Classpath</em></a></h4>
<div class="ulist">
<ul>
<li>
<p>Le <em>Classpath</em> précise la liste des bibliothèques ou des classes compilées utilisées par l&#8217;environnement Java</p>
</li>
<li>
<p>Le compilateur ou la machine virtuelle ont besoin d&#8217;avoir accès aux classes compilées</p>
</li>
<li>
<p>Il peut être défini en ligne de commande ou par la variable d&#8217;environnement <code>CLASSPATH</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_constructions_de_base_du_langage_java"><a class="anchor" href="#_constructions_de_base_du_langage_java"></a><a class="link" href="#_constructions_de_base_du_langage_java">1.4.10. Constructions de base du langage Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Java différencie majuscules et minuscules</p>
</li>
<li>
<p>Java possède une syntaxe proche du C</p>
<div class="ulist">
<ul>
<li>
<p>se retrouve à tous les niveaux (commentaires, types, opérateurs, &#8230;&#8203;)</p>
</li>
<li>
<p>chaque instruction se termine par un <code>;</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Commentaires</p>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>/* &#8230;&#8203; */</code></dt>
<dd>
<p>le texte entre <code>/<strong></code> et <code></strong>/</code> est ignoré</p>
</dd>
<dt class="hdlist1"><code>// &#8230;&#8203;</code></dt>
<dd>
<p>le texte jusqu&#8217;à la fin de la ligne est ignoré</p>
</dd>
</dl>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_types_primitifs"><a class="anchor" href="#_types_primitifs"></a><a class="link" href="#_types_primitifs">1.4.11. Types primitifs</a></h4>
<div class="paragraph">
<p>Un <em>type primitif</em> est un type de base du langage, i.e. non défini par l&#8217;utilisateur.
<strong>En Java, les valeurs de ces types ne sont pas des objets</strong>.</p>
</div>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>boolean</code></dt>
<dd>
<p><code>true</code> ou <code>false</code></p>
</dd>
<dt class="hdlist1"><code>byte</code></dt>
<dd>
<p>entier de -128 à 127 (les types entiers sont signés)</p>
</dd>
<dt class="hdlist1"><code>short</code></dt>
<dd>
<p>entier de -32768 à 32767</p>
</dd>
<dt class="hdlist1"><code>int</code></dt>
<dd>
<p>entier de -2<sup>31</sup> à 2<sup>31</sup> - 1</p>
</dd>
<dt class="hdlist1"><code>long</code></dt>
<dd>
<p>entier de -2<sup>63</sup> à 2<sup>63</sup> - 1</p>
</dd>
<dt class="hdlist1"><code>char</code></dt>
<dd>
<p>caractère Unicode sur 16 bits de <code>\u0000</code> à <code>\uffff</code></p>
</dd>
<dt class="hdlist1"><code>float</code></dt>
<dd>
<p>nombre en virgule flottante simple précision (32 bits IEEE 754)</p>
</dd>
<dt class="hdlist1"><code>double</code></dt>
<dd>
<p>nombre en virgule flottante double précision (64 bits IEEE 754)</p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_littéraux"><a class="anchor" href="#_littéraux"></a><a class="link" href="#_littéraux">1.4.12. Littéraux</a></h4>
<div class="paragraph">
<p>Un <em>littéral</em> est la représentation dans le code source d&#8217;une valeur d&#8217;un type.</p>
</div>
<div class="dlist">
<dl>
<dt class="hdlist1">Entiers</dt>
<dd>
<p><code>123</code> de type <code>int</code>, <code>123L</code> de type <code>long</code>, <code>0x123</code> en hexadécimal, <code>0b101</code> en binaire</p>
</dd>
<dt class="hdlist1">Flottants</dt>
<dd>
<p><code>1.23E-4</code> de type <code>double</code>, <code>1.23E-4F</code> de type <code>float</code></p>
</dd>
<dt class="hdlist1">Booléens</dt>
<dd>
<p><code>true</code> ou <code>false</code></p>
</dd>
<dt class="hdlist1">Caractères</dt>
<dd>
<p><code>'a'</code>, <code>'\t'</code> ou <code>'\u0000'</code></p>
</dd>
<dt class="hdlist1">Chaînes</dt>
<dd>
<p><code>"texte"</code></p>
</dd>
<dt class="hdlist1">Null</dt>
<dd>
<p><code>null</code> (valeur des références non initialisées)</p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_déclarations_et_initialisations_de_variables"><a class="anchor" href="#_exemple_de_déclarations_et_initialisations_de_variables"></a><a class="link" href="#_exemple_de_déclarations_et_initialisations_de_variables">1.4.13. Exemple de déclarations et initialisations de variables</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Exemples de déclaration avec initialisation
// (pas indispensable mais conseillé)

byte aByte = 12;            // Un entier sur 8 bits
short aShort = 130;         // Un entier sur 16 bits
int anInteger = -153456;    // Un entier sur 32 bits

// Remarquer le L pour le litteral de type long
// (sinon erreur a la compilation: entier trop grand)
long aLong = 987654321234L; // Un entier sur 64 bits

// Remarquer le F pour le litteral de type float
// (sinon erreur a la compilation: perte de precision)
float aFloat = 1.3F;        // Un reel simple precision
double aDouble = -1.5E-4;   // Un reel double precision

char aChar = 'S';           // Un caractere
boolean aBoolean = true;    // Un booleen

// La constante est introduite par le mot-cle final
final int aConst = 0;       // Une constante</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_références_12"><a class="anchor" href="#_références_12"></a><a class="link" href="#_références_12">1.4.14. Références 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les variables de type tableau, énumération, objet ou interface sont en fait des <em>références</em></p>
</li>
<li>
<p>La valeur d&#8217;une telle variable est une <em>référence vers</em> (<em>l&#8217;adresse de</em>) une donnée</p>
</li>
<li>
<p>Dans d&#8217;autres langages, une référence est appelée <em>pointeur</em> ou <em>adresse mémoire</em></p>
</li>
<li>
<p>En Java, la différence réside dans le fait qu&#8217;on ne manipule pas directement l&#8217;adresse mémoire: le nom de la variable est utilisé à la place</p>
<div class="ulist">
<ul>
<li>
<p>pas d&#8217;arithmétique des pointeurs en Java</p>
</li>
<li>
<p>les références assurent une meilleure sécurité (moins d&#8217;erreurs de programmation)</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;association (l&#8217;affectation) d&#8217;une donnée à une variable <em>lie</em> l&#8217;identificateur et la donnée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_références_22"><a class="anchor" href="#_références_22"></a><a class="link" href="#_références_22">1.4.15. Références 2/2</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/reference.png" alt="reference">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_référence_vs_pointeur"><a class="anchor" href="#_référence_vs_pointeur"></a><a class="link" href="#_référence_vs_pointeur">1.4.16. Référence vs. pointeur</a></h4>
<div class="ulist">
<ul>
<li>
<p>Dans les deux cas, ce sont des variables (ou des constantes) dont la valeur (le contenu) est une adresse mémoire</p>
</li>
<li>
<p>Un pointeur est un concept de bas-niveau permettant une manipulation précise de l&#8217;adresse (arithmétique des pointeurs, pointeur de fonction, &#8230;&#8203;)</p>
</li>
<li>
<p>Une référence est une <em>abstraction</em> de plus haut niveau qui fournit une interface plus simple mais plus limitée pour manipuler l&#8217;adresse</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_gestion_de_la_mémoire_dans_la_jvm"><a class="anchor" href="#_gestion_de_la_mémoire_dans_la_jvm"></a><a class="link" href="#_gestion_de_la_mémoire_dans_la_jvm">1.4.17. Gestion de la mémoire dans la JVM</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les variables locales (types primitifs et références vers des objets du tas) sont créées sur la pile (<em>stack</em>)</p>
</li>
<li>
<p>Lors de la création d&#8217;un object, la mémoire est allouée dans une zone mémoire appelée le <em>tas</em> (<em>heap</em>)</p>
</li>
<li>
<p>La libération de la mémoire est automatique et gérée par le <em>ramasse-miette</em> (<em>garbage collector</em>)</p>
<div class="ulist">
<ul>
<li>
<p>le GC s&#8217;exécute lorque certaines conditions sont réunies</p>
</li>
</ul>
</div>
</li>
<li>
<p>Certains paramètres de la JVM permettent de contrôler le GC et les zones mémoires (<code>-mx</code>|<code>-Xmx</code>, <code>-XX:+UseParallelGC</code>, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux"><a class="anchor" href="#_tableaux"></a><a class="link" href="#_tableaux">1.4.18. Tableaux</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>tableau</em> est une structure de données regroupant plusieurs valeurs de même type</p>
</li>
<li>
<p>La taille d&#8217;un tableau est déterminée lors de sa création (à l&#8217;exécution)</p>
</li>
<li>
<p>La taille d&#8217;un tableau ne varie pas par la suite</p>
</li>
<li>
<p>Un tableau peut contenir des références</p>
<div class="ulist">
<ul>
<li>
<p>tableau d&#8217;objets ou tableau de tableaux</p>
</li>
<li>
<p>permet de créer des tableaux à plusieurs dimensions</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/array.png" alt="array">
</div>
<div class="title">Figure 6. <a href="http://docs.oracle.com/javase/tutorial/java/nutsandbolts/arrays.html">The Java Tutorials: Arrays</a></div>
</div>
</div>
<div class="sect3">
<h4 id="_déclaration_et_création_de_tableaux"><a class="anchor" href="#_déclaration_et_création_de_tableaux"></a><a class="link" href="#_déclaration_et_création_de_tableaux">1.4.19. Déclaration et création de tableaux</a></h4>
<div class="ulist">
<ul>
<li>
<p>La déclaration d&#8217;une variable de type tableau se fait en ajoutant <code>[]</code> au type des éléments</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La création du tableau se fait en utilisant l&#8217;opérateur <code>new</code> suivi du type des éléments du tableau et de sa taille entre <code>[]</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">new int[10];</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La référence retournée par <code>new</code> peut être liée à une variable</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Il est possible de créer et d&#8217;initialiser un tableau en une seule étape</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = { 1, 5, 10 };</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_manipulation_de_tableaux"><a class="anchor" href="#_manipulation_de_tableaux"></a><a class="link" href="#_manipulation_de_tableaux">1.4.20. Manipulation de tableaux</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;accès aux éléments d&#8217;un tableau se fait en utilisant le nom du tableau suivi de l&#8217;indice entre <code>[]</code> (exemple: <code>unTableau[2]</code>)</p>
</li>
<li>
<p>La taille d&#8217;un tableau peut être obtenue en utilisant la propriété <code>length</code> (exemple: <code>unTableau.length</code>)</p>
</li>
<li>
<p>La méthode de classe <code>arraycopy</code> de <code>System</code> permet de copier efficacement un tableau</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_16"><a class="anchor" href="#_tableaux_et_références_16"></a><a class="link" href="#_tableaux_et_références_16">1.4.21. Tableaux et références 1/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref1.png" alt="tabref1">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_26"><a class="anchor" href="#_tableaux_et_références_26"></a><a class="link" href="#_tableaux_et_références_26">1.4.22. Tableaux et références 2/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];
int[] leMemeTableau = unTableau;</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref2.png" alt="tabref2">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_36"><a class="anchor" href="#_tableaux_et_références_36"></a><a class="link" href="#_tableaux_et_références_36">1.4.23. Tableaux et références 3/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];
int[] leMemeTableau = unTableau;
leMemeTableau[0] = 12;</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref3.png" alt="tabref3">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_46"><a class="anchor" href="#_tableaux_et_références_46"></a><a class="link" href="#_tableaux_et_références_46">1.4.24. Tableaux et références 4/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];
int[] leMemeTableau = unTableau;
leMemeTableau[0] = 12;
int[] unAutreTableau = new int[5];</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref4.png" alt="tabref4">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_56"><a class="anchor" href="#_tableaux_et_références_56"></a><a class="link" href="#_tableaux_et_références_56">1.4.25. Tableaux et références 5/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];
int[] leMemeTableau = unTableau;
leMemeTableau[0] = 12;
int[] unAutreTableau = new int[5];
leMemeTableau = unAutreTableau;</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref5.png" alt="tabref5">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_tableaux_et_références_66"><a class="anchor" href="#_tableaux_et_références_66"></a><a class="link" href="#_tableaux_et_références_66">1.4.26. Tableaux et références 6/6</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[] unTableau = new int[10];
int[] leMemeTableau = unTableau;
leMemeTableau[0] = 12;
int[] unAutreTableau = new int[5];
leMemeTableau = unAutreTableau;
leMemeTableau[0] = 21;</code></pre>
</div>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/tabref6.png" alt="tabref6">
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_python_refcard"><a class="anchor" href="#_python_refcard"></a><a class="link" href="#_python_refcard">1.5. Python RefCard</a></h3>
<div class="sect3">
<h4 id="_le_langage_python"><a class="anchor" href="#_le_langage_python"></a><a class="link" href="#_le_langage_python">1.5.1. Le langage Python</a></h4>
<div class="ulist">
<ul>
<li>
<p>Créé en 1990 par Guido Van Rossum</p>
</li>
<li>
<p>Caractéristiques</p>
<div class="ulist">
<ul>
<li>
<p>compilé/interprété</p>
</li>
<li>
<p>langage de scripts</p>
</li>
<li>
<p>système de typage implicite, dynamique, fort</p>
</li>
<li>
<p>support de la programmation procédurale, OO, fonctionnelle (partiel)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
En 12/2023, deux versions incompatibles de Python co-existent (<a href="https://wiki.python.org/moin/Python2orPython3">2.7 et 3.11</a>)
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_domaines_dapplication"><a class="anchor" href="#_quelques_domaines_dapplication"></a><a class="link" href="#_quelques_domaines_dapplication">1.5.2. Quelques domaines d&#8217;application</a></h4>
<div class="ulist">
<ul>
<li>
<p>Langage de scripts</p>
</li>
<li>
<p>Programmation scientifique</p>
<div class="ulist">
<ul>
<li>
<p>analyse de données, bioinformatique (analyse du génôme)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Développement web</p>
<div class="ulist">
<ul>
<li>
<p>plusieurs frameworks populaires</p>
</li>
</ul>
</div>
</li>
<li>
<p>Développement d&#8217;outils pour le développement logiciel</p>
</li>
<li>
<p>Enseignement de l&#8217;informatique</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_implémentations"><a class="anchor" href="#_implémentations"></a><a class="link" href="#_implémentations">1.5.3. Implémentations</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://fr.wikipedia.org/wiki/CPython">CPython</a> est l&#8217;implémentation de référence</p>
</li>
<li>
<p>Principales implémentations alternatives</p>
<div class="ulist">
<ul>
<li>
<p><a href="http://www.jython.org/">Jython</a> pour la JVM,</p>
</li>
<li>
<p><a href="http://ironpython.net/">IronPython</a> pour .Net,</p>
</li>
<li>
<p><a href="http://pypy.org/">PyPy</a></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_distributions"><a class="anchor" href="#_distributions"></a><a class="link" href="#_distributions">1.5.4. Distributions</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://www.python.org/downloads/">Langage seul</a></p>
</li>
<li>
<p>Paquets sous Linux (
<a href="https://packages.debian.org/stretch/python">python</a>/ <a href="https://packages.debian.org/stretch/python3">python3</a> sous Debian,
<a href="http://packages.ubuntu.com/xenial/python">python</a>/ <a href="http://packages.ubuntu.com/xenial/python3">python3</a> sous Ubuntu, &#8230;&#8203;)</p>
</li>
<li>
<p><a href="https://www.continuum.io/anaconda-overview">Anaconda</a></p>
</li>
<li>
<p><a href="https://www.activestate.com/activepython">ActivePython</a></p>
</li>
<li>
<p><a href="http://python-xy.github.io/">Python(x,y)</a></p>
</li>
<li>
<p><a href="https://software.intel.com/en-us/intel-distribution-for-python">Intel Distribution for Python</a></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_outils_de_développement"><a class="anchor" href="#_quelques_outils_de_développement"></a><a class="link" href="#_quelques_outils_de_développement">1.5.5. Quelques outils de développement</a></h4>
<div class="ulist">
<ul>
<li>
<p>REPL :
<a href="https://ipython.org/">IPython</a></p>
</li>
<li>
<p>Notebook :
<a href="https://jupyter.org/">Jupyter</a></p>
</li>
<li>
<p>IDE :
<a href="https://pythonhosted.org/spyder/">Spyder</a>,
<a href="https://www.jetbrains.com/pycharm/">PyCharm</a>,
<a href="http://www.pydev.org/">PyDev</a>,
<a href="https://marketplace.visualstudio.com/items?itemName=donjayamanne.python">Python pour VS Code</a>,
<a href="https://microsoft.github.io/PTVS/">Python Tools for Visual Studio</a></p>
</li>
<li>
<p>Guide de style :
<a href="https://www.python.org/dev/peps/pep-0008/">PEP 8</a>,
<a href="http://pep8.org/">PEP 8 — the Style Guide for Python Code</a>,
<a href="https://google.github.io/styleguide/pyguide.html">Google Python Style Guide</a></p>
</li>
<li>
<p>Documentation :
<a href="https://docs.python.org/3/library/pydoc.html">pydoc</a></p>
</li>
<li>
<p>Audit de code :
<a href="https://www.pylint.org/">Pylint</a></p>
</li>
<li>
<p>Gestion des paquets :
<a href="https://pip.pypa.io/en/stable/">pip</a>,
<a href="https://pypi.python.org/pypihttps://pypi.python.org/pypi">PyPI</a></p>
</li>
<li>
<p>Environnement virtuel :
<a href="https://pypi.python.org/pypi/virtualenv">virtualenv</a>,
<a href="https://virtualenvwrapper.readthedocs.io/en/latest/">virtualenvwrapper</a>,
<a href="http://docs.pipenv.org/en/latest/">pipenv</a></p>
</li>
<li>
<p>Débogage :
<a href="https://docs.python.org/3/library/pdb.html">pdb</a>/
<a href="https://github.com/gotcha/ipdb">ipdb</a></p>
</li>
<li>
<p>Tests unitaires :
<a href="https://docs.python.org/3/library/unittest.html">unittest</a></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_lancer_un_interpréteur_interactif"><a class="anchor" href="#_lancer_un_interpréteur_interactif"></a><a class="link" href="#_lancer_un_interpréteur_interactif">1.5.6. Lancer un interpréteur interactif</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lancer le REPL (cmd: python3)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ python3
Python 3.10.9 (main, Dec 15 2022, 17:11:09) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
&gt;&gt;&gt; quit()
$</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Lancer IPython (cmd: ipython3)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ ipython3
Python 3.5.3rc1 (default, Jan  3 2023, 04:40:57)
Type "copyright", "credits" or "license" for more information.

IPython 5.1.0 -- An enhanced Interactive Python.
?         -&gt; Introduction and overview of IPython's features.
%quickref -&gt; Quick reference.
help      -&gt; Python's own help system.
object?   -&gt; Details about 'object', use 'object??' for extra details.

In [1]: quit
$</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_lancer_un_notebook_jupiter"><a class="anchor" href="#_lancer_un_notebook_jupiter"></a><a class="link" href="#_lancer_un_notebook_jupiter">1.5.7. Lancer un notebook Jupiter</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lancement sur <a href="http://localhost:8888/" class="bare">http://localhost:8888/</a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ jupyter-notebook
[I 09:55:27.102 NotebookApp] Writing notebook server cookie secret to /run/user/1000/jupyter/notebook_cookie_secret
[W 09:55:27.136 NotebookApp] Widgets are unavailable. On Debian, notebook support for widgets is provided by the package jupyter-nbextension-jupyter-js-widgets
[I 09:55:27.151 NotebookApp] Serving notebooks from local directory: /home/hal
[I 09:55:27.151 NotebookApp] 0 active kernels
[I 09:55:27.151 NotebookApp] The Jupyter Notebook is running at: http://localhost:8888/
[I 09:55:27.151 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Arrêt en tapant deux fois Ctrl+C</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_script_python"><a class="anchor" href="#_exemple_de_script_python"></a><a class="link" href="#_exemple_de_script_python">1.5.8. Exemple de script Python</a></h4>
<div class="listingblock">
<div class="title">Fichier <code>intro/first_script.py</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">#!/usr/bin/env python3
# -*- coding: utf-8 -*-

"""Ce module est un exemple simple de script Python.

    Un commentaire débute par # et se termine en fin de ligne.
    Un script débute par un shebang (optionnel).
    Le shebang est inutile dans le cas d'un module non exécuté directement
    La seconde ligne de commentaire précise l'encodage du fichier (optionnel).
    On trouve ensuite la docstring du module qui documente le module lui-même (optionnel).
"""

print(
    """
        Ce code est exécuté dans tous les cas.
    """)

if __name__ == '__main__':
    # L'indentation définit un bloc de code imbriqué
    print(
        """
            Ce bloc de code est exécuté uniquement quand le module est invoqué
            directement par l'interpréteur, i.e. pas importé
        """)</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exécuter_un_programme_python"><a class="anchor" href="#_exécuter_un_programme_python"></a><a class="link" href="#_exécuter_un_programme_python">1.5.9. Exécuter un programme Python</a></h4>
<div class="ulist">
<ul>
<li>
<p>En appelant l&#8217;interpréteur</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ python3 intro/first_script.py

        Ce code est exécuté dans tous les cas.


            Ce bloc de code est exécuté uniquement quand le module est invoqué
            directement par l'interpréteur, i.e. pas importé</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Directement par le shell (utilise le <em>shebang</em>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ chmod +x intro/first_script.py
$ intro/first_script.py</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_généralités"><a class="anchor" href="#_généralités"></a><a class="link" href="#_généralités">1.5.10. Généralités</a></h4>
<div class="ulist">
<ul>
<li>
<p>Commentaire introduit par <code>#</code></p>
</li>
<li>
<p>Différence entre minuscules et majuscules</p>
</li>
<li>
<p>L&#8217;indentation définit l&#8217;imbrication des blocs</p>
</li>
<li>
<p>Pas de constante</p>
<div class="ulist">
<ul>
<li>
<p>variable qu&#8217;on ne modifie pas</p>
</li>
<li>
<p>par convention, nommée en majuscule et avec des <code>_</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Toutes les données sont représentées par des <em>objets</em></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_principaux_types_prédéfinis_12"><a class="anchor" href="#_principaux_types_prédéfinis_12"></a><a class="link" href="#_principaux_types_prédéfinis_12">1.5.11. Principaux types prédéfinis 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>numbers.Number</code> représente les nombres (immuables)</p>
<div class="ulist">
<ul>
<li>
<p><code>numbers.Integral</code> pour les entiers</p>
<div class="ulist">
<ul>
<li>
<p><code>int</code> nombre entier sans limite de taille</p>
</li>
<li>
<p><code>bool</code> possède les valeurs <code>True</code> et <code>False</code></p>
</li>
</ul>
</div>
</li>
<li>
<p><code>float</code> (<code>numbers.Real</code>) nombre en virgule flottante double précision</p>
</li>
<li>
<p><code>complex</code> (<code>numbers.Complex</code>) nombre complexe représenté comme une paire de <code>float</code></p>
</li>
</ul>
</div>
</li>
<li>
<p><code>None</code> possède une seule valeur <code>None</code></p>
</li>
<li>
<p>cf. <a href="https://docs.python.org/3/reference/datamodel.html#the-standard-type-hierarchy">The standard type hierarchy</a></p>
</li>
</ul>
</div>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
Les exemples de cette section sont disponibles dans le notebook <a href="https://nbviewer.jupyter.org/urls/bitbucket.org/hal_prism/cours.poo.exemples.python/raw/master/intro/Python%20RefCard.ipynb"><code>intro/Python RefCard.ipynb</code></a>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_principaux_types_prédéfinis_22"><a class="anchor" href="#_principaux_types_prédéfinis_22"></a><a class="link" href="#_principaux_types_prédéfinis_22">1.5.12. Principaux types prédéfinis 2/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>séquence</em> représente une collection ordonnée (indexée par des entiers)</p>
<div class="ulist">
<ul>
<li>
<p>une <em>séquence immuable</em> ne change pas après sa création</p>
<div class="ulist">
<ul>
<li>
<p>une <em>chaîne de caractère</em> est une séquence de caractères unicodes</p>
</li>
<li>
<p>un <em>tuple</em> représente un n-uplet d&#8217;objets quelconques</p>
</li>
</ul>
</div>
</li>
<li>
<p>une <em>séquence mutable</em> supporte les modifications</p>
<div class="ulist">
<ul>
<li>
<p>une <em>liste</em> est formée d&#8217;éléments quelconques</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</li>
<li>
<p>Un <em>ensemble</em> représente une collection non ordonnée d&#8217;éléments uniques</p>
<div class="ulist">
<ul>
<li>
<p>un <em>ensemble</em> est modifiable</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un <em>dictionnaire</em> représente une collection modifiable de couples (clé, valeur)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_littéraux_2"><a class="anchor" href="#_littéraux_2"></a><a class="link" href="#_littéraux_2">1.5.13. Littéraux</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>littéral</em> est la représentation dans le code source d&#8217;une valeur d&#8217;un type</p>
</li>
<li>
<p><code>int</code> : <code>1234</code>, <code>0b11001</code> en binaire, <code>0o177</code> en octal, <code>0xAFF</code> en héxa, <code>_</code> est permis (v 3.6)</p>
</li>
<li>
<p><code>float</code> : <code>3.14</code>, <code>10.</code>, <code>.001</code>, <code>1e100</code>, <code>3.14e-10</code></p>
</li>
<li>
<p>Imaginaire : littéral <code>float</code> suffixé par <code>j</code> construit un complexe de partie réelle nulle (<code>3+4j</code> pour une partie réelle non nulle)</p>
</li>
<li>
<p>Chaîne : <code>"chaîne"</code>, <code>'chaîne'</code>, <code>"""chaîne multi-lignes"""</code>, <code>'''chaîne multi-lignes'''</code>, préfixée par <code>r</code> pour éviter l&#8217;interprétation, par <code>f</code> pour une chaîne formatée (v 3.6)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_liaison_des_variables_et_référence"><a class="anchor" href="#_liaison_des_variables_et_référence"></a><a class="link" href="#_liaison_des_variables_et_référence">1.5.14. Liaison des variables et référence</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les variables sont en fait des <em>références</em></p>
</li>
<li>
<p>La valeur d&#8217;une telle variable est une référence vers (l&#8217;adresse de) une donnée</p>
<div class="ulist">
<ul>
<li>
<p>dans d&#8217;autres langages, une référence est appelée <em>pointeur</em></p>
</li>
<li>
<p>dans les deux cas, ce sont des variables dont la valeur (le contenu) est une adresse mémoire</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une référence est une <em>abstraction</em> de plus haut niveau</p>
<div class="ulist">
<ul>
<li>
<p>fournit une interface plus simple pour manipuler l&#8217;adresse</p>
</li>
<li>
<p>ne permet pas de manipuler directement l&#8217;adresse mémoire</p>
</li>
<li>
<p>un pointeur est un concept de bas-niveau permettant une manipulation directe de l&#8217;adresse (arithmétique des pointeurs, pointeur de fonction, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;association (l&#8217;affectation) d&#8217;une donnée à une variable <em>lie</em> l&#8217;identificateur et la donnée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_structures_de_contrôle"><a class="anchor" href="#_structures_de_contrôle"></a><a class="link" href="#_structures_de_contrôle">1.5.15. Structures de contrôle</a></h4>
<div class="ulist">
<ul>
<li>
<p>instruction <code>pass</code></p>
</li>
<li>
<p><code>if i &lt; 10:</code>, <code>elif i &gt; 100:</code>, <code>else:</code></p>
</li>
<li>
<p><code>while i &lt; 10:</code></p>
</li>
<li>
<p><code>for idx in seq:</code>, <code>for i in range(0, 10, 3):</code></p>
</li>
<li>
<p><code>break</code>, <code>continue</code>, <code>else:</code> pour une boucle</p>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
Il faut bien respecter l&#8217;indentation.
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_opérateurs_spécifiques"><a class="anchor" href="#_quelques_opérateurs_spécifiques"></a><a class="link" href="#_quelques_opérateurs_spécifiques">1.5.16. Quelques opérateurs spécifiques</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>/</code> représente la division en virgule flottante</p>
</li>
<li>
<p><code>//</code> représente la division entière</p>
</li>
<li>
<p><code>**</code> représente l&#8217;élévation à la puissance</p>
</li>
<li>
<p><code>a if condition else b</code> est une expression conditionnelle</p>
</li>
<li>
<p>pas d&#8217;opérateur de conversion de types</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_fonction"><a class="anchor" href="#_fonction"></a><a class="link" href="#_fonction">1.5.17. Fonction</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lors de l&#8217;appel, les paramètres formels sont liés aux arguments</p>
</li>
<li>
<p>Un appel de fonction retourne toujours une valeur (éventuellement <code>None</code>)</p>
</li>
<li>
<p>Les fonctions peuvent être imbriquées</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">def fib(n):
    """Print a Fibonacci series up to n."""
    a, b = 0, 1
    while a &lt; n:
        print(a, end=' ')
        a, b = b, a+b
    print()

fib(2000) # Appel de la fonction</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_manipulation_de_chaînes"><a class="anchor" href="#_exemple_de_manipulation_de_chaînes"></a><a class="link" href="#_exemple_de_manipulation_de_chaînes">1.5.18. Exemple de manipulation de chaînes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une chaîne est une instance immuable de la classe <a href="https://docs.python.org/3/library/stdtypes.html#textseq"><code>str</code></a></p>
</li>
<li>
<p>Le module <a href="https://docs.python.org/3/library/string.html"><code>string</code></a> complète les possibilités de manipulation de chaînes</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">word = 3 * 'un' + 'ium' # 'unununium'
word[0]   # character in position 0
word[-1]  # last character
word[2:5] # characters from position 2 (included) to 5 (excluded)
word[:2]  # character from the beginning to position 2 (excluded)
word[4:]  # characters from position 4 (included) to the end
len(word) # size of the string</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_manipulation_de_tuples"><a class="anchor" href="#_exemple_de_manipulation_de_tuples"></a><a class="link" href="#_exemple_de_manipulation_de_tuples">1.5.19. Exemple de manipulation de tuples</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un tuple supporte les opérations sur les <a href="https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range">séquences</a></p>
</li>
<li>
<p>Un tuple est une instance immuable de la classe <a href="https://docs.python.org/3/library/stdtypes.html#tuple">tuple</a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">t = () # tuple vide
t = 12345, # singleton
t = 12345, 54321, 'hello!'
t[0] # premier élément</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_manipulation_de_listes"><a class="anchor" href="#_exemple_de_manipulation_de_listes"></a><a class="link" href="#_exemple_de_manipulation_de_listes">1.5.20. Exemple de manipulation de listes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une liste supporte les opérations sur les <a href="https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range">séquences</a></p>
</li>
<li>
<p>Une liste est une instance de la classe <a href="https://docs.python.org/3/library/stdtypes.html#list"><code>list</code></a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">squares = [1, 4, 9, 16, 25]
squares = [x**2 for x in range(10)] # liste en compréhension
del squares[0] # supprime le premier élément
cubes = [1, 8, 27, 65, 125]
cubes[3] = 64 # modifiable
del cubes # supprime la variable</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_manipulation_densembles"><a class="anchor" href="#_exemple_de_manipulation_densembles"></a><a class="link" href="#_exemple_de_manipulation_densembles">1.5.21. Exemple de manipulation d&#8217;ensembles</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un ensemble est une instance de la classe <a href="https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset"><code>set</code></a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">basket = set() # ensemble vide
basket = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'}
'orange' in basket # test d'appartenance
a = set('abracadabra') # les doublons sont éliminés
b = set('alacazam')
a - b # différence
a | b # union
a &amp; b # intersection
a ^ b # a union b privé de a inter b
a = {x for x in 'abracadabra' if x not in 'abc'} # ensemble en compréhension</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_manipulation_de_dictionnaires"><a class="anchor" href="#_exemple_de_manipulation_de_dictionnaires"></a><a class="link" href="#_exemple_de_manipulation_de_dictionnaires">1.5.22. Exemple de manipulation de dictionnaires</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un dictionnaire est une instance de la classe <a href="https://docs.python.org/3/library/stdtypes.html#mapping-types-dict"><code>dict</code></a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">tel = {'jack': 4098, 'sape': 4139}
tel['guido'] = 4127
del tel['sape']</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_références"><a class="anchor" href="#_références"></a><a class="link" href="#_références">1.5.23. Références</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="https://www.python.org/">Site officiel</a></p>
<div class="ulist">
<ul>
<li>
<p><a href="https://docs.python.org/3/tutorial/index.html">Tutoriel</a>,
<a href="https://docs.python.org/3/reference/index.html">Référence du langage</a>,
<a href="https://docs.python.org/3/library/index.html">Référence de la bibliothèque standard</a>,
<a href="https://www.python.org/dev/peps/pep-0008/">Guide de style</a>,
<a href="https://www.python.org/dev/peps/pep-0020/">The Zen of Python</a></p>
</li>
</ul>
</div>
</li>
<li>
<p>Page Wikipedia (<a href="https://fr.wikipedia.org/wiki/Python_%28langage%29">fr</a>, <a href="https://en.wikipedia.org/wiki/Python_%28programming_language%29">en</a>)</p>
</li>
<li>
<p><a href="https://perso.limsi.fr/pointal/python:courspython3">Une introduction à Python 3</a>,
<a href="https://perso.limsi.fr/pointal/python:memento">Mémento Python 3</a>,
<a href="https://perso.limsi.fr/pointal/python:abrege">Abrégé Dense Python 3.2</a>, L. Pointal</p>
</li>
<li>
<p><a href="https://openclassrooms.com/courses/apprenez-a-programmer-en-python">Apprenez à programmer en Python</a>, cours Open Classrooms</p>
</li>
<li>
<p><a href="https://apprendre-python.com/">Apprendre le langage de programmation python</a></p>
</li>
<li>
<p><a href="http://python-guide-pt-br.readthedocs.io/en/latest/">The Hitchhiker’s Guide to Python!</a> (<a href="https://python-guide-fr.readthedocs.io/fr/latest/">fr</a>), Kenneth Reitz (livre)</p>
</li>
<li>
<p><a href="https://dzone.com/refcardz/core-python">Core Python</a>, DZone Refcard</p>
</li>
<li>
<p><a href="https://the-hitchhikers-guide-to-packaging.readthedocs.io/en/latest/index.html">The Hitchhiker’s Guide to Packaging</a></p>
</li>
<li>
<p><a href="http://www.diveintopython3.net/">Dive Into Python 3</a>, Mark Pilgrim (livre)</p>
</li>
<li>
<p><a href="http://inventwithpython.com/">Invent with Python</a>, Albert Sweigart (livres)</p>
</li>
<li>
<p><a href="http://programarcadegames.com/">Program Arcade Games With Python And Pygame</a>
(<a href="http://programarcadegames.com/index.php?lang=fr">fr</a>), Paul Craven (livre)</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_références_poojava"><a class="anchor" href="#_références_poojava"></a><a class="link" href="#_références_poojava">Références (POO/Java)</a></h3>
<div class="ulist bibliography">
<ul class="bibliography">
<li>
<p><a id="BK16"></a>[BK16] <strong>D. Barnes and M. Köllin</strong>. <a href="http://www.bluej.org/objects-first/"><em>Objects First with Java</em></a>.  Pearson. 2016.</p>
</li>
<li>
<p><a id="Bloch08"></a>[Bloch08] <strong>J. Bloch</strong>. <em>Effective Java</em>.  Pearson. 2018.</p>
</li>
<li>
<p><a id="Dar14"></a>[Dar14] <strong>I. Darwin</strong>. <a href="http://shop.oreilly.com/product/0636920026518.do"><em>Java Cookbook</em></a>.  O&#8217;Reilly Media. 2014.</p>
</li>
<li>
<p><a id="HC12"></a>[HC12] <strong>C. S. Horstmann and G. Cornell</strong>. <a href="http://www.horstmann.com/corejava.html"><em>Core Java - Fundamentals</em></a>.  Prentice Hall. 2021.</p>
</li>
<li>
<p><a id="HC13"></a>[HC13] <strong>C. S. Horstmann and G. Cornell</strong>. <a href="http://www.horstmann.com/corejava.html"><em>Core Java - Advanced Features</em></a>.  Prentice Hall. 2022.</p>
</li>
<li>
<p><a id="JavaAPI"></a>[JavaAPI]  <a href="https://docs.oracle.com/en/java/javase/19/docs/api/index.html"><em>The Java API Documentation</em></a>.   2022.</p>
</li>
<li>
<p><a id="JavaDevGuide"></a>[JavaDevGuide]  <a href="https://docs.oracle.com/en/java/javase/19/books.html"><em>Java Platform Standard Edition 19 Documentation</em></a>.   2022.</p>
</li>
<li>
<p><a id="JavaTutorial"></a>[JavaTutorial]  <a href="https://docs.oracle.com/javase/tutorial/index.html"><em>The Java Tutorials</em></a>.   2022.</p>
</li>
</ul>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_python"><a class="anchor" href="#_exercices_python"></a><a class="link" href="#_exercices_python">1.6. Exercices (Python)</a></h3>
<div class="sect3">
<h4 id="_installation_de_lenvironnement"><a class="anchor" href="#_installation_de_lenvironnement"></a><a class="link" href="#_installation_de_lenvironnement">1.6.1. Installation de l&#8217;environnement</a></h4>
<div class="sect4">
<h5 id="_vérification_de_linstallation_python"><a class="anchor" href="#_vérification_de_linstallation_python"></a><a class="link" href="#_vérification_de_linstallation_python">Vérification de l&#8217;installation Python</a></h5>
<div class="ulist">
<ul>
<li>
<p>Sous Linux, il est préférable d&#8217;utiliser le système de paquets de l&#8217;OS</p>
<div class="ulist">
<ul>
<li>
<p><a href="https://packages.debian.org/stretch/python3">python3</a>,
<a href="https://packages.debian.org/stretch/ipython3">ipython3</a>,
<a href="https://packages.debian.org/stretch/python3-pip">python3-pip</a>,
<a href="https://packages.debian.org/stretch/jupyter-notebook">jupyter-notebook</a> sous Debian,</p>
</li>
<li>
<p><a href="http://packages.ubuntu.com/xenial/python3">python3</a>,
<a href="http://packages.ubuntu.com/xenial/python3">ipython3</a>,
<a href="http://packages.ubuntu.com/xenial/python3-pip">python3-pip</a>,
jupyter-notebook (non dispo. sous xenial) sous Ubuntu</p>
</li>
</ul>
</div>
</li>
<li>
<p>Sous Windows, il suffit d&#8217;installer une distribution comme <a href="https://www.continuum.io/anaconda-overview">Anaconda</a></p>
</li>
<li>
<p>Sous Mac OS X, utiliser <a href="https://brew.sh/">Homebrew</a>.
La procédure est détaillée sur la page <a href="http://python-guide-pt-br.readthedocs.io/en/latest/starting/install3/osx/">Installing Python 3 on Mac OS X</a>.
La distribution <a href="https://www.continuum.io/anaconda-overview">Anaconda</a> est également disponible sous Mac OS X.</p>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Vérifiez l&#8217;installation en reproduisant les instructions des sections
<a href="#_lancer_un_interpréteur_interactif">Lancer un interpréteur interactif</a> et
<a href="#_lancer_un_notebook_jupyter">Lancer un notebook Jupyter</a>.</p>
</li>
</ol>
</div>
</li>
</ul>
</div>
</div>
<div class="sect4">
<h5 id="_création_dun_compte_bitbucket"><a class="anchor" href="#_création_dun_compte_bitbucket"></a><a class="link" href="#_création_dun_compte_bitbucket">Création d&#8217;un compte Bitbucket</a></h5>
<div class="paragraph">
<p>Les plateformes <a href="https://bitbucket.org/">Bitbucket</a> (et <a href="https://github.com/">Github</a>) permettent d&#8217;héberger des projets en utilisant un système de gestion de versions (<a href="https://git-scm.com/">git</a>).</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Créez-vous un compte sur <a href="https://bitbucket.org/account/signup/">Bitbucket</a>.</p>
</li>
<li>
<p>Faites un <em>fork</em> du dépôt <a href="https://bitbucket.org/hal_prism/cours.poo.exemples.python.git" class="bare">https://bitbucket.org/hal_prism/cours.poo.exemples.python.git</a> dans votre espace Bitbucket.</p>
</li>
<li>
<p>Cloner localement votre nouveau dépôt.</p>
</li>
</ol>
</div>
</div>
<div class="sect4">
<h5 id="_création_dun_compte_sagemathcloud_optionnel"><a class="anchor" href="#_création_dun_compte_sagemathcloud_optionnel"></a><a class="link" href="#_création_dun_compte_sagemathcloud_optionnel">Création d&#8217;un compte SageMathCloud (optionnel)</a></h5>
<div class="paragraph">
<p>La plateforme <a href="https://cloud.sagemath.com/settings">SageMathCloud</a> offre un ensemble d&#8217;outils pour le calcul scientifique.
Un compte gratuit donne accès à une machine virtuelle sur laquelle sont installés de nombreux logiciels de calcul scientifique ainsi qu&#8217;à une interface graphique dans le navigateur permettant d&#8217;ouvrir un notebook, un terminal&#8230;&#8203;</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Créez-vous un compte sur <a href="https://cloud.sagemath.com/settings">SageMathCloud</a>.</p>
</li>
<li>
<p>Créez un projet.</p>
</li>
<li>
<p>Ajoutez un terminal dans votre projet pour reproduir les instructions des sections
<a href="#_lancer_un_interpréteur_interactif">Lancer un interpréteur interactif</a> et
<a href="#_lancer_un_notebook_jupyter">Lancer un notebook Jupyter</a>.</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_premiers_pas_en_python"><a class="anchor" href="#_premiers_pas_en_python"></a><a class="link" href="#_premiers_pas_en_python">1.6.2. Premiers pas en Python</a></h4>
<div class="paragraph">
<p>Dans cette section, vous utiliserez comme base le répertoire <code>intro</code> des <a href="https://bitbucket.org/hal_prism/cours.poo.exemples.python.git">exemples</a> du cours.
N&#8217;hésitez pas à faire des modifications dans les exemples proposés.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Exécutez le script de la section <a href="#_exemple_de_script_python">Exemple de script Python</a> en suivant les instructions de la section <a href="#_exécuter_un_programme_python">Exécuter un programme Python</a>.</p>
</li>
<li>
<p>Dans un notebook, ouvrez (ou reproduisez) et exécutez le fichier <code>Python RefCard.ipynb</code> qui reprend les exemples du cours.</p>
</li>
<li>
<p>Répondez aux questions suivantes</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Dans la documentation du langage, où se trouve la documentation de la fonction <code>print</code> (pour Python 3.6, pour Python 2.7) ? Même question pour l&#8217;instruction <code>print</code> de Python 2.7.</p>
</li>
<li>
<p>Où se trouve la documentation de l&#8217;instruction <code>assert</code> ?</p>
</li>
<li>
<p>Quelle convention utilise-t-on pour nommer les fonctions en Python ?</p>
</li>
<li>
<p>En dehors de la classe <code>str</code>, quels modules de la bibliothèque standard permettent de manipuler du texte ?</p>
</li>
<li>
<p>Dans l&#8217;index <a href="https://pypi.python.org/pypi">PyPI</a>, combien de bibliothèques sont liées au thème <em>Games/Entertainment</em> pour la version 3.6 de Python ?</p>
</li>
<li>
<p>En Python 3, quelle est la différence entre les opérateurs <code>/</code> et <code>//</code> ?</p>
</li>
<li>
<p>En utilisant les listes en compréhension, générer les tables de multiplication jusqu&#8217;à 10.</p>
</li>
</ol>
</div>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_vue_densemble_des_concepts_objet"><a class="anchor" href="#_vue_densemble_des_concepts_objet"></a><a class="link" href="#_vue_densemble_des_concepts_objet">2. Vue d&#8217;ensemble des concepts objet</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_objet_et_message"><a class="anchor" href="#_objet_et_message"></a><a class="link" href="#_objet_et_message">2.1. Objet et message</a></h3>
<div class="sect3">
<h4 id="_système_orienté_objet"><a class="anchor" href="#_système_orienté_objet"></a><a class="link" href="#_système_orienté_objet">2.1.1. Système orienté objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lors de son exécution, un <em>système OO</em> est <strong>un ensemble d&#8217;objets qui interagissent</strong></p>
</li>
<li>
<p>Les objets forment donc l'<em>aspect dynamique</em> (à l&#8217;exécution) d&#8217;un système OO</p>
</li>
<li>
<p>Ces objets représentent soit</p>
<div class="ulist">
<ul>
<li>
<p>des entités du monde réel (&#8658; ce sont donc des modèles d&#8217;entités réelles), soit</p>
</li>
<li>
<p>des objets "techniques" nécessaires durant l&#8217;exécution du programme.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_objet"><a class="anchor" href="#_objet"></a><a class="link" href="#_objet">2.1.2. Objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>objet</em> est formé de deux composants indissociables</p>
<div class="ulist">
<ul>
<li>
<p>son <em>état</em>, i.e. les valeurs prises par des variables le décrivant (<em>propriétés</em>)</p>
</li>
<li>
<p>son <em>comportement</em>, i.e. les opérations qui lui sont applicables</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un objet est une <em>instance</em> d&#8217;une <em>classe</em></p>
</li>
<li>
<p>Un objet peut avoir plusieurs types, i.e. supporter plusieurs interfaces</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_des_points_et_des_cercles"><a class="anchor" href="#_exemple_des_points_et_des_cercles"></a><a class="link" href="#_exemple_des_points_et_des_cercles">2.1.3. Exemple : des points et des cercles</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/points_and_circles.png" alt="points and circles" width="174" height="176">
</div>
<div class="title">Figure 7. Diagramme d&#8217;objets UML</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Les objets <code>point1</code> et <code>point2</code> sont des points, <code>cercle1</code> est un cercle</p>
</li>
<li>
<p>L&#8217;état de chaque objet est représenté par la valeur de ses propriétés</p>
</li>
<li>
<p>Le centre du cercle est une référence sur un objet point</p>
</li>
<li>
<p>Le comportement n&#8217;est pas représenté au niveau des objets</p>
<div class="ulist">
<ul>
<li>
<p>une opération est invoquée par rapport à un objet</p>
</li>
<li>
<p>mais est rattachée à la classe (le code est partagé par tous les objets d&#8217;une classe)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Les objets <code>point1</code> et <code>point2</code> sont égaux mais pas identiques</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_des_points_et_des_cercles_java"><a class="anchor" href="#_exemple_des_points_et_des_cercles_java"></a><a class="link" href="#_exemple_des_points_et_des_cercles_java">2.1.4. Exemple : des points et des cercles (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Point2D p1 = new Point2D(1.0, 2.0);
Point2D p2 = new Point2D(1.0);
Point2D p3 = new Point2D();
Point2D unAutreP3 = p3;
assert p3 == unAutreP3; // 2 points identiques

Cercle2D c1 = new Cercle2D(p1, 3.0);
Cercle2D c2 = new Cercle2D(new Point2D(2.0, 4.0), 5.0);
Cercle2D c3 = new Cercle2D();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_des_points_et_des_cercles_python"><a class="anchor" href="#_exemple_des_points_et_des_cercles_python"></a><a class="link" href="#_exemple_des_points_et_des_cercles_python">2.1.5. Exemple : des points et des cercles (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">point1 = point2d.Point2D(1.0, 2.0)
point2 = point2d.Point2D(1.0, 2.0)
cercle1 = cercle2d.Cercle2D(point1, 2.0)</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_communication_par_messages"><a class="anchor" href="#_communication_par_messages"></a><a class="link" href="#_communication_par_messages">2.1.6. Communication par messages</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un objet solitaire n&#8217;a que peu d&#8217;intérêt &#8658; différents objets doivent pouvoir interagir</p>
</li>
<li>
<p>Un <em>message</em> est un moyen de communication (d&#8217;interaction) entre objets</p>
</li>
<li>
<p><strong>Les messages sont les seuls moyens d&#8217;interaction entre objets</strong></p>
<div class="ulist">
<ul>
<li>
<p>&#8658; l&#8217;état interne ne doit pas être manipulé directement</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le (ou les) type(s) d&#8217;un objet détermine les messages qu&#8217;il peut recevoir</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_message"><a class="anchor" href="#_message"></a><a class="link" href="#_message">2.1.7. Message</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un message est une requête envoyée à un objet pour demander l&#8217;exécution d&#8217;une opération</p>
</li>
<li>
<p>Un message comporte trois composants:</p>
<div class="ulist">
<ul>
<li>
<p><strong>l&#8217;objet auquel il est envoyé</strong> (le destinataire du message),</p>
</li>
<li>
<p>le nom de l&#8217;opération à invoquer,</p>
</li>
<li>
<p>les paramètres effectifs.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_déplacer_un_cercle"><a class="anchor" href="#_exemple_déplacer_un_cercle"></a><a class="link" href="#_exemple_déplacer_un_cercle">2.1.8. Exemple : déplacer un cercle</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/moving_circle.png" alt="moving circle" width="347" height="309">
</div>
<div class="title">Figure 8. Diagramme de séquence UML</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;utilisateur envoie un message à un objet (à une instance de) cercle</p>
</li>
<li>
<p>Le message se traduit par l&#8217;exécution de l&#8217;opération <code>translate(1.0, 2.0)</code> par l&#8217;objet cercle</p>
</li>
<li>
<p>Durant cette exécution, le cercle envoie un message à l&#8217;objet point (translater le cercle revient à translater son centre)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_déplacer_un_cercle_java"><a class="anchor" href="#_exemple_déplacer_un_cercle_java"></a><a class="link" href="#_exemple_déplacer_un_cercle_java">2.1.9. Exemple : déplacer un cercle (Java)</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le message <em>translate</em> est envoyé à <code>cercle1</code> (<code>cercle1.translate(1.0, 2.0)</code>)</p>
<div class="ulist">
<ul>
<li>
<p>lors de cette exécution, le message <em>translate</em> est envoyé au centre du cercle (<code>centre.translate(1.0, 2.0)</code>)</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;opération <code>translate</code> du point est exécutée</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_déplacer_un_cercle_python"><a class="anchor" href="#_exemple_déplacer_un_cercle_python"></a><a class="link" href="#_exemple_déplacer_un_cercle_python">2.1.10. Exemple : déplacer un cercle (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">cercle1.translate(2.0, 3.0)</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le message <em>translate</em> est envoyé à <code>cercle1</code> (<code>cercle1.translate(1.0, 2.0)</code>)</p>
<div class="ulist">
<ul>
<li>
<p>lors de cette exécution , le message <em>translate</em> est envoyé au centre du cercle (<code>self.centre.translate(1.0, 2.0)</code>)</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;opération <code>translate</code> du point est exécutée</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_type_et_classe"><a class="anchor" href="#_type_et_classe"></a><a class="link" href="#_type_et_classe">2.2. Type et classe</a></h3>
<div class="sect3">
<h4 id="_type"><a class="anchor" href="#_type"></a><a class="link" href="#_type">2.2.1. Type</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>type</em> est un modèle abstrait réunissant à un haut degré les traits essentiels de tous les êtres ou de tous les objets de même nature</p>
</li>
<li>
<p>En informatique, un <em>type (de donnée)</em> spécifie:</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;ensemble des valeurs possibles pour cette donnée (définition en <em>extension</em>),</p>
</li>
<li>
<p>l&#8217;ensemble des opérations applicables à cette donnée (définition en <em>intention</em>).</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un type spécifie l'<em>interface</em> par laquelle une donnée peut être manipulée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_un_type_déplaçable"><a class="anchor" href="#_exemple_un_type_déplaçable"></a><a class="link" href="#_exemple_un_type_déplaçable">2.2.2. Exemple : un type Déplaçable</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/deplacable.png" alt="deplacable" width="196" height="77">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_un_type_déplaçable_java"><a class="anchor" href="#_exemple_un_type_déplaçable_java"></a><a class="link" href="#_exemple_un_type_déplaçable_java">2.2.3. Exemple : un type Déplaçable (Java)</a></h4>
<div class="ulist">
<ul>
<li>
<p>En Java, un type peut être représenté par une interface.</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.coo;

public interface Deplacable {
    /**
     * Translate l'objet.
     *
     * @param dx deplacement en abscisse
     * @param dy deplacement en ordonnées
     */
    void translate(double dx, double dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_type_python"><a class="anchor" href="#_type_python"></a><a class="link" href="#_type_python">2.2.4. Type (Python)</a></h4>
<div class="ulist">
<ul>
<li>
<p>En Python, tout objet acceptant les messages déclarés dans un type est de ce type</p>
</li>
<li>
<p>Cette propriété se nomme <em>duck typing</em></p>
</li>
<li>
<p>Elle est commune à plusieurs langages à typage dynamique</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_classe_i"><a class="anchor" href="#_classe_i"></a><a class="link" href="#_classe_i">2.2.5. Classe I</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>classe</em> est un "modèle" (un "moule") pour une catégorie d&#8217;objets structurellement identiques</p>
</li>
<li>
<p>Une classe définit donc l&#8217;implémentation d&#8217;un objet (son état interne et le codage de ses opérations)</p>
</li>
<li>
<p>L&#8217;ensemble des classes décrit l'<em>aspect statique</em> d&#8217;un système OO</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_classe_ii"><a class="anchor" href="#_classe_ii"></a><a class="link" href="#_classe_ii">2.2.6. Classe II</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe comporte:</p>
<div class="ulist">
<ul>
<li>
<p>la définition des <em>attributs</em> (ou <em>variables d&#8217;instance</em>),</p>
</li>
<li>
<p>la <em>signature</em> des opérations (ou <em>méthodes</em>),</p>
</li>
<li>
<p>la <em>réalisation</em> (ou <em>définition</em>) des méthodes.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Chaque instance aura sa propre copie des attributs (son état)</p>
</li>
<li>
<p>La signature d&#8217;une opération englobe son nom et le type de ses paramètres</p>
</li>
<li>
<p>L&#8217;ensemble des signatures de méthodes représente l&#8217;interface de la classe (publique)</p>
</li>
<li>
<p>L&#8217;ensemble des définitions d&#8217;attributs et de méthodes forme l&#8217;implémentation de la classe (privé)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_les_classes_cercle2d_et_point2d"><a class="anchor" href="#_exemple_les_classes_cercle2d_et_point2d"></a><a class="link" href="#_exemple_les_classes_cercle2d_et_point2d">2.2.7. Exemple : les classes <code>Cercle2D</code> et <code>Point2D</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/classe_point_cercle.png" alt="classe point cercle" width="195" height="238">
</div>
<div class="title">Figure 9. Diagramme de classes UML</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Un rectangle représente une classe</p>
<div class="ulist">
<ul>
<li>
<p>1er pavé: nom de la classe</p>
</li>
<li>
<p>2ième pavé: attributs</p>
</li>
<li>
<p>3ième pavé: signature des méthodes</p>
</li>
</ul>
</div>
</li>
<li>
<p>en général, les attributs sont privés et les méthodes publiques</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_les_classes_cercle2d_et_point2d_mode_abrégé"><a class="anchor" href="#_exemple_les_classes_cercle2d_et_point2d_mode_abrégé"></a><a class="link" href="#_exemple_les_classes_cercle2d_et_point2d_mode_abrégé">2.2.8. Exemple : les classes <code>Cercle2D</code> et <code>Point2D</code> (mode abrégé)</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/classe_point_cercle_abrev.png" alt="classe point cercle abrev" width="104" height="174">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_cercle2d_java"><a class="anchor" href="#_exemple_la_classe_cercle2d_java"></a><a class="link" href="#_exemple_la_classe_cercle2d_java">2.2.9. Exemple : la classe <code>Cercle2D</code> (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.coo;

public class Cercle2D implements Deplacable {
    /** Le centre du cercle. */
    private Point2D centre;

    /** Le rayon du cercle */
    private double rayon;

    /**
     * Initialise un cercle avec un centre et un rayon.
     * @param centre Le centre
     * @param rayon Le rayon
     */
    public Cercle2D(Point2D centre, double rayon) { /* ... */ }

    /**
     * Initialise un cercle centré à l'origine et de rayon 1.
     */
    public Cercle2D() { /* ... */ }

    public Point2D getCentre() { return centre; }
    public double getRayon() { return rayon; }

    /**
     * Translate le cercle.
     * @param dx déplacement en abscisse.
     * @param dy déplacement en ordonnées.
     */
    public void translate(double dx, double dy) { /* ... */ }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_cercle2d_python"><a class="anchor" href="#_exemple_la_classe_cercle2d_python"></a><a class="link" href="#_exemple_la_classe_cercle2d_python">2.2.10. Exemple : la classe <code>Cercle2D</code> (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">"""Définition de la classe Cercle2D"""
from coo.forme import Forme


class Cercle2D(Forme):
    """Représente un cercle en 2 dimensions"""

    def __init__(self, centre, rayon):
        """Initialise un cercle à partir d'un point et d'un rayon"""
        self.centre = centre
        self.rayon = rayon

    def __str__(self):
        return "Cercle2D({}, {})".format(self.centre, self.rayon)

    def translate(self, dx, dy):
        """Déplace le cercle"""
        self.centre.translate(dx, dy)</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_classe_et_type"><a class="anchor" href="#_classe_et_type"></a><a class="link" href="#_classe_et_type">2.2.11. Classe et type</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe implémente un ou plusieurs types, i.e. respecte une ou plusieurs interfaces</p>
</li>
<li>
<p>Un objet peut avoir plusieurs types mais est une instance d&#8217;une seule classe</p>
</li>
<li>
<p>Des objets de classes différentes peuvent avoir le même type</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_cercles_et_points_sont_de_type_déplaçable"><a class="anchor" href="#_exemple_cercles_et_points_sont_de_type_déplaçable"></a><a class="link" href="#_exemple_cercles_et_points_sont_de_type_déplaçable">2.2.12. Exemple : cercles et points sont de type Déplaçable</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/classe_et_type.png" alt="classe et type" width="267" height="359">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_instanciation_dune_classe"><a class="anchor" href="#_instanciation_dune_classe"></a><a class="link" href="#_instanciation_dune_classe">2.2.13. Instanciation d&#8217;une classe</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le mécanisme d'<em>instanciation</em> permet de créer des objets à partir d&#8217;une classe</p>
</li>
<li>
<p>Chaque objet est une instance d&#8217;une classe</p>
</li>
<li>
<p>Lors de l&#8217;instanciation,</p>
<div class="ulist">
<ul>
<li>
<p>de la mémoire est allouée pour l&#8217;objet,</p>
</li>
<li>
<p>l&#8217;objet est initialisé (appel du constructeur) afin de respecter l&#8217;invariant de la classe.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_application_modélisation_dun_robot"><a class="anchor" href="#_application_modélisation_dun_robot"></a><a class="link" href="#_application_modélisation_dun_robot">2.2.14. Application : modélisation d&#8217;un robot</a></h4>
<div class="paragraph">
<p>On veut modéliser des robots se déplaçant sur un terrain.
Ce terrain est découpé en cases carrées repérées par deux coordonnées.
Chaque case peut être vide ou contenir un mur ou un robot.
Les robots sont très rudimentaires et ne disposent que d&#8217;une boussole.
Ils ne connaissent donc que leur orientation (Nord, Est, Sud, Ouest).
Un robot doit pouvoir avancer d&#8217;une case et tourner d&#8217;un quart de tour à droite.
Un robot ne peut se déplacer d&#8217;une case à une autre que si la case de destination est vide.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Représenter en UML la classe <code>Robot</code></p>
</li>
<li>
<p>Faire de même avec la classe <code>Terrain</code></p>
</li>
<li>
<p>Représenter sur un diagramme de séquence les échanges de messages pour le déplacement d&#8217;un robot</p>
</li>
</ol>
</div>
<div class="paragraph">
<p>On suppose maintenant qu&#8217;un robot peut en détecter un autre qui passe devant lui.
Par exemple, quand un robot se déplace, il peut passer dans le champ de vision d&#8217;un autre.
Ce dernier devra alors être averti.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Modifier le diagramme précédent pour y intégrer la détection des déplacements</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_héritage"><a class="anchor" href="#_héritage"></a><a class="link" href="#_héritage">2.3. Héritage</a></h3>
<div class="sect3">
<h4 id="_sous_type"><a class="anchor" href="#_sous_type"></a><a class="link" href="#_sous_type">2.3.1. Sous-type</a></h4>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="paragraph">
<p>Un type T<sub>1</sub> est un <em>sous-type</em> d&#8217;un type T<sub>2</sub> si l&#8217;interface de T<sub>1</sub> contient l&#8217;interface de T<sub>2</sub>.</p>
</div>
<div class="paragraph">
<p>De façon duale, un type T<sub>1</sub> est un <em>sous-type</em> d&#8217;un type T<sub>2</sub> si l&#8217;ensemble des instances de T<sub>2</sub> inclut l&#8217;ensemble des instances de T<sub>1</sub>.</p>
</div>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Un sous-type possède une interface plus riche, i.e. au moins toutes les opérations du super-type</p>
</li>
<li>
<p>De manière équivalente, l&#8217;extension du super-type contient l&#8217;extension du sous-type, i.e. tout objet du sous-type est aussi instance du super-type</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_déplaçable_et_modifiable"><a class="anchor" href="#_exemple_déplaçable_et_modifiable"></a><a class="link" href="#_exemple_déplaçable_et_modifiable">2.3.2. Exemple : Déplaçable et Modifiable</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/deplacable_et_redimensionnable.png" alt="deplacable et redimensionnable" width="205" height="199">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_héritage_2"><a class="anchor" href="#_héritage_2"></a><a class="link" href="#_héritage_2">2.3.3. Héritage</a></h4>
<div class="ulist">
<ul>
<li>
<p>L'<em>héritage</em> permet de définir l&#8217;implémentation d&#8217;une classe à partir de l&#8217;implémentation d&#8217;une autre</p>
</li>
<li>
<p>Ce mécanisme permet, lors de la définition d&#8217;une nouvelle classe, de ne préciser que ce qui change par rapport à une classe existante</p>
</li>
<li>
<p>Une <em>hiérarchie de classes</em> permet de gérer la complexité, en ordonnant les classes au sein d&#8217;arborescences d&#8217;abstraction croissante</p>
</li>
<li>
<p>Si Y hérite de X, on dit que</p>
<div class="ulist">
<ul>
<li>
<p>Y est une classe <em>fille</em> (<em>sous-classe</em>, <em>classe dérivée</em>) et que</p>
</li>
<li>
<p>X est une classe <em>mère</em> (<em>super-classe</em>, <em>classe de base</em>)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_rectangle_et_rectangle_plein"><a class="anchor" href="#_exemple_rectangle_et_rectangle_plein"></a><a class="link" href="#_exemple_rectangle_et_rectangle_plein">2.3.4. Exemple : rectangle et rectangle plein</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/rectangle_et_rectangle_plein.png" alt="rectangle et rectangle plein" width="195" height="237">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_rectangle2dplein_java"><a class="anchor" href="#_exemple_la_classe_rectangle2dplein_java"></a><a class="link" href="#_exemple_la_classe_rectangle2dplein_java">2.3.5. Exemple : la classe Rectangle2DPlein (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un rectangle plein en deux dimensions.
 *
 * @author Stéphane Lopes
 * @version nov. 2008
 */
class Rectangle2DPlein extends Rectangle2D {
    /**
     * La couleur de remplissage
     */
    private Color couleur;

    /**
     * Initialise le rectangle plein.
     *
     * @param supGauche Le coin supérieur gauche.
     * @param infDroit  Le coin inférieur droit.
     * @param couleur   La couleur de remplissage.
     */
    public Rectangle2DPlein(Point2D supGauche,
                            Point2D infDroit,
                            Color couleur) {
        super(supGauche, infDroit);
        assert couleur != null;
        this.couleur = couleur;
    }

    /**
     * Renvoie la couleur.
     *
     * @return la couleur.
     */
    public Color getCouleur() {
        return couleur;
    }</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_classe_rectangle2dplein_java"><a class="anchor" href="#_exemple_utilisation_de_la_classe_rectangle2dplein_java"></a><a class="link" href="#_exemple_utilisation_de_la_classe_rectangle2dplein_java">2.3.6. Exemple : utilisation de la classe Rectangle2DPlein (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Déclaration et création d'un rectangle rouge
Rectangle2DPlein rp = new Rectangle2DPlein(new Point2D(1.0, 2.0),
        new Point2D(3.0, 0.0),
        Color.RED);
assert rp.getCouleur() == Color.RED;

// Déclaration d'un rectangle et
// liaison avec un rectangle plein
Rectangle2D r = new Rectangle2DPlein(new Point2D(1.0, 2.0),
        new Point2D(2.0, 1.0),
        Color.YELLOW);
assert r.getLargeur() == 1;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;affectation d&#8217;une instance de <code>Rectangle2DPlein</code> à une références sur un <code>Rectangle2D</code> est autorisée</p>
</li>
<li>
<p>À partir de <code>r1</code>, l&#8217;accès à <code>getCouleur</code> est impossible (échoue à la compilation) car <code>getCouleur</code> ne fait pas parti de l&#8217;interface de <code>Rectangle2D</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_rectangle2dplein_python"><a class="anchor" href="#_exemple_la_classe_rectangle2dplein_python"></a><a class="link" href="#_exemple_la_classe_rectangle2dplein_python">2.3.7. Exemple : la classe Rectangle2DPlein (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">"""Définition de la classe Rectangle2DPlein"""

from coo.rectangle2d import Rectangle2D


class Rectangle2DPlein(Rectangle2D):
    def __init__(self, orig, tailleX, tailleY, couleur):
        """Initialise un rectangle à partir d'un point, d'une taille et d'une couleur"""
        Rectangle2D.__init__(self, orig, tailleX, tailleY)
        self.couleur = couleur

    def __str__(self):
        return "Rectangle2DPlein({}, {}, {})".format(self.orig, self.fin, self.couleur)

    def colorie(self, couleur):
        """Modifie la couleur du rectangle"""
        self.couleur = couleur</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La super-classe est indiqué entre parenthèse après le nom de la classe</p>
</li>
<li>
<p>Le constructeur de la super-classe est appelé dans le constructeur</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_héritage_et_sous_typage"><a class="anchor" href="#_héritage_et_sous_typage"></a><a class="link" href="#_héritage_et_sous_typage">2.3.8. Héritage et sous-typage</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;héritage (ou <em>héritage d&#8217;implémentation</em>) est un mécanisme technique de réutilisation</p>
</li>
<li>
<p>Le sous-typage (ou <em>héritage d&#8217;interface</em>) décrit comment un objet peut être utilisé à la place d&#8217;un autre</p>
</li>
<li>
<p>Si Y est une sous-type de X, cela signifie que "Y est une sorte de X" (relation <em>IS-A</em>)</p>
</li>
<li>
<p>Dans un langage de programmation, les deux visions peuvent être représentées de la même façon:
le mécanisme d&#8217;héritage permet d&#8217;implémenter l&#8217;un ou l&#8217;autre</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_héritage_dimplémentation_et_dinterface"><a class="anchor" href="#_exemple_héritage_dimplémentation_et_dinterface"></a><a class="link" href="#_exemple_héritage_dimplémentation_et_dinterface">2.3.9. Exemple : héritage d&#8217;implémentation et d&#8217;interface</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/heritage_et_interface.png" alt="heritage et interface" width="420" height="359">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_polymorphisme"><a class="anchor" href="#_polymorphisme"></a><a class="link" href="#_polymorphisme">2.3.10. Polymorphisme</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le <em>polymorphisme</em> est l&#8217;aptitude qu&#8217;ont des objets à réagir différemment à un même message</p>
</li>
<li>
<p>L&#8217;intérêt est de pouvoir gérer une collection d&#8217;objets de façon homogène tout en conservant le comportement propre à chaque type d&#8217;objet</p>
</li>
<li>
<p>Une méthode commune à une hiérarchie de classe peut avoir plusieurs implémentations dans différentes classes</p>
</li>
<li>
<p>Une sous-classe peut <em>redéfinir</em> une méthode de sa super-classe pour spécialiser son comportement</p>
</li>
<li>
<p>Le choix de la méthode à appeler est retardé jusqu&#8217;à l&#8217;exécution du programme (<em>liaison dynamique ou retardée</em>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_description_pour_les_rectangles"><a class="anchor" href="#_exemple_une_description_pour_les_rectangles"></a><a class="link" href="#_exemple_une_description_pour_les_rectangles">2.3.11. Exemple : une description pour les rectangles</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/description_des_rectangles.png" alt="description des rectangles" width="195" height="263">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_description_dans_rectangle2d_java"><a class="anchor" href="#_exemple_la_description_dans_rectangle2d_java"></a><a class="link" href="#_exemple_la_description_dans_rectangle2d_java">2.3.12. Exemple : la description dans Rectangle2D (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Retourne une chaîne représentant l'objet.
 * @return la chaîne.
 */
@Override
public String toString() {
    return String.format("O = %s L = %s, H = %s", orig, getLargeur(), getHauteur());
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_description_dans_rectangle2dplein_java"><a class="anchor" href="#_exemple_la_description_dans_rectangle2dplein_java"></a><a class="link" href="#_exemple_la_description_dans_rectangle2dplein_java">2.3.13. Exemple : la description dans Rectangle2DPlein (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Retourn une chaîne représentant l'objet.
 *
 * @return la chaîne.
 */
@Override
public String toString() {
    return String.format("%s, couleur : %s", super.getDesc(), couleur);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_description_dans_rectangle2d_python"><a class="anchor" href="#_exemple_la_description_dans_rectangle2d_python"></a><a class="link" href="#_exemple_la_description_dans_rectangle2d_python">2.3.14. Exemple : la description dans Rectangle2D (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">"""Définition de la classe Rectangle2D"""

from coo.forme import Forme
from coo.point2d import Point2D

class Rectangle2D(Forme):
    def __init__(self, orig, tailleX, tailleY):
        """Initialise un rectangle à partir d'un point et d'une taille en X et Y"""
        self.orig = orig
        self.fin = Point2D(orig.x + tailleX, orig.y + tailleY)

    def __str__(self):
        return "Rectangle2D({}, {})".format(self.orig, self.fin)

    def translate(self, dx, dy):
        """Déplace le rectangle de dx en abscisse et de dy en ordonnée"""
        self.orig.translate(dx, dy)
        self.fin.translate(dx, dy)</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La méthode <code>str</code> fournit la description</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_description_dans_rectangle2dplein_python"><a class="anchor" href="#_exemple_la_description_dans_rectangle2dplein_python"></a><a class="link" href="#_exemple_la_description_dans_rectangle2dplein_python">2.3.15. Exemple : la description dans Rectangle2DPlein (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">"""Définition de la classe Rectangle2DPlein"""

from coo.rectangle2d import Rectangle2D


class Rectangle2DPlein(Rectangle2D):
    def __init__(self, orig, tailleX, tailleY, couleur):
        """Initialise un rectangle à partir d'un point, d'une taille et d'une couleur"""
        Rectangle2D.__init__(self, orig, tailleX, tailleY)
        self.couleur = couleur

    def __str__(self):
        return "Rectangle2DPlein({}, {}, {})".format(self.orig, self.fin, self.couleur)

    def colorie(self, couleur):
        """Modifie la couleur du rectangle"""
        self.couleur = couleur</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La méthode <code>str</code> est redéfinie dans <code>Rectangle2DPlein</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_classe_abstraite"><a class="anchor" href="#_classe_abstraite"></a><a class="link" href="#_classe_abstraite">2.3.16. Classe abstraite</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>classe abstraite</em> représente un concept abstrait qui ne peux pas être instancié</p>
</li>
<li>
<p>En général, son comportement ne peut pas être intégralement implémenté à cause de son niveau de généralisation</p>
</li>
<li>
<p>Elle sera donc seulement utilisée comme classe de base dans une hiérarchie d&#8217;héritage</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_hiérarchie_dhéritage_des_figures"><a class="anchor" href="#_exemple_la_hiérarchie_dhéritage_des_figures"></a><a class="link" href="#_exemple_la_hiérarchie_dhéritage_des_figures">2.3.17. Exemple : La hiérarchie d&#8217;héritage des figures</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/hierarchie_heritage.png" alt="hierarchie heritage" width="409" height="199">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_classe_abstraite_java"><a class="anchor" href="#_exemple_une_classe_abstraite_java"></a><a class="link" href="#_exemple_une_classe_abstraite_java">2.3.18. Exemple : une classe abstraite (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Une figure fermée.
 *
 * @version  Version1
 * @author   Authonr1
 *
 */
abstract class FigureFermee2D {
    /**
     * Translate la figure.
     * @param dx déplacement en abscisse.
     * @param dy déplacement en ordonnée.
     */
    public abstract void translate(double dx, double dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_redéfinition_dune_méthode_java"><a class="anchor" href="#_exemple_redéfinition_dune_méthode_java"></a><a class="link" href="#_exemple_redéfinition_dune_méthode_java">2.3.19. Exemple : redéfinition d&#8217;une méthode (Java)</a></h4>
<div class="listingblock">
<div class="title">Translation dans la classe <code>Rectangle2D</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Translate le rectangle.
 * @param dx déplacement en abscisse.
 * @param dy déplacement en ordonnées.
 */
@Override
public void translate(double dx, double dy) {
    orig.add(dx, dy);
    fin.add(dx, dy);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Translation dans la classe <code>Cercle2D</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Translate le cercle.
 *
 * @param dx déplacement en abscisse.
 * @param dy déplacement en ordonnées.
 */
@Override
public void translate(double dx, double dy) {
    centre.add(dx, dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_dune_classe_abstraite_java"><a class="anchor" href="#_exemple_utilisation_dune_classe_abstraite_java"></a><a class="link" href="#_exemple_utilisation_dune_classe_abstraite_java">2.3.20. Exemple : utilisation d&#8217;une classe abstraite (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Création du tableau de références
final int NB_FIGURES = 4;
FigureFermee2D[] figures = new FigureFermee2D[NB_FIGURES];

// Création des formes
figures[0] = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));
figures[1] = new Cercle2D(new Point2D(1.0, 2.0), 3.0);
figures[2] = new Rectangle2D(new Point2D(5.0, 5.0),
        new Point2D(7.0, 3.0));
figures[3] = new Cercle2D(new Point2D(4.0, 5.0), 2.0);

// Réalise une translation de la figure
for (int i = 0; i &lt; figures.length; ++i) {
    figures[i].translate(1.0, 2.0);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_abstraite_forme_python"><a class="anchor" href="#_exemple_la_classe_abstraite_forme_python"></a><a class="link" href="#_exemple_la_classe_abstraite_forme_python">2.3.21. Exemple : la classe abstraite Forme (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">"""Classe de base pour les formes"""

from abc import ABC, abstractmethod

class Forme(ABC):
    @abstractmethod
    def translate(self, dx, dy):
        """Déplace la forme d'un décalage en x et en y"""
        pass</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_héritage_multiple_et_à_répétition"><a class="anchor" href="#_héritage_multiple_et_à_répétition"></a><a class="link" href="#_héritage_multiple_et_à_répétition">2.3.22. Héritage multiple et à répétition</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>héritage multiple</em> se produit lorsqu&#8217;une classe possède plusieurs super-classes</p>
</li>
<li>
<p>Un <em>héritage à répétition</em> se produit lorsqu&#8217;une classe hérite plusieurs fois d&#8217;une même super-classe</p>
</li>
<li>
<p>Ces types d&#8217;héritage peuvent provoquer des conflits aux niveaux des attributs et méthodes</p>
<div class="ulist">
<ul>
<li>
<p>deux classes de base peuvent posséder la même méthode,</p>
</li>
<li>
<p>un attribut peut être hérité selon plusieurs chemins dans le graphe d&#8217;héritage.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_hiérarchie_pour_les_véhicules"><a class="anchor" href="#_exemple_une_hiérarchie_pour_les_véhicules"></a><a class="link" href="#_exemple_une_hiérarchie_pour_les_véhicules">2.3.23. Exemple : une hiérarchie pour les véhicules</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/heritage_multiple.png" alt="heritage multiple" width="417" height="321">
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Combien de numéros d&#8217;immatriculation possède la voiture amphibie ?</p>
</li>
<li>
<p>Quelle opération est invoquée quand une voiture amphibie reçoit le message <code>avance</code> ?</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_hiérarchie_de_véhicules_python"><a class="anchor" href="#_exemple_la_hiérarchie_de_véhicules_python"></a><a class="link" href="#_exemple_la_hiérarchie_de_véhicules_python">2.3.24. Exemple : la hiérarchie de véhicules (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">#!/usr/bin/env python3

"""Exemple d'héritage multiple"""

class Vehicule(object):
    def __init__(self, immat):
        self.immat = immat

    def avance(self, distance):
        print("avance dans Vehicule")

class Bateau(Vehicule):
    def __init__(self, immat):
        Vehicule.__init__(self, immat)

    def avance(self, distance):
        print("avance dans Bateau")

class Voiture(Vehicule):
    def __init__(self, immat):
        Vehicule.__init__(self, immat)

    def avance(self, distance):
        print("avance dans Voiture")

class VoitureAmphibie(Bateau, Vehicule):
    pass

if __name__ == '__main__':
    va = VoitureAmphibie("VA123")
    va.avance(12)
    print(va.immat)</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_relations_entre_classes"><a class="anchor" href="#_relations_entre_classes"></a><a class="link" href="#_relations_entre_classes">2.4. Relations entre classes</a></h3>
<div class="sect3">
<h4 id="_types_de_relations_entre_classes"><a class="anchor" href="#_types_de_relations_entre_classes"></a><a class="link" href="#_types_de_relations_entre_classes">2.4.1. Types de relations entre classes</a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1">Dépendance</dt>
<dd>
<div class="ulist">
<ul>
<li>
<p>liaison limitée dans le temps entre objets (non structurelle)</p>
</li>
</ul>
</div>
</dd>
<dt class="hdlist1">Association</dt>
<dd>
<div class="ulist">
<ul>
<li>
<p>relation structurelle</p>
</li>
<li>
<p>cas particuliers : <strong>Agrégation</strong>, <strong>Composition</strong></p>
</li>
</ul>
</div>
</dd>
<dt class="hdlist1">Spécialisation/généralisation</dt>
<dd>
<div class="ulist">
<ul>
<li>
<p>relation d&#8217;héritage ou de sous-typage</p>
</li>
<li>
<p>cas particulier : <strong>Réalisation</strong> (relation entre une classe et un type)</p>
</li>
</ul>
</div>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_relation_de_dépendance"><a class="anchor" href="#_relation_de_dépendance"></a><a class="link" href="#_relation_de_dépendance">2.4.2. Relation de dépendance</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un élément A dépend d&#8217;un élément B si A utilise les services de B, i.e. son interface</p>
</li>
<li>
<p>Un changement dans l&#8217;interface de B peut donc avoir des répercussions sur A</p>
<div class="ulist">
<ul>
<li>
<p>par contre, son implémentation peut être modifiée sans affecter A</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une <em>objet local à une méthode</em> ou <em>un paramètre de méthode</em> sont des exemples de ce type de relation</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_association"><a class="anchor" href="#_association"></a><a class="link" href="#_association">2.4.3. Association</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>association</em> représente une connexion sémantique bidirectionnelle entre une (<em>association réflexive</em>) ou plusieurs classes</p>
<div class="ulist">
<ul>
<li>
<p>les participants de l&#8217;association possèdent des références des uns vers les autres</p>
</li>
<li>
<p>est donc structurelle et permanente</p>
</li>
</ul>
</div>
</li>
<li>
<p>L'<em>arité</em> d&#8217;une association représente le nombre de participants à l&#8217;association (association <em>binaire</em>, <em>ternaire</em>, <em>n-aire</em>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_lassociation_binaire_apparaît_dans"><a class="anchor" href="#_exemple_lassociation_binaire_apparaît_dans"></a><a class="link" href="#_exemple_lassociation_binaire_apparaît_dans">2.4.4. Exemple : l&#8217;association binaire "Apparaît Dans"</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/apparait-dans.png" alt="apparait dans" width="208" height="295">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_apparaît_dans_java"><a class="anchor" href="#_exemple_apparaît_dans_java"></a><a class="link" href="#_exemple_apparaît_dans_java">2.4.5. Exemple : "Apparaît Dans" (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class ApparaitDans {
  private Cercle figure;
  private Dessin dessin;
  private int nbOccurences;

  public ApparaitDans(Cercle figure, Dessin dessin, int nbOccurences) {
    this.figure = figure;
    this.dessin = dessin
    this.nbOccurences = nbOccurences;
  }
  // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_apparaît_dans_python"><a class="anchor" href="#_exemple_apparaît_dans_python"></a><a class="link" href="#_exemple_apparaît_dans_python">2.4.6. Exemple : "Apparaît Dans" (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">class Cercle:
    pass

class Dessin:
    pass

class ApparaitDans:
    def __init__(self, dessin, cercle, position):
        self.dessin = dessin
        self.cercle = cercle
        self.position = position</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_association_ternaire"><a class="anchor" href="#_exemple_une_association_ternaire"></a><a class="link" href="#_exemple_une_association_ternaire">2.4.7. Exemple : une association ternaire</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/assocn.png" alt="assocn">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_association_ternaire_java"><a class="anchor" href="#_exemple_une_association_ternaire_java"></a><a class="link" href="#_exemple_une_association_ternaire_java">2.4.8. Exemple : une association ternaire (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class Cours {
    private Etudiant etudiant;
    private Professeur professeur;
    private Salle salle;
    private int jour;
    private int heure;
    private int duree;
    // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_association_ternaire_python"><a class="anchor" href="#_exemple_une_association_ternaire_python"></a><a class="link" href="#_exemple_une_association_ternaire_python">2.4.9. Exemple : une association ternaire (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">class Cours:
    def __init__(self, etudiant, professeur, salle,
                 jour, heure, durée):
        self.etudiant = etudiant
        self.professeur = professeur
        self.salle = salle
        self.jour = jour
        self.heure = heure
        self.duree = duree</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_agrégation"><a class="anchor" href="#_agrégation"></a><a class="link" href="#_agrégation">2.4.10. Agrégation</a></h4>
<div class="ulist">
<ul>
<li>
<p>L'<em>agrégation</em> est une association non symétrique, qui exprime un couplage fort et une relation de subordination</p>
<div class="ulist">
<ul>
<li>
<p>représente une relation de type "ensemble/élément" (ou tout/partie) entre des classes</p>
</li>
</ul>
</div>
</li>
<li>
<p>La classe représentant l&#8217;ensemble est parfois appelée <em>agrégat</em></p>
</li>
<li>
<p>À un même moment, une instance d&#8217;élément agrégé peut être liée à plusieurs agrégats (l&#8217;élément agrégé peut être partagé)</p>
<div class="ulist">
<ul>
<li>
<p>une instance d&#8217;élément agrégé peut exister sans agrégat (et inversement)</p>
</li>
<li>
<p>les cycles de vies de l&#8217;agrégat et de ses éléments agrégés peuvent être indépendants</p>
</li>
<li>
<p>si on détruit une agrégation, on ne détruit pas automatiquement ses composants</p>
</li>
<li>
<p>agrégation par "référence"</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;agrégat est en général responsable de la création/suppression du composant</p>
<div class="ulist">
<ul>
<li>
<p>&#8658; doit savoir comment créer le composant</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_agrégation_entre_figure_et_cercle"><a class="anchor" href="#_exemple_agrégation_entre_figure_et_cercle"></a><a class="link" href="#_exemple_agrégation_entre_figure_et_cercle">2.4.11. Exemple : agrégation entre Figure et Cercle</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/figure_et_cercle.png" alt="figure et cercle" width="126" height="174">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_figure_et_cercle_java"><a class="anchor" href="#_exemple_figure_et_cercle_java"></a><a class="link" href="#_exemple_figure_et_cercle_java">2.4.12. Exemple : Figure et Cercle (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class Figure {
  /** L'ensemble de cercles composants la figure. */
  private List&lt;Cercle&gt; elements;
  // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_figure_et_cercle_python"><a class="anchor" href="#_exemple_figure_et_cercle_python"></a><a class="link" href="#_exemple_figure_et_cercle_python">2.4.13. Exemple : Figure et Cercle (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">class Figure:
    def __init__(self, listeDeCercles):
        self.listeDeCercles = copy.copy(listeDeCercles)</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_composition"><a class="anchor" href="#_composition"></a><a class="link" href="#_composition">2.4.14. Composition</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>composition</em> est une agrégation forte (agrégation par valeur)</p>
</li>
<li>
<p>À un même moment, une instance de composant ne peut être liée qu&#8217;à un seul agrégat</p>
<div class="ulist">
<ul>
<li>
<p>les cycles de vies des éléments (les "composants") et de l&#8217;agrégat sont liés</p>
</li>
<li>
<p>si l&#8217;agrégat est détruit (ou copié), ses composants le sont aussi</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
Le choix de modélisation entre agrégation et composition est souvent subjectif
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_le_centre_dun_cercle"><a class="anchor" href="#_exemple_le_centre_dun_cercle"></a><a class="link" href="#_exemple_le_centre_dun_cercle">2.4.15. Exemple : le centre d&#8217;un Cercle</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/cercle_et_centre.png" alt="cercle et centre" width="107" height="174">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_le_centre_dun_cercle_java"><a class="anchor" href="#_exemple_le_centre_dun_cercle_java"></a><a class="link" href="#_exemple_le_centre_dun_cercle_java">2.4.16. Exemple : le centre d&#8217;un Cercle (Java)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class Cercle {
  /** Le centre du cercle. */
  private Point centre;

  public Cercle(final Point centre, final double rayon) {
    this.centre = centre.clone();
    // ...
  }
  // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_le_centre_dun_cercle_python"><a class="anchor" href="#_exemple_le_centre_dun_cercle_python"></a><a class="link" href="#_exemple_le_centre_dun_cercle_python">2.4.17. Exemple : le centre d&#8217;un Cercle (Python)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="python" class="language-python hljs">class Cercle:
    def __init__(self, centre, rayon):
        self.centre = copy.deepcopy(centre)
        self.rayon = rayon</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_spécialisationgénéralisation"><a class="anchor" href="#_spécialisationgénéralisation"></a><a class="link" href="#_spécialisationgénéralisation">2.4.18. Spécialisation/Généralisation</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe fille hérite de l&#8217;ensemble des caractéristiques des super-classes</p>
<div class="ulist">
<ul>
<li>
<p>tout changement dans la classe mère peut entraîner des changements dans la classe fille</p>
</li>
</ul>
</div>
</li>
<li>
<p>Hériter d&#8217;un type limite l&#8217;impact des changements</p>
<div class="ulist">
<ul>
<li>
<p>seule l&#8217;interface est réutilisée</p>
</li>
</ul>
</div>
</li>
<li>
<p>Contrôler la visibilité des membres d&#8217;une classe permet également de limiter l&#8217;impact des changements</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_relations_et_dépendances"><a class="anchor" href="#_relations_et_dépendances"></a><a class="link" href="#_relations_et_dépendances">2.4.19. Relations et dépendances</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les relations entre classes peuvent être ordonnées par rapport aux dépendances qu&#8217;elles génèrent</p>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/types_dependencies.png" alt="types dependencies">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="http://rcardin.github.io/programming/oop/software-engineering/2017/04/10/dependency-dot.html">Dependency</a> (blog)</p>
</div>
</div>
<div class="sect3">
<h4 id="_dépendances_et_changements"><a class="anchor" href="#_dépendances_et_changements"></a><a class="link" href="#_dépendances_et_changements">2.4.20. Dépendances et changements</a></h4>
<div class="ulist">
<ul>
<li>
<p>Quand une dépendance existe entre deux éléments, un changement de l&#8217;un affecte le second</p>
</li>
<li>
<p>Le <em>couplage</em> est une mesure de la probabilité qu&#8217;un changement d&#8217;un élément entraîne une modification de l&#8217;autre</p>
</li>
<li>
<p>En développement logiciel, les dépendances entre élément doivent être minimisées</p>
<div class="ulist">
<ul>
<li>
<p>pour construire des composantes <em>faiblement couplés</em></p>
</li>
<li>
<p>le changement d&#8217;un composant aura moins d&#8217;impact sur le reste du code</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_module"><a class="anchor" href="#_module"></a><a class="link" href="#_module">2.5. Module</a></h3>
<div class="sect3">
<h4 id="_module_2"><a class="anchor" href="#_module_2"></a><a class="link" href="#_module_2">2.5.1. Module</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>module</em> (ou <em>package)</em> est l&#8217;unité de base de décomposition d&#8217;un système</p>
</li>
<li>
<p>Il permet d&#8217;organiser logiquement des modèles</p>
</li>
<li>
<p>Un module s&#8217;appuie sur la notion d'<em>encapsulation</em></p>
<div class="ulist">
<ul>
<li>
<p>publie une interface, i.e. ce qui est accessible de l&#8217;extérieur</p>
</li>
<li>
<p>utilise le principe de <em>masquage de l&#8217;information</em>, i.e. ce qui ne fait pas parti de l&#8217;interface est dissimulé</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utilité_dun_module"><a class="anchor" href="#_utilité_dun_module"></a><a class="link" href="#_utilité_dun_module">2.5.2. Utilité d&#8217;un module</a></h4>
<div class="ulist">
<ul>
<li>
<p>Sert de brique de base pour la construction d&#8217;une architecture</p>
</li>
<li>
<p>Représente le bon niveau de granularité pour la réutilisation</p>
</li>
<li>
<p>Est un <em>espace de noms</em> qui permet de gérer les conflits</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_qualité_dun_module"><a class="anchor" href="#_qualité_dun_module"></a><a class="link" href="#_qualité_dun_module">2.5.3. Qualité d&#8217;un module</a></h4>
<div class="ulist">
<ul>
<li>
<p>La conception d&#8217;un module devrait conduire à un <em>couplage faible</em> et une <em>forte cohésion</em></p>
<div class="dlist">
<dl>
<dt class="hdlist1">couplage</dt>
<dd>
<p>désigne l&#8217;importance des liaisons entre les éléments &#8658; <strong>doit être réduit</strong></p>
</dd>
<dt class="hdlist1">cohésion</dt>
<dd>
<p>mesure le recouvrement entre un élément de conception et la tâche logique à accomplir &#8658; <strong>doit être élevé</strong>, i.e. chaque élément est responsable d&#8217;une tâche précise</p>
</dd>
</dl>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_architecture_multi_couches"><a class="anchor" href="#_exemple_une_architecture_multi_couches"></a><a class="link" href="#_exemple_une_architecture_multi_couches">2.5.4. Exemple : une architecture multi-couches</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/package-diagram.png" alt="package diagram" width="821" height="487">
</div>
<div class="title">Figure 10. Diagramme de packages UML</div>
</div>
</div>
<div class="sect3">
<h4 id="_package_java"><a class="anchor" href="#_package_java"></a><a class="link" href="#_package_java">2.5.5. Package (Java)</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le concept de module est implémenté par les <em>packages</em></p>
</li>
<li>
<p>Le mot clé <code>package</code> placé en début de fichier permet l&#8217;ajout d&#8217;éléments dans un module</p>
</li>
<li>
<p>Le mot clé <code>import</code> permet l&#8217;accès aux éléments d&#8217;un module</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_module_python"><a class="anchor" href="#_module_python"></a><a class="link" href="#_module_python">2.5.6. Module (Python)</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>module</em> est un fichier source contenant des définitions et des instructions Python</p>
<div class="ulist">
<ul>
<li>
<p>le fichier source doit être nommé comme le module et avec l&#8217;extension <code>.py</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>À l&#8217;intérieur d&#8217;un module, son nom est accessible par la variable globale <code><em>name</em></code></p>
<div class="ulist">
<ul>
<li>
<p>un module exécuté comme un script possède le nom <code><em>main</em></code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Un module peut ensuite être <em>importé</em> dans un autre</p>
</li>
<li>
<p>Les modules sont recherchés par l&#8217;interpréteur dans les répertoires de la variable <code>sys.path</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_package_python"><a class="anchor" href="#_package_python"></a><a class="link" href="#_package_python">2.5.7. Package (Python)</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>package</em> regroupe et structure un ensemble de modules</p>
</li>
<li>
<p>Chaque répertoire d&#8217;un package doit contenir un fichier <code><em>init</em>.py</code> (même vide)</p>
</li>
<li>
<p>Un module d&#8217;un package est référencé en séparant par un <code>.</code> les noms des éléments</p>
<div class="ulist">
<ul>
<li>
<p>par exemple, <code>sound.effects.echo</code> fait référence au module <code>echo</code> du sous-package <code>effects</code> du package <code>echo</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_python_2"><a class="anchor" href="#_exercices_python_2"></a><a class="link" href="#_exercices_python_2">2.6. Exercices (Python)</a></h3>
<div class="paragraph">
<p>Dans cette section, la bibliothèque <a href="https://www.pygame.org/"><code>pygame</code></a> est utilisée pour l&#8217;affichage graphique (<a href="https://www.pygame.org/docs/">documentation</a> de l&#8217;API).</p>
</div>
<div class="sect3">
<h4 id="_une_application_graphique_simple"><a class="anchor" href="#_une_application_graphique_simple"></a><a class="link" href="#_une_application_graphique_simple">2.6.1. Une application graphique simple</a></h4>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Créez un script <code>simple_app.py</code> dans le répertoire <code>gui</code>.</p>
</li>
<li>
<p>Importez la classe <code>PygameApplication</code> du module <code>pgutil.pygame_application</code>.</p>
</li>
<li>
<p>Créez une instance de la classe <code>PygameApplication</code></p>
</li>
<li>
<p>Explorez le contenu de la classe</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>quelles sont les grandes étapes de l&#8217;éxécution ?</p>
</li>
<li>
<p>quel attribut encapsule la logique de l&#8217;affichage ?</p>
</li>
</ol>
</div>
</li>
<li>
<p>Définissez une sous-classe de <code>PygameScene</code>.</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>quelles méthodes propose cette class ?</p>
</li>
<li>
<p>quand sont-elles invoquées ?</p>
</li>
<li>
<p>redéfinissez la méthode <code>draw</code> pour afficher un cercle au centre de la fenêtre.</p>
</li>
</ol>
</div>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_gérer_la_souris"><a class="anchor" href="#_gérer_la_souris"></a><a class="link" href="#_gérer_la_souris">2.6.2. Gérer la souris</a></h4>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Copiez le script précédent sous le nom <code>simple_app_with_mouse.py</code>.</p>
</li>
<li>
<p>Affichez maintenant un nouveau cercle à l&#8217;endroit où l&#8217;utilisateur clique.</p>
</li>
<li>
<p>Même question mais le cercle doit cette fois être déplacé, i.e. un seul cercle est présent à l&#8217;écran.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_échapper_aux_robots"><a class="anchor" href="#_échapper_aux_robots"></a><a class="link" href="#_échapper_aux_robots">2.6.3. Échapper aux robots</a></h4>
<div class="paragraph">
<p>Le but de cet exercice est de développer un jeu simple où un joueur, <em>Tux</em>, doit échapper à des robots.
Ce jeu fait appel à la notion de <a href="https://www.pygame.org/docs/tut/SpriteIntro.html"><code>Sprite</code></a> (<a href="http://programarcadegames.com/index.php?chapter=introduction_to_sprites">tutoriel</a>).</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Selon le même modèle que précédement, créez une application <code>robot_escape.py</code> utilisant une scène <code>robot_escape_scene.py</code>.</p>
</li>
<li>
<p>Définissez la classe <code>RobotSprite</code> comme sous-classe de la classe <code>Sprite</code> de pygame.</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>dans le constructeur, charger l&#8217;image du robot et initialiser le sprite</p>
</li>
<li>
<p>ajouter la méthode <code>update</code> qui permet le déplacement du robot</p>
</li>
<li>
<p>intégrez le robot dans la scène</p>
</li>
<li>
<p>vous pouvez définir plusieurs robots avec des déplacements différents.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Définissez la classe <code>PlayerSprite</code> qui représente le joueur humain. Il doit pouvoir être déplacé à l&#8217;aide des touches fléchées.</p>
</li>
<li>
<p>Ajoutez la détection de collision entre le joueur et le (ou les) robots. Par exemple, suite à une collision, vous pouvez faire redémarrer le jeu dans la situation initiale.</p>
</li>
<li>
<p>Ajoutez un objectif (une zone identifiée sur le plateau) : le joueur gagne s&#8217;il atteint cet objectif</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_java"><a class="anchor" href="#_exercices_java"></a><a class="link" href="#_exercices_java">2.7. Exercices (Java)</a></h3>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>Utilisation de l&#8217;environnement de développement <a href="https://www.bluej.org/">BlueJ</a>.</p>
</li>
<li>
<p>Les seules sources d&#8217;information externes autorisées sont</p>
<div class="ulist">
<ul>
<li>
<p>la référence de l&#8217;<a href="http://docs.oracle.com/javase/8/docs/api/">API Java</a>,</p>
</li>
<li>
<p>le <a href="http://docs.oracle.com/javase/tutorial/">tutoriel</a> Java,</p>
</li>
<li>
<p>la <a href="http://www.bluej.org/doc/documentation.html">documentation</a> de <a href="https://www.bluej.org/">BlueJ</a>.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Exécution interactive uniquement avec <a href="https://www.bluej.org/">BlueJ</a> (pas de méthode <code>main</code> ni d&#8217;affichage).</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="sect3">
<h4 id="_découverte_de_bluej"><a class="anchor" href="#_découverte_de_bluej"></a><a class="link" href="#_découverte_de_bluej">2.7.1. Découverte de BlueJ</a></h4>
<div class="paragraph">
<p>Dans cette exercice, vous apprendrez les manipulations de base de l&#8217;environnement <a href="https://www.bluej.org/">BlueJ</a>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Ouvrez le projet d&#8217;exemple <code>people2</code> (<em>Projects/Open Projet&#8230;&#8203;</em>).
Les projets d&#8217;exemples se trouvent dans le répertoire d&#8217;installation de BlueJ sous Windows ou dans <code>/usr/share/doc/BlueJ</code> sous Linux.</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Quelles classes y-a-t-il dans ce projet ?</p>
</li>
<li>
<p>Quelles relations existe-t-il entre ces classes ?</p>
</li>
</ol>
</div>
</li>
<li>
<p>Compilez le projet (Bouton <em>Compile</em>)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Quels logiciels faut-il pour compiler un projet en Java ? pour l&#8217;exécuter ?</p>
</li>
</ol>
</div>
</li>
<li>
<p>Création d&#8217;objet (<em>menu contextuel d&#8217;une classe</em>)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Quels constructeurs sont disponibles pour chaque classe ?</p>
</li>
<li>
<p>Pourquoi la classe <code>Person</code> n&#8217;en a-t-elle aucun ?</p>
</li>
<li>
<p>Créez un employé (<em>Staff</em>) <em>p1</em> ayant pour nom <em>Smith</em>, pour année de naissance <em>1980</em> et pour numéro de bureau <em>D100</em>.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Invocation de méthode (<em>menu contextuel d&#8217;un objet</em>)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Quelles méthodes propose <em>p1</em> ?</p>
</li>
<li>
<p>Exécutez les méthodes <code>getRoom()</code> et <code>getName</code>. Dans quelles classes sont-elles définies ?</p>
</li>
<li>
<p>Exécutez la méthode <code>setAddress</code> .</p>
</li>
</ol>
</div>
</li>
<li>
<p>Évaluation à la volée de code Java (<em>View/Show Code Pad</em>).
Les manipulations ci-dessous sont à réaliser dans le Code Pad.</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Créez un étudiant en précisant son nom, son année de naissance et son identifiant.</p>
</li>
<li>
<p>Copiez-le (<em>glisser-déposer</em>) dans la fenêtre des objets.</p>
</li>
<li>
<p>Exécutez la méthode <code>getName</code> dans le <em>Code Pad</em>.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Inspection d&#8217;un objet (<em>menu contextuel d&#8217;un objet</em>)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Inspectez l&#8217;objet <em>p1</em> ?</p>
</li>
<li>
<p>De quels attributs son état est-il formé ?</p>
</li>
<li>
<p>Pouvez-vous inspecter tous ses attributs ? Pourquoi ?</p>
</li>
</ol>
</div>
</li>
<li>
<p>Éditez le code Java de la classe <code>Staff</code> (<em>double-click sur la classe</em>)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Quels éléments du langage trouve-t-on dans cette classe ?</p>
</li>
<li>
<p>À quoi correspondent les couleurs de fond ?</p>
</li>
<li>
<p>Visualisez la documentation de la classe (<em>liste déroulante en haut à droite</em>).</p>
</li>
<li>
<p>Quelle relation y-a-t-il entre la documentation et le code source ? Modifiez un commentaire dans le code et visualisez à nouveau la documentation ?</p>
</li>
<li>
<p>Quel parallèle peut-on établir avec les fichiers <code>.h</code> et <code>.c</code> du langage C ?</p>
</li>
</ol>
</div>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_manipulation_dobjets"><a class="anchor" href="#_manipulation_dobjets"></a><a class="link" href="#_manipulation_dobjets">2.7.2. Manipulation d&#8217;objets</a></h4>
<div class="paragraph">
<p>Dans cette exercice, vous effectuerez les manipulations tout d&#8217;abord de façon interactive, puis en tapant les instructions dans le <em>Code Pad</em>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Ouvrez le projet d&#8217;exemple <a href="https://www.bluej.org/">BlueJ</a> <em>shapes</em> et compiler-le.</p>
</li>
<li>
<p>Réalisez les manipulations suivantes</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>Créez un cercle et rendez-le visible.</p>
</li>
<li>
<p>Déplacez-le horizontalement de 100 unités.</p>
</li>
<li>
<p>Changez sa couleur en rouge.</p>
</li>
<li>
<p>Déplacez-le verticalement de 50 unités.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Représentez la scène suivante :</p>
<div class="ulist">
<ul>
<li>
<p>une maison (carré bleu et triangle rouge),</p>
</li>
<li>
<p>un soleil jaune au-dessus et à droite de la maison.</p>
</li>
</ul>
</div>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_modification_dune_classe"><a class="anchor" href="#_modification_dune_classe"></a><a class="link" href="#_modification_dune_classe">2.7.3. Modification d&#8217;une classe</a></h4>
<div class="paragraph">
<p>Cet exercice utilise le <a href="http://e-campus2.uvsq.fr/Members/steplope/Fichiers/entreprise-bluej.zip/at_download/file">projet <code>Entreprise</code></a> (cf. figure <a href="#entreprise">ci-dessous</a>) à ouvrir sous <a href="https://www.bluej.org/">BlueJ</a> (<em>Project/Open Non Bluej&#8230;&#8203;</em>).</p>
</div>
<div id="entreprise" class="imageblock">
<div class="content">
<img src="figs/entreprise.png" alt="entreprise" width="575" height="117">
</div>
<div class="title">Figure 11. Diagramme de classe du projet <code>Entreprise</code></div>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Modifiez la classe <code>Employe</code> comme suit:</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>ajoutez l&#8217;attribut privé <code>age</code>,</p>
</li>
<li>
<p>modifiez les méthodes pour prendre en compte ce changement,</p>
</li>
<li>
<p>recompilez et testez ce changement.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Mettez à jour les commentaires Javadoc et vérifier la documentation de la classe.</p>
</li>
<li>
<p>Ajoutez la méthode <code>toString</code> à la classe <code>Entreprise</code> : cette méthode retourne une chaîne de caractères contenant le nom de l&#8217;entreprise et la liste de ses employés (prénom, nom et âge),</p>
</li>
<li>
<p>recompiler les deux classes et tester les nouvelles méthodes.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dun_débogueur"><a class="anchor" href="#_utilisation_dun_débogueur"></a><a class="link" href="#_utilisation_dun_débogueur">2.7.4. Utilisation d&#8217;un débogueur</a></h4>
<div class="paragraph">
<p>Cet exercice utilise le même projet que l&#8217;exercice précédent.
Pour chaque test, vous créerez une entreprise et deux employés que l&#8217;entreprise embauchera puis vous invoquerez <code>toString</code> sur l&#8217;entreprise.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Faites afficher le débogueur intégré à <a href="https://www.bluej.org/">BlueJ</a> (<em>View/Show Debugger</em>).
Quels éléments sont visibles dans le débogueur ?
Quelles actions peut-on effectuer à partir du débogueur ?</p>
</li>
<li>
<p>Lancer un premier test et vérifier le comportement du programme.</p>
</li>
<li>
<p>Lancer un second test en saisissant la valeur <code>null</code> lors de l&#8217;embauche du deuxième employé</p>
<div class="ulist">
<ul>
<li>
<p>Que se passe-t-il ?</p>
</li>
<li>
<p>Quelle instruction pose problème ?</p>
</li>
</ul>
</div>
</li>
<li>
<p>Placer un point d&#8217;arrêt (<em>breakpoint</em>) au début de la méthode <code>toString</code> de <code>Entreprise</code> (<em>click dans la marge de l&#8217;éditeur</em>).</p>
</li>
<li>
<p>Reproduisez le second test:</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>l&#8217;exécution doit s&#8217;arrêter au niveau du <em>breakpoint</em>,</p>
</li>
<li>
<p>faites exécuter la méthode pas à pas en consultant la valeur des variables,</p>
</li>
<li>
<p>quelle différence existe-t-il entre les commandes <em>Step</em> et <em>Step Into</em> du débogueur ?</p>
</li>
<li>
<p>pour quel employé le problème se pose-t-il ?</p>
</li>
<li>
<p>quelle est donc finalement la cause de l&#8217;erreur ?</p>
</li>
</ol>
</div>
</li>
<li>
<p>Modifiez la classe <code>Entreprise</code> pour éviter le problème.</p>
</li>
<li>
<p>Vérifiez en reproduisant à nouveau le second test.</p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_objets_et_classes"><a class="anchor" href="#_objets_et_classes"></a><a class="link" href="#_objets_et_classes">3. Objets et classes</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_caractéristiques_dun_objet"><a class="anchor" href="#_caractéristiques_dun_objet"></a><a class="link" href="#_caractéristiques_dun_objet">3.1. Caractéristiques d&#8217;un objet</a></h3>
<div class="sect3">
<h4 id="_état_dun_objet"><a class="anchor" href="#_état_dun_objet"></a><a class="link" href="#_état_dun_objet">3.1.1. État d&#8217;un objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;état d&#8217;un objet est l&#8217;ensemble de ses caractéristiques <strong>internes</strong>, <strong>cachées</strong> aux autres objets</p>
</li>
<li>
<p>Les propriétés représentant l&#8217;état d&#8217;un objet particulier sont appelées <em>variables d&#8217;instance</em> ou <em>attributs</em> ou <em>données membres</em></p>
</li>
<li>
<p>Chaque objet possède un état courant décrit par la valeur de ses attributs et donc sa propre copie des variables d&#8217;instance</p>
</li>
<li>
<p>Les attributs conservent leurs valeurs durant toute la durée de vie d&#8217;un objet</p>
</li>
<li>
<p>Les attributs peuvent être des objets</p>
<div class="ulist">
<ul>
<li>
<p>un objet peut donc être la racine d&#8217;une arborescence d&#8217;autres objets</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_comportement_dun_objet"><a class="anchor" href="#_comportement_dun_objet"></a><a class="link" href="#_comportement_dun_objet">3.1.2. Comportement d&#8217;un objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le comportement d&#8217;un objet regroupe les caractéristiques <strong>externes</strong> mises à la disposition des autres objets</p>
</li>
<li>
<p>Chaque opération est décrite par sa <em>signature</em> (son nom, les objets qu&#8217;elle prend comme paramètre et le type de retour)</p>
</li>
<li>
<p>L&#8217;ensemble de ces opérations forme l'<em>interface</em> de l&#8217;objet</p>
</li>
<li>
<p>Les opérations propres à un objet sont appelées <em>méthodes d&#8217;instance</em> ou <em>fonctions membres</em> (fonctions associées à l&#8217;objet)</p>
</li>
<li>
<p><strong>Ces opérations sont invoquées par rapport à un objet particulier</strong></p>
<div class="ulist">
<ul>
<li>
<p>une méthode sait quel objet l&#8217;a invoquée</p>
</li>
<li>
<p>donc, une méthode a accès aux attributs de l&#8217;objet qui l&#8217;a invoquée</p>
</li>
<li>
<p>comme une fonction avec un paramètre caché vers l&#8217;objet lui-même</p>
</li>
</ul>
</div>
</li>
<li>
<p><strong>Les opérations sont les seules moyens de manipuler l&#8217;état interne d&#8217;un objet (<em>encapsulation</em>)</strong></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_création_dobjets"><a class="anchor" href="#_création_dobjets"></a><a class="link" href="#_création_dobjets">3.1.3. Création d&#8217;objets</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un objet est créé (instancié) à partir d&#8217;une classe</p>
<div class="ulist">
<ul>
<li>
<p>certains (rares) langages créent de nouveaux objets par clonage d&#8217;un objet (<em>prototype</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>La création provoque la réservation de mémoire pour l&#8217;objet et l&#8217;invocation du constructeur qui initialise l&#8217;objet</p>
<div class="ulist">
<ul>
<li>
<p>le constructeur est une méthode invoquée automatiquement lors de la création de l&#8217;objet</p>
</li>
<li>
<p>son rôle est d&#8217;initialiser l&#8217;objet pour que ce dernier respecte l&#8217;invariant de la classe</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;opération de création retourne une <em>référence</em> sur l&#8217;objet</p>
</li>
<li>
<p>Cette référence doit être liée (affectée) à un identificateur (variable) pour permettre l&#8217;accès à l&#8217;objet</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_identité_et_égalité"><a class="anchor" href="#_identité_et_égalité"></a><a class="link" href="#_identité_et_égalité">3.1.4. Identité et égalité</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un objet possède une <em>identité</em> (identifiant interne) qui caractérise son existence de façon indépendante de son état</p>
<div class="ulist">
<ul>
<li>
<p>tester l&#8217;identité de deux objets compare leurs identités</p>
</li>
</ul>
</div>
</li>
<li>
<p>Deux objets sont égaux si leurs états sont les mêmes</p>
<div class="ulist">
<ul>
<li>
<p>tester l&#8217;égalité de deux objets compare leurs attributs</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="paragraph">
<p><strong>égalité &ne; identité</strong></p>
</div>
<div class="ulist">
<ul>
<li>
<p>deux objets peuvent être égaux (même état interne) sans être identiques (même objet)</p>
</li>
<li>
<p>deux objets identiques sont forcément égaux</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_des_points_et_des_cercles"><a class="anchor" href="#_des_points_et_des_cercles"></a><a class="link" href="#_des_points_et_des_cercles">3.1.5. Des points et des cercles</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/objets.png" alt="objets">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_affectation_et_copie_dobjets"><a class="anchor" href="#_affectation_et_copie_dobjets"></a><a class="link" href="#_affectation_et_copie_dobjets">3.1.6. Affectation et copie d&#8217;objets</a></h4>
<div class="ulist">
<ul>
<li>
<p>L'<em>affectation</em> d&#8217;un objet à une variable crée un <em>lien</em> entre la variable et l&#8217;objet</p>
</li>
<li>
<p>Créer une <em>copie</em> d&#8217;un objet nécessite de créer récursivement une copie de ses attributs (<em>copie profonde</em> ou <em>deep copy</em>)</p>
</li>
<li>
<p>Une autre sémantique possible est de ne copier que l&#8217;objet racine et de partager ses attributs (<em>copie superficielle</em> ou <em>shallow copy</em>)</p>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>La simple déclaration d&#8217;une variable ne crée pas d&#8217;objet mais uniquement une <strong>référence invalide</strong></p>
</li>
<li>
<p>La déclaration crée un identificateur qui sera lié à l&#8217;objet en utilisant une affectation</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_les_objets_en_java"><a class="anchor" href="#_les_objets_en_java"></a><a class="link" href="#_les_objets_en_java">3.2. Les objets en Java</a></h3>
<div class="sect3">
<h4 id="_création_dobjets_2"><a class="anchor" href="#_création_dobjets_2"></a><a class="link" href="#_création_dobjets_2">3.2.1. Création d&#8217;objets</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un objet est créé à partir d&#8217;une classe en utilisant le mot-clé <code>new</code> (<code>new Point2D(1.0, 2.0)</code>)</p>
</li>
<li>
<p>L&#8217;utilisation de <code>new</code> provoque la réservation de mémoire pour l&#8217;objet et l&#8217;invocation du constructeur qui initialise l&#8217;objet</p>
</li>
<li>
<p><code>new</code> retourne une référence sur l&#8217;objet créé</p>
</li>
<li>
<p>Cette référence doit être liée à une variable pour permettre l&#8217;accès à l&#8217;objet</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_déclaration_et_affectation"><a class="anchor" href="#_déclaration_et_affectation"></a><a class="link" href="#_déclaration_et_affectation">3.2.2. Déclaration et affectation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La syntaxe pour la déclaration d&#8217;une variable est <code>type nom</code> (<code>Point2D p1</code>)</p>
<div class="ulist">
<ul>
<li>
<p><strong>la déclaration ne crée pas d&#8217;objet</strong> mais uniquement une référence</p>
</li>
<li>
<p>la variable est invalide tant qu&#8217;elle n&#8217;est pas liée à un objet (<em>null reference</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une affectation va lier une variable à un objet <code>variable = objet</code></p>
</li>
<li>
<p>Il est possible de lier la variable lors de sa déclaration (<code>Point2D p1 = new Point2D(1.0, 2.0);</code>)</p>
</li>
<li>
<p>Il est conseillé de toujours initialiser une variable lors de sa déclaration (si possible)</p>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/objets_java.png" alt="objets java">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_instanciation_de_cercle_et_de_points"><a class="anchor" href="#_exemple_instanciation_de_cercle_et_de_points"></a><a class="link" href="#_exemple_instanciation_de_cercle_et_de_points">3.2.3. Exemple : instanciation de cercle et de points</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Point2D p1 = new Point2D(1.0, 2.0);
Point2D p2 = new Point2D(1.0);
Point2D p3 = new Point2D();
Point2D unAutreP3 = p3;
assert p3 == unAutreP3; // 2 points identiques

Cercle2D c1 = new Cercle2D(p1, 3.0);
Cercle2D c2 = new Cercle2D(new Point2D(2.0, 4.0), 5.0);
Cercle2D c3 = new Cercle2D();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_manipulation"><a class="anchor" href="#_manipulation"></a><a class="link" href="#_manipulation">3.2.4. Manipulation</a></h4>
<div class="sect4">
<h5 id="_accès_aux_attributs"><a class="anchor" href="#_accès_aux_attributs"></a><a class="link" href="#_accès_aux_attributs">Accès aux attributs</a></h5>
<div class="ulist">
<ul>
<li>
<p>Juste par le nom de l&#8217;attribut quand on se trouve dans la portée de l&#8217;attribut (exemple: <code>x</code>)</p>
</li>
<li>
<p>En qualifiant/préfixant avec le nom d&#8217;une référence sur l&#8217;objet à l&#8217;extérieur (exemple: <code>p1.x</code>)</p>
</li>
<li>
<p><strong>La manipulation directe d&#8217;attributs en dehors de la classe est interdite</strong> (violation de l&#8217;encapsulation)</p>
</li>
</ul>
</div>
</div>
<div class="sect4">
<h5 id="_invocation_dune_méthode"><a class="anchor" href="#_invocation_dune_méthode"></a><a class="link" href="#_invocation_dune_méthode">Invocation d&#8217;une méthode</a></h5>
<div class="ulist">
<ul>
<li>
<p>Même syntaxe que pour les attributs mais avec la liste des paramètres (exemple: <code>p1.getAbscisse()</code>)</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_destruction"><a class="anchor" href="#_destruction"></a><a class="link" href="#_destruction">3.2.5. Destruction</a></h4>
<div class="ulist">
<ul>
<li>
<p>Quand un objet n&#8217;est plus utilisé, il doit être retiré de la mémoire</p>
</li>
<li>
<p>La destruction des objets en Java est automatique</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;environnement d&#8217;exécution de Java supprime les objets lorsqu&#8217;il détermine qu&#8217;ils ne sont plus utilisés</p>
</li>
<li>
<p>un objet est éligible pour la destruction quand plus aucune référence n&#8217;est liée à lui</p>
</li>
</ul>
</div>
</li>
<li>
<p>Ce processus de suppression s&#8217;appelle <em>ramasse-miette</em> (<em>garbage collector</em>)</p>
</li>
<li>
<p>Avant de détruire l&#8217;objet, le ramasse-miette invoque la méthode <code>protected void finalize()</code> de l&#8217;objet</p>
<div class="ulist">
<ul>
<li>
<p>utilisée pour restituer les ressources allouées par l&#8217;objet</p>
</li>
<li>
<p><code>finalize</code> est membre de la classe <code>Object</code></p>
</li>
<li>
<p><code>super.finalize()</code> doit être d&#8217;appeler à la fin de la méthode</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_les_chaînes_de_caractères_en_java"><a class="anchor" href="#_les_chaînes_de_caractères_en_java"></a><a class="link" href="#_les_chaînes_de_caractères_en_java">3.3. Les chaînes de caractères en Java</a></h3>
<div class="sect3">
<h4 id="_les_chaînes_de_caractères_en_java_2"><a class="anchor" href="#_les_chaînes_de_caractères_en_java_2"></a><a class="link" href="#_les_chaînes_de_caractères_en_java_2">3.3.1. Les chaînes de caractères en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Java fournit trois classes pour les chaînes de caractères: <code>String</code>, <code>StringBuffer</code> et <code>StringBuilder</code></p>
</li>
<li>
<p><code>String</code> est dédiée aux chaînes de caractères immuables, i.e. dont la valeur ne change pas</p>
</li>
<li>
<p><code>StringBuilder</code> est dédiée aux chaînes de caractères pouvant être modifiées (contexte <em>mono-thread</em>)</p>
</li>
<li>
<p><code>StringBuffer</code> est dédiée aux chaînes de caractères pouvant être modifiées (contexte <em>multi-threads</em>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_création_dune_chaîne_string"><a class="anchor" href="#_création_dune_chaîne_string"></a><a class="link" href="#_création_dune_chaîne_string">3.3.2. Création d&#8217;une chaîne (<code>String</code>)</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une instance de <code>String</code> représente une chaîne au format UTF-16</p>
</li>
<li>
<p>Une chaîne est souvent créée à partir d&#8217;un littéral de type chaîne (une suite de caractères entre guillemets)</p>
<div class="ulist">
<ul>
<li>
<p>quand Java rencontre un littéral de type chaîne, il crée un objet de type <code>String</code> dont la valeur est le littéral</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une chaîne peut aussi être créée en utilisant l&#8217;un des constructeurs de <code>String</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_accesseurs_de_string"><a class="anchor" href="#_quelques_accesseurs_de_string"></a><a class="link" href="#_quelques_accesseurs_de_string">3.3.3. Quelques accesseurs de <code>String</code></a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>length()</code></dt>
<dd>
<p>taille de la chaîne,</p>
</dd>
<dt class="hdlist1"><code>charAt(int)</code></dt>
<dd>
<p>caractère à l&#8217;indice spécifié,</p>
</dd>
<dt class="hdlist1"><code>substring(int, int)</code></dt>
<dd>
<p>extraction d&#8217;une sous-chaîne,</p>
</dd>
<dt class="hdlist1"><code>indexOf(&#8230;&#8203;)</code>, <code>lastIndexOf(&#8230;&#8203;)</code></dt>
<dd>
<p>recherche dans la chaîne</p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_autres_usages_de_string"><a class="anchor" href="#_autres_usages_de_string"></a><a class="link" href="#_autres_usages_de_string">3.3.4. Autres usages de <code>String</code></a></h4>
<div class="ulist">
<ul>
<li>
<p><strong>Un littéral chaîne peut être utilisé à tout endroit où un objet <code>String</code> peut l&#8217;être</strong></p>
<div class="ulist">
<ul>
<li>
<p>on peut invoquer des méthodes de <code>String</code> sur un littéral chaîne</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;opérateur <code>+</code> permet de concaténer des objets de type <code>String</code></p>
<div class="ulist">
<ul>
<li>
<p>c&#8217;est le seul opérateur surchargé pour un objet en Java</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une chaîne peut être utilisée avec l&#8217;instruction <code>switch</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_classes_stringbuilder_et_stringbuffer"><a class="anchor" href="#_les_classes_stringbuilder_et_stringbuffer"></a><a class="link" href="#_les_classes_stringbuilder_et_stringbuffer">3.3.5. Les classes <code>StringBuilder</code> et <code>StringBuffer</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Les instances disposent à peu prés des mêmes accesseurs que <code>String</code></p>
</li>
<li>
<p>Quelques mutateurs:</p>
<div class="dlist">
<dl>
<dt class="hdlist1"><code>append(&#8230;&#8203;)</code></dt>
<dd>
<p>ajout de caractères</p>
</dd>
<dt class="hdlist1"><code>delete(&#8230;&#8203;)</code></dt>
<dd>
<p>suppression de caractères</p>
</dd>
<dt class="hdlist1"><code>insert(&#8230;&#8203;)</code></dt>
<dd>
<p>insertion de caractères</p>
</dd>
</dl>
</div>
</li>
<li>
<p><code>StringBuilder</code> est optimisée pour un environnement <em>mono-thread</em></p>
</li>
<li>
<p><code>StringBuffer</code> est à utiliser dans un contexte <em>multi-threads</em></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_manipulation_de_chaînes_de_caractères"><a class="anchor" href="#_exemple_manipulation_de_chaînes_de_caractères"></a><a class="link" href="#_exemple_manipulation_de_chaînes_de_caractères">3.3.6. Exemple : Manipulation de chaînes de caractères</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">String source = "abcde";
int len = source.length();
StringBuilder dest = new StringBuilder(len);

for (int i = (len - 1); i &gt;= 0; --i) {
    dest.append(source.charAt(i));
}

assert dest.toString().equals("edcba") : dest;</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_caractéristiques_dune_classe"><a class="anchor" href="#_caractéristiques_dune_classe"></a><a class="link" href="#_caractéristiques_dune_classe">3.4. Caractéristiques d&#8217;une classe</a></h3>
<div class="sect3">
<h4 id="_catégories_de_méthodes"><a class="anchor" href="#_catégories_de_méthodes"></a><a class="link" href="#_catégories_de_méthodes">3.4.1. Catégories de méthodes</a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1">Accesseur</dt>
<dd>
<p>permet de consulter l&#8217;état d&#8217;un objet</p>
</dd>
<dt class="hdlist1">Mutateur</dt>
<dd>
<p>modifie l&#8217;état d&#8217;un objet (doit préserver l&#8217;invariant)</p>
</dd>
<dt class="hdlist1">Constructeur</dt>
<dd>
<p>initialise un objet afin de le placer dans un état cohérent</p>
</dd>
<dt class="hdlist1">Destructeur</dt>
<dd>
<p>libère les ressources allouées par l&#8217;objet</p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_surcharge_de_méthode"><a class="anchor" href="#_surcharge_de_méthode"></a><a class="link" href="#_surcharge_de_méthode">3.4.2. Surcharge de méthode</a></h4>
<div class="ulist">
<ul>
<li>
<p>La <em>surcharge</em> (ou <em>polymorphisme ad hoc</em>) d&#8217;une méthode consiste à définir plusieurs méthodes de même nom mais ayant des signatures différentes</p>
</li>
<li>
<p>Une opération n&#8217;est donc plus simplement identifiée par son nom mais également par le nombre, l&#8217;ordre et le type de ses arguments</p>
</li>
<li>
<p>Le choix de la méthode est résolu lors de la compilation</p>
</li>
</ul>
</div>
<div class="exampleblock">
<div class="content">
<div class="ulist">
<ul>
<li>
<p>La surcharge est souvent utilisée pour définir plusieurs constructeurs de façon à initialiser les objets de différentes manières</p>
</li>
<li>
<p>Une alternative plus souple consiste à appliquer un modèle de conception <a href="http://fr.wikipedia.org/wiki/Fabrique_\%28patron_de_conception\%29">Fabrique</a> (<em>Factory</em>)</p>
</li>
</ul>
</div>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_accès_aux_membres"><a class="anchor" href="#_accès_aux_membres"></a><a class="link" href="#_accès_aux_membres">3.4.3. Accès aux membres</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe peut contrôler l&#8217;accès à ses membres (données ou fonctions)</p>
<div class="dlist">
<dl>
<dt class="hdlist1">privé</dt>
<dd>
<p>accès limité à la classe</p>
</dd>
<dt class="hdlist1">protégé</dt>
<dd>
<p>accès limité à la classe et à ses sous-classes</p>
</dd>
<dt class="hdlist1">module</dt>
<dd>
<p>accès limité au module (<em>package</em>) contenant la classe</p>
</dd>
<dt class="hdlist1">public</dt>
<dd>
<p>accès non limité</p>
</dd>
</dl>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_invariant_de_classe"><a class="anchor" href="#_invariant_de_classe"></a><a class="link" href="#_invariant_de_classe">3.4.4. Invariant de classe</a></h4>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
l'<em>invariant d&#8217;une classe</em> impose une contrainte sur l&#8217;état des instances de la classe. Chaque objet doit respecter les conditions imposées par l&#8217;invariant.
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;invariant est établi lors de la création d&#8217;une instance</p>
</li>
<li>
<p>Il doit être vérifié avant l&#8217;exécution d&#8217;une opération publique</p>
</li>
<li>
<p>Chaque opération publique doit rétablir l&#8217;invariant avant de se terminer</p>
</li>
<li>
<p>L&#8217;invariant peut être violé temporairement lors de l&#8217;exécution d&#8217;une opération</p>
</li>
<li>
<p>Avec un langage de programmation, l&#8217;invariant peut être exprimé avec des assertions ou avec une construction spécifique</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_les_classes_en_java"><a class="anchor" href="#_les_classes_en_java"></a><a class="link" href="#_les_classes_en_java">3.5. Les classes en Java</a></h3>
<div class="sect3">
<h4 id="_définir_une_classe"><a class="anchor" href="#_définir_une_classe"></a><a class="link" href="#_définir_une_classe">3.5.1. Définir une classe</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
La <em>définition</em> d&#8217;une classe comporte deux parties: la <em>déclaration</em> et le <em>corps</em> de la classe
</td>
</tr>
</table>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un bref commentaire.
 * Un commentaire plus détaillé...
 * @version janv. 2023
 * @author Prénom NOM
 */
class NomClasse { // Déclaration de la classe
  // Corps de la classe
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La déclaration précise au compilateur un certain nombre d&#8217;informations sur la classe (son nom, &#8230;&#8203;)</p>
</li>
<li>
<p>Le corps de la classe contient les attributs et les méthodes (les <em>membres</em>) de la classe</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_déclarer_des_attributs"><a class="anchor" href="#_déclarer_des_attributs"></a><a class="link" href="#_déclarer_des_attributs">3.5.2. Déclarer des attributs</a></h4>
<div class="ulist">
<ul>
<li>
<p>La déclaration d&#8217;un attribut spécifie son nom et son type</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/** Description de l'attribut. */
Type nom;
/** Description de l'attribut. */
final Type nom;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><strong>L&#8217;initialisation des attributs se fait dans un constructeur</strong></p>
</li>
<li>
<p><code>final</code> est optionnel et permet de déclarer un attribut qui ne pourra être affecté qu&#8217;une unique fois</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_pseudo_attribut_this"><a class="anchor" href="#_pseudo_attribut_this"></a><a class="link" href="#_pseudo_attribut_this">3.5.3. Pseudo-attribut <code>this</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Chaque classe possède un attribut privé particulier nommé <code>this</code> qui référence l&#8217;objet courant</p>
</li>
<li>
<p>Cette attribut est maintenu par le système et ne peut pas être modifié par le programmeur</p>
</li>
<li>
<p><code>this</code> n&#8217;est accessible que dans le corps de la classe</p>
</li>
<li>
<p>Usage</p>
<div class="ulist">
<ul>
<li>
<p>passer l&#8217;objet courant en paramètre d&#8217;une méthode (<code>unObjet.uneMethode(this)</code>)</p>
</li>
<li>
<p>lever certaines ambiguïtés à propos des membres (<code>this.centre = centre</code>)</p>
</li>
<li>
<p>invoquer un autre constructeur dans un constructeur (<code>this(centre, 1)</code>)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_les_attributs_dun_cercle"><a class="anchor" href="#_exemple_les_attributs_dun_cercle"></a><a class="link" href="#_exemple_les_attributs_dun_cercle">3.5.4. Exemple : les attributs d&#8217;un cercle</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.classes;

import fr.uvsq.info.poo.coo.Point2D;

/**
 * Un cercle en deux dimensions.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
class Cercle2D {
    /** Le centre du cercle. */
    private Point2D centre;

    /** Le rayon du cercle */
    private final double rayon;</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_définir_des_méthodes"><a class="anchor" href="#_définir_des_méthodes"></a><a class="link" href="#_définir_des_méthodes">3.5.5. Définir des méthodes</a></h4>
<div class="ulist">
<ul>
<li>
<p>La <em>définition</em> d&#8217;une méthode comporte deux parties: la <em>déclaration</em> et le <em>corps</em> (l'<em>implémentation</em>) de la méthode</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Brêve description de la méthode.
 * Une description plus longue...
 * @param param1 description du paramêtre
 * @param ...
 * @return description de la valeur de retour
 */
TypeRetour nomMethode(listeDeParametres) { // Déclaration
  // Corps de la méthode
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><code>TypeRetour</code> est le type de la valeur retournée ou <code>void</code> si aucune valeur n&#8217;est retournée</p>
</li>
<li>
<p>Dans le corps de la méthode, on utilise l&#8217;opérateur <code>return</code> pour renvoyer une valeur</p>
</li>
<li>
<p>Un constructeur a le même nom que sa classe et ne possède pas de type de retour</p>
<div class="ulist">
<ul>
<li>
<p>bien que l&#8217;on puisse initialiser les attributs directement (affection lors de leur déclaration ou bloc d&#8217;initialisation), il est préférable de toujours le faire dans le constructeur (plus de souplesse, initialisations à un seul endroit)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_paramètres_de_méthode"><a class="anchor" href="#_paramètres_de_méthode"></a><a class="link" href="#_paramètres_de_méthode">3.5.6. Paramètres de méthode</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>listeDeParamètres</code> est une liste de déclarations de variables séparées par des virgules</p>
<div class="ulist">
<ul>
<li>
<p>un paramètre peut être vu comme une variable locale à la méthode</p>
</li>
<li>
<p><code>final</code> peut préfixer la déclaration si le paramètre ne doit pas être modifié</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le passage de paramètres se fait <em>par valeur</em></p>
<div class="ulist">
<ul>
<li>
<p>la valeur d&#8217;un paramètre d&#8217;un type primitif ne peut pas être modifiée</p>
</li>
<li>
<p>la valeur d&#8217;une référence ne peut pas être modifiée mais l&#8217;objet référencé peut l&#8217;être (comme avec un pointeur en C)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_les_constructeurs_de_la_classe_cercle2d"><a class="anchor" href="#_exemple_les_constructeurs_de_la_classe_cercle2d"></a><a class="link" href="#_exemple_les_constructeurs_de_la_classe_cercle2d">3.5.7. Exemple : les constructeurs de la classe <code>Cercle2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Initialise un cercle avec un centre et un rayon.
 * @param centre Le centre.
 * @param rayon Le rayon.
 */
public Cercle2D(final Point2D centre, final double rayon) {
    this.centre = centre;
    this.rayon = rayon;
}

/**
 * Initialise un cercle centré à l'origine et de rayon 1
 */
public Cercle2D() {
    this(new Point2D(), 1.0);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_les_accesseurs_de_la_classe_cercle2d"><a class="anchor" href="#_exemple_les_accesseurs_de_la_classe_cercle2d"></a><a class="link" href="#_exemple_les_accesseurs_de_la_classe_cercle2d">3.5.8. Exemple : les accesseurs de la classe <code>Cercle2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Renvoie le centre du cercle.
 * @return le centre du cercle.
 */
public Point2D getCentre() {
    return centre;
}

/**
 * Renvoie le rayon du cercle.
 * @return le rayon du cercle.
 */
public double getRayon() {
    return rayon;
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_le_mutateur_de_la_classe_cercle2d"><a class="anchor" href="#_exemple_le_mutateur_de_la_classe_cercle2d"></a><a class="link" href="#_exemple_le_mutateur_de_la_classe_cercle2d">3.5.9. Exemple : le mutateur de la classe <code>Cercle2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Translate le cercle.
 * @param dx deplacement en abscisse.
 * @param dy deplacement en ordonnees.
 */
public void translate(final double dx, final double dy) {
    centre.translate(dx, dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_contrôle_daccès_aux_membres_en_java"><a class="anchor" href="#_contrôle_daccès_aux_membres_en_java"></a><a class="link" href="#_contrôle_daccès_aux_membres_en_java">3.5.10. Contrôle d&#8217;accès aux membres en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le contrôle de l&#8217;accès aux membres permet de spécifier l&#8217;interface d&#8217;un classe</p>
</li>
<li>
<p>Le niveau d&#8217;accès est précisé en ajoutant un mot-clé devant la déclaration du membre (attribut ou méthode)</p>
</li>
<li>
<p>Il peut prendre l&#8217;une des valeurs <code>private, public, protected</code> ou être absent</p>
</li>
</ul>
</div>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Niveau</th>
<th class="tableblock halign-left valign-top">Classe</th>
<th class="tableblock halign-left valign-top">Module</th>
<th class="tableblock halign-left valign-top">Sous-classe</th>
<th class="tableblock halign-left valign-top">Extérieur</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>private</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">aucun</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>protected</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>public</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">X</p></td>
</tr>
</tbody>
</table>
<div class="ulist">
<ul>
<li>
<p>La restriction d&#8217;accès s&#8217;applique au niveau de la classe et non pas de l&#8217;objet</p>
</li>
<li>
<p><strong>Les attributs sont déclarés <code>private</code></strong> pour respecter l&#8217;encapsulation</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_la_classe_cercle2d_dans_son_ensemble"><a class="anchor" href="#_la_classe_cercle2d_dans_son_ensemble"></a><a class="link" href="#_la_classe_cercle2d_dans_son_ensemble">3.5.11. La classe <code>Cercle2D</code> dans son ensemble</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// tag::cercle-attr[]
package fr.uvsq.info.poo.classes;

import fr.uvsq.info.poo.coo.Point2D;

/**
 * Un cercle en deux dimensions.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
class Cercle2D {
    /** Le centre du cercle. */
    private Point2D centre;

    /** Le rayon du cercle */
    private final double rayon;
// end::cercle-attr[]
// tag::cercle-cons[]
    /**
     * Initialise un cercle avec un centre et un rayon.
     * @param centre Le centre.
     * @param rayon Le rayon.
     */
    public Cercle2D(final Point2D centre, final double rayon) {
        this.centre = centre;
        this.rayon = rayon;
    }

    /**
     * Initialise un cercle centré à l'origine et de rayon 1
     */
    public Cercle2D() {
        this(new Point2D(), 1.0);
    }
// end::cercle-cons[]

// tag::cercle-access[]
    /**
     * Renvoie le centre du cercle.
     * @return le centre du cercle.
     */
    public Point2D getCentre() {
        return centre;
    }

    /**
     * Renvoie le rayon du cercle.
     * @return le rayon du cercle.
     */
    public double getRayon() {
        return rayon;
    }
// end::cercle-access[]

// tag::cercle-mut[]
    /**
     * Translate le cercle.
     * @param dx deplacement en abscisse.
     * @param dy deplacement en ordonnees.
     */
    public void translate(final double dx, final double dy) {
        centre.translate(dx, dy);
    }
// end::cercle-mut[]

    /**
     * Retourne une chaine decrivant le cercle.
     * @return la representation textuelle du cercle.
     */
    @Override
    public String toString() {
        return String.format("[(%f, %f), %f]", centre.getAbscisse(), centre.getOrdonnee(), rayon);
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exercice_manipulation_dobjets_et_définition_de_classes"><a class="anchor" href="#_exercice_manipulation_dobjets_et_définition_de_classes"></a><a class="link" href="#_exercice_manipulation_dobjets_et_définition_de_classes">3.5.12. Exercice : manipulation d&#8217;objets et définition de classes</a></h4>
<div class="paragraph">
<p>Pour cet exercice, on reprendra les spécifications obtenues lors de l&#8217;exercice précédent.</p>
</div>
<div class="ulist">
<ul>
<li>
<p>Soit le terrain suivant (M = mur, R = robot, N = nord, O = ouest).</p>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/diag-1d620dd3b33c38f00693d7fa69eae0b8.png" alt="diag 1d620dd3b33c38f00693d7fa69eae0b8" width="140" height="126">
</div>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Écrire les instructions Java permettant de créer ce terrain puis de déplacer le robot (0, 0) en (1, 1).</p>
</li>
<li>
<p>Écrire en Java la classe <code>Robot</code>.</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_métaclasse_et_membres_de_classe"><a class="anchor" href="#_métaclasse_et_membres_de_classe"></a><a class="link" href="#_métaclasse_et_membres_de_classe">3.6. Métaclasse et membres de classe</a></h3>
<div class="sect3">
<h4 id="_métaclasse"><a class="anchor" href="#_métaclasse"></a><a class="link" href="#_métaclasse">3.6.1. Métaclasse</a></h4>
<div class="ulist">
<ul>
<li>
<p>La relation qui existe entre objet et classe est une relation d&#8217;instanciation</p>
</li>
<li>
<p>De même, on peut considérer une classe comme une instance de classe de plus "haut niveau", dite <em>métaclasse</em></p>
</li>
<li>
<p>Cette notion permet d&#8217;introduire des <em>méthodes de classe</em> et des <em>attributs de classe</em>, i.e. des membres associés à la classe et non pas à une instance particulière</p>
</li>
<li>
<p>Une <em>méthode de classe</em> peut être invoquée sans instance particulière</p>
</li>
<li>
<p>Un <em>attribut de classe</em> est associé à la classe elle-même et non pas à une instance particulière</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_compter_le_nombre_dinstances_de_cercle"><a class="anchor" href="#_exemple_compter_le_nombre_dinstances_de_cercle"></a><a class="link" href="#_exemple_compter_le_nombre_dinstances_de_cercle">3.6.2. Exemple : compter le nombre d&#8217;instances de cercle</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/membres_de_classe.png" alt="membres de classe" width="320" height="141">
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_membres_de_classe_en_java"><a class="anchor" href="#_membres_de_classe_en_java"></a><a class="link" href="#_membres_de_classe_en_java">3.7. Membres de classe en Java</a></h3>
<div class="sect3">
<h4 id="_membres_de_classe_en_java_2"><a class="anchor" href="#_membres_de_classe_en_java_2"></a><a class="link" href="#_membres_de_classe_en_java_2">3.7.1. Membres de classe en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un membre de classe se déclare avec le mot-clé <code>static</code></p>
</li>
<li>
<p><strong>L&#8217;accès à un membre de classe se fait par l&#8217;intermédiaire de la classe</strong></p>
</li>
<li>
<p>Pour un attribut de classe, le système alloue un espace mémoire pour un attribut par classe (et non pas un attribut par instance)</p>
</li>
<li>
<p>Un attribut de classe est souvent utilisé pour définir une constante (<code>static final</code>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static final double E = 2.718281828459045d;
public static final double PI = 3.141592653589793d;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;initialisation d&#8217;un attribut de classe peut se faire directement ou en utilisant un <em>bloc d&#8217;initialisation statique</em></p>
</li>
<li>
<p>Un <em>bloc d&#8217;initialisation statique</em> est un bloc de code Java classique commençant par le mot-clé <code>static</code> et placé dans le corps de la classe</p>
</li>
<li>
<p><strong>Une méthode de classe ne peut pas accéder aux attributs d&#8217;instance</strong> (pas de <code>this</code>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_compter_les_instances_de_cercle"><a class="anchor" href="#_exemple_compter_les_instances_de_cercle"></a><a class="link" href="#_exemple_compter_les_instances_de_cercle">3.7.2. Exemple : compter les instances de cercle</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un cercle en deux dimensions.
 *
 * @author Author1
 * @version Version 1.0
 */
class Cercle2DWithCpt extends Cercle2D {
    /**
     * Le nombre d'instances de Cercle2DWithCpt
     */
    static int nbInstances = 0;

    /**
     * Initialise un cercle avec un centre et un rayon.
     *
     * @param centre Le centre.
     * @param rayon  Le rayon.
     */
    public Cercle2DWithCpt(Point2D centre, double rayon) {
        super(centre, rayon);
        ++nbInstances;
    }

    /**
     * Retourne le nombre d'instances de la classe.
     *
     * @return le nombre d'instances.
     */
    public static int getNbInstances() {
        return nbInstances;
    }

    /**
     * Décrémentation du nombre d'instances quand l'objet est détruit.
     */
    @Override
    protected void finalize() throws Throwable {
        --nbInstances;
        super.finalize();
    }</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_invoquer_une_méthode_de_classe"><a class="anchor" href="#_exemple_invoquer_une_méthode_de_classe"></a><a class="link" href="#_exemple_invoquer_une_méthode_de_classe">3.7.3. Exemple : invoquer une méthode de classe</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">assert Cercle2DWithCpt.getNbInstances() == 0 :
        Cercle2DWithCpt.getNbInstances();

// Creation des cercles
Cercle2DWithCpt c1 = new Cercle2DWithCpt(new Point2D(2.0, 4.0),
        5.0);
Cercle2DWithCpt c2 = new Cercle2DWithCpt(new Point2D(1.0, 2.0),
        4.0);
Cercle2DWithCpt c3 = new Cercle2DWithCpt(new Point2D(3.0, 4.0),
        2.0);

assert Cercle2DWithCpt.getNbInstances() == 3 :
        Cercle2DWithCpt.getNbInstances();

// Simple liaison
Cercle2DWithCpt unAutreC3 = c3;

assert Cercle2DWithCpt.getNbInstances() == 3 :
        Cercle2DWithCpt.getNbInstances();

// Suppression d'un instance
c1 = null;
System.gc();
Thread.sleep(1000);

assert Cercle2DWithCpt.getNbInstances() == 2 :
        Cercle2DWithCpt.getNbInstances();</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_le_programme_principal_en_java"><a class="anchor" href="#_le_programme_principal_en_java"></a><a class="link" href="#_le_programme_principal_en_java">3.8. Le programme principal en Java</a></h3>
<div class="sect3">
<h4 id="_rôle_du_programme_principal"><a class="anchor" href="#_rôle_du_programme_principal"></a><a class="link" href="#_rôle_du_programme_principal">3.8.1. Rôle du programme principal</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un système OO en cours d&#8217;exécution est une collection d&#8217;objets qui interagissent</p>
</li>
<li>
<p>Le lancement du programme doit donc permettre d&#8217;instancier ces objets</p>
<div class="ulist">
<ul>
<li>
<p>en général, le programme principal se limite à créer un <em>objet application</em> qui se charge d&#8217;instancier les autres objets</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_le_programme_principal_en_java_la_méthode_main"><a class="anchor" href="#_le_programme_principal_en_java_la_méthode_main"></a><a class="link" href="#_le_programme_principal_en_java_la_méthode_main">3.8.2. Le programme principal en Java : la méthode <code>main</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Le point d&#8217;entrée d&#8217;une application Java est une méthode de classe nommée <code>main</code></p>
</li>
<li>
<p>Lors de l&#8217;exécution, l&#8217;interpréteur Java est invoqué avec le nom d&#8217;une classe qui doit implémenter une méthode <code>main</code></p>
</li>
<li>
<p>La déclaration de la méthode <code>main</code> est <code>public static void main(String[] args)</code></p>
</li>
<li>
<p>Le paramètre de <code>main</code> est un tableau de chaînes de caractères contenant les <em>arguments de ligne de commande</em> passés lors de l&#8217;appel du programme</p>
</li>
<li>
<p>On limite en général le code se trouvant dans le <code>main</code> au strict minimum: création d&#8217;un objet application et invocation d&#8217;une méthode</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_le_programme_principal_en_java_avec_une_énumération"><a class="anchor" href="#_exemple_le_programme_principal_en_java_avec_une_énumération"></a><a class="link" href="#_exemple_le_programme_principal_en_java_avec_une_énumération">3.8.3. Exemple : le programme principal en Java (avec une énumération)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.classes;

/**
 * Représente l'application.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
enum ApplicationVide {
    ENVIRONNEMENT;

    /*
     * Méthode principale du programme.
     * @param args les arguments de ligne de commande
     */
    public void run(String[] args) {
      // ...
    }

    /*
     * Point d'entrée du programme.
     * @param args les arguments de ligne de commande
     */
    public static void main(String[] args) {
      ENVIRONNEMENT.run(args);
    }
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_énumération_en_java"><a class="anchor" href="#_énumération_en_java"></a><a class="link" href="#_énumération_en_java">3.9. Énumération en Java</a></h3>
<div class="sect3">
<h4 id="_complément_sur_le_type_énuméré"><a class="anchor" href="#_complément_sur_le_type_énuméré"></a><a class="link" href="#_complément_sur_le_type_énuméré">3.9.1. Complément sur le type énuméré</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un type énuméré en Java est en fait une classe dont les instances sont connues lors de la compilation</p>
</li>
<li>
<p>Les constantes d&#8217;un type énuméré peuvent être utilisées partout où un objet peut l&#8217;être</p>
</li>
<li>
<p>Un type énuméré peut donc contenir des méthodes et des attributs</p>
</li>
<li>
<p>De plus, le compilateur ajoute automatiquement certaines méthodes</p>
<div class="ulist">
<ul>
<li>
<p><code>values()</code> retourne un tableau contenant les constantes dans l&#8217;ordre de leur déclaration</p>
</li>
<li>
<p>un type énuméré hérite implicitement de la classe <code>Enum</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_un_type_énuméré_pour_les_planètes"><a class="anchor" href="#_exemple_un_type_énuméré_pour_les_planètes"></a><a class="link" href="#_exemple_un_type_énuméré_pour_les_planètes">3.9.2. Exemple : un type énuméré pour les planètes</a></h4>
<div class="listingblock">
<div class="title">Source : <a href="https://docs.oracle.com/javase/tutorial/java/javaOO/enum.html">The Java Tutorials - Enum Types</a></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public enum Planet {
    MERCURY (3.303e+23, 2.4397e6),
    VENUS   (4.869e+24, 6.0518e6),
    EARTH   (5.976e+24, 6.37814e6),
    MARS    (6.421e+23, 3.3972e6),
    JUPITER (1.9e+27,   7.1492e7),
    SATURN  (5.688e+26, 6.0268e7),
    URANUS  (8.686e+25, 2.5559e7),
    NEPTUNE (1.024e+26, 2.4746e7);

    private final double mass;   // in kilograms
    private final double radius; // in meters
    Planet(double mass, double radius) {
        this.mass = mass;
        this.radius = radius;
    }
    private double mass() { return mass; }
    private double radius() { return radius; }

    // universal gravitational constant  (m3 kg-1 s-2)
    public static final double G = 6.67300E-11;

    double surfaceGravity() {
        return G * mass / (radius * radius);
    }
    double surfaceWeight(double otherMass) {
        return otherMass * surfaceGravity();
    }
    public static void main(String[] args) {
        if (args.length != 1) {
            System.err.println("Usage: java Planet &lt;earth_weight&gt;");
            System.exit(-1);
        }
        double earthWeight = Double.parseDouble(args[0]);
        double mass = earthWeight/EARTH.surfaceGravity();
        for (Planet p : Planet.values())
           System.out.printf("Your weight on %s is %f%n",
                             p, p.surfaceWeight(mass));
    }
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_généricité"><a class="anchor" href="#_généricité"></a><a class="link" href="#_généricité">3.10. Généricité</a></h3>
<div class="sect3">
<h4 id="_généricité_2"><a class="anchor" href="#_généricité_2"></a><a class="link" href="#_généricité_2">3.10.1. Généricité</a></h4>
<div class="ulist">
<ul>
<li>
<p>La <em>généricité</em> permet de paramétrer une classe par un ou plusieurs paramètres formels (généralement des types)</p>
</li>
<li>
<p>La généricité permet de définir une famille de classes, chaque classe étant instanciée lors du passage des paramètres effectifs</p>
</li>
<li>
<p>Une classe paramétrée (ou générique) est donc une métaclasse particulière</p>
</li>
<li>
<p>Il peut être souhaitable de limiter les paramètres possibles : la généricité est alors <em>contrainte</em></p>
</li>
<li>
<p>Utiliser un type paramétré améliore la vérification de type lors de la compilation</p>
</li>
<li>
<p>Cette notion est orthogonale au paradigme OO : on parle de <em>programmation générique</em></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_un_cercle_générique"><a class="anchor" href="#_exemple_un_cercle_générique"></a><a class="link" href="#_exemple_un_cercle_générique">3.10.2. Exemple : un cercle générique</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/generic.png" alt="generic" width="230" height="129">
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_généricité_en_java"><a class="anchor" href="#_généricité_en_java"></a><a class="link" href="#_généricité_en_java">3.11. Généricité en Java</a></h3>
<div class="sect3">
<h4 id="_généricité_en_java_2"><a class="anchor" href="#_généricité_en_java_2"></a><a class="link" href="#_généricité_en_java_2">3.11.1. Généricité en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les <em>paramètres formels de type</em> sont placés entre &#8220;&lt;&#8221; et &#8220;&gt;&#8221;</p>
</li>
<li>
<p>Un paramètre effectif est obligatoirement une classe (pas un type primitif)</p>
</li>
<li>
<p>Le mécanisme implémentant la généricité en Java se nomme <em>Type erasure</em></p>
</li>
<li>
<p>Ce mécanisme supprime toute trace de la généricité dans le bytecode &#8658; il n&#8217;existe pas d&#8217;information concernant la généricité à l&#8217;exécution</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_classe_générique_en_java"><a class="anchor" href="#_classe_générique_en_java"></a><a class="link" href="#_classe_générique_en_java">3.11.2. Classe générique en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les <em>paramètres formels de type</em> sont placés entre &#8220;&lt;&#8221; et &#8220;&gt;&#8221; juste après le nom de la classe</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class Cercle&lt;T&gt; {
  //...
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le paramètre de type peut ensuite être utilisé comme tout autre type dans la définition de la classe</p>
</li>
<li>
<p>La déclaration d&#8217;une variable de ce type nécessite de passer le type effectif à la classe paramétrée</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Cercle&lt;Point2D&gt; c = //...</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>la création d&#8217;une instance ne répète pas le type effectif (<em>diamond notation</em>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Cercle&lt;Point2D&gt; c = new Cercle&lt;&gt;(/* ... */);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_définition_de_la_classe_générique_cercle"><a class="anchor" href="#_exemple_définition_de_la_classe_générique_cercle"></a><a class="link" href="#_exemple_définition_de_la_classe_générique_cercle">3.11.3. Exemple : définition de la classe générique <code>Cercle</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un cercle générique.
 * Ce cercle peut s'adapter au cas à 2 ou à 3 dimensions.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
class Cercle&lt;T&gt; {
    /** Le centre du cercle. */
    private T centre;

    /** Le rayon du cercle */
    private double rayon;

    /**
     * Initialise un cercle avec un centre et un rayon.
     * @param centre Le centre.
     * @param rayon Le rayon.
     */
    public Cercle(T centre, double rayon) {
        this.centre = centre;
        this.rayon = rayon;
    }

    public T getCentre() {
        return centre;
    }

    public double getRayon() {
        return rayon;
    }</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_classe_générique_cercle"><a class="anchor" href="#_exemple_utilisation_de_la_classe_générique_cercle"></a><a class="link" href="#_exemple_utilisation_de_la_classe_générique_cercle">3.11.4. Exemple : utilisation de la classe générique <code>Cercle</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// En 2 dimensions
Point2D p1 = new Point2D(1.0, 2.0);
Cercle&lt;Point2D&gt; c1 = new Cercle&lt;Point2D&gt;(p1, 3.0);

// Invocation d'une methode de Point2D
double xCentre = c1.getCentre().getAbscisse();

// En 3 dimensions
Point3D p2 = new Point3D(3.0, 4.0, 5.0);
Cercle&lt;Point3D&gt; c2 = new Cercle&lt;Point3D&gt;(p2, 3.0);

// Invocation d'une methode de Point3D
double zCentre = c2.getCentre().getZ();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_méthode_générique_en_java"><a class="anchor" href="#_méthode_générique_en_java"></a><a class="link" href="#_méthode_générique_en_java">3.11.5. Méthode générique en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Il est possible de déclarer des méthodes génériques</p>
</li>
<li>
<p>Le paramètre de type formel est alors précisé avant la déclaration</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static &lt;T&gt; T max(T o1, T o2) // ...</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La portée de ce paramètre est alors restreinte à la méthode</p>
</li>
<li>
<p>L&#8217;invocation de la méthode peut préciser le type effectif ou se baser sur l'<em>inférence de type</em></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Type effectif explicite
Integer i = uneClasse.&lt;Integer&gt;max(i1, i2);

// Type effectif déterminé par inférence de type
Integer i = uneClasse.max(i1, i2);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_généricité_contrainte_en_java"><a class="anchor" href="#_généricité_contrainte_en_java"></a><a class="link" href="#_généricité_contrainte_en_java">3.11.6. Généricité contrainte en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Il est possible d&#8217;imposer que le paramètre de type formel soit un sous-type d&#8217;un autre type avec le mot-clé <code>extends</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static &lt;T extends Number&gt; T max(T o1, T o2) // ...</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le mot-clé <code>super</code> permet d&#8217;imposer que le paramètre de type formel soit un super-type d&#8217;un autre type (exemple : <code>&lt;T super Number&gt;</code>)</p>
</li>
<li>
<p>Il peut être nécessaire d&#8217;utiliser le caractère <em>joker</em> <code>?</code> si le type effectif n&#8217;est pas connu</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Une boite qui peut contenir des nombres
Boite&lt;? extends Number&gt; b = //...

// Un boite qui peut contenir n'importe quoi
Boite&lt;?&gt; b = //...</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>En complément : <a href="https://docs.oracle.com/javase/tutorial/java/generics/wildcardGuidelines.html">The Java Tutorials - Guidelines for Wildcard Use</a></p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_java_2"><a class="anchor" href="#_exercices_java_2"></a><a class="link" href="#_exercices_java_2">3.12. Exercices (Java)</a></h3>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>Utilisation de l&#8217;environnement de développement <a href="https://www.bluej.org/">BlueJ</a> : chaque exercice nécessite la création d&#8217;un nouveau projet.</p>
</li>
<li>
<p>Les seules sources d&#8217;information externes autorisées sont</p>
<div class="ulist">
<ul>
<li>
<p>la référence de l&#8217;<a href="http://docs.oracle.com/javase/8/docs/api/">API Java</a>,</p>
</li>
<li>
<p>le <a href="http://docs.oracle.com/javase/tutorial/">tutoriel</a> Java,</p>
</li>
<li>
<p>la <a href="http://www.bluej.org/doc/documentation.html">documentation</a> de <a href="https://www.bluej.org/">BlueJ</a>.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Exécution interactive uniquement avec <a href="https://www.bluej.org/">BlueJ</a> (pas de méthode <code>main</code> ni d&#8217;affichage).</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="sect3">
<h4 id="_création_dune_classe_simple"><a class="anchor" href="#_création_dune_classe_simple"></a><a class="link" href="#_création_dune_classe_simple">3.12.1. Création d&#8217;une classe simple</a></h4>
<div class="paragraph">
<p>L&#8217;objet de cet exercice est de réaliser une classe <code>ChaineCryptee</code> qui permettra de chiffrer/déchiffrer une chaîne de caractères (composée de lettres majuscules et d&#8217;espace).
Le chiffrement utilise une méthode par décalage.
La valeur du décalage représente la clé de chiffrement.
Par exemple, une clé de valeur trois transformera un <code>'A'</code> en <code>'D'</code>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Créez la classe <code>ChaineCryptee</code> avec pour attribut la chaîne <strong>en clair</strong> et le décalage.</p>
</li>
<li>
<p>Ajoutez un constructeur pour initialiser les instances à partir d&#8217;une chaîne en clair et du décalage.</p>
</li>
<li>
<p>Ajoutez la méthode <code>String decrypte()</code> qui retourne la chaîne en clair.</p>
</li>
<li>
<p>Ajoutez la méthode <code>String crypte()</code> qui retourne la chaîne chiffrée.
Vous pourrez utilisez pour cela la méthode <code>decaleCaractere</code> (voir le listing ci-dessous).</p>
</li>
<li>
<p>Comment se comporte votre classe si la chaîne passée au constructeur est <code>null</code> ?
Vous pouvez utiliser le débogueur pour identifier le problème (s&#8217;il y a un problème) au niveau de <code>crypte</code>.</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>si la méthode a échoué, modifiez la classe pour prendre en compte la chaîne <code>null</code>,</p>
</li>
<li>
<p>vérifiez avec le débogueur que le problème est réglé.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Faites afficher l&#8217;interface de la classe (la documentation <code>JavaDoc</code>).
Le comportement de votre classe en cas de chaîne <code>null</code> doit être expliqué dans la documentation.</p>
</li>
<li>
<p>Changez la représentation interne de la classe : seule la chaîne cryptée est stockée (plus la chaîne en clair).</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>effectuez les modifications nécessaires sans changer l&#8217;interface de la classe.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Ajoutez la possibilité d&#8217;initialiser une instance à partir d&#8217;une chaîne cryptée et d&#8217;un décalage.
Pour éviter l&#8217;ambiguïté au niveau du constructeur, vous utiliserez le <a href="http://fr.wikipedia.org/wiki/Fabrique_%28patron_de_conception%29#Autres_avantages_et_variantes">modèle de conception Fabrication</a>.
Pour cela,</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>créez les méthodes de classe <code>ChaineCryptee deCryptee(String, int)</code> et <code>ChaineCryptee deEnClair(String, int)</code>,</p>
</li>
<li>
<p>rendez le constructeur privé.
La création des instances se fait maintenant à l&#8217;aide des deux méthodes de classe.</p>
</li>
</ol>
</div>
</li>
</ol>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Décale un caractère majuscule.
 * Les lettres en majuscule ('A' - 'Z') sont décalées de &lt;code&gt;decalage&lt;/code&gt;
 * caractères de façon circulaire. Les autres caractères ne sont pas modifiés.
 *
 * @param c le caractère à décaler
 * @param decalage le décalage à appliquer
 * @return le caractère décalé
 */
private static char decaleCaractere(char c, int decalage) {
    return (c &lt; 'A' || c &gt; 'Z')? c : (char)(((c - 'A' + decalage) % 26) + 'A');
}</code></pre>
</div>
</div>
<div class="paragraph">
<p>À la fin de cet exercice, la classe <code>ChaineCryptee</code> doit avoir la structure suivante</p>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/encryptedstring.png" alt="encryptedstring" width="434" height="167">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_classes_et_associations"><a class="anchor" href="#_classes_et_associations"></a><a class="link" href="#_classes_et_associations">3.12.2. Classes et associations</a></h4>
<div id="exo:clientserveur" class="paragraph">
<p>On souhaite <strong>simuler</strong> le comportement d&#8217;un logiciel de discussion client/serveur.
Pour pouvoir discuter, un client doit au préalable se connecter au serveur.
Lorsque le client envoie un message au serveur, ce dernier le transmet à tous les clients avec le nom de l&#8217;émetteur.</p>
</div>
<div class="paragraph">
<p>Un diagramme de classes possible pour cet énoncé est donné par la figure suivante.</p>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/chat.png" alt="chat" width="586" height="130">
</div>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Donnez un diagramme de séquence UML décrivant le scénario suivant:</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>le serveur <em>s</em> est actuellement connecté avec les clients <em>c<sub>1</sub></em> et <em>c<sub>2</sub></em>,</p>
</li>
<li>
<p>le client <em>c<sub>3</sub></em> se connecte à <em>s</em>,</p>
</li>
<li>
<p>le client envoie le message <em>Bonjour</em> aux clients connectés.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Implémentez les classes <code>Client</code> et <code>Serveur</code>.</p>
</li>
<li>
<p>déroulez le scénario de la question 1 dans Bluej.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_agrégation_et_composition"><a class="anchor" href="#_agrégation_et_composition"></a><a class="link" href="#_agrégation_et_composition">3.12.3. Agrégation et composition</a></h4>
<div class="paragraph">
<p>Un document est décrit par un titre, le nom de son auteur, l&#8217;année de publication et une liste de références sur d&#8217;autres documents (par exemple, des documents traitant du même sujet).
Une bibliothèque gère un ensemble de documents.</p>
</div>
<div class="paragraph">
<p>Les opérations que l&#8217;on souhaite pouvoir effectuer sont les suivantes :</p>
</div>
<div class="ulist">
<ul>
<li>
<p>initialisation d&#8217;un document avec son titre, l&#8217;auteur et une année,</p>
</li>
<li>
<p>ajout d&#8217;une référence dans un document,</p>
</li>
<li>
<p>affichage (construire une chaîne de caractères le représentant) d&#8217;un document (avec ses références sous la forme <em>titre, auteur</em>),</p>
</li>
<li>
<p>ajout d&#8217;un document dans la bibliothèque,</p>
</li>
<li>
<p>recherche par titre d&#8217;un document dans la bibliothèque,</p>
</li>
<li>
<p>recherche des documents citant un document.</p>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Modélisez cette énoncé à l&#8217;aide d&#8217;un diagramme de classe.</p>
</li>
<li>
<p>Implémentez ce modèle.</p>
</li>
</ol>
</div>
</li>
</ul>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_héritage_3"><a class="anchor" href="#_héritage_3"></a><a class="link" href="#_héritage_3">4. Héritage</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_héritage_en_java"><a class="anchor" href="#_héritage_en_java"></a><a class="link" href="#_héritage_en_java">4.1. Héritage en Java</a></h3>
<div class="sect3">
<h4 id="_héritage_en_java_2"><a class="anchor" href="#_héritage_en_java_2"></a><a class="link" href="#_héritage_en_java_2">4.1.1. Héritage en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>On spécifie qu&#8217;une classe est une sous-classe d&#8217;une autre en utilisant <code>extends</code> dans la déclaration <code>class NomClasse extends NomSuperClasse</code></p>
</li>
<li>
<p>Une classe ne peut avoir qu&#8217;une seule super-classe (pas d&#8217;héritage multiple)</p>
</li>
<li>
<p>Si <code>extends</code> n&#8217;est pas précisé, la classe hérite de la classe <code>Object</code></p>
</li>
<li>
<p><strong>Une classe Java a une et une seule super-classe</strong></p>
</li>
<li>
<p>Une classe déclarée <code>final</code> ne peut plus être spécialisée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_héritage_et_membres"><a class="anchor" href="#_héritage_et_membres"></a><a class="link" href="#_héritage_et_membres">4.1.2. Héritage et membres</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe <em>C</em> hérite de sa super-classe <em>S</em> les attributs et méthodes qu&#8217;elle possède</p>
<div class="ulist">
<ul>
<li>
<p>tous les attributs de <em>S</em> font partie de l&#8217;état des instances de <em>C</em></p>
</li>
<li>
<p>les méthodes publiques de <em>S</em> font partie de l&#8217;interface publique de <em>C</em></p>
</li>
</ul>
</div>
</li>
<li>
<p>Les attributs et méthodes d&#8217;une super-classe ne sont pas formcément accessibles</p>
<div class="ulist">
<ul>
<li>
<p>les attributs privées de <em>S</em> ne sont pas accessibles dans <em>C</em></p>
</li>
<li>
<p>les méthodes non privées de <em>S</em> sont accessibles dans <em>C</em></p>
</li>
<li>
<p>les constructeurs de <em>S</em> sont utilisables dans les constructeurs de <em>C</em> mais ne font pas partie de l&#8217;interface publique de <em>C</em></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_masquage_de_membres"><a class="anchor" href="#_masquage_de_membres"></a><a class="link" href="#_masquage_de_membres">4.1.3. Masquage de membres</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe peut masquer un membre de sa super-classe si elle possède un membre de même nom (ou de même signature)</p>
</li>
<li>
<p>Le mot clé <code>super</code> permet d&#8217;accéder aux membres masqués d&#8217;une super-classe</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_rectangle_et_rectangle_plein_2"><a class="anchor" href="#_exemple_rectangle_et_rectangle_plein_2"></a><a class="link" href="#_exemple_rectangle_et_rectangle_plein_2">4.1.4. Exemple : rectangle et rectangle plein</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/rectangle_et_rectangle_plein_2.png" alt="rectangle et rectangle plein 2" width="476" height="289">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_définition_de_la_classe_rectangle2dplein_en_java"><a class="anchor" href="#_exemple_définition_de_la_classe_rectangle2dplein_en_java"></a><a class="link" href="#_exemple_définition_de_la_classe_rectangle2dplein_en_java">4.1.5. Exemple : définition de la classe <code>Rectangle2DPlein</code> en Java</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un rectangle plein en deux dimensions.
 *
 * @author Stéphane Lopes
 * @version nov. 2008
 */
class Rectangle2DPlein extends Rectangle2D {
    /**
     * La couleur de remplissage
     */
    private Color couleur;

    /**
     * Initialise le rectangle plein.
     *
     * @param supGauche Le coin supérieur gauche.
     * @param infDroit  Le coin inférieur droit.
     * @param couleur   La couleur de remplissage.
     */
    public Rectangle2DPlein(Point2D supGauche,
                            Point2D infDroit,
                            Color couleur) {
        super(supGauche, infDroit);
        assert couleur != null;
        this.couleur = couleur;
    }

    /**
     * Renvoie la couleur.
     *
     * @return la couleur.
     */
    public Color getCouleur() {
        return couleur;
    }</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><code>extends</code> exprime l&#8217;héritage</p>
</li>
<li>
<p>seule les attributs supplémentaires sont déclarés dans la sous-classe</p>
</li>
<li>
<p>dans le constructeur, <code>super</code> permet d&#8217;appeler le constructeur de la super-classe</p>
</li>
<li>
<p>seule les méthodes supplémentaires sont définies dans la sous-classe</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_classe_rectangle2dplein"><a class="anchor" href="#_exemple_utilisation_de_la_classe_rectangle2dplein"></a><a class="link" href="#_exemple_utilisation_de_la_classe_rectangle2dplein">4.1.6. Exemple : utilisation de la classe <code>Rectangle2DPlein</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Déclaration et création d'un rectangle rouge
Rectangle2DPlein rp = new Rectangle2DPlein(new Point2D(1.0, 2.0),
        new Point2D(3.0, 0.0),
        Color.RED);
assert rp.getCouleur() == Color.RED;

// Déclaration d'un rectangle et
// liaison avec un rectangle plein
Rectangle2D r = new Rectangle2DPlein(new Point2D(1.0, 2.0),
        new Point2D(2.0, 1.0),
        Color.YELLOW);
assert r.getLargeur() == 1;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;affectation d&#8217;une instance de <code>Rectangle2DPlein</code> à une référence sur un <code>Rectangle2D</code> respecte le <em>principe de substitution de Liskov</em></p>
</li>
<li>
<p>À partir de <code>r1</code>, l&#8217;accès à <code>getCouleur</code> est impossible (échoue à la compilation) car <code>getCouleur</code> ne fait pas partie de l&#8217;interface de <code>Rectangle2D</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_application_lhéritage"><a class="anchor" href="#_application_lhéritage"></a><a class="link" href="#_application_lhéritage">4.1.7. Application : l&#8217;héritage</a></h4>
<div class="paragraph">
<p>Deux nouveaux types de robot sont créés :</p>
</div>
<div class="ulist">
<ul>
<li>
<p>Les <em>transporteurs</em> qui peuvent ramasser un objet, le transporter et le déposer,</p>
</li>
<li>
<p>Les <em>destructeurs</em> qui peuvent détruire ce qui se trouve sur la case devant eux.</p>
</li>
</ul>
</div>
<div class="paragraph">
<p>Soit le terrain suivant (M = mur, T = transporteur, D = destructeur, N = nord, E = est, S = sud, O = ouest).</p>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/diag-ec08285cbd25a750ec2365b9ab9cbbc1.png" alt="diag ec08285cbd25a750ec2365b9ab9cbbc1" width="140" height="154">
</div>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Donner un diagramme de classes représentant les nouveaux robots</p>
</li>
<li>
<p>Écrire les instructions permettant de créer ce terrain puis de déplacer l&#8217;objet se trouvant en (0, 0) en (2, 2).</p>
</li>
<li>
<p>Donner l&#8217;implémentation des deux classes <code>Transporteur</code> et <code>Destructeur</code>.</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_polymorphisme_en_java"><a class="anchor" href="#_polymorphisme_en_java"></a><a class="link" href="#_polymorphisme_en_java">4.2. Polymorphisme en Java</a></h3>
<div class="sect3">
<h4 id="_redéfinition_de_méthode"><a class="anchor" href="#_redéfinition_de_méthode"></a><a class="link" href="#_redéfinition_de_méthode">4.2.1. Redéfinition de méthode</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une sous-classe peut <em>redéfinir</em> (<em>override</em>) une ou plusieurs méthodes de sa super-classe</p>
</li>
<li>
<p>La <em>redéfinition</em> (<em>overriding</em>) consiste à définir dans une sous-classe, une méthode ayant même signature et même type de retour qu&#8217;une méthode de la super-classe</p>
<div class="ulist">
<ul>
<li>
<p>la méthode de la super-classe est alors masquée</p>
</li>
<li>
<p>il est toujours possible d&#8217;appeler la méthode redéfinie en utilisant le mot-clé <code>super</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_redéfinition_et_polymorphisme"><a class="anchor" href="#_redéfinition_et_polymorphisme"></a><a class="link" href="#_redéfinition_et_polymorphisme">4.2.2. Redéfinition et polymorphisme</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le polymorphisme est le mécanisme permettant de sélectionner la méthode redéfinie appropriée</p>
</li>
<li>
<p>La redéfinition ne permet plus au compilateur de sélectionner la méthode adéquat</p>
</li>
<li>
<p>C&#8217;est le type de l&#8217;objet (et non pas de la référence) qui permettra de déterminer la méthode à invoquer et ce type ne peut être connu qu&#8217;au moment de l&#8217;exécution</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_compléments_sur_la_redéfinition_de_méthode"><a class="anchor" href="#_compléments_sur_la_redéfinition_de_méthode"></a><a class="link" href="#_compléments_sur_la_redéfinition_de_méthode">4.2.3. Compléments sur la redéfinition de méthode</a></h4>
<div class="ulist">
<ul>
<li>
<p>La déclaration de la méthode redéfinie est toujours précédée de l&#8217;annotation <code>@Override</code></p>
</li>
<li>
<p>Le contrôle d&#8217;accès peut être relaxé lors de la redéfinition</p>
</li>
<li>
<p>Une méthode déclarée <code>final</code> ne peut pas être redéfinie</p>
</li>
<li>
<p>Une méthode de classe ne peut pas être redéfinie</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_une_description_pour_les_rectangles_2"><a class="anchor" href="#_exemple_une_description_pour_les_rectangles_2"></a><a class="link" href="#_exemple_une_description_pour_les_rectangles_2">4.2.4. Exemple : une description pour les rectangles</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/rectangle_et_rectangle_plein_polym.png" alt="rectangle et rectangle plein polym" width="476" height="315">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_rectangle2d"><a class="anchor" href="#_exemple_la_classe_rectangle2d"></a><a class="link" href="#_exemple_la_classe_rectangle2d">4.2.5. Exemple : la classe <code>Rectangle2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un rectangle en deux dimensions.
 * Les côtés du rectangle sont toujours parallèles aux axes.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
class Rectangle2D extends FigureFermee2D implements Cloneable {
    /** Coordonnées du coin supérieur gauche */
    private Point2D orig;

    /** Coordonnées du coin inférieur droit */
    private Point2D fin;

    /**
     * Initialise le rectangle.
     * @param supGauche Le coin supérieur gauche.
     * @param infDroit Le coin inférieur droit.
     */
    public Rectangle2D(Point2D supGauche, Point2D infDroit) {
        assert supGauche.getX() &lt;= infDroit.getX() &amp;&amp;
               supGauche.getY() &gt;= infDroit.getY();
        orig = supGauche;
        fin = infDroit;
    }

    public Point2D getSupGauche() { return orig; }

    public double getLargeur() {
        return fin.getX() - orig.getX();
    }

    public double getHauteur() {
        return orig.getY() - fin.getY();
    }

    /**
     * Retourne une description du rectangle.
     * @return la description.
     */
    public String getDesc() {
        return String.format("O = %s L = %s, H = %s", orig, getLargeur(), getHauteur());
    }</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_rectangle2dplein"><a class="anchor" href="#_exemple_la_classe_rectangle2dplein"></a><a class="link" href="#_exemple_la_classe_rectangle2dplein">4.2.6. Exemple : la classe <code>Rectangle2DPlein</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Un rectangle plein en deux dimensions.
 *
 * @author Stéphane Lopes
 * @version nov. 2008
 */
class Rectangle2DPlein extends Rectangle2D {
    /**
     * La couleur de remplissage
     */
    private Color couleur;

    /**
     * Initialise le rectangle plein.
     *
     * @param supGauche Le coin supérieur gauche.
     * @param infDroit  Le coin inférieur droit.
     * @param couleur   La couleur de remplissage.
     */
    public Rectangle2DPlein(Point2D supGauche,
                            Point2D infDroit,
                            Color couleur) {
        super(supGauche, infDroit);
        assert couleur != null;
        this.couleur = couleur;
    }

    /**
     * Renvoie la couleur.
     *
     * @return la couleur.
     */
    public Color getCouleur() {
        return couleur;
    }</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_du_polymorphisme"><a class="anchor" href="#_exemple_utilisation_du_polymorphisme"></a><a class="link" href="#_exemple_utilisation_du_polymorphisme">4.2.7. Exemple : utilisation du polymorphisme</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Création d'un tableau de références sur des Rectangle2D
final int NB_RECTANGLES = 2;
Rectangle2D[] figures = new Rectangle2D[NB_RECTANGLES];

// Un rectangle
figures[0] = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));

// Un rectangle plein
figures[1] = new Rectangle2DPlein(new Point2D(1.0, 3.0),
        new Point2D(3.0, 2.0),
        Color.BLUE);

// getDesc() de Rectangle2D
assert figures[0].getDesc().equals("O = (0.0, 5.0) L = 2.0 H = 3.0");

// getDesc() de Rectangle2DPlein
assert figures[1].getDesc().equals("O = (1.0, 3.0) L = 2.0 H = 1.0, couleur : (0, 0, 255)");</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_application_le_polymorphisme_et_la_redéfinition"><a class="anchor" href="#_application_le_polymorphisme_et_la_redéfinition"></a><a class="link" href="#_application_le_polymorphisme_et_la_redéfinition">4.2.8. Application : le polymorphisme et la redéfinition</a></h4>
<div class="paragraph">
<p>Une amélioration importante a été apportée aux robots: ils sont maintenant programmables.
Chaque type de robot possède son propre comportement.
Quand ils en reçoivent l&#8217;ordre, ils exécutent l&#8217;action programmée (un ensemble d&#8217;instructions élémentaires).
Plusieurs robots de types différents se trouvent sur le terrain.
On veut pouvoir déclencher l&#8217;exécution du programme de l&#8217;ensemble des robots.</p>
</div>
<div class="ulist">
<ul>
<li>
<p>Donner un diagramme de classe des robots</p>
</li>
<li>
<p>Implémenter les changements dans les classes <code>Robot</code>, <code>Transporteur</code> et <code>Destructeur</code></p>
</li>
<li>
<p>Écrire un programme déclenchant l&#8217;exécution de l&#8217;action pour l&#8217;ensemble des robots</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_la_classe_object"><a class="anchor" href="#_la_classe_object"></a><a class="link" href="#_la_classe_object">4.3. La classe <code>Object</code></a></h3>
<div class="sect3">
<h4 id="_la_classe_object_2"><a class="anchor" href="#_la_classe_object_2"></a><a class="link" href="#_la_classe_object_2">4.3.1. La classe <code>Object</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>La classe <code>Objet</code> définit et implémente le comportement dont chaque classe Java a besoin</p>
</li>
<li>
<p>C&#8217;est la plus générale des classes Java</p>
</li>
<li>
<p>Chaque classe Java hérite directement ou indirectement de <code>Object</code> (tout objet y compris les tableaux implémente les méthodes de <code>Object</code>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_méthodes_de_la_classe_object"><a class="anchor" href="#_les_méthodes_de_la_classe_object"></a><a class="link" href="#_les_méthodes_de_la_classe_object">4.3.2. Les méthodes de la classe <code>Object</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Certaines méthodes de <code>Object</code> peuvent être redéfinies pour s&#8217;adapter à la sous-classe</p>
</li>
<li>
<p><code>protected Object clone()</code> permet de dupliquer un objet</p>
</li>
<li>
<p><code>boolean equals(Object obj)</code> permet de tester l&#8217;égalité de deux objets et <code>int hashCode()</code> de renvoyer une valeur de hashage</p>
<div class="ulist">
<ul>
<li>
<p><code>Object.equals</code> teste l&#8217;identité</p>
</li>
<li>
<p><code>equals</code> et <code>hashCode</code> doivent être redéfinies ensembles</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>protected void finalize()</code> représente le destructeur d&#8217;un objet</p>
</li>
<li>
<p><code>String toString()</code> retourne une chaîne représentant l&#8217;objet</p>
<div class="ulist">
<ul>
<li>
<p><code>toString</code> est très utile pour le débogage &#8658; toujours la redéfinir</p>
</li>
</ul>
</div>
</li>
<li>
<p>Autres méthodes</p>
<div class="ulist">
<ul>
<li>
<p><code>Class getClass()</code> retourne un objet de type <code>Class</code> représentant la classe de l&#8217;objet</p>
<div class="ulist">
<ul>
<li>
<p>la classe <code>Class</code> est par exemple utile pour créer des objets dont la classe n&#8217;est pas connu à la compilation</p>
</li>
</ul>
</div>
</li>
<li>
<p>quelques méthodes pour les <em>threads</em></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2d"><a class="anchor" href="#_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2d"></a><a class="link" href="#_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2d">4.3.3. Exemple : redéfinition de la méthode <code>toString()</code> de <code>Rectangle2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Retourne une chaîne représentant l'objet.
 * @return la chaîne.
 */
@Override
public String toString() {
    return String.format("O = %s L = %s, H = %s", orig, getLargeur(), getHauteur());
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2dplein"><a class="anchor" href="#_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2dplein"></a><a class="link" href="#_exemple_redéfinition_de_la_méthode_tostring_de_rectangle2dplein">4.3.4. Exemple : redéfinition de la méthode <code>toString()</code> de <code>Rectangle2DPlein</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Retourn une chaîne représentant l'objet.
 *
 * @return la chaîne.
 */
@Override
public String toString() {
    return String.format("%s, couleur : %s", super.getDesc(), couleur);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Test de toString
assert figures[0].toString().equals("O = (0.0, 5.0) [5.0, 0.0] L = 2.0 H = 3.0");
assert figures[1].toString().equals("O = (1.0, 3.0) [3.1622776601683795, 0.3217505543966422] L = 2.0 H = 1.0 couleur = java.awt.Color[r=0,g=0,b=255]");</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_copie_dobjets"><a class="anchor" href="#_copie_dobjets"></a><a class="link" href="#_copie_dobjets">4.3.5. Copie d&#8217;objets</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;opération de copie peut avoir différentes sémantiques</p>
<div class="ulist">
<ul>
<li>
<p><em>copie profonde</em> (<em>deep copy</em>)</p>
</li>
<li>
<p><em>copie superficielle</em> (<em>shallow copy</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>La copie peut être obtenue de plusieurs manières</p>
<div class="ulist">
<ul>
<li>
<p>par un <em>constructeur de copie</em></p>
</li>
<li>
<p>par une méthode de classe (<em>méthode de fabrication</em>)</p>
</li>
<li>
<p>par clonage (implémentation de l&#8217;interface <code>Cloneable</code> et redéfinition de la méthode <code>Object.clone</code>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;usage de <code>clone</code> est déconseillée</p>
<div class="ulist">
<ul>
<li>
<p><a href="http://www.artima.com/intv/bloch13.html">Copy Constructor versus Cloning</a>, Josh Bloch, 2002</p>
</li>
<li>
<p><a href="https://programmingmitra.blogspot.fr/2017/01/Java-cloning-copy-constructor-versus-Object-clone-or-cloning.html">Java Cloning - Copy Constructor versus Cloning</a>, Naresh Joshi, 2017</p>
</li>
<li>
<p><a href="https://stackoverflow.com/questions/1106102/clone-vs-copy-constructor-vs-factory-method">clone() vs copy constructor vs factory method?</a>, stackoverflow, 2009</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_egalité_dobjets_la_méthode_equals"><a class="anchor" href="#_egalité_dobjets_la_méthode_equals"></a><a class="link" href="#_egalité_dobjets_la_méthode_equals">4.3.6. Egalité d&#8217;objets : la méthode <code>equals</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>La méthode <code>boolean equals(Object o)</code> teste l&#8217;égalité de deux objets</p>
</li>
<li>
<p>La méthode <code>equals</code> de la classe <code>Object</code> se contente de tester l&#8217;égalité des références des objets, i.e. l&#8217;identité</p>
</li>
<li>
<p>Il est donc en général nécessaire de redéfinir <code>equals</code> pour le test d&#8217;égalité</p>
</li>
<li>
<p>Rappel: l&#8217;opérateur <code>==</code> teste l&#8217;identité de ses opérandes, i.e. l&#8217;égalité des références</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_egalité_dobjets_contraintes_de_equals"><a class="anchor" href="#_egalité_dobjets_contraintes_de_equals"></a><a class="link" href="#_egalité_dobjets_contraintes_de_equals">4.3.7. Egalité d&#8217;objets : contraintes de <code>equals</code></a></h4>
<div class="ulist">
<ul>
<li>
<p><code>equals</code> implémente une relation d&#8217;équivalence pour des références d&#8217;objet non nulles</p>
<div class="ulist">
<ul>
<li>
<p><code>x.equals(x) == true</code></p>
</li>
<li>
<p><code>x.equals(y) == true</code> si et seulement si <code>y.equals(x) == true</code></p>
</li>
<li>
<p>si <code>x.equals(y) == true</code> et <code>y.equals(z) == true</code> alors <code>x.equals(z) == true</code></p>
</li>
<li>
<p><code>x.equals(null) == false</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Toute classe qui redéfinit <code>equals</code> doit également redéfinir <code>hashCode()</code></p>
<div class="ulist">
<ul>
<li>
<p>si deux objets sont égaux au sens de <code>equals</code> alors <code>hashCode</code> doit produire le même résultat pour les deux objets</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_égalité_de_rectangles"><a class="anchor" href="#_exemple_égalité_de_rectangles"></a><a class="link" href="#_exemple_égalité_de_rectangles">4.3.8. Exemple : égalité de rectangles</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.inheritance;

import javafx.geometry.Point2D;

// tag::rect[]
/**
 * Un rectangle en deux dimensions.
 * Les côtés du rectangle sont toujours parallèles aux axes.
 *
 * @version  Version 1.0
 * @author   Author1
 *
 */
class Rectangle2D extends FigureFermee2D implements Cloneable {
    /** Coordonnées du coin supérieur gauche */
    private Point2D orig;

    /** Coordonnées du coin inférieur droit */
    private Point2D fin;

    /**
     * Initialise le rectangle.
     * @param supGauche Le coin supérieur gauche.
     * @param infDroit Le coin inférieur droit.
     */
    public Rectangle2D(Point2D supGauche, Point2D infDroit) {
        assert supGauche.getX() &lt;= infDroit.getX() &amp;&amp;
               supGauche.getY() &gt;= infDroit.getY();
        orig = supGauche;
        fin = infDroit;
    }

    public Point2D getSupGauche() { return orig; }

    public double getLargeur() {
        return fin.getX() - orig.getX();
    }

    public double getHauteur() {
        return orig.getY() - fin.getY();
    }

    /**
     * Retourne une description du rectangle.
     * @return la description.
     */
    public String getDesc() {
        return String.format("O = %s L = %s, H = %s", orig, getLargeur(), getHauteur());
    }
// end::rect[]

    // tag::rect-tostring[]
    /**
     * Retourne une chaîne représentant l'objet.
     * @return la chaîne.
     */
    @Override
    public String toString() {
        return String.format("O = %s L = %s, H = %s", orig, getLargeur(), getHauteur());
    }
    // end::rect-tostring[]

    /**
     * Retourne une copie "profonde" de l'objet.
     * @return la copie.
     */
    @Override
    public Object clone() throws CloneNotSupportedException {
        Rectangle2D r = (Rectangle2D)super.clone();
        r.orig = new Point2D(orig.getX(), orig.getY());
        r.fin = new Point2D(fin.getX(), fin.getY());
        return r;
    }

    // tag::rect-equals[]
    /**
     * Teste l'égalité de deux rectangles.
     * @param obj le rectangle à comparer.
     * @return true si les objets sont égaux.
     */
    @Override
    public boolean equals(Object obj) {
        if (obj instanceof Rectangle2D) {
            Rectangle2D r = (Rectangle2D)obj;
            return orig.equals(r.orig) &amp;&amp; fin.equals(r.fin);
        }
        return false;
    }

    /**
     * Retourne une valeur de hashage pour l'objet.
     * @return la valeur de hashage.
     */
    @Override
    public int hashCode() {
        return orig.hashCode() ^ fin.hashCode();
    }
    // end::rect-equals[]

    // tag::rect-translate[]
    /**
     * Translate le rectangle.
     * @param dx déplacement en abscisse.
     * @param dy déplacement en ordonnées.
     */
    @Override
    public void translate(double dx, double dy) {
        orig.add(dx, dy);
        fin.add(dx, dy);
    }
    // end::rect-translate[]
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_contraintes_de_equals"><a class="anchor" href="#_exemple_contraintes_de_equals"></a><a class="link" href="#_exemple_contraintes_de_equals">4.3.9. Exemple : contraintes de <code>equals</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Rectangle2D r1 = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));
Rectangle2D r2 = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));
Rectangle2D r3 = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));
assert r1.equals(r1);    // Réflexivité
assert r1.equals(r2) &amp;&amp; r2.equals(r1); // Symétrie
assert r1.equals(r2) &amp;&amp; r2.equals(r3) &amp;&amp;
        !r1.equals(r3) == false; // Transitivité
assert r1.equals(null) == false;
assert r1.hashCode() == r2.hashCode();</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_classe_abstraite_en_java"><a class="anchor" href="#_classe_abstraite_en_java"></a><a class="link" href="#_classe_abstraite_en_java">4.4. Classe abstraite en Java</a></h3>
<div class="sect3">
<h4 id="_classe_abstraite_en_java_2"><a class="anchor" href="#_classe_abstraite_en_java_2"></a><a class="link" href="#_classe_abstraite_en_java_2">4.4.1. Classe abstraite en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une classe est spécifiée abstraite en ajoutant le mot-clé <code>abstract</code> dans sa déclaration</p>
</li>
<li>
<p>L&#8217;instanciation d&#8217;une telle classe est alors refusée par le compilateur</p>
</li>
<li>
<p>Une classe abstraite contient généralement des <em>méthodes abstraites</em>, i.e. qui ne possèdent pas d&#8217;implémentation</p>
<div class="ulist">
<ul>
<li>
<p>une classe abstraite peut cependant ne pas avoir de méthodes abstraites</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une méthode est déclarée abstraite en utilisant le mot-clé <code>abstract</code> lors de sa déclaration</p>
</li>
<li>
<p>Toute sous-classe non abstraite d&#8217;une classe abstraite doit redéfinir les méthodes abstraites de cette classe</p>
</li>
<li>
<p>Une classe possédant des méthodes abstraites est obligatoirement abstraite</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_hiérarchie_dhéritage_des_figures_2"><a class="anchor" href="#_exemple_la_hiérarchie_dhéritage_des_figures_2"></a><a class="link" href="#_exemple_la_hiérarchie_dhéritage_des_figures_2">4.4.2. Exemple : la hiérarchie d&#8217;héritage des figures</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/abstract_class.png" alt="abstract class" width="409" height="199">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_la_classe_abstraite_figurefermee2d"><a class="anchor" href="#_exemple_la_classe_abstraite_figurefermee2d"></a><a class="link" href="#_exemple_la_classe_abstraite_figurefermee2d">4.4.3. Exemple : la classe abstraite <code>FigureFermee2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.inheritance;

/**
 * Une figure fermée.
 *
 * @version  Version1
 * @author   Author1
 *
 */
abstract class FigureFermee2D {
    /**
     * Translate la figure.
     * @param dx déplacement en abscisse.
     * @param dy déplacement en ordonnée.
     */
    public abstract void translate(double dx, double dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_redéfinition_du_déplacement"><a class="anchor" href="#_exemple_redéfinition_du_déplacement"></a><a class="link" href="#_exemple_redéfinition_du_déplacement">4.4.4. Exemple : redéfinition du déplacement</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Translate le rectangle.
 * @param dx déplacement en abscisse.
 * @param dy déplacement en ordonnées.
 */
@Override
public void translate(double dx, double dy) {
    orig.add(dx, dy);
    fin.add(dx, dy);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Translate le cercle.
 *
 * @param dx déplacement en abscisse.
 * @param dy déplacement en ordonnées.
 */
@Override
public void translate(double dx, double dy) {
    centre.add(dx, dy);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_classe_abstraite_figurefermee2d"><a class="anchor" href="#_exemple_utilisation_de_la_classe_abstraite_figurefermee2d"></a><a class="link" href="#_exemple_utilisation_de_la_classe_abstraite_figurefermee2d">4.4.5. Exemple : utilisation de la classe abstraite <code>FigureFermee2D</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Création du tableau de références
final int NB_FIGURES = 4;
FigureFermee2D[] figures = new FigureFermee2D[NB_FIGURES];

// Création des formes
figures[0] = new Rectangle2D(new Point2D(0.0, 5.0),
        new Point2D(2.0, 2.0));
figures[1] = new Cercle2D(new Point2D(1.0, 2.0), 3.0);
figures[2] = new Rectangle2D(new Point2D(5.0, 5.0),
        new Point2D(7.0, 3.0));
figures[3] = new Cercle2D(new Point2D(4.0, 5.0), 2.0);

// Réalise une translation de la figure
for (int i = 0; i &lt; figures.length; ++i) {
    figures[i].translate(1.0, 2.0);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_application_les_classes_abstraites"><a class="anchor" href="#_application_les_classes_abstraites"></a><a class="link" href="#_application_les_classes_abstraites">4.4.6. Application : les classes abstraites</a></h4>
<div class="paragraph">
<p>On souhaite maintenant ajouter sur le terrain un type de case sensible à la charge (pont par exemple).
Chaque élément mobile (robot ou objet transportable) devra donc posséder un poids.
Le poids d&#8217;une instance de robot sera toujours de 1 unité.
Une instance de destructeur aura un poids de 2 unités de plus que le robot.
Une instance de transporteur aura un poids de 1 unités de plus que le robot auquel il faudra ajouter le poids de l&#8217;objet transporté.
Le poids par défaut des objets transportables est de 1 unité mais chaque objet pourra avoir un poids différent précisé lors de sa création.
On souhaite pouvoir connaître le poids de tout élément se trouvant sur le terrain.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Modéliser la prise en compte du poids au niveau des éléments mobiles</p>
</li>
<li>
<p>Implémenter les classes correspondantes</p>
</li>
</ol>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_la_classe_number"><a class="anchor" href="#_la_classe_number"></a><a class="link" href="#_la_classe_number">4.5. La classe <code>Number</code></a></h3>
<div class="sect3">
<h4 id="_la_classe_number_2"><a class="anchor" href="#_la_classe_number_2"></a><a class="link" href="#_la_classe_number_2">4.5.1. La classe <code>Number</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>La classe <code>Number</code> est une classe abstraite de la librairie Java</p>
</li>
<li>
<p>Elle définit le comportement commun aux classes pour la gestion des nombres (les conversions)</p>
</li>
<li>
<p>Elle possède plusieurs sous-classes</p>
<div class="ulist">
<ul>
<li>
<p>les adaptateurs : <code>Byte</code>, <code>Double</code>, <code>Float</code>, <code>Integer</code>, <code>Long</code>, <code>Short</code></p>
</li>
<li>
<p><code>BigDecimal</code>, <code>BigInteger</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Ces classes offrent une vue "objet" des types primitifs</p>
</li>
</ul>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
La plupart des fonctions arithmétiques sont des méthodes de classe de la classe <code>Math</code>.
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_autoboxingautounboxing"><a class="anchor" href="#_autoboxingautounboxing"></a><a class="link" href="#_autoboxingautounboxing">4.5.2. <em>autoboxing</em>/<em>autounboxing</em></a></h4>
<div class="ulist">
<ul>
<li>
<p>Ce mécanisme permet d&#8217;éviter la conversion manuelle entre type primitif et adaptateur</p>
</li>
<li>
<p>C&#8217;est simplement une facilité d&#8217;écriture (<em>sucre syntaxique</em>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Integer i = 12; // à la place de : Integer i = Integer.valueOf(12);
int n = i; // à la place de : int n = i.intValue();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_adaptateurs"><a class="anchor" href="#_les_adaptateurs"></a><a class="link" href="#_les_adaptateurs">4.5.3. Les <em>adaptateurs</em></a></h4>
<div class="ulist">
<ul>
<li>
<p>Il existe d&#8217;autres adaptateurs : <code>Boolean</code>, <code>Character</code>, <code>Void</code></p>
</li>
<li>
<p>Les adaptateurs sont des exemples du <a href="https://fr.wikipedia.org/wiki/Adaptateur_(patron_de_conception)"><em>pattern de conception Adaptateur</em></a></p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_interface"><a class="anchor" href="#_interface"></a><a class="link" href="#_interface">4.6. Interface</a></h3>
<div class="sect3">
<h4 id="_du_point_de_vue_des_types"><a class="anchor" href="#_du_point_de_vue_des_types"></a><a class="link" href="#_du_point_de_vue_des_types">4.6.1. Du point de vue des types</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>interface</em> regroupe uniquement des signatures d&#8217;opérations et des déclarations de constantes mais aucune implémentation</p>
</li>
<li>
<p>Une interface permet donc de définir un type</p>
</li>
<li>
<p>Les interfaces peuvent être organisées en hiérarchies</p>
</li>
<li>
<p>Un lien entre interface est une relation de sous-typage</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_du_point_de_vue_des_services"><a class="anchor" href="#_du_point_de_vue_des_services"></a><a class="link" href="#_du_point_de_vue_des_services">4.6.2. Du point de vue des services</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>interface</em> fournit une vue totale ou partielle d&#8217;un ensemble de services offerts par une classe (un composant)</p>
</li>
<li>
<p>Une interface est analogue à un protocole de comportement (un contrat sur un comportement)</p>
</li>
<li>
<p>Une classe peut <em>implémenter</em> une ou plusieurs interfaces</p>
</li>
<li>
<p>Une interface est formellement équivalente à une classe abstraite ne possédant que des méthodes abstraites</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dune_interface"><a class="anchor" href="#_utilisation_dune_interface"></a><a class="link" href="#_utilisation_dune_interface">4.6.3. Utilisation d&#8217;une interface</a></h4>
<div class="ulist">
<ul>
<li>
<p>Permet à des objets d&#8217;interagir même s&#8217;ils ne sont pas en relation</p>
</li>
<li>
<p>Permet de capturer des similarités entre classes non reliées sans définir artificiellement une relation</p>
</li>
<li>
<p>Permet de déclarer des méthodes qu&#8217;une ou plusieurs classes doivent implémenter</p>
</li>
<li>
<p>Permet de révéler l&#8217;interface de programmation d&#8217;un objet sans révéler sa classe</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_interface_et_implémentation_dinterface"><a class="anchor" href="#_exemple_interface_et_implémentation_dinterface"></a><a class="link" href="#_exemple_interface_et_implémentation_dinterface">4.6.4. Exemple : interface et implémentation d&#8217;interface</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/interface.png" alt="interface" width="275" height="384">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_définition_dune_interface_en_java"><a class="anchor" href="#_définition_dune_interface_en_java"></a><a class="link" href="#_définition_dune_interface_en_java">4.6.5. Définition d&#8217;une interface en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>La définition d&#8217;une interface comporte une déclaration et un corps</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">interface UneInterface extends UneSecondeInterface, UneAutreInterface {
  final String uneChaine = "abcde";
  final double unDouble = 123.456;
  void uneMethode(int unEntier, String uneChaine);
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Une interface peut avoir plusieurs super-interfaces</p>
</li>
<li>
<p>Toutes les méthodes de l&#8217;interface sont implicitement <code>public</code> et <code>abstract</code></p>
</li>
<li>
<p>Toutes les constantes de l&#8217;interface sont implicitement <code>public</code>, <code>static</code>, et <code>final</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dune_interface_2"><a class="anchor" href="#_utilisation_dune_interface_2"></a><a class="link" href="#_utilisation_dune_interface_2">4.6.6. Utilisation d&#8217;une interface</a></h4>
<div class="ulist">
<ul>
<li>
<p>Pour déclarer une classe qui implémente une ou plusieurs interfaces, on ajoute <code>implements ListeInterfaces</code> dans sa déclaration (après la clause <code>extends</code> si elle existe)</p>
</li>
<li>
<p>La classe doit alors implémenter toutes les méthodes de l&#8217;interface ou être déclarée abstraite</p>
</li>
<li>
<p>Une interface est utilisée comme un type (par exemple comme paramètre d&#8217;une méthode)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_définir_lordre_naturel_des_objets_interface_comparable"><a class="anchor" href="#_exemple_définir_lordre_naturel_des_objets_interface_comparable"></a><a class="link" href="#_exemple_définir_lordre_naturel_des_objets_interface_comparable">4.6.7. Exemple : définir l'<em>ordre naturel</em> des objets (interface <code>Comparable</code>)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Comparable est une interface de la librairie Java

/**
 * This interface imposes a total ordering on the objects
 * of each class that implements it. ...
 */
interface Comparable&lt;T&gt; {
  /**
   * Compares this object with the specified object for order. ...
   */
  public int compareTo(T o);
}

// ...
class Rectangle2D implements Comparable&lt;Rectangle2D&gt; {
  // ...
  public int compareTo(Rectangle2D o) {
    // Code pour la comparaison
  }
  // ...
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_java_3"><a class="anchor" href="#_exercices_java_3"></a><a class="link" href="#_exercices_java_3">4.7. Exercices (Java)</a></h3>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>Utilisation de l&#8217;environnement de développement <a href="https://www.bluej.org/">BlueJ</a></p>
</li>
<li>
<p>Les seules sources d&#8217;information externes autorisées sont</p>
<div class="ulist">
<ul>
<li>
<p>la référence de l&#8217;<a href="http://docs.oracle.com/javase/8/docs/api/">API Java</a>,</p>
</li>
<li>
<p>le <a href="http://docs.oracle.com/javase/tutorial/">tutoriel</a> Java,</p>
</li>
<li>
<p>la <a href="http://www.bluej.org/doc/documentation.html">documentation</a> de <a href="https://www.bluej.org/">BlueJ</a>.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="sect3">
<h4 id="_héritage_et_polymorphisme"><a class="anchor" href="#_héritage_et_polymorphisme"></a><a class="link" href="#_héritage_et_polymorphisme">4.7.1. Héritage et polymorphisme</a></h4>
<div class="paragraph">
<p>On souhaite réaliser une application pour gérer une collection de CD et de DVD.
Un CD possède un titre, le nom de l&#8217;artiste ou du groupe, et le nombre de titres.
Un DVD possède un titre, un réalisateur et une année de sortie.</p>
</div>
<div class="paragraph">
<p>L&#8217;application devra permettre de :</p>
</div>
<div class="ulist">
<ul>
<li>
<p>créer des documents (CD ou DVD),</p>
</li>
<li>
<p>consulter les informations d&#8217;un document,</p>
</li>
<li>
<p>ajouter un document dans la collection,</p>
</li>
<li>
<p>lister les documents de la collection,</p>
</li>
<li>
<p>rechercher les documents contenant un mot clé dans le titre ou dans le groupe/réalisateur.</p>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Donner un diagramme de classe UML modélisant ce problème.</p>
</li>
<li>
<p>Proposer une implémentation de cette modélisation.</p>
</li>
</ol>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_création_dune_classe_respectant_les_conventions_du_langage_java"><a class="anchor" href="#_création_dune_classe_respectant_les_conventions_du_langage_java"></a><a class="link" href="#_création_dune_classe_respectant_les_conventions_du_langage_java">4.7.2. Création d&#8217;une classe respectant les conventions du langage Java</a></h4>
<div class="paragraph">
<p>L&#8217;objectif de cet exercice est de réaliser une classe <strong>immuable</strong> <code>Fraction</code> qui représente un nombre rationnel.
  Un exemple d&#8217;interface pour une telle classe est donné par la classe <a href="http://commons.apache.org/proper/commons-math/javadocs/api-3.6.1/org/apache/commons/math3/fraction/Fraction.html"><code>Fraction</code></a> de la bibliothèque <a href="http://commons.apache.org/math/">Apache Commons Math</a>.</p>
</div>
<div class="paragraph">
<p>Une fraction comporte un numérateur et un dénominateur (nombres entiers).</p>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
Vous respecterez les conventions Java quand cela est approprié (égalité, conversion, comparaison, &#8230;&#8203;).
</td>
</tr>
</table>
</div>
<div class="paragraph">
<p>Implémentez la classe en fournissant l&#8217;interface suivante:</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>initialisation avec (i) un numérateur et un dénominateur, (ii) juste avec le numérateur (dénominateur égal à <em>1</em>) ou (iii) sans argument (numérateur égal <em>0</em> et dénominateur égal à <em>1</em>),</p>
</li>
<li>
<p>les constantes ZERO (0, 1) et UN (1, 1),</p>
</li>
<li>
<p>consultation du numérateur et du dénominateur,</p>
</li>
<li>
<p>consultation de la valeur sous la forme d&#8217;un nombre en virgule flottante (<code>double</code>),</p>
</li>
<li>
<p>addition de deux fractions,</p>
</li>
<li>
<p>test d&#8217;égalité entre fractions (deux fractions sont égales si elles représentent la même fraction réduite),</p>
</li>
<li>
<p>conversion en chaîne de caractères,</p>
</li>
<li>
<p>comparaison de fractions selon l&#8217;ordre naturel.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_héritage_polymorphisme_et_classe_abstraite"><a class="anchor" href="#_héritage_polymorphisme_et_classe_abstraite"></a><a class="link" href="#_héritage_polymorphisme_et_classe_abstraite">4.7.3. Héritage, polymorphisme et classe abstraite</a></h4>
<div class="paragraph">
<p>On veut simuler le fonctionnement d&#8217;un système de fichiers.
Un fichier est représenté par son nom et sa taille.
Un répertoire est défini par son nom et peut contenir des fichiers et/ou des répertoires.
La base de l&#8217;arborescence du système de fichier est le répertoire racine.</p>
</div>
<div class="paragraph">
<p>On veut pouvoir calculer la taille totale d&#8217;un répertoire.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Représenter sur un diagramme de classes UML une hiérarchie de classe modélisant ce problème. Le modèle de conception <a href="http://fr.wikipedia.org/wiki/Objet_composite">Composite</a> peut être utilisé pour cela.</p>
</li>
<li>
<p>Proposer une implémentation de ce modèle.</p>
</li>
<li>
<p>Créer une arborescence de test et vérifier le calcul de la taille.</p>
</li>
<li>
<p>Modifier le programme pour qu&#8217;un répertoire ne puisse pas être ajouté à lui-même.</p>
</li>
<li>
<p>Modifier le programme pour qu&#8217;un répertoire ne puisse pas être ajouté comme descendant de lui-même.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_de_la_ligne_de_commande"><a class="anchor" href="#_utilisation_de_la_ligne_de_commande"></a><a class="link" href="#_utilisation_de_la_ligne_de_commande">4.7.4. Utilisation de la ligne de commande</a></h4>
<div class="paragraph">
<p>Le but de cet exercice est de vous familiariser avec les outils Java en ligne de commande.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Créer le répertoire <code>FileSystem</code> contenant les sous-répertoires <code>src</code> et <code>classes</code>.</p>
</li>
<li>
<p>Placer les fichiers <code>.java</code> de l&#8217;exercice précédent dans le sous-répertoire <code>src</code>.</p>
</li>
<li>
<p>Compiler les sources en incluant les informations de débogage et de façon à placer les <code>.class</code> dans le répertoire <code>classes</code> (cf. <a href="http://docs.oracle.com/javase/8/docs/technotes/tools/unix/javac.html">documentation de <code>javac</a></code>).</p>
</li>
<li>
<p>Ajouter un programme principal contenant le code de test de l&#8217;exercice précédent et recompiler.</p>
</li>
<li>
<p>Exécuter le programme (cf. <a href="http://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html">documentation de <code>java</a></code>).</p>
</li>
<li>
<p>Créer une archive Java pour le programme (cf. <a href="http://docs.oracle.com/javase/8/docs/technotes/tools/unix/jar.html">documentation de <code>jar</a></code>) et exécuter à nouveau le programme à partir de l&#8217;archive.</p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_module_et_bibliothèques"><a class="anchor" href="#_module_et_bibliothèques"></a><a class="link" href="#_module_et_bibliothèques">5. Module et bibliothèques</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_module_en_java"><a class="anchor" href="#_module_en_java"></a><a class="link" href="#_module_en_java">5.1. Module en Java</a></h3>
<div class="sect3">
<h4 id="_définition_dun_module"><a class="anchor" href="#_définition_dun_module"></a><a class="link" href="#_définition_dun_module">5.1.1. Définition d&#8217;un module</a></h4>
<div class="ulist">
<ul>
<li>
<p>Pour créer un module ou y ajouter une classe ou une interface, on place une instruction <code>package</code> au début du fichier source</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package monpackage;</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Tout ce qui est défini dans le fichier source fait alors parti du module</p>
</li>
<li>
<p>Sans instruction de ce type, les éléments se trouvent dans le module par défaut (non nommé)</p>
</li>
<li>
<p>Les noms des modules respectent en général une convention (par exemple, <code>uvsq.in404.monpackage</code>)</p>
</li>
<li>
<p>La librairie Java est organisée en module (<code>java.lang</code>, <code>java.util</code>, <code>java.io</code>, \dots)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_interface_dun_module"><a class="anchor" href="#_interface_dun_module"></a><a class="link" href="#_interface_dun_module">5.1.2. Interface d&#8217;un module</a></h4>
<div class="ulist">
<ul>
<li>
<p>Seul les éléments publics sont accessibles à l&#8217;extérieur du module</p>
</li>
<li>
<p>Pour rendre une classe ou une interface publique, on spécifie le mot-clé <code>public</code> dans sa déclaration</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public class MaClasse { //...</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dun_module"><a class="anchor" href="#_utilisation_dun_module"></a><a class="link" href="#_utilisation_dun_module">5.1.3. Utilisation d&#8217;un module</a></h4>
<div class="ulist">
<ul>
<li>
<p>Différentes façons d&#8217;utiliser les éléments public d&#8217;un module</p>
<div class="ulist">
<ul>
<li>
<p>utiliser son nom qualifié (par exemple, <code>uvsq.in404.monpackage.MaClasse</code>)</p>
</li>
<li>
<p>importer l&#8217;élément (par exemple, <code>import uvsq.in404.monpackage.MaClasse;</code> placé en début de fichier source)</p>
</li>
<li>
<p>importer le module complet (par exemple, <code>import uvsq.in404.monpackage.*;</code> placé en début de fichier source)</p>
</li>
<li>
<p>importer les classes imbriquées (<code>import uvsq.in404.monpackage.MaClasse.*;</code>)</p>
</li>
<li>
<p>importer les membres de classes (<code>import static uvsq.in404.monpackage.MaClasse.*;</code>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Les directives <code>import</code> se placent avant toute définition de classes ou d&#8217;interfaces mais après l&#8217;instruction <code>package</code></p>
</li>
<li>
<p>Deux modules sont automatiquement importés : le module par défaut et <code>java.lang</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_module_et_gestion_des_sources_en_java"><a class="anchor" href="#_module_et_gestion_des_sources_en_java"></a><a class="link" href="#_module_et_gestion_des_sources_en_java">5.1.4. Module et gestion des sources en Java</a></h4>
<div class="ulist">
<ul>
<li>
<p>Dans un fichier source</p>
<div class="ulist">
<ul>
<li>
<p>plusieurs éléments (classes, interfaces, &#8230;&#8203;) peuvent être définies</p>
</li>
<li>
<p>un seul élément peut être public</p>
</li>
<li>
<p>le nom de l&#8217;élément public doit être le même que le nom du fichier</p>
</li>
</ul>
</div>
</li>
<li>
<p>On se limite de préférence à une classe par fichier source</p>
<div class="ulist">
<ul>
<li>
<p>le nom du fichier <code>.java</code> est le même que le nom de l&#8217;élément qu&#8217;il contient</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le nom du répertoire doit refléter le nom du paquetage</p>
<div class="ulist">
<ul>
<li>
<p>la classe <code>uvsq.in404.monpackage.MaClasse</code> doit se trouver dans le fichier <code>MaClasse.java</code> du répertoire <code>uvsq/in404/monpackage</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_module_et_compilation"><a class="anchor" href="#_module_et_compilation"></a><a class="link" href="#_module_et_compilation">5.1.5. Module et compilation</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lors de la compilation, un fichier <code>.class</code> est créé pour chaque élément</p>
</li>
<li>
<p>La hiérarchie de répertoires contenant les <code>.class</code> reflète les noms des modules</p>
</li>
<li>
<p>Les répertoires où sont recherchées les classes lors de l&#8217;exécution sont listés dans le <em>class path</em></p>
</li>
<li>
<p>Par défaut, le répertoire courant et la librairie Java se trouve dans le <em>class path</em></p>
</li>
<li>
<p>La façon dont le <em>class path</em> est défini dépend de la plateforme</p>
<div class="ulist">
<ul>
<li>
<p>en général, on définit une variable d&#8217;environnement <code>CLASSPATH</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Le <em>class path</em> contient des chemins vers</p>
<div class="ulist">
<ul>
<li>
<p>des répertoires contenant une arborescence de <code>.class</code></p>
</li>
<li>
<p>des fichiers <code>.jar</code></p>
</li>
<li>
<p>des fichiers <code>.zip</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_bibliothèques_en_java"><a class="anchor" href="#_bibliothèques_en_java"></a><a class="link" href="#_bibliothèques_en_java">5.2. Bibliothèques en Java</a></h3>
<div class="sect3">
<h4 id="_écosystème_java_et_bibliothèques"><a class="anchor" href="#_écosystème_java_et_bibliothèques"></a><a class="link" href="#_écosystème_java_et_bibliothèques">5.2.1. Écosystème Java et bibliothèques</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;écosystème Java fournit un nombre important de bibliothèques et d&#8217;outils de développement</p>
</li>
<li>
<p>Dans un projet de développement logiciel, le choix des bibliothèques à utiliser est une étape importante</p>
<div class="ulist">
<ul>
<li>
<p>fonctionnalités, complexité, support de la communauté, licence, &#8230;&#8203;</p>
</li>
</ul>
</div>
</li>
<li>
<p>La plupart des programmes Java font appel à des <em>bibliothèques tierces</em> (<em>third party libraries</em>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dun_bibliothèque_tierce"><a class="anchor" href="#_utilisation_dun_bibliothèque_tierce"></a><a class="link" href="#_utilisation_dun_bibliothèque_tierce">5.2.2. Utilisation d&#8217;un bibliothèque tierce</a></h4>
<div class="ulist">
<ul>
<li>
<p>Récupérer la bibliothèque</p>
<div class="ulist">
<ul>
<li>
<p>manuellement (téléchargement)</p>
</li>
<li>
<p>automatiquement (outils de gestion des dépendances comme <em>maven</em> ou <em>gradle</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Inclure la bibliothèque dans le projet</p>
<div class="ulist">
<ul>
<li>
<p>le <code>CLASSPATH</code> doit être modifié pour faire référence aux archives (<code>jar</code> en général) de la bibliothèque</p>
</li>
</ul>
</div>
</li>
<li>
<p>Consulter l&#8217;interface de la bibliothèque</p>
<div class="ulist">
<ul>
<li>
<p>toute bibliothèque Java est distribuée avec sa documentation au format <em>javadoc</em></p>
</li>
</ul>
</div>
</li>
<li>
<p>Importer les modules nécessaires dans les fichiers sources</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;utilisation d&#8217;une classe de la bibliothèque nécessite d&#8217;importer le package Java adéquat</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_bibliothèque_apache_commons_math_14"><a class="anchor" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_14"></a><a class="link" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_14">5.2.3. Exemple : utilisation de la bibliothèque <em>Apache Commons Math</em> 1/4</a></h4>
<div class="ulist">
<ul>
<li>
<p>Télécharger et décompresser le fichier <a href="http://commons.apache.org/proper/commons-math/download_math.cgi">commons-math3-3.6.1-bin.tar.gz</a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">~/commons-math3-3.4.1 $ ls
commons-math3-3.4.1.jar          docs/        NOTICE.txt
commons-math3-3.4.1-javadoc.jar  LICENSE.txt  RELEASE-NOTES.txt</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_bibliothèque_apache_commons_math_24"><a class="anchor" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_24"></a><a class="link" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_24">5.2.4. Exemple : utilisation de la bibliothèque <em>Apache Commons Math</em> 2/4</a></h4>
<div class="ulist">
<ul>
<li>
<p>Ajouter la bibliothèque au projet (IDE ou outil de <em>build</em>)</p>
</li>
</ul>
</div>
<div class="imageblock">
<div class="content">
<img src="figs/bluej-3rdparty.png" alt="bluej 3rdparty">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_bibliothèque_apache_commons_math_34"><a class="anchor" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_34"></a><a class="link" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_34">5.2.5. Exemple : utilisation de la bibliothèque <em>Apache Commons Math</em> 3/4</a></h4>
<div class="ulist">
<ul>
<li>
<p>Importer les classes des packages nécessaires</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">import org.apache.commons.math3.fraction.Fraction;

public class Main {
    public static void main(String[] args) {
        Fraction f = new Fraction(1, 3);
        System.out.println(f);
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_utilisation_de_la_bibliothèque_apache_commons_math_44"><a class="anchor" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_44"></a><a class="link" href="#_exemple_utilisation_de_la_bibliothèque_apache_commons_math_44">5.2.6. Exemple : utilisation de la bibliothèque <em>Apache Commons Math</em> 4/4</a></h4>
<div class="ulist">
<ul>
<li>
<p>Compiler en précisant la bibliothèque dans le CLASSPATH (en ligne de commande)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ javac -cp ../commons-math3-3.6.1/commons-math3-3.6.1.jar Main.java</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Éxécuter en précisant la bibliothèque dans le CLASSPATH (en ligne de commande)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="bash" class="language-bash hljs">$ java -cp ../commons-math3-3.6.1/commons-math3-3.6.1.jar:. Main</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_java_4"><a class="anchor" href="#_exercices_java_4"></a><a class="link" href="#_exercices_java_4">5.3. Exercices (Java)</a></h3>
<div class="sect3">
<h4 id="_module_et_bibliothèque"><a class="anchor" href="#_module_et_bibliothèque"></a><a class="link" href="#_module_et_bibliothèque">5.3.1. Module et bibliothèque</a></h4>
<div class="paragraph">
<p>Dans cet exercice, vous reprendrez le code source de l&#8217;exercice <em>simulation de client/serveur</em>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Placez l&#8217;ensemble du code source dans le package <code>in404.exo61</code>.</p>
</li>
<li>
<p>Ajoutez une classe contenant le programme principal qui implémentera le scénario de la question 1 de l&#8217;exercice.</p>
</li>
<li>
<p>Déplacez la classe <code>Client</code> dans le package <code>in404.exo61.client</code> et la classe <code>Serveur</code> dans le package <code>in404.exo61.serveur</code>. Apportez les modifications nécessaires au programme principal.</p>
</li>
<li>
<p>Construisez une archive <code>jar</code> contenant les classes compilées <code>in404.exo61.client.Client</code> et <code>in404.exo61.serveur.Serveur</code>. Modifiez le projet pour qu&#8217;il utilise cette bibliothèque.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_dune_bibliothèque_tierce"><a class="anchor" href="#_utilisation_dune_bibliothèque_tierce"></a><a class="link" href="#_utilisation_dune_bibliothèque_tierce">5.3.2. Utilisation d&#8217;une bibliothèque tierce</a></h4>
<div class="paragraph">
<p>Vous utiliserez ici la bibliothèque <a href="http://commons.apache.org/proper/commons-math/">Apache Commons Math</a>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>En consultant la documentation Javadoc sur le site, identifiez la classe (et son package) permettant la manipulation de nombres complexes.</p>
</li>
<li>
<p>Ajoutez la bibliothèque à votre projet.</p>
</li>
<li>
<p>Écrivez un programme principal pour tester quelques méthodes de la classe.</p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_gestion_derreurs_et_exceptions"><a class="anchor" href="#_gestion_derreurs_et_exceptions"></a><a class="link" href="#_gestion_derreurs_et_exceptions">6. Gestion d&#8217;erreurs et exceptions</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_les_erreurs_en_programmation"><a class="anchor" href="#_les_erreurs_en_programmation"></a><a class="link" href="#_les_erreurs_en_programmation">6.1. Les erreurs en programmation</a></h3>
<div class="sect3">
<h4 id="_les_erreurs_sont_communes"><a class="anchor" href="#_les_erreurs_sont_communes"></a><a class="link" href="#_les_erreurs_sont_communes">6.1.1. Les erreurs sont communes</a></h4>
<div class="paragraph">
<p>Des erreurs se produisent lors de l&#8217;exécution d&#8217;un programme</p>
</div>
<div class="ulist">
<div class="title">Différents types d&#8217;erreurs</div>
<ul>
<li>
<p>Erreurs de syntaxe</p>
<div class="ulist">
<ul>
<li>
<p>détectées par le compilateur</p>
</li>
</ul>
</div>
</li>
<li>
<p>Erreurs d&#8217;exécution</p>
<div class="ulist">
<ul>
<li>
<p>générées par l&#8217;environnement (plus de mémoire disponible, division par zéro, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Erreurs de logique (<em>bogues</em>)</p>
<div class="ulist">
<ul>
<li>
<p>liées à une erreur du développeur</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_plusieurs_questions_à_se_poser"><a class="anchor" href="#_plusieurs_questions_à_se_poser"></a><a class="link" href="#_plusieurs_questions_à_se_poser">6.1.2. Plusieurs questions à se poser</a></h4>
<div class="ulist">
<ul>
<li>
<p>Que considère-t&#8217;on comme une erreur ?</p>
</li>
<li>
<p>Quelle est la gravité de l&#8217;erreur ?</p>
</li>
<li>
<p>Comment détecter l&#8217;erreur ?</p>
</li>
<li>
<p>Comment propager l&#8217;information sur l&#8217;erreur ?</p>
</li>
<li>
<p>Comment et où gérer l&#8217;erreur ?</p>
</li>
<li>
<p>Comment signaler l&#8217;erreur ?</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quest_ce_quune_erreur"><a class="anchor" href="#_quest_ce_quune_erreur"></a><a class="link" href="#_quest_ce_quune_erreur">6.1.3. Qu&#8217;est-ce qu&#8217;une erreur ?</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un événement dans une fonction <em>f</em> est une erreur dans l&#8217;un des cas suivants :</p>
<div class="ulist">
<ul>
<li>
<p>il viole une des préconditions de <em>f</em>,</p>
<div class="ulist">
<ul>
<li>
<p>peut être considéré comme une erreur de programmation &#8658; utilisation des assertions</p>
</li>
</ul>
</div>
</li>
<li>
<p>il empêche <em>f</em> de remplir une des préconditions de ses appelés,</p>
</li>
<li>
<p>il empêche de réaliser une postcondition de <em>f</em>,</p>
</li>
<li>
<p>il empêche <em>f</em> de rétablir un invariant dont elle a la responsabilité.</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
Les autres événements ne doivent pas être considérés comme des erreurs
</td>
</tr>
</table>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_gestion_derreurs"><a class="anchor" href="#_gestion_derreurs"></a><a class="link" href="#_gestion_derreurs">6.2. Gestion d&#8217;erreurs</a></h3>
<div class="sect3">
<h4 id="_erreur_vs_bogue"><a class="anchor" href="#_erreur_vs_bogue"></a><a class="link" href="#_erreur_vs_bogue">6.2.1. Erreur vs. bogue</a></h4>
<div class="ulist">
<ul>
<li>
<p>La <em>gestion d&#8217;erreurs</em> est chargée des erreurs d&#8217;exécution</p>
</li>
<li>
<p>Les erreurs de logique (bogues) doivent être éliminées durant le développement en utilisant :</p>
<div class="ulist">
<ul>
<li>
<p>les <em>assertions</em></p>
</li>
<li>
<p>le <em>débogage</em></p>
</li>
<li>
<p>les <em>tests</em></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_réaction_à_une_erreur"><a class="anchor" href="#_réaction_à_une_erreur"></a><a class="link" href="#_réaction_à_une_erreur">6.2.2. Réaction à une erreur</a></h4>
<div class="ulist">
<ul>
<li>
<p>Ignorer le problème</p>
<div class="ulist">
<ul>
<li>
<p>en général, c&#8217;est une mauvaise idée&#8230;&#8203;</p>
</li>
</ul>
</div>
</li>
<li>
<p>Retourner un code d&#8217;erreur</p>
<div class="ulist">
<ul>
<li>
<p>possible si une valeur de retour est disponible pour cela</p>
</li>
</ul>
</div>
</li>
<li>
<p>Utiliser une variable globale</p>
<div class="ulist">
<ul>
<li>
<p>son état doit être consulté</p>
</li>
</ul>
</div>
</li>
<li>
<p>Lancer une exception</p>
<div class="ulist">
<ul>
<li>
<p>propage l&#8217;erreur selon la pile d&#8217;appel du programme</p>
</li>
</ul>
</div>
</li>
<li>
<p>Utiliser le <em>type `Option`</em></p>
<div class="ulist">
<ul>
<li>
<p>technique issue de la programmation fonctionnelle</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_retourner_un_code_derreur"><a class="anchor" href="#_retourner_un_code_derreur"></a><a class="link" href="#_retourner_un_code_derreur">6.2.3. Retourner un code d&#8217;erreur</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static double sqrtWithReturnCode(double d) {
    return Double.isNaN(d) || d &lt; 0.0 ?
            Double.NaN :
            sqrt(d);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">double result = sqrtWithReturnCode(value);
if (Double.isNaN(result)) {
    System.err.println("Argument illégal (négatif ou égal à NaN).");
} else {
    System.out.printf("sqrt(%f) = %f\n", value, result);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_utiliser_une_variable_globale"><a class="anchor" href="#_utiliser_une_variable_globale"></a><a class="link" href="#_utiliser_une_variable_globale">6.2.4. Utiliser une variable globale</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static enum SqrtError { None, NegArg, NaNArg; }
private static SqrtError sqrtError = SqrtError.None;
public static SqrtError getSqrtError() { return sqrtError; }
public static double sqrtWithGlobalCode(double d) {
    if (Double.isNaN(d)) {
        sqrtError = SqrtError.NaNArg;
    } else if (d &lt; 0) {
        sqrtError = SqrtError.NegArg;
    }
    return sqrt(d);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">double result = sqrtWithGlobalCode(value);
if (getSqrtError() != SqrtError.None) {
    System.err.println("Argument illégal (négatif ou égal à NaN).");
} else {
    System.out.printf("sqrt(%f) = %f\n", value, result);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_lancer_une_exception"><a class="anchor" href="#_lancer_une_exception"></a><a class="link" href="#_lancer_une_exception">6.2.5. Lancer une exception</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static double sqrtWithException(double d) {
    if (Double.isNaN(d) || d &lt; 0.0) {
        throw new IllegalArgumentException("Argument négatif ou NaN");
    }
    return sqrt(d);
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">double result;
try {
    result = sqrtWithException(value);
    System.out.printf("sqrt(%f) = %f\n", value, result);
} catch (IllegalArgumentException ex) {
    ex.printStackTrace(System.err);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_utiliser_le_type_option"><a class="anchor" href="#_utiliser_le_type_option"></a><a class="link" href="#_utiliser_le_type_option">6.2.6. Utiliser le type <code>Option</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static Optional&lt;Double&gt; sqrtWithOption(double d) {
    return Double.isNaN(d) || d &lt; 0.0 ?
            Optional.empty() :
            Optional.of(sqrt(d));
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Optional&lt;Double&gt; result = sqrtWithOption(value);
System.out.printf("sqrt(%f) = %f\n", value, result.orElse(Double.NaN));</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exceptions"><a class="anchor" href="#_exceptions"></a><a class="link" href="#_exceptions">6.3. Exceptions</a></h3>
<div class="sect3">
<h4 id="_définition"><a class="anchor" href="#_définition"></a><a class="link" href="#_définition">6.3.1. Définition</a></h4>
<div class="ulist">
<ul>
<li>
<p>Le terme <em>exception</em> est un raccourci pour <em>événement exceptionnel</em></p>
</li>
<li>
<p>Une <em>exception</em> est un événement se produisant lors de l&#8217;exécution d&#8217;un programme et qui bouleverse le flôt normal d&#8217;instructions</p>
</li>
<li>
<p>Le mécanisme des exceptions est destiné à gérer les erreurs ou les cas exceptionnels (une partie du système n&#8217;a pas pu réaliser ce qui lui était demandé)</p>
<div class="ulist">
<ul>
<li>
<p>"Exceptionnel" ne signifie pas "qui ne se produit presque jamais" ou "désastreux"</p>
</li>
</ul>
</div>
</li>
<li>
<p>Différents types d&#8217;erreurs peuvent générer des exceptions</p>
</li>
<li>
<p>Une exception contient des informations sur l&#8217;erreur qui l&#8217;a produite</p>
</li>
<li>
<p>Les exceptions peuvent être regroupées et organisées en hiérarchie</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_fonctionnement"><a class="anchor" href="#_fonctionnement"></a><a class="link" href="#_fonctionnement">6.3.2. Fonctionnement</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;action de générer une exception s&#8217;appelle <em>lancer</em> (<em>throw</em>) ou <em>lever</em> (<em>raise</em>) une exception</p>
</li>
<li>
<p>Le système d&#8217;exécution doit alors trouver une portion de code sachant <em>gérer</em> (<em>handle</em>) ou <em>capturer</em> (<em>catch</em>) cette exception</p>
</li>
<li>
<p>Les candidats pour la gestion de l&#8217;exception sont les méthodes de la pile d&#8217;appel</p>
</li>
<li>
<p>Le système d&#8217;exécution remonte la pile d&#8217;appel jusqu&#8217;à trouver un <em>gestionnaire d&#8217;exception</em> (<em>exception handler</em>) approprié</p>
</li>
<li>
<p>Chaque gestionnaire d&#8217;exception gère un type d&#8217;exception particulier</p>
</li>
<li>
<p>Le gestionnaire d&#8217;exception choisi par le système traite l&#8217;exception</p>
</li>
<li>
<p>Si aucun gestionnaire approprié n&#8217;est trouvé, le système stoppe le programme</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_remarques"><a class="anchor" href="#_remarques"></a><a class="link" href="#_remarques">6.3.3. Remarques</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une exception peut être <em>redéclenchée</em></p>
</li>
<li>
<p>un gestionnaire d&#8217;exceptions peut faire un traitement partiel puis "passer la main"</p>
</li>
<li>
<p>L&#8217;ordre des gestionnaires est important</p>
<div class="ulist">
<ul>
<li>
<p>toujours du plus spécialisé au plus général</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_avantages_des_exceptions"><a class="anchor" href="#_avantages_des_exceptions"></a><a class="link" href="#_avantages_des_exceptions">6.3.4. Avantages des exceptions</a></h4>
<div class="ulist">
<ul>
<li>
<p>Séparation du code de gestion d&#8217;erreurs et du code "normal"</p>
<div class="ulist">
<ul>
<li>
<p>évite les "empilements" d&#8217;instructions conditionnelles</p>
</li>
<li>
<p>améliore la lisibilité du code</p>
</li>
</ul>
</div>
</li>
<li>
<p>Propagation des erreurs en suivant la pile d&#8217;appels de méthodes</p>
<div class="ulist">
<ul>
<li>
<p>simplification de la propagation</p>
</li>
<li>
<p>les méthodes que l&#8217;erreur ne concerne pas n&#8217;en tiennent pas compte</p>
</li>
</ul>
</div>
</li>
<li>
<p>Regroupement des types d&#8217;erreurs</p>
<div class="ulist">
<ul>
<li>
<p>possibilité de gérer ensemble des exceptions de même type</p>
</li>
<li>
<p>par exemple, exceptions concernant un tableau ou un fichier</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<strong>La gestion d&#8217;erreurs reste une tâche difficile !</strong>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_inconvénients_des_exceptions"><a class="anchor" href="#_inconvénients_des_exceptions"></a><a class="link" href="#_inconvénients_des_exceptions">6.3.5. Inconvénients des exceptions</a></h4>
<div class="ulist">
<ul>
<li>
<p>Moins structurées qu&#8217;une gestion locale</p>
<div class="ulist">
<ul>
<li>
<p>revers de la séparation code de gestion d&#8217;erreurs/code normal</p>
</li>
</ul>
</div>
</li>
<li>
<p>Moins efficace</p>
<div class="ulist">
<ul>
<li>
<p>le mécanisme de propagation a un coût</p>
</li>
</ul>
</div>
</li>
<li>
<p>Peut rendre certaines situations complexes</p>
</li>
</ul>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
<strong>Le mécanisme des exceptions offre une alternative aux techniques traditionnelles lorsque celles-ci se révèlent insuffisantes, peu élégantes et susceptibles d&#8217;introduire des erreurs</strong>
</td>
</tr>
</table>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exceptions_en_java"><a class="anchor" href="#_exceptions_en_java"></a><a class="link" href="#_exceptions_en_java">6.4. Exceptions en Java</a></h3>
<div class="sect3">
<h4 id="_généralités_2"><a class="anchor" href="#_généralités_2"></a><a class="link" href="#_généralités_2">6.4.1. Généralités</a></h4>
<div class="ulist">
<ul>
<li>
<p>Trois catégories d&#8217;exceptions</p>
<div class="ulist">
<ul>
<li>
<p>une <em>exception non contrôlée</em> (<em>unchecked exceptions</em>) n&#8217;est pas destinée à être traitée par le
programme</p>
<div class="ulist">
<ul>
<li>
<p>une <em>erreur</em> (<em>error</em>) a une cause externe à l&#8217;application</p>
</li>
<li>
<p>une <em>exception d&#8217;exécution</em> (<em>runtime exception</em>) est provoquée par la JVM</p>
</li>
</ul>
</div>
</li>
<li>
<p>une <em>exception contrôlée</em> (<em>checked exception</em>) est une exception qui n&#8217;est pas lancée par le système d&#8217;exécution Java (<em>runtime exception</em>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une exception est une instance d&#8217;une classe dérivée de <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Throwable.html"><code>Throwable</code></a></p>
</li>
<li>
<p>Une méthode doit soit <em>traiter</em>, soit <em>spécifier</em> toute <em>exception contrôlée</em> qui peut se produire dans cette méthode</p>
<div class="ulist">
<ul>
<li>
<p><em>traiter</em> = fournir un gestionnaire d&#8217;exception pour ce type d&#8217;exception</p>
</li>
<li>
<p><em>spécifier</em> = préciser dans sa signature qu&#8217;elle peut la lancer</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le compilateur ne requiert pas que les exceptions du système d&#8217;exécution soient traitée ou spécifiée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_le_traitement_dune_exception_comprend"><a class="anchor" href="#_le_traitement_dune_exception_comprend"></a><a class="link" href="#_le_traitement_dune_exception_comprend">6.4.2. Le traitement d&#8217;une exception comprend</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un bloc <code>try</code></p>
<div class="ulist">
<ul>
<li>
<p>autour de la séquence d&#8217;instructions susceptible de lancer une exception</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un ou plusieurs blocs <code>catch</code></p>
<div class="ulist">
<ul>
<li>
<p>représentant les gestionnaires d&#8217;exceptions</p>
</li>
</ul>
</div>
</li>
<li>
<p>Au plus un bloc <code>finally</code></p>
<div class="ulist">
<ul>
<li>
<p>toujours exécuté</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_le_bloc_try"><a class="anchor" href="#_le_bloc_try"></a><a class="link" href="#_le_bloc_try">6.4.3. Le bloc <code>try</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Le bloc <code>try</code> englobe les instructions susceptibles de lancer une exception</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">try {
    // Instructions
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;instruction <code>try</code> <em>gouverne</em> les instructions englobées</p>
</li>
<li>
<p>Il définit la portée des gestionnaires d&#8217;exceptions qui lui sont associés</p>
</li>
<li>
<p>Une instruction <code>try</code> <strong>doit</strong> être accompagnée d&#8217;au moins un bloc <code>catch</code> ou <code>finally</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_blocs_catch"><a class="anchor" href="#_les_blocs_catch"></a><a class="link" href="#_les_blocs_catch">6.4.4. Les blocs <code>catch</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Les blocs <code>catch</code> représentent les gestionnaires d&#8217;exceptions</p>
</li>
<li>
<p>Un ou plusieurs blocs <code>catch</code> sont placés immédiatement après un bloc <code>try</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">try {
    // Instructions
} catch ( /* ... */ ) {
    // Instructions
} catch ( /* ... */ ) {
    // Instructions
} // ...</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Les blocs <code>catch</code> doivent être ordonnés du plus spécialisé au plus général</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_détail_dun_bloc_catch"><a class="anchor" href="#_détail_dun_bloc_catch"></a><a class="link" href="#_détail_dun_bloc_catch">6.4.5. Détail d&#8217;un bloc <code>catch</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;instruction <code>catch</code> requiert un unique paramètre</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">catch (&lt;Type&gt; &lt;variable&gt;) {
    // Instructions
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><code>&lt;Type&gt;</code> représente le type de l&#8217;exception et doit être une classe dérivant de <code>Throwable</code></p>
</li>
<li>
<p><code>&lt;variable&gt;</code> est le nom de la variable liée à l&#8217;exception (locale au gestionnaire)</p>
</li>
<li>
<p>L&#8217;argument du <code>catch</code> ressemble à la déclaration d&#8217;un paramètre de méthode</p>
</li>
<li>
<p>Un gestionnaire peut capturer plusieurs types d&#8217;exceptions</p>
<div class="ulist">
<ul>
<li>
<p>en capturant une superclasse pour une exception</p>
</li>
<li>
<p>en utilisant plusieurs types dans la clause <code>catch</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">catch (Type1|Type2|Type3 ex) { //...</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_le_bloc_finally"><a class="anchor" href="#_le_bloc_finally"></a><a class="link" href="#_le_bloc_finally">6.4.6. Le bloc <code>finally</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Le bloc <code>finally</code> founit un mécanisme pour "nettoyer" l&#8217;état du programme</p>
</li>
<li>
<p>Les instructions du bloc <code>finally</code> sont toujours exécutées</p>
</li>
<li>
<p>Le bloc <code>finally</code> se place après les gestionnaires d&#8217;exceptions du bloc <code>try</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">finally {
    // Instructions
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_des_gestionnaires_dexception_pour_une_pile"><a class="anchor" href="#_des_gestionnaires_dexception_pour_une_pile"></a><a class="link" href="#_des_gestionnaires_dexception_pour_une_pile">6.4.7. Des gestionnaires d&#8217;exception pour une pile</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">try {
    Pile unePile = new Pile(2);
    unePile.empile("azerty");
    unePile.empile("qsdfgh");
    unePile.empile("wxcvbn");
    assert false : "Jamais atteint";
    String str = (String) unePile.depile();
} catch (PileVideException e) {
    assert e.getMessage().equals("La Pile est vide");
} catch (PileException e) {
    assert e.getMessage().equals("La Pile est pleine");
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exception_et_allocation_de_ressources"><a class="anchor" href="#_exception_et_allocation_de_ressources"></a><a class="link" href="#_exception_et_allocation_de_ressources">6.4.8. Exception et allocation de ressources</a></h4>
<div class="ulist">
<ul>
<li>
<p>La construction <em>try-with-resources</em> gère automatiquement la fermeture des ressources</p>
</li>
<li>
<p>Les classes représentant les ressources doivent implémenter l&#8217;interface <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/AutoCloseable.html"><code>AutoCloseable</code></a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">try (
    java.util.zip.ZipFile zf =
       new java.util.zip.ZipFile(zipFileName);
    java.io.BufferedWriter writer =
       java.nio.file.Files.newBufferedWriter(outputFilePath, charset)
) {
    // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_spécification_dexceptions"><a class="anchor" href="#_spécification_dexceptions"></a><a class="link" href="#_spécification_dexceptions">6.4.9. Spécification d&#8217;exceptions</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>spécification d&#8217;exception</em> précise qu&#8217;une méthode ne capture pas l&#8217;exception considérée mais peut la lancer</p>
</li>
<li>
<p>Pour spécifier qu&#8217;une ou plusieurs exceptions peuvent être lancées par une méthode, on utilise la clause <code>throws</code> dans la signature de la méthode</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">TypeRetour nomMethode throws Type1Exception, Type2Exception {
    //...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_spécification_dexceptions_pour_la_pile"><a class="anchor" href="#_spécification_dexceptions_pour_la_pile"></a><a class="link" href="#_spécification_dexceptions_pour_la_pile">6.4.10. Spécification d&#8217;exceptions pour la pile</a></h4>
<div class="listingblock">
<div class="title"><code>empile</code> peut lancer une exception de type <code>PilePleineException</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Empile un élément au sommet de la pile.
 *
 * @param unObjet l'objet à empiler
 * @throws PilePleineException s'il n'y a plus de place
 */
public void empile(Object unObjet) throws PilePleineException {</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title"><code>depile</code> peut lancer une exception de type <code>PileVideException</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Dépile l'élément se trouvant au sommet de la pile.
 *
 * @return l'élément au sommet
 * @throws PileVideException s'il n'y a pas d'élément
 */
public Object depile() throws PileVideException {</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_lancement_dexceptions"><a class="anchor" href="#_lancement_dexceptions"></a><a class="link" href="#_lancement_dexceptions">6.4.11. Lancement d&#8217;exceptions</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;instruction <code>throw</code> est utilisée pour lancer une exception</p>
</li>
<li>
<p>Le mot-clé <code>throw</code> doit être suivi d&#8217;une instance d&#8217;une classe dérivée de <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Throwable.html"><code>Throwable</code></a></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">throw new ClasseDerivéeDeThrowable();</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Une exception peut être relancée à partir d&#8217;un bloc <code>catch</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_lancements_dexceptions_pour_la_pile"><a class="anchor" href="#_lancements_dexceptions_pour_la_pile"></a><a class="link" href="#_lancements_dexceptions_pour_la_pile">6.4.12. Lancements d&#8217;exceptions pour la pile</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Empile un élément au sommet de la pile.
 *
 * @param unObjet l'objet à empiler
 * @throws PilePleineException s'il n'y a plus de place
 */
public void empile(Object unObjet) throws PilePleineException {
    if (sommet == contenu.length) {
        throw new PilePleineException();
    }
    contenu[sommet++] = unObjet;
}

/**
 * Dépile l'élément se trouvant au sommet de la pile.
 *
 * @return l'élément au sommet
 * @throws PileVideException s'il n'y a pas d'élément
 */
public Object depile() throws PileVideException {
    if (sommet == 0) {
        throw new PileVideException();
    }
    return contenu[--sommet];
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_la_classe_throwable"><a class="anchor" href="#_la_classe_throwable"></a><a class="link" href="#_la_classe_throwable">6.4.13. La classe <code>Throwable</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>La classe <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Throwable.html"><code>Throwable</code></a> est la super-classe de toutes les exceptions ou erreurs du langage Java</p>
</li>
<li>
<p>Seules les instances de cette classe (ou d&#8217;une de ses sous-classe) peuvent être lancées</p>
</li>
<li>
<p>Seule cette classe (ou l&#8217;une de ses sous-classe) peut être l&#8217;argument d&#8217;un <code>catch</code></p>
</li>
<li>
<p>Contient un instantané de la <em>pile d&#8217;exécution</em> au moment de la création de l&#8217;instance</p>
</li>
<li>
<p>Peut contenir une <em>cause</em> (une autre instance de <code>Throwable</code>) afin de gérer une <em>chaîne d&#8217;exceptions</em></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_méthodes_de_la_classe_throwable"><a class="anchor" href="#_les_méthodes_de_la_classe_throwable"></a><a class="link" href="#_les_méthodes_de_la_classe_throwable">6.4.14. Les méthodes de la classe <code>Throwable</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/throwable.png" alt="throwable">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_hiérarchie_dexceptions_de_la_librairie_java"><a class="anchor" href="#_hiérarchie_dexceptions_de_la_librairie_java"></a><a class="link" href="#_hiérarchie_dexceptions_de_la_librairie_java">6.4.15. Hiérarchie d&#8217;exceptions de la librairie Java</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/throwable_hier.png" alt="throwable hier">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_créer_des_classes_exceptions"><a class="anchor" href="#_créer_des_classes_exceptions"></a><a class="link" href="#_créer_des_classes_exceptions">6.4.16. Créer des classes exceptions</a></h4>
<div class="ulist">
<ul>
<li>
<p>Déterminer dans quelles méthodes et sous quelles conditions des exceptions seront lancées</p>
</li>
<li>
<p>Choisir le type de chaque exception</p>
<div class="ulist">
<ul>
<li>
<p>utiliser une exception existante</p>
</li>
<li>
<p>en créer une nouvelle</p>
</li>
</ul>
</div>
</li>
<li>
<p>Choisir quelle sera la super-classe des exceptions définies</p>
<div class="ulist">
<ul>
<li>
<p><a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Exception.html"><code>Exception</code></a> ou l&#8217;une de ses sous-classes</p>
</li>
<li>
<p>Les exceptions dérivée de <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/RuntimeException.html"><code>RuntimeException</code></a> ne sont pas contrôlées</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_la_hiérarchie_dexceptions_pour_une_pile"><a class="anchor" href="#_la_hiérarchie_dexceptions_pour_une_pile"></a><a class="link" href="#_la_hiérarchie_dexceptions_pour_une_pile">6.4.17. La hiérarchie d&#8217;exceptions pour une pile</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/pile-exception-hierarchie.png" alt="pile exception hierarchie" width="346" height="282">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_la_classe_pileexception"><a class="anchor" href="#_la_classe_pileexception"></a><a class="link" href="#_la_classe_pileexception">6.4.18. La classe <code>PileException</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.errors;

/**
 * La racine de la hiérarchie d'exception pour la pile.
 *
 * @author Author1
 * @version Version1
 */
class PileException extends Exception {
    /**
     * Initialise une instance de &lt;code&gt;PileException&lt;/code&gt;.
     *
     * @param message le message d'erreur.
     */
    public PileException(String message) {
        super(message);
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_la_classe_pilevideexception"><a class="anchor" href="#_la_classe_pilevideexception"></a><a class="link" href="#_la_classe_pilevideexception">6.4.19. La classe <code>PileVideException</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.errors;

/**
 * Exception pour la pile vide.
 *
 * @author Author1
 * @version Version1
 */
class PileVideException extends PileException {
    /**
     * Initialise une instance de &lt;code&gt;PileVideException&lt;/code&gt;.
     */
    public PileVideException() {
        super("La Pile est vide");
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_la_classe_pilepleineexception"><a class="anchor" href="#_la_classe_pilepleineexception"></a><a class="link" href="#_la_classe_pilepleineexception">6.4.20. La classe <code>PilePleineException</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.errors;

/**
 * Exception pour la pile pleine.
 *
 * @author Author1
 * @version Version1
 */
class PilePleineException extends PileException {
    /**
     * Initialise une instance de &lt;code&gt;PilePleineException&lt;/code&gt;.
     */
    public PilePleineException() {
        super("La Pile est pleine");
    }
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices"><a class="anchor" href="#_exercices"></a><a class="link" href="#_exercices">6.5. Exercices</a></h3>
<div class="sect3">
<h4 id="_calculatrice_rpn"><a class="anchor" href="#_calculatrice_rpn"></a><a class="link" href="#_calculatrice_rpn">6.5.1. Calculatrice RPN</a></h4>
<div class="paragraph">
<p>Dans cette exercice, on souhaite réaliser une calculatrice fonctionnant en mode RPN
(<a href="http://fr.wikipedia.org/wiki/Notation_polonaise_inverse"><em>Reverse Polish Notation</em></a>).
Cette notation post-fixée permet de représenter des formules arithmétiques sans parenthèses.
Par exemple, l&#8217;expression \$2 xx (3 + 4)\$ pourra s&#8217;écrire \$2 3 4 + xx\$.</p>
</div>
<div class="paragraph">
<p>Cette calculatrice devra supporter les opérations de base (<code>+, -, *, /</code>) sur des nombres réels.
L&#8217;intervalle de nombres supporté sera spécifié par deux constantes
(<code>MAX_VALUE</code> pour le plus grand nombre en valeur absolue,
<code>MIN_VALUE</code> pour le plus petit nombre en valeur absolue).
L&#8217;utilisateur saisira au clavier soit un nombre, soit une opération, soit <code>exit</code> pour sortir.
Chaque saisie se terminera par <em>entrée</em>.
Après chaque saisie, le programme affichera l&#8217;expression courante.</p>
</div>
<div class="paragraph">
<p>L&#8217;implémentation pourra utiliser une pile de la façon suivante&#160;:</p>
</div>
<div class="ulist">
<ul>
<li>
<p>les opérandes sont empilées lors de leur saisie,</p>
</li>
<li>
<p>les opérations sont effectuées immédiatement en considérant les opérandes se trouvant au sommet de la pile,</p>
</li>
<li>
<p>le résultat d&#8217;une opération est empilé.</p>
</li>
</ul>
</div>
<div class="olist arabic">
<div class="title">Questions</div>
<ol class="arabic">
<li>
<p>Déterminer les cas d&#8217;erreur.
En déduire les exceptions nécessaires pour la gestion des erreurs de cette application.</p>
</li>
<li>
<p>Organiser ces exceptions en hiérarchie et choisissez une classe de base dans la librairie Java</p>
</li>
<li>
<p>Implémenter l&#8217;énumération <code>Operation</code> de la façon suivante&#160;:</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>déclarer l&#8217;attribut <code>symbole</code> représentant le symbole de l&#8217;opération (<code>+</code>, <code>-</code>, &#8230;&#8203;),</p>
</li>
<li>
<p>définir le constructeur prenant en paramètre le symbole de l&#8217;opération,</p>
</li>
<li>
<p>déclarer la méthode abstraite <code>eval</code> retournant le résultat de l&#8217;évaluation de l&#8217;opération sur deux opérandes,</p>
</li>
<li>
<p>définir les constantes <code>PLUS</code>, <code>MOINS</code>, <code>MULT</code> et <code>DIV</code>,</p>
</li>
<li>
<p>pour chacune des constantes, redéfinir la méthode <code>eval</code>.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Implémenter la classe <code>MoteurRPN</code> possédant les capacités suivantes&#160;:</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>enregistrer une opérandes,</p>
</li>
<li>
<p>appliquer une opération sur les opérandes,</p>
</li>
<li>
<p>retourner l&#8217;ensemble des opérandes stockées.</p>
</li>
</ol>
</div>
</li>
<li>
<p>Implémenter la classe <code>SaisieRPN</code> qui gère les interactions avec l&#8217;utilisateur et invoque le moteur RPN.
La classe <a href="http://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html"><code>java.util.Scanner</code></a> permet de gérer les saisies.</p>
</li>
<li>
<p>Implémenter l&#8217;énumération <code>CalculatriceRPN</code> qui contiendra le programme principal.</p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_entréessorties_et_persistance"><a class="anchor" href="#_entréessorties_et_persistance"></a><a class="link" href="#_entréessorties_et_persistance">7. Entrées/sorties et persistance</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_entréessorties_flux_et_persistance"><a class="anchor" href="#_entréessorties_flux_et_persistance"></a><a class="link" href="#_entréessorties_flux_et_persistance">7.1. Entrées/sorties, flux et persistance</a></h3>
<div class="sect3">
<h4 id="_entréesortie_et_langage_de_programmation"><a class="anchor" href="#_entréesortie_et_langage_de_programmation"></a><a class="link" href="#_entréesortie_et_langage_de_programmation">7.1.1. Entrée/sortie et langage de programmation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La conception et l&#8217;implémentation d&#8217;une bibliothèque d&#8217;entrée/sortie (I/O) est une tâche difficile</p>
<div class="ulist">
<ul>
<li>
<p>la source ou la destination des données peut varier (mémoire, fichier, réseau, &#8230;&#8203;)</p>
</li>
<li>
<p>les types définis par l&#8217;utilisateur doivent être pris en charge</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le concept de <em>flux</em> est une proposition pour cela</p>
</li>
<li>
<p>La <em>persistance</em> et la <em>sérialisation</em> sont également nécessaires pour les I/O en POO</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_flux"><a class="anchor" href="#_flux"></a><a class="link" href="#_flux">7.1.2. Flux</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>flux</em> (<em>stream</em>) est un canal reliant une source (ou une destination) à un programme</p>
</li>
<li>
<p>Une source de données (ou une destination) peut être un fichier, la mémoire, le réseau, &#8230;&#8203;</p>
</li>
<li>
<p>Un flux peut être ouvert en lecture et/ou en écriture</p>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
Les données sont lues ou écrites séquentiellement
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_flux_en_lecture"><a class="anchor" href="#_flux_en_lecture"></a><a class="link" href="#_flux_en_lecture">7.1.3. Flux en lecture</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/io-ins.png" alt="io ins">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="https://docs.oracle.com/javase/tutorial/essential/io/streams.html">The Java Tutorial</a></p>
</div>
</div>
<div class="sect3">
<h4 id="_flux_en_écriture"><a class="anchor" href="#_flux_en_écriture"></a><a class="link" href="#_flux_en_écriture">7.1.4. Flux en écriture</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/io-outs.png" alt="io outs">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="https://docs.oracle.com/javase/tutorial/essential/io/streams.html">The Java Tutorial</a></p>
</div>
</div>
<div class="sect3">
<h4 id="_persistance"><a class="anchor" href="#_persistance"></a><a class="link" href="#_persistance">7.1.5. Persistance</a></h4>
<div class="ulist">
<ul>
<li>
<p>C&#8217;est la capacité de sauvegarder l&#8217;état des objets, i.e. les données finales de l&#8217;application</p>
</li>
<li>
<p>Elle peut être réalisée avec</p>
<div class="ulist">
<ul>
<li>
<p>la bibliothèque d&#8217;I/O du langage,</p>
</li>
<li>
<p>à l&#8217;aide de bibliothèques spécialisées,</p>
</li>
<li>
<p>grâce à un SGBD externe.</p>
</li>
</ul>
</div>
</li>
<li>
<p>La persistance pose un certain nombre de problèmes</p>
<div class="ulist">
<ul>
<li>
<p>sauvegarde de l&#8217;état de l&#8217;objet</p>
</li>
<li>
<p>gestion des types de données</p>
</li>
<li>
<p>gestion des références</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_sérialisation"><a class="anchor" href="#_sérialisation"></a><a class="link" href="#_sérialisation">7.1.6. Sérialisation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La <em>sérialisation</em> est un processus permettant de transformer un objet en flux d&#8217;octets</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_io_en_java"><a class="anchor" href="#_io_en_java"></a><a class="link" href="#_io_en_java">7.2. I/O en Java</a></h3>
<div class="sect3">
<h4 id="_structure_et_fonctionalités"><a class="anchor" href="#_structure_et_fonctionalités"></a><a class="link" href="#_structure_et_fonctionalités">7.2.1. Structure et fonctionalités</a></h4>
<div class="paragraph">
<p>La bibliothèque standard Java fournit de nombreuses fonctionnalités liées aux E/S</p>
</div>
<div class="ulist">
<ul>
<li>
<p>la gestion des flux (
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/package-summary.html"><code>java.io</code></a>)</p>
</li>
<li>
<p>les fichiers à accés aléatoires (
<a href="https://docs.oracle.com/javase/8/docs/api/java/nio/channels/SeekableByteChannel.html"><code>java.nio.channels.SeekableByteChannel</code></a>,
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/RandomAccessFile.html"><code>RandomAccessFile</code></a>)</p>
</li>
<li>
<p>des fonctionnalités avancées (
<a href="https://docs.oracle.com/javase/8/docs/api/java/nio/package-summary.html"><code>java.nio.channels</code></a>)</p>
</li>
<li>
<p>l&#8217;interaction avec le système de fichiers (
<a href="https://docs.oracle.com/javase/8/docs/api/java/nio/file/package-summary.html"><code>java.nio.file</code></a>,
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/File.html"><code>File</code></a>)</p>
</li>
<li>
<p>l&#8217;entrée et la sortie standard (
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/PrintStream.html"><code>PrintStream</code></a>,
<a href="https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html"><code>java.util.Scanner</code></a>,
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/Console.html"><code>Console</code></a>)</p>
</li>
<li>
<p>la gestion des archives (
<a href="https://docs.oracle.com/javase/8/docs/api/java/util/zip/package-summary.html"><code>java.util.zip</code></a>,
<a href="https://docs.oracle.com/javase/8/docs/api/java/util/jar/package-summary.html"><code>java.util.jar</code></a>)</p>
</li>
<li>
<p>les fichiers d&#8217;image (
<a href="https://docs.oracle.com/javase/8/docs/api/javax/imageio/package-summary.html"><code>javax.imageio</code></a>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_gestion_des_flux"><a class="anchor" href="#_gestion_des_flux"></a><a class="link" href="#_gestion_des_flux">7.2.2. Gestion des flux</a></h4>
<div class="ulist">
<ul>
<li>
<p>La librairie se divise en deux hiérarchies de classes</p>
<div class="ulist">
<ul>
<li>
<p>les flux de caractères (I/O de texte)</p>
</li>
<li>
<p>les flux d&#8217;octets (I/O binaire)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un flux est automatiquement ouvert lors de sa création</p>
</li>
<li>
<p>La fermeture d&#8217;un flux se fait explicitement avec la méthode <code>close</code></p>
</li>
<li>
<p>La plupart des méthodes peuvent lancer une exception dérivée de
<a href="https://docs.oracle.com/javase/8/docs/api/java/io/IOException.html"><code>IOException</code></a></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_flux_de_caractères"><a class="anchor" href="#_flux_de_caractères"></a><a class="link" href="#_flux_de_caractères">7.2.3. Flux de caractères</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les classes <code>Reader</code> et <code>Writer</code> sont les super-classes abstraites pour les flux de caractères</p>
</li>
<li>
<p>La plate-forme Java manipule des caractères en se basant sur Unicode</p>
</li>
<li>
<p>Les flux de caractères permettent de convertir ce format interne de/vers le format local</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_reader_et_writer"><a class="anchor" href="#_reader_et_writer"></a><a class="link" href="#_reader_et_writer">7.2.4. <code>Reader</code> et <code>Writer</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/reader_writer.png" alt="reader writer">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_hiérarchie_de_reader"><a class="anchor" href="#_hiérarchie_de_reader"></a><a class="link" href="#_hiérarchie_de_reader">7.2.5. Hiérarchie de <code>Reader</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/reader-hierarchie.png" alt="reader hierarchie" width="957" height="282">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_hiérarchie_de_writer"><a class="anchor" href="#_hiérarchie_de_writer"></a><a class="link" href="#_hiérarchie_de_writer">7.2.6. Hiérarchie de <code>Writer</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/writer-hierarchie.png" alt="writer hierarchie" width="1044" height="282">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_flux_doctets"><a class="anchor" href="#_flux_doctets"></a><a class="link" href="#_flux_doctets">7.2.7. Flux d&#8217;octets</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les classes <code>InputStream</code> et <code>OutputStream</code> sont les super-classes abstraites pour les flux d&#8217;octets</p>
</li>
<li>
<p>Les flux d&#8217;octets supportent la lecture et l&#8217;écriture d&#8217;octets (8 bits)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_inputstream_et_outputstream"><a class="anchor" href="#_inputstream_et_outputstream"></a><a class="link" href="#_inputstream_et_outputstream">7.2.8. <code>InputStream</code> et <code>OutputStream</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/input_output.png" alt="input output">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_hiérarchie_de_inputstream"><a class="anchor" href="#_hiérarchie_de_inputstream"></a><a class="link" href="#_hiérarchie_de_inputstream">7.2.9. Hiérarchie de <code>InputStream</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/inputstream-hierarchie.png" alt="inputstream hierarchie" width="1095" height="282">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_hiérarchie_de_outputstream"><a class="anchor" href="#_hiérarchie_de_outputstream"></a><a class="link" href="#_hiérarchie_de_outputstream">7.2.10. Hiérarchie de <code>OutputStream</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/outputstream-hierarchie.png" alt="outputstream hierarchie" width="943" height="282">
</div>
</div>
</div>
<div class="sect3">
<h4 id="_java_nio"><a class="anchor" href="#_java_nio"></a><a class="link" href="#_java_nio">7.2.11. <code>java.nio</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/nio-fileiomethods.png" alt="nio fileiomethods">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="https://docs.oracle.com/javase/tutorial/essential/io/file.html">Java Tutorial</a> - Reading, Writing, and Creating Files</p>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_utilisation_des_flux"><a class="anchor" href="#_utilisation_des_flux"></a><a class="link" href="#_utilisation_des_flux">7.3. Utilisation des flux</a></h3>
<div class="sect3">
<h4 id="_principaux_flux_par_type_dio"><a class="anchor" href="#_principaux_flux_par_type_dio"></a><a class="link" href="#_principaux_flux_par_type_dio">7.3.1. Principaux flux par type d&#8217;I/O</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 33.3333%;">
<col style="width: 33.3333%;">
<col style="width: 33.3334%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Type d&#8217;I/O</th>
<th class="tableblock halign-left valign-top">Flux de catactères</th>
<th class="tableblock halign-left valign-top">Flux d&#8217;octets</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top" rowspan="2"><p class="tableblock">Mémoire</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>CharArrayReader</code>, <code>CharArrayWriter</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>ByteArrayInputStream</code>, <code>ByteArrayOutputStream</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>StringReader</code>, <code>StringWriter</code></p></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Fichier</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>FileReader</code>, <code>FileWriter</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>FileInputStream</code>, <code>FileOutputStream</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Affichage</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>PrintWriter</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>PrintStream</code></p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_principaux_flux_par_fonction"><a class="anchor" href="#_principaux_flux_par_fonction"></a><a class="link" href="#_principaux_flux_par_fonction">7.3.2. Principaux flux par fonction</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 33.3333%;">
<col style="width: 33.3333%;">
<col style="width: 33.3334%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Type d&#8217;I/O</th>
<th class="tableblock halign-left valign-top">Flux de catactères</th>
<th class="tableblock halign-left valign-top">Flux d&#8217;octets</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Avec buffer</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>BufferedReader</code>, <code>BufferedWriter</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>BufferedInputStream</code>, <code>BufferedOutputStream</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Conv. de données</p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>DataInputStream</code>, <code>DataOutputStream</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Sérialisation</p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>ObjectInputStream</code>, <code>ObjectOutputStream</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Conv. oct./car.</p></td>
<td class="tableblock halign-left valign-top" colspan="2"><p class="tableblock"><code>InputStreamReader</code>, <code>OutputStreamWriter</code></p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_flux_de_fichiers"><a class="anchor" href="#_flux_de_fichiers"></a><a class="link" href="#_flux_de_fichiers">7.3.3. Flux de fichiers</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les classes des flux de fichiers sont</p>
<div class="ulist">
<ul>
<li>
<p><code>FileReader/FileWriter</code> pour l&#8217;accès aux fichiers textes</p>
</li>
<li>
<p><code>FileInputStream/FileOutputStream</code> pour les fichiers binaires</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un flux de fichier peut être créé</p>
<div class="ulist">
<ul>
<li>
<p>à partir d&#8217;un nom de fichier sous la forme d&#8217;une chaîne de caractères</p>
</li>
<li>
<p>d&#8217;une instance de <code>File</code></p>
</li>
<li>
<p>d&#8217;une méthode de classe de
<a href="http://docs.oracle.com/javase/8/docs/api/java/nio/file/Files.html"><code>java.nio.file.Files</code></a> (<code>newInputStream</code>, &#8230;&#8203;)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_copie_dun_fichier_texte"><a class="anchor" href="#_copie_dun_fichier_texte"></a><a class="link" href="#_copie_dun_fichier_texte">7.3.4. Copie d&#8217;un fichier texte</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Copie un fichier caractère par caractère.
 */
private static void textFileCopy(String inFilename, String outFilename) throws IOException {
    try (
            FileReader in = new FileReader(inFilename);
            FileWriter out = new FileWriter(outFilename)
    ) {
        int c;
        while ((c = in.read()) != END_OF_STREAM) {
            out.write(c);
        }
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_copie_dun_fichier_texte_avec_buffer"><a class="anchor" href="#_copie_dun_fichier_texte_avec_buffer"></a><a class="link" href="#_copie_dun_fichier_texte_avec_buffer">7.3.5. Copie d&#8217;un fichier texte (avec buffer)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Copie un fichier en utilisant un buffer.
 */
private static void bufferedTextFileCopy(String inFilename, String outFilename) throws IOException {
    Path inPath = Paths.get(inFilename);
    Path outPath = Paths.get(outFilename);
    try (
            BufferedReader in = Files.newBufferedReader(inPath);
            BufferedWriter out = Files.newBufferedWriter(outPath)
    ) {
        String line;
        while ((line = in.readLine()) != null) {
            out.write(line);
            out.newLine();
        }
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_copie_dun_fichier_texte_avec_readalllines"><a class="anchor" href="#_copie_dun_fichier_texte_avec_readalllines"></a><a class="link" href="#_copie_dun_fichier_texte_avec_readalllines">7.3.6. Copie d&#8217;un fichier texte (avec readAllLines)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Copie un fichier texte.
 * Le fichier doit être de taille raisonnable car il est chargé en totalité en mémoire.
 */
private static void simpleTextFileCopy(String inFilename, String outFilename) throws IOException {
    Path inPath = Paths.get(inFilename);
    Path outPath = Paths.get(outFilename);
    List&lt;String&gt; lines = Files.readAllLines(inPath);
    Files.write(outPath, lines);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_copie_dun_fichier_binaire"><a class="anchor" href="#_copie_dun_fichier_binaire"></a><a class="link" href="#_copie_dun_fichier_binaire">7.3.7. Copie d&#8217;un fichier binaire</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Copie un fichier octet par octet.
 */
private static void binaryFileCopy(String inFilename, String outFilename) throws IOException {
    try (
            FileInputStream in = new FileInputStream(inFilename);
            FileOutputStream out = new FileOutputStream(outFilename)
    ) {
        int c;
        while ((c = in.read()) != END_OF_STREAM) {
            out.write(c);
        }
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_flux_de_filtrage"><a class="anchor" href="#_flux_de_filtrage"></a><a class="link" href="#_flux_de_filtrage">7.3.8. Flux de filtrage</a></h4>
<div class="ulist">
<ul>
<li>
<p>Certaines classes de flux sont destinées à appliquer un traitement sur (à <em>filtrer</em>) un flux</p>
</li>
<li>
<p>Les super-classes abstraites pour cela sont</p>
<div class="ulist">
<ul>
<li>
<p><code>FilterReader/FilterWriter</code> pour les caractères</p>
</li>
<li>
<p><code>FilterOutputStream/FilterInputStream</code> pour les octets</p>
</li>
</ul>
</div>
</li>
<li>
<p>Des flux personnalisés peuvent être définis en héritant de ces classes</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_principaux_flux_de_filtrage"><a class="anchor" href="#_principaux_flux_de_filtrage"></a><a class="link" href="#_principaux_flux_de_filtrage">7.3.9. Principaux flux de filtrage</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les principaux flux de filtrage pour les flux d&#8217;octets sont</p>
<div class="ulist">
<ul>
<li>
<p><code>DataInputStream</code> et <code>DataOutputStream</code> pour les I/O des types primitifs</p>
</li>
<li>
<p><code>BufferedInputStream</code> et <code>BufferedOutputStream</code> pour des I/O avec buffer</p>
</li>
<li>
<p><code>PrintStream</code> pour l&#8217;affichage des données</p>
</li>
<li>
<p><code>PushbackInputStream</code> pour pouvoir "annuler" la lecture d&#8217;une séquence d&#8217;octets</p>
</li>
</ul>
</div>
</li>
<li>
<p>Le seul flux de filtrage pour les flux de caractères est <code>PushbackReader</code> (permet d'"annuler" la lecture d&#8217;une séquence de caractères)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_flux_de_filtrage_et_modèle_de_conception_décorateur"><a class="anchor" href="#_flux_de_filtrage_et_modèle_de_conception_décorateur"></a><a class="link" href="#_flux_de_filtrage_et_modèle_de_conception_décorateur">7.3.10. Flux de filtrage et modèle de conception <em>Décorateur</em></a></h4>
<div class="ulist">
<ul>
<li>
<p>Un flux de filtrage est construit à partir d&#8217;un autre flux selon le modèle de conception <a href="https://en.wikipedia.org/wiki/Decorator_pattern"><em>Décorateur</em></a></p>
</li>
<li>
<p>Le flux résultant propose des fonctionnalités plus riches que le flux initial</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">FileInputStream words = new FileInputStream("words.dat");
BufferedInputStream in = new BufferedInputStream(words);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_ecriture_des_types_primitifs"><a class="anchor" href="#_ecriture_des_types_primitifs"></a><a class="link" href="#_ecriture_des_types_primitifs">7.3.11. Ecriture des types primitifs</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static void writeDateToFile(String filename, int numberOfItems, double[] prices, int[] units, String[] descs) throws IOException {
    try (DataOutputStream out =
                 new DataOutputStream(
                         new BufferedOutputStream(
                                 new FileOutputStream(filename)))
    ) {
        for (int i = 0; i &lt; numberOfItems; i++) {
            out.writeDouble(prices[i]);
            out.writeInt(units[i]);
            out.writeUTF(descs[i]);
        }
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_lecture_des_types_primitifs"><a class="anchor" href="#_lecture_des_types_primitifs"></a><a class="link" href="#_lecture_des_types_primitifs">7.3.12. Lecture des types primitifs</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public static void readDateFromFile(String filename, int numberOfItems, double[] prices, int[] units, String[] descs) throws IOException {
    try (DataInputStream out =
                 new DataInputStream(
                         new BufferedInputStream(
                                 new FileInputStream(filename)))
    ) {
        for (int i = 0; i &lt; numberOfItems; i++) {
            prices[i] = out.readDouble();
            units[i] = out.readInt();
            descs[i] = out.readUTF();
        }
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_entrée_et_sortie_standards_en_java"><a class="anchor" href="#_entrée_et_sortie_standards_en_java"></a><a class="link" href="#_entrée_et_sortie_standards_en_java">7.3.13. Entrée et sortie standards en Java</a></h4>
<div class="paragraph">
<p>La classe <code>System</code> fournit des flux pour :</p>
</div>
<div class="ulist">
<ul>
<li>
<p>l&#8217;entrée standard (attribut <code>in</code> de type <code>PrintStream</code>)</p>
</li>
<li>
<p>la sortie standard (attribut <code>out</code> de type <code>InputStream</code>)</p>
</li>
<li>
<p>la sortie d&#8217;erreurs (attribut <code>err</code> de type <code>PrintStream</code>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_flux_daffichage_printstream_ou_printwriter"><a class="anchor" href="#_flux_daffichage_printstream_ou_printwriter"></a><a class="link" href="#_flux_daffichage_printstream_ou_printwriter">7.3.14. Flux d&#8217;affichage <code>PrintStream</code> (ou <code>PrintWriter</code>)</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>PrintStream format( /* &#8230;&#8203; */)</code> affiche une chaîne selon un format</p>
<div class="ulist">
<ul>
<li>
<p>cf.  <a href="http://docs.oracle.com/javase/8/docs/api/java/util/Formatter.html"><code>java.util.Formatter</code></a></p>
</li>
<li>
<p><code>PrintStream printf(/* &#8230;&#8203; */)</code> fait la même chose</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>void print(/* &#8230;&#8203; */)</code> affiche différents types de données sur le flux</p>
<div class="ulist">
<ul>
<li>
<p><code>void println(/* &#8230;&#8203; */)</code> idem mais suivi d&#8217;un retour à la ligne</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>PrintStream append(/* &#8230;&#8203; */)</code> ajoute des caractères au flux</p>
</li>
<li>
<p><code>void flush()</code> force la sortie des caractères</p>
</li>
<li>
<p>Ne lancent jamais d&#8217;exception mais positionnent un indicateur interne</p>
<div class="ulist">
<ul>
<li>
<p>interrogeable avec la méthode <code>boolean checkError()</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_lire_à_partir_de_lentrée_standard"><a class="anchor" href="#_lire_à_partir_de_lentrée_standard"></a><a class="link" href="#_lire_à_partir_de_lentrée_standard">7.3.15. Lire à partir de l&#8217;entrée standard</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;entrée standard est utilisée en décorant <code>System.in</code> avec <code>InputStreamReader</code>
(voire avec <code>BufferedReader</code>)</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">InputStreamReader stdin = new InputStreamReader(System.in);
BufferedReader bufferedStdin = new BufferedReader(stdin));</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La classe <a href="http://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html"><code>java.util.Scanner</code></a> simplifie le processus de saisie</p>
<div class="ulist">
<ul>
<li>
<p>permet de découper un flux en <em>token</em></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_accéder_à_lentrée_et_la_sortie_standard_avec_scanner"><a class="anchor" href="#_accéder_à_lentrée_et_la_sortie_standard_avec_scanner"></a><a class="link" href="#_accéder_à_lentrée_et_la_sortie_standard_avec_scanner">7.3.16. Accéder à l&#8217;entrée et la sortie standard (avec Scanner)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">System.out.println("Votre nom et votre âge ? ");

Scanner s = new Scanner(System.in);
String nom = s.next();
int age = s.nextInt();

System.out.format("Votre nom est %s et vous avez %5d ans.%n", nom, age);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_accéder_à_lentrée_et_la_sortie_standard_avec_bufferedreader"><a class="anchor" href="#_accéder_à_lentrée_et_la_sortie_standard_avec_bufferedreader"></a><a class="link" href="#_accéder_à_lentrée_et_la_sortie_standard_avec_bufferedreader">7.3.17. Accéder à l&#8217;entrée et la sortie standard (avec BufferedReader)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">System.out.println("Votre nom et votre age ? ");

BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
String nom = in.readLine();
int age = Integer.parseInt(in.readLine());

System.out.format("Votre nom est %s et vous avez %5d ans.%n", nom, age);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_utiliser_la_classe_console"><a class="anchor" href="#_utiliser_la_classe_console"></a><a class="link" href="#_utiliser_la_classe_console">7.3.18. Utiliser la classe <code>Console</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>La classe <a href="http://docs.oracle.com/javase/8/docs/api/index.html?java/io/BufferedReader.html"><code>Console</code></a> est une alternative pour l&#8217;accès à l&#8217;entrée et à la sortie standard</p>
</li>
<li>
<p>Un objet de ce type est initialisé avec la méthode <code>System.console()</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Console c = System.console();
if (c == null) {
    System.err.println("No console.");
    System.exit(1);
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_sérialisation_en_java"><a class="anchor" href="#_sérialisation_en_java"></a><a class="link" href="#_sérialisation_en_java">7.4. Sérialisation en Java</a></h3>
<div class="sect3">
<h4 id="_sérialisation_2"><a class="anchor" href="#_sérialisation_2"></a><a class="link" href="#_sérialisation_2">7.4.1. Sérialisation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La sérialisation est assurée par les classes <code>ObjectInputStream</code> et <code>ObjectOutputStream</code></p>
</li>
<li>
<p><code>ObjectOutputStream</code> implémente les interfaces <code>DataOutput</code> et <code>ObjectOutput</code></p>
</li>
<li>
<p><code>ObjectInputStream</code> implémente les interfaces <code>DataInput</code> et <code>ObjectInput</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_ecrire_des_objets_dans_un_flux"><a class="anchor" href="#_ecrire_des_objets_dans_un_flux"></a><a class="link" href="#_ecrire_des_objets_dans_un_flux">7.4.2. Ecrire des objets dans un flux</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">private static void writeObjectsToFile(Student[] students, String filename) throws IOException {
    try (ObjectOutputStream oos =
                 new ObjectOutputStream(
                         new FileOutputStream(filename))
    ) {
        oos.writeObject(LocalDate.now());
        oos.writeObject(students);
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_lire_des_objets_à_partir_dun_flux"><a class="anchor" href="#_lire_des_objets_à_partir_dun_flux"></a><a class="link" href="#_lire_des_objets_à_partir_dun_flux">7.4.3. Lire des objets à partir d&#8217;un flux</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">private static LocalDate readObjectsFromFile(Student[] students, String filename) throws IOException, ClassNotFoundException {
    try (ObjectInputStream ois =
                 new ObjectInputStream(
                         new FileInputStream(filename))
    ) {
        LocalDate date = (LocalDate) ois.readObject();
        students = (Student[]) ois.readObject();
        return date;
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_rendre_une_classe_sérialisable"><a class="anchor" href="#_rendre_une_classe_sérialisable"></a><a class="link" href="#_rendre_une_classe_sérialisable">7.4.4. Rendre une classe sérialisable</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un objet est sérialisable uniquement si sa classe implémente l&#8217;interface <code>Serializable</code></p>
</li>
<li>
<p>L&#8217;interface <code>Serializable</code> ne comporte aucune méthode et ne sert qu&#8217;à spécifier les classes sérialisables</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_une_classe_sérialisable"><a class="anchor" href="#_une_classe_sérialisable"></a><a class="link" href="#_une_classe_sérialisable">7.4.5. Une classe sérialisable</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.io;

import java.io.Serializable;

public class Student implements Serializable {
    private int number;
    private String name;

    public Student(int number, String name) {
        this.number = number;
        this.name = name;
    }

    @Override
    public String toString() {
        return String.format("Student{number: %d, name: '%s'}", number, name);
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_gérer_la_version_des_classes"><a class="anchor" href="#_gérer_la_version_des_classes"></a><a class="link" href="#_gérer_la_version_des_classes">7.4.6. Gérer la version des classes</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;attribut de classe <a href="http://docs.oracle.com/javase/8/docs/api/java/io/Serializable.html"><code>serialVersionUID</code></a> précise la version d&#8217;une classe sérialisable</p>
</li>
<li>
<p>Il permet de déterminer si un objet correspond bien à la classe présente dans la JVM</p>
</li>
<li>
<p>Il est généré par la JVM s&#8217;il n&#8217;est pas défini dans la classe</p>
</li>
<li>
<p>Le développeur peut gérer les versions lui-même</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">private static final long serialVersionUID = 354054054054L;</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_contrôler_la_sérialisation"><a class="anchor" href="#_contrôler_la_sérialisation"></a><a class="link" href="#_contrôler_la_sérialisation">7.4.7. Contrôler la sérialisation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La sérialisation est gérée par les méthodes</p>
<div class="ulist">
<ul>
<li>
<p><code>defaultWriteObject</code> de <code>ObjectOutputStream</code></p>
</li>
<li>
<p><code>defaultReadObject</code> de <code>ObjectInputStream</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Le comportement par défaut de la sérialisation d&#8217;un objet est de stocker</p>
<div class="ulist">
<ul>
<li>
<p>la classe de l&#8217;objet</p>
</li>
<li>
<p>la signature de la classe</p>
</li>
<li>
<p>la valeur des attributs d&#8217;instances y compris les références (mais pas les attributs <code>transcient</code>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Il est possible d&#8217;adapter le comportement par défaut en redéfinissant <code>writeObject</code> et <code>readObject</code></p>
</li>
<li>
<p>L&#8217;interface <code>Externalizable</code> permet d&#8217;avoir un contrôle complet du processus de sérialisation</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_2"><a class="anchor" href="#_exercices_2"></a><a class="link" href="#_exercices_2">7.5. Exercices</a></h3>
<div class="sect3">
<h4 id="_utilisation_des_flux_de_caractères"><a class="anchor" href="#_utilisation_des_flux_de_caractères"></a><a class="link" href="#_utilisation_des_flux_de_caractères">7.5.1. Utilisation des flux de caractères</a></h4>
<div class="paragraph">
<p>Le but de cette exercice est de réaliser quelques outils de manipulation de fichiers textes.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Écrire un programme prenant en argument un nom de fichier et affichant le nombre de lignes de ce fichier.
Quelle classe du package <code>java.io</code> vous sera utile pour cette tâche ?</p>
</li>
<li>
<p>Ècrire un programme prenant en argument une chaîne de caractères et un nom de fichier et qui affiche les lignes (avec leur numéro) du fichier contenant la chaîne.
Quelle classe du package <code>java.io</code> vous sera utile pour cette tâche ?</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_implémentation_dun_flux_de_filtrage"><a class="anchor" href="#_implémentation_dun_flux_de_filtrage"></a><a class="link" href="#_implémentation_dun_flux_de_filtrage">7.5.2. Implémentation d&#8217;un flux de filtrage</a></h4>
<div class="paragraph">
<p>Cette exercice consiste à implémenter une commande <code>grep</code> simplifiée.
Parmi les nombreuses options de cette commande, vous implémenterez le sous-ensemble suivant
(cf. <a href="http://manpagesfr.free.fr/man/man1/grep.1.html">page de manuel</a>) :
<code>--help</code>, <code>-e|--regexp</code>, <code>-f|--file</code>, <code>-i|--ignore-case</code>, <code>-n|--line-number</code>.</p>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
<div class="paragraph">
<p>Vous utiliserez la bibliothèque</p>
</div>
<div class="ulist">
<ul>
<li>
<p><a href="http://commons.apache.org/cli/">Apache Commons CLI</a> pour la manipulation des arguments de ligne de commande,</p>
</li>
<li>
<p>de manipulation d&#8217;expressions rationnelles du JDK (cf.
<a href="http://docs.oracle.com/javase/tutorial/essential/regex/index.html">Tutoriel</a>).</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="olist arabic">
<div class="title">Questions</div>
<ol class="arabic">
<li>
<p>Réalisez le flux de filtrage <code>GrepReader</code> qui lit un flux en retournant uniquement les lignes correspondant au motif recherché</p>
</li>
<li>
<p>Réaliser la classe principale <code>GrepApp</code></p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_gestion_des_collections"><a class="anchor" href="#_gestion_des_collections"></a><a class="link" href="#_gestion_des_collections">8. Gestion des collections</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_introduction_2"><a class="anchor" href="#_introduction_2"></a><a class="link" href="#_introduction_2">8.1. Introduction</a></h3>
<div class="sect3">
<h4 id="_collection"><a class="anchor" href="#_collection"></a><a class="link" href="#_collection">8.1.1. Collection</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>collection</em> (<em>conteneur</em>) est un objet qui regroupe plusieurs éléments en une seule unité</p>
</li>
<li>
<p>Une collection peut être utilisée pour stocker et manipuler des données et pour transmettre des données d&#8217;une méthode à une autre</p>
</li>
<li>
<p>Une collection regroupe généralement des objets de même type</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_bibliothèques_pour_les_collections"><a class="anchor" href="#_bibliothèques_pour_les_collections"></a><a class="link" href="#_bibliothèques_pour_les_collections">8.1.2. Bibliothèques pour les collections</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>bibliothèque pour les collections</em> (<em>collection framework</em>) est une architecture unifiée pour représenter et manipuler des collections</p>
</li>
<li>
<p>Elle différencie trois composants :</p>
<div class="ulist">
<ul>
<li>
<p>des <em>interfaces</em> permettent de manipuler des collections indépendamment de leurs implémentations</p>
</li>
<li>
<p>des <em>implémentations</em> représentent les structures de données proprement dites</p>
</li>
<li>
<p>des <em>algorithmes</em> effectuent des traitements par l&#8217;intermédiaire des interfaces</p>
</li>
</ul>
</div>
</li>
<li>
<p>Ce type de bibliothèque s&#8217;appuie en général sur la généricité pour le contrôle des types</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_exemples_de_bibliothèques_pour_les_collections"><a class="anchor" href="#_quelques_exemples_de_bibliothèques_pour_les_collections"></a><a class="link" href="#_quelques_exemples_de_bibliothèques_pour_les_collections">8.1.3. Quelques exemples de bibliothèques pour les collections</a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1">Java</dt>
<dd>
<p><a href="http://docs.oracle.com/javase/8/docs/technotes/guides/collections/overview.html"><em>Java Collections Framework</em></a>,
<a href="https://commons.apache.org/proper/commons-collections/"><em>Apache Commons Collections</em></a>,
<a href="https://github.com/google/guava/wiki"><em>Google Guava</em></a></p>
</dd>
<dt class="hdlist1">C++</dt>
<dd>
<p><a href="http://www.cplusplus.com/reference/stl/"><em>Standard Containers</em></a> de la STL (<em>Standard Template Library</em>),
<a href="http://www.boost.org/"><em>Boost</em></a></p>
</dd>
<dt class="hdlist1">Python</dt>
<dd>
<p>built-in containers <a href="https://docs.python.org/3/library/stdtypes.html#dict"><code>dict</code></a>,
<a href="https://docs.python.org/3/library/stdtypes.html#list"><code>list</code></a>,
<a href="https://docs.python.org/3/library/stdtypes.html#set"><code>set</code></a>, and
<a href="https://docs.python.org/3/library/stdtypes.html#tuple"><code>tuple</code></a></p>
</dd>
<dt class="hdlist1">C#</dt>
<dd>
<p><a href="https://msdn.microsoft.com/fr-fr/library/mt654013.aspx"><em>Collections</em></a></p>
</dd>
<dt class="hdlist1">Rust</dt>
<dd>
<p><a href="https://doc.rust-lang.org/std/collections/"><code>std::collections</code></a></p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_motivations"><a class="anchor" href="#_motivations"></a><a class="link" href="#_motivations">8.1.4. Motivations</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/axes.svg" alt="axes">
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>\$i xx j\$ versions différentes du même algorithme pour supporter tous les conteneurs</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
&#8658;
</td>
<td class="hdlist2">
<p>pour <em>k</em> algorithmes, \$i xx j xx k\$ programmes</p>
</td>
</tr>
</table>
</div>
</li>
<li>
<p>La généricité permet de paramétrer par rapport aux types</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
&#8658;
</td>
<td class="hdlist2">
<p>réduit à \$j xx k\$ programmes</p>
</td>
</tr>
</table>
</div>
</li>
<li>
<p>Abstraction de la notion de collection (un algo. fonctionne sur toute collection)</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
&#8658;
</td>
<td class="hdlist2">
<p>réduit à \$j + k\$ programmes</p>
</td>
</tr>
</table>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_intérêt_dune_bibliothèque_pour_les_collections_12"><a class="anchor" href="#_intérêt_dune_bibliothèque_pour_les_collections_12"></a><a class="link" href="#_intérêt_dune_bibliothèque_pour_les_collections_12">8.1.5. Intérêt d&#8217;une bibliothèque pour les collections 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Réduit l&#8217;effort de programmation</p>
<div class="ulist">
<ul>
<li>
<p>fournit des SDD et des algorithmes permettant de se concentrer sur les parties importantes d&#8217;un problème sans s&#8217;occuper de détails d&#8217;implémentation</p>
</li>
</ul>
</div>
</li>
<li>
<p>Améliore la qualité et les performances du programme</p>
<div class="ulist">
<ul>
<li>
<p>fournit des SDD et des algorithmes de haute qualité et efficaces.</p>
</li>
<li>
<p>il est aussi possible de remplacer simplement une SDD par une autre</p>
</li>
</ul>
</div>
</li>
<li>
<p>Permet l&#8217;interopérabilité d&#8217;API</p>
<div class="ulist">
<ul>
<li>
<p>Les API peuvent échanger des collections</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_intérêt_dune_bibliothèque_pour_les_collections_22"><a class="anchor" href="#_intérêt_dune_bibliothèque_pour_les_collections_22"></a><a class="link" href="#_intérêt_dune_bibliothèque_pour_les_collections_22">8.1.6. Intérêt d&#8217;une bibliothèque pour les collections 2/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Réduit l&#8217;effort d&#8217;apprentissage et d&#8217;utilisation</p>
<div class="ulist">
<ul>
<li>
<p>permet de se concentrer sur une seule API</p>
</li>
</ul>
</div>
</li>
<li>
<p>Réduit l&#8217;effort de conception de nouvelles API</p>
<div class="ulist">
<ul>
<li>
<p>les nouvelles API s&#8217;appuient sur les collections existantes</p>
</li>
</ul>
</div>
</li>
<li>
<p>Améliore la réutilisabilité du logiciel</p>
<div class="ulist">
<ul>
<li>
<p>une nouvelle SDD ou un nouvel algorithme s&#8217;intégrant dans la bibliothèque est immédiatement utilisable avec le reste</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_collections_en_java"><a class="anchor" href="#_collections_en_java"></a><a class="link" href="#_collections_en_java">8.1.7. Collections en Java</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/collections.png" alt="collections">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="http://www.novixys.com/blog/java-collections/">Java Collections</a></p>
</div>
</div>
<div class="sect3">
<h4 id="_dictionnaires_en_java"><a class="anchor" href="#_dictionnaires_en_java"></a><a class="link" href="#_dictionnaires_en_java">8.1.8. Dictionnaires en Java</a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/maps.png" alt="maps">
</div>
</div>
<div class="paragraph">
<p>Source : <a href="http://www.novixys.com/blog/java-collections/">Java Collections</a></p>
</div>
</div>
<div class="sect3">
<h4 id="_caractéristiques_communes"><a class="anchor" href="#_caractéristiques_communes"></a><a class="link" href="#_caractéristiques_communes">8.1.9. Caractéristiques communes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une collection Java ne peut pas contenir une donnée d&#8217;un type primitif (uniquement des objets)</p>
</li>
<li>
<p>Les composants de la bibliothèque de collections se trouvent dans <code>java.util</code></p>
</li>
<li>
<p>Le découpage interface/implémentation repose sur le modèle de conception <a href="https://en.wikipedia.org/wiki/Bridge_pattern">Pont</a></p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_interfaces"><a class="anchor" href="#_interfaces"></a><a class="link" href="#_interfaces">8.2. Interfaces</a></h3>
<div class="sect3">
<h4 id="_les_interfaces"><a class="anchor" href="#_les_interfaces"></a><a class="link" href="#_les_interfaces">8.2.1. Les interfaces</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les interfaces sont utilisées pour manipuler des collections et les transmettre d&#8217;une méthode à une autre</p>
</li>
<li>
<p>Les interfaces permettent de manipuler les collections indépendamment des différentes implémentations</p>
<div class="ulist">
<ul>
<li>
<p>représente les types de structures de données</p>
</li>
<li>
<p>il est préférable de manipuler les collections par les interfaces plutôt que par les implémentations</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une implémentation a la possibilité de ne pas supporter toutes les méthodes de modification de l&#8217;interface (lancement de l&#8217;exception <code>UnsupportedOperationException</code>)</p>
</li>
<li>
<p>Les implémentations du JDK implémentent toutes les méthodes optionnelles</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_la_hiérarchie_de_collection"><a class="anchor" href="#_la_hiérarchie_de_collection"></a><a class="link" href="#_la_hiérarchie_de_collection">8.2.2. La hiérarchie de <code>Collection</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/collection-hierarchie.svg" alt="collection hierarchie" width="331" height="499">
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><code>Iterable</code> autorise l&#8217;utilisation du <em>foreach</em></p>
</li>
<li>
<p>D&#8217;autres interfaces existent mais sont liées à la concurrence</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_la_hiérarchie_de_map"><a class="anchor" href="#_la_hiérarchie_de_map"></a><a class="link" href="#_la_hiérarchie_de_map">8.2.3. La hiérarchie de <code>Map</code></a></h4>
<div class="imageblock">
<div class="content">
<img src="figs/map-hierarchie.svg" alt="map hierarchie" width="150" height="283">
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La hiérarchie de <code>Map</code> représentent des tableaux associatifs (dictionnaires)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_collection_12"><a class="anchor" href="#_linterface_collection_12"></a><a class="link" href="#_linterface_collection_12">8.2.4. L&#8217;interface <code>Collection</code> 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>Collection</code> est la racine de la hiérarchie de collection</p>
</li>
<li>
<p>Le JDK ne fournit pas d&#8217;implémentation spécifique pour cette interface</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
&#8658;
</td>
<td class="hdlist2">
<p>toutes les implémentations conviennent</p>
</td>
</tr>
</table>
</div>
</li>
<li>
<p>C&#8217;est le plus petit dénominateur commun pour les implémentations</p>
</li>
<li>
<p>Elle doit être utilisée quand un maximum de généralité est souhaitée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_collection_22"><a class="anchor" href="#_linterface_collection_22"></a><a class="link" href="#_linterface_collection_22">8.2.5. L&#8217;interface <code>Collection</code> 2/2</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface Collection&lt;E&gt; extends Iterable&lt;E&gt; {
  // Opérations simples
  int size();
  boolean isEmpty();
  boolean contains(Object element);
  boolean add(E element);    // Optionnel
  boolean remove(Object element); // Optionnel
  boolean equals(Object o);
  int hashCode();
  Iterator&lt;E&gt; iterator();

  // Opérations de groupe
  boolean containsAll(Collection&lt;?&gt; c);
  boolean addAll(Collection&lt;? extends E&gt; c);    // Optionnel
  boolean removeAll(Collection&lt;?&gt; c); // Optionnel
  default boolean removeIf(Predicate&lt;? super E&gt; filter);
  boolean retainAll(Collection&lt;?&gt; c); // Optionnel
  void clear();    // Optionnel

  // Conversions
  Object[] toArray();
  &lt;T&gt; T[] toArray(T[] a);

  // Itération et Streams
  Iterator&lt;E&gt; iterator();
  default Spliterator&lt;E&gt; spliterator();
  default Stream&lt;E&gt; stream();
  default Stream&lt;E&gt; parallelStream();
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_des_collections"><a class="anchor" href="#_parcourir_des_collections"></a><a class="link" href="#_parcourir_des_collections">8.2.6. Parcourir des collections</a></h4>
<div class="paragraph">
<p>Trois techniques permettent de parcourir des collections</p>
</div>
<div class="ulist">
<ul>
<li>
<p>Les <em>Streams</em></p>
</li>
<li>
<p>La boucle <em>for-each</em></p>
</li>
<li>
<p>Les itérateurs</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_les_streams"><a class="anchor" href="#_les_streams"></a><a class="link" href="#_les_streams">8.2.7. Les <em>Streams</em></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">String joined = elements.stream()
    .filter(e -&gt; e.getColor() == Color.RED)
    .map(Object::toString)
    .collect(Collectors.joining(", "));</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Plus de détails dans le chapitre suivant</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_boucle_for_each"><a class="anchor" href="#_boucle_for_each"></a><a class="link" href="#_boucle_for_each">8.2.8. Boucle <em>for-each</em></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">for (String element : uneCollectionDeChaines) {
    // Manipuler element
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La boucle <em>for-each</em> ne permet pas de modifier la collection lors de l&#8217;itération</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
&#8658;
</td>
<td class="hdlist2">
<p>utiliser un itérateur dans ce cas</p>
</td>
</tr>
</table>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_itérateur"><a class="anchor" href="#_itérateur"></a><a class="link" href="#_itérateur">8.2.9. Itérateur</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>itérateur</em> permet de parcourir une collection</p>
</li>
<li>
<p>La notion d&#8217;itérateur est implantée en Java par l&#8217;interface <code>Iterator</code></p>
</li>
<li>
<p>Un itérateur peut être vu comme un marqueur se trouvant entre deux éléments</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface Iterator&lt;E&gt; {
    boolean hasNext();
    E next();
    default void remove() {
        throw new UnsupportedOperationException("remove");
    }
    default void forEachRemaining(Consumer&lt;? super E&gt; action) {
        Objects.requireNonNull(action);
        while (hasNext())
            action.accept(next());
    }
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>L&#8217;utilisation de <code>remove</code> est le seul moyen sûr de modifier une collection lors du parcours</p>
</li>
<li>
<p>On ne peut utiliser <code>remove()</code> qu&#8217;une seule fois par appel à <code>next()</code></p>
</li>
<li>
<p>Un itérateur est basé sur le modèle de conception <a href="https://en.wikipedia.org/wiki/Iterator_pattern">Itérateur</a></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_parcours_dune_collection_avec_un_itérateur"><a class="anchor" href="#_parcours_dune_collection_avec_un_itérateur"></a><a class="link" href="#_parcours_dune_collection_avec_un_itérateur">8.2.10. Parcours d&#8217;une collection avec un itérateur</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">for (Iterator&lt;String&gt; i = uneCollectionDeChaines.iterator(); i.hasNext(); ) {
  String element = i.next(); // Récupère l'élément et passe au suivant
  // ...
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_set"><a class="anchor" href="#_linterface_set"></a><a class="link" href="#_linterface_set">8.2.11. L&#8217;interface <code>Set</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>Set</code> représente une collection sans duplicat</p>
<div class="ulist">
<ul>
<li>
<p>modélise le concept mathématique d&#8217;ensemble</p>
</li>
</ul>
</div>
</li>
<li>
<p>L&#8217;interface <code>Set</code> n&#8217;ajoute aucune méthode à l&#8217;interface <code>Collection</code></p>
</li>
<li>
<p>Deux ensembles sont égaux s&#8217;ils contiennent les mêmes éléments</p>
</li>
<li>
<p>Sémantique des méthodes de groupe</p>
<div class="ulist">
<ul>
<li>
<p><code>s1.containsAll(s2)</code> retourne <code>true</code> si \$s_2 sube s_1\$</p>
</li>
<li>
<p><code>s1.addAll(s2)</code> transforme s1 en \$s_1 uu s_2\$</p>
</li>
<li>
<p><code>s1.retainAll(s2)</code> transforme s1 en \$s_1 nn s_2\$</p>
</li>
<li>
<p><code>s1.removeAll(s2)</code> transforme s1 en \$s_1 \\ s_2\$</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_list_12"><a class="anchor" href="#_linterface_list_12"></a><a class="link" href="#_linterface_list_12">8.2.12. L&#8217;interface <code>List</code> 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>List</code> représente une <em>séquence</em> d&#8217;éléments, i.e. une collection ordonnée</p>
</li>
<li>
<p>L&#8217;interface <code>List</code> possède des opérations pour:</p>
<div class="ulist">
<ul>
<li>
<p>accéder aux éléments d&#8217;une liste par leurs indices</p>
</li>
<li>
<p>retourner l&#8217;indice d&#8217;un objet que l&#8217;on recherche</p>
</li>
<li>
<p>étendre la sémantique des itérateurs</p>
</li>
<li>
<p>manipuler des sous-listes</p>
</li>
</ul>
</div>
</li>
<li>
<p>Deux listes sont égales si elles possèdent les mêmes éléments dans le même ordre</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_list_22"><a class="anchor" href="#_linterface_list_22"></a><a class="link" href="#_linterface_list_22">8.2.13. L&#8217;interface <code>List</code> 2/2</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface List&lt;E&gt; extends Collection&lt;E&gt; {
  // Accès par position
  E get(int index);
  E set(int index, E element);            // Optionnel
  void add(int index, E element);              // Optionnel
  E remove(int index);                         // Optionnel
  boolean addAll(int index, Collection&lt;? extends E&gt; c); // Optionnel

  // Opération de groupe
  default void replaceAll(UnaryOperator&lt;E&gt; operator) {
        Objects.requireNonNull(operator);
        final ListIterator&lt;E&gt; li = this.listIterator();
        while (li.hasNext()) {
            li.set(operator.apply(li.next()));
        }
    }
  default void sort(Comparator&lt;? super E&gt; c) {
        Collections.sort(this, c);
    }

  // Recherche
  int indexOf(Object o);
  int lastIndexOf(Object o);

  // Itération
  ListIterator&lt;E&gt; listIterator();
  ListIterator&lt;E&gt; listIterator(int index);

  // Vue en sous-liste
  List&lt;E&gt; subList(int from, int to);
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_itérateur_de_liste"><a class="anchor" href="#_itérateur_de_liste"></a><a class="link" href="#_itérateur_de_liste">8.2.14. Itérateur de liste</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>ListIterator</code> étend l&#8217;interface <code>Iterator</code> pour permettre un parcours dans les deux sens</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface ListIterator&lt;E&gt; extends Iterator&lt;E&gt; {
    boolean hasPrevious();
    E previous();

    int nextIndex();
    int previousIndex();

    void set(E o);     // Optionnel
    void add(E o);     // Optionnel
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_queue"><a class="anchor" href="#_linterface_queue"></a><a class="link" href="#_linterface_queue">8.2.15. L&#8217;interface <code>Queue</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>Queue</code> représente une file</p>
</li>
<li>
<p>Les méthodes sont proposées sous deux formes</p>
</li>
</ul>
</div>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 33.3333%;">
<col style="width: 33.3333%;">
<col style="width: 33.3334%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top"></th>
<th class="tableblock halign-left valign-top">lance une exception</th>
<th class="tableblock halign-left valign-top">retourne une valeur spéciale</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Insertion</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>add(e)</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>offer(e)</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Suppression</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>remove()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>poll()</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Accès</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>element()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>peek()</code></p></td>
</tr>
</tbody>
</table>
<div class="ulist">
<ul>
<li>
<p>La stratégie d&#8217;insertion/suppression est définie par l&#8217;implémentation</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_dequeue"><a class="anchor" href="#_linterface_dequeue"></a><a class="link" href="#_linterface_dequeue">8.2.16. L&#8217;interface <code>DeQueue</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>DeQueue</code> représente une file à double entrée</p>
</li>
</ul>
</div>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
<col style="width: 20%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top"></th>
<th class="tableblock halign-left valign-top" colspan="2">Accès en tête</th>
<th class="tableblock halign-left valign-top" colspan="2">Accès en queue</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Exception</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Valeur spéciale</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Exception</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Valeur spéciale</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Insertion</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>addFirst(e)</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>offerFirst(e)</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>addLast(e)</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>offerLast(e)</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Suppression</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>removeFirst()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>pollFirst()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>removeLast()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>pollLast()</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><strong>Accès</strong></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>getFirst()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>peekFirst()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>getLast()</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>peekLast()</code></p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_linterface_map_12"><a class="anchor" href="#_linterface_map_12"></a><a class="link" href="#_linterface_map_12">8.2.17. L&#8217;interface <code>Map</code> 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <code>Map</code> représente un <em>tableau associatif</em> (<em>dictionnaire</em>)</p>
<div class="ulist">
<ul>
<li>
<p>i.e. un objet qui associe une clé à chaque valeur</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une clé peut correspondre à au plus une valeur</p>
<div class="ulist">
<ul>
<li>
<p>pas de multi-map en Java &#8658; utiliser une map avec une liste de valeurs associées à chaque clé</p>
</li>
</ul>
</div>
</li>
<li>
<p>Deux tableaux associatifs sont égaux s&#8217;ils représentent les mêmes associations clé/valeur</p>
</li>
</ul>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
Les objets mutables comme clés d&#8217;une <code>Map</code> peuvent poser problème
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_map_22"><a class="anchor" href="#_linterface_map_22"></a><a class="link" href="#_linterface_map_22">8.2.18. L&#8217;interface <code>Map</code> 2/2</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface Map&lt;K, V&gt; {
  // Opérations de base
  int size();
  boolean isEmpty();
  V put(K key, V value);
  V get(Object key);
  V remove(Object key);
  boolean containsKey(Object key);
  boolean containsValue(Object value);

  // Opérations sur des groupes
  void putAll(Map&lt;? extends K,? extends V&gt; t);
  void clear();

  // Vues
  public Set&lt;K&gt; keySet();
  public Collection&lt;V&gt; values();
  public Set&lt;Map.Entry&lt;K,V&gt;&gt; entrySet();

  // Interface pour entrySet
  public interface Entry&lt;K, V&gt; {
    K getKey();
    V getValue();
    V setValue(V value);
  }

  // + des méthodes par défaut
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_map"><a class="anchor" href="#_parcourir_une_map"></a><a class="link" href="#_parcourir_une_map">8.2.19. Parcourir une <code>Map</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Les méthodes de <em>vue comme collection</em> permettent de voir une <code>Map</code> comme une collection de trois façons différentes</p>
<div class="hdlist">
<table>
<tr>
<td class="hdlist1">
<code>keySet</code>
</td>
<td class="hdlist2">
<p>représente l'<strong>ensemble</strong> des clés</p>
</td>
</tr>
<tr>
<td class="hdlist1">
<code>values</code>
</td>
<td class="hdlist2">
<p>représente la <strong>collection</strong> des valeurs</p>
</td>
</tr>
<tr>
<td class="hdlist1">
<code>entrySet</code>
</td>
<td class="hdlist2">
<p>représente l&#8217;ensemble des couples <em>(clé, valeur)</em></p>
</td>
</tr>
</table>
</div>
</li>
<li>
<p>Ces méthodes fournissent un moyen pour parcourir une <code>Map</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_construire_lhistogramme_dune_image"><a class="anchor" href="#_construire_lhistogramme_dune_image"></a><a class="link" href="#_construire_lhistogramme_dune_image">8.2.20. Construire l&#8217;histogramme d&#8217;une image</a></h4>
<div class="listingblock">
<div class="title">Méthode de construction de l&#8217;histogramme</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Produit l'histogramme d'une image.
 *
 * @param img l'image à analyser
 * @return l'histogramme de l'image sous la forme d'un dictionnaire (couleur, fréquence)
 */
public static Map&lt;Integer, Long&gt; frequency(int[][] img) {
    Stream&lt;Integer&gt; imgColors = Arrays.stream(img)
            .flatMap(c -&gt; Arrays.stream(c).boxed());
    Map&lt;Integer, Long&gt; frequencyMap = imgColors.collect(
            Collectors.groupingBy(
                    Function.identity(), Collectors.counting()
            )
    );
    return frequencyMap;
}</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Manipulation de l&#8217;histogramme</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">int[][] image = {
        {0, 1, 12, 1},
        {1, 12, 12, 12},
        {0, 12, 12, 0}
};

Map&lt;Integer, Long&gt; histogramme = frequency(image);
System.out.println(histogramme); // {0=3, 1=3, 12=6}
System.out.println(histogramme.keySet()); // [0, 1, 12]

Optional&lt;Long&gt; max = histogramme.values().stream()
        .max(Comparator.naturalOrder());
System.out.format("Fréq. max. : %d%n", max.orElse(-1L)); // Fréq. max. : 6</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_ordonner_des_objets"><a class="anchor" href="#_ordonner_des_objets"></a><a class="link" href="#_ordonner_des_objets">8.2.21. Ordonner des objets</a></h4>
<div class="ulist">
<div class="title">Le problème</div>
<ul>
<li>
<p>Comment ordonner des objets selon leur <em>ordre naturel</em> (lexicographique pour les chaînes, chronologique pour les dates, &#8230;&#8203;) ?</p>
</li>
</ul>
</div>
<div class="ulist">
<div class="title">En Java</div>
<ul>
<li>
<p>La solution proposée est d&#8217;implémenter l&#8217;interface <code>Comparable</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_comparable"><a class="anchor" href="#_linterface_comparable"></a><a class="link" href="#_linterface_comparable">8.2.22. L&#8217;interface <code>Comparable</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface Comparable&lt;T&gt; {
  public int compareTo(&lt;T&gt; o);
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La plupart des classes de la librairie Java implémentent cette interface</p>
</li>
<li>
<p><code>compareTo</code> doit retourner un entier négatif (respectivement zéro, un entier positif) si l&#8217;objet est inférieur (respectivement égal, supérieur) au paramètre</p>
</li>
<li>
<p>Si l&#8217;argument n&#8217;est pas du bon type, <code>compareTo</code> doit lancer l&#8217;exception <code>ClassCastException</code></p>
</li>
<li>
<p>L&#8217;ordre ainsi défini doit induire un <em>ordre partiel</em> (cf. la documentation de <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Comparable.html"><code>Comparable</code></a>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_définir_un_ordre_naturel_sur_des_personnes"><a class="anchor" href="#_définir_un_ordre_naturel_sur_des_personnes"></a><a class="link" href="#_définir_un_ordre_naturel_sur_des_personnes">8.2.23. Définir un ordre naturel sur des personnes</a></h4>
<div class="listingblock">
<div class="title">Déclaration de la classe</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">class Person implements Comparable&lt;Person&gt; {</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Redéfinition de la comparaison selon l&#8217;ordre naturel</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">/**
 * Compare deux personnes.
 * La comparaison se fait d'abord selon l'ordre
 * lexicographique du nom puis selon le prénom.
 *
 * @param p une personne
 * @return la valeur de comparaison entre les chaînes représentant les noms
 * ou entre les prénoms si les noms sont égaux.
 */
@Override
public int compareTo(Person p) {
    int cmpNom = nom.compareTo(p.nom);
    return (cmpNom != 0 ? cmpNom : prenom.compareTo(p.prenom));
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_ordonner_des_objets_selon_un_ordre_spécifique"><a class="anchor" href="#_ordonner_des_objets_selon_un_ordre_spécifique"></a><a class="link" href="#_ordonner_des_objets_selon_un_ordre_spécifique">8.2.24. Ordonner des objets selon un ordre spécifique</a></h4>
<div class="ulist">
<div class="title">Le problème</div>
<ul>
<li>
<p>Comment ordonner des objets selon un ordre particulier (différent de l&#8217;ordre naturel) ?</p>
</li>
</ul>
</div>
<div class="ulist">
<div class="title">En Java</div>
<ul>
<li>
<p>La solution proposée est de fournir un <em>comparateur</em>, i.e. une instance d&#8217;une classe implémentant l&#8217;interface <code>Comparator</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_comparator"><a class="anchor" href="#_linterface_comparator"></a><a class="link" href="#_linterface_comparator">8.2.25. L&#8217;interface <code>Comparator</code></a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface Comparator&lt;T&gt; {
  int compare(T o1, T o2);
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p><code>compare</code> doit retourner un entier négatif (respectivement zéro, un entier positif) si le premier paramètre est inférieur (respectivement égal, supérieur) au second</p>
</li>
<li>
<p>Si l&#8217;argument n&#8217;est pas du bon type, <code>compare</code> doit lancer l&#8217;exception <code>ClassCastException</code></p>
</li>
<li>
<p>L&#8217;ordre ainsi défini doit induire un <em>ordre partiel</em> (cf. la documentation de <a href="https://docs.oracle.com/javase/8/docs/api/java/util/Comparator.html"><code>Comparator</code></a>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_définir_un_ordre_spécifique_sur_des_personnes"><a class="anchor" href="#_définir_un_ordre_spécifique_sur_des_personnes"></a><a class="link" href="#_définir_un_ordre_spécifique_sur_des_personnes">8.2.26. Définir un ordre spécifique sur des personnes</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">package fr.uvsq.info.poo.collections;

import java.util.Comparator;

/**
 * Permet de comparer des personnes selon leur âge.
 *
 * @author Author1
 * @version Version1
 */
class ByAgeComparator implements Comparator&lt;Person&gt; {
    /**
     * Compare deux personnes selon leur âge.
     *
     * @return l'écart d'age entre les deux personnes.
     */
    public int compare(Person p1, Person p2) {
        return p1.getAge() - p2.getAge();
    }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_trier_une_liste_de_personnes"><a class="anchor" href="#_trier_une_liste_de_personnes"></a><a class="link" href="#_trier_une_liste_de_personnes">8.2.27. Trier une liste de personnes</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Person&gt; lst = Arrays.asList(
        new Person("Ariane", "Dupond", 9),
        new Person("Cassiopée", "Dupond", 8),
        new Person("Hélios", "Martin", 4)
);

Collections.sort(lst); // tri selon l'ordre naturel
System.out.println(lst);

Collections.sort(lst, new ByAgeComparator()); // peut être remplacé par
lst.sort((p1, p2) -&gt; p1.getAge() - p2.getAge()); // peut être remplacé par
lst.sort(Comparator.comparing(Person::getAge)); // tri selon l'âge
System.out.println(lst);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_sortedset_12"><a class="anchor" href="#_linterface_sortedset_12"></a><a class="link" href="#_linterface_sortedset_12">8.2.28. L&#8217;interface <code>SortedSet</code> 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Cette interface permet de maintenir les éléments d&#8217;une ensemble en ordre croissant selon l&#8217;ordre naturel ou un ordre spécifié par un comparateur</p>
</li>
<li>
<p>Elle fournit des méthodes pour:</p>
<div class="ulist">
<ul>
<li>
<p>manipuler un interval d&#8217;éléments</p>
</li>
<li>
<p>accéder au plus petit ou au plus grand élément</p>
</li>
<li>
<p>récupérer le comparateur utilisé (s&#8217;il existe)</p>
</li>
</ul>
</div>
</li>
<li>
<p>Les opérations héritées de <code>Set</code> fonctionnent à l&#8217;identique mais :</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;itérateur respecte l&#8217;ordre</p>
</li>
<li>
<p><code>toArray</code> conserve l&#8217;ordre</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_sortedset_22"><a class="anchor" href="#_linterface_sortedset_22"></a><a class="link" href="#_linterface_sortedset_22">8.2.29. L&#8217;interface <code>SortedSet</code> 2/2</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface SortedSet&lt;E&gt; extends Set&lt;E&gt; {
  // Vue par intervalle
  SortedSet&lt;E&gt; subSet(E fromElement, E toElement);
  SortedSet&lt;E&gt; headSet(E toElement);
  SortedSet&lt;E&gt; tailSet(E fromElement);

  // Extrémités
  E first();
  E last();

  // Comparateur
  Comparator&lt;? super E&gt; comparator();
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_sortedmap_12"><a class="anchor" href="#_linterface_sortedmap_12"></a><a class="link" href="#_linterface_sortedmap_12">8.2.30. L&#8217;interface <code>SortedMap</code> 1/2</a></h4>
<div class="ulist">
<ul>
<li>
<p>Cette interface permet de maintenir une <code>Map</code> ordonnée selon l&#8217;odre naturel de ses clés ou selon un comparateur</p>
</li>
<li>
<p>Elle fournit des méthodes pour:</p>
<div class="ulist">
<ul>
<li>
<p>manipuler un interval d&#8217;éléments</p>
</li>
<li>
<p>accéder au plus petit ou au plus grand élément</p>
</li>
<li>
<p>récupérer le comparateur utilisé (s&#8217;il existe)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_sortedmap_22"><a class="anchor" href="#_linterface_sortedmap_22"></a><a class="link" href="#_linterface_sortedmap_22">8.2.31. L&#8217;interface <code>SortedMap</code> 2/2</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public interface SortedMap&lt;K, V&gt; extends Map&lt;K, V&gt; {
  // Range-view
  SortedMap&lt;K, V&gt; subMap(K fromKey, K toKey);
  SortedMap&lt;K, V&gt; headMap(K toKey);
  SortedMap&lt;K, V&gt; tailMap(K fromKey);

  // Endpoints
  K firstKey();
  K lastKey();

  // Comparator access
  Comparator&lt;? super K&gt; comparator();
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_implémentations_2"><a class="anchor" href="#_implémentations_2"></a><a class="link" href="#_implémentations_2">8.3. Implémentations</a></h3>
<div class="sect3">
<h4 id="_les_implémentations"><a class="anchor" href="#_les_implémentations"></a><a class="link" href="#_les_implémentations">8.3.1. Les implémentations</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les implémentations sont les structures de données proprement dites</p>
</li>
<li>
<p>On en trouve plusieurs sortes en Java</p>
<div class="ulist">
<ul>
<li>
<p>les <em>implémentations généralistes</em> sont les plus couramment utilisées</p>
</li>
<li>
<p>les <em>implémentations spécialisées</em> sont conçues pour un cas particulier</p>
</li>
<li>
<p>les <em>implémentations supportant la concurrence</em> pour les applications multi-threads</p>
</li>
<li>
<p>les <em>implémentations "décorations"</em> permettent de modifier les caractéristiques d&#8217;une autre implémentation</p>
</li>
<li>
<p>les <em>implémentations "simples"</em> sont des implémentations minimalistes optimisées pour un cas particulier (singleton par exemple)</p>
</li>
<li>
<p>les <em>implémentations abstraites</em> servent de base pour le développement d&#8217;implémentation personnalisée</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_implémentations_généralistes"><a class="anchor" href="#_implémentations_généralistes"></a><a class="link" href="#_implémentations_généralistes">8.3.2. Implémentations généralistes</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.6666%;">
<col style="width: 16.667%;">
</colgroup>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Interface</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Hashage</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Tableau dyn.</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Arbre équ.</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Liste chaînée</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Hash. + chaîn.</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>Set</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code><strong>HashSet</strong></code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>TreeSet</code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>LinkedHashSet</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>List</code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code><strong>ArrayList</strong></code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>LinkedList</code></p></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>Queue</code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code><strong>ArrayDeque</strong></code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>LinkedList</code></p></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>DeQueue</code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code><strong>ArrayDeque</strong></code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>LinkedList</code></p></td>
<td class="tableblock halign-left valign-top"></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>Map</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code><strong>HashMap</strong></code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>TreeMap</code></p></td>
<td class="tableblock halign-left valign-top"></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>LinkedHashMap</code></p></td>
</tr>
</tbody>
</table>
<div class="ulist">
<ul>
<li>
<p>Les implémentations principales sont en gras</p>
</li>
<li>
<p><code>TreeSet</code> (respectivement <code>TreeMap</code>) implémente également <code>SortedSet</code> (respectivement <code>SortedMap</code>)</p>
</li>
<li>
<p><code>Queue</code> possède aussi pour implémentation <code>PriorityQueue</code></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_caractéristiques_des_implémentations_généralistes"><a class="anchor" href="#_caractéristiques_des_implémentations_généralistes"></a><a class="link" href="#_caractéristiques_des_implémentations_généralistes">8.3.3. Caractéristiques des implémentations généralistes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Toutes les implémentations implémentent toutes les méthodes optionnelles</p>
</li>
<li>
<p>Toutes sont sérialisables</p>
</li>
<li>
<p>Toutes supportent l&#8217;opération <code>clone</code></p>
</li>
<li>
<p>Elles ne sont pas synchronisées (pour des raisons de performance)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utilisation_des_implémentations_généralistes"><a class="anchor" href="#_utilisation_des_implémentations_généralistes"></a><a class="link" href="#_utilisation_des_implémentations_généralistes">8.3.4. Utilisation des implémentations généralistes</a></h4>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Choisir un type d&#8217;implémentation</p>
</li>
<li>
<p>Créer une instance de cette implémentation</p>
</li>
<li>
<p>La lier à une référence sur l&#8217;interface correspondante</p>
<div class="ulist">
<ul>
<li>
<p>le programme reste alors indépendant du choix de l&#8217;implémentation</p>
</li>
</ul>
</div>
</li>
</ol>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Set&lt;Integer&gt; unEnsemble = new HashSet&lt;&gt;();
List&lt;Integer&gt; uneList = new ArrayList&lt;&gt;();
Map&lt;String, String&gt; uneMap = new HashMap&lt;&gt;();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_implémentations_généralistes_de_set"><a class="anchor" href="#_les_implémentations_généralistes_de_set"></a><a class="link" href="#_les_implémentations_généralistes_de_set">8.3.5. Les implémentations généralistes de <code>Set</code></a></h4>
<div class="ulist">
<ul>
<li>
<p><code>HashSet</code> est plus rapide mais ne garantit pas l&#8217;ordre</p>
<div class="ulist">
<ul>
<li>
<p>la plupart des opérations sont en temps constant</p>
</li>
<li>
<p>la <em>capacité</em> et le <em>facteur de charge</em> permettent d&#8217;affiner les performances de <code>HashSet</code></p>
</li>
</ul>
</div>
</li>
<li>
<p><code>TreeSet</code> maintient l&#8217;ordre des éléments</p>
<div class="ulist">
<ul>
<li>
<p>la plupart des opérations sont en temps logarithmique</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock tip">
<table>
<tr>
<td class="icon">
<i class="fa icon-tip" title="Tip"></i>
</td>
<td class="content">
on choisit <code>HashSet</code> sauf si on a besoin d&#8217;un ordre sur les éléments
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_les_implémentations_généralistes_de_map"><a class="anchor" href="#_les_implémentations_généralistes_de_map"></a><a class="link" href="#_les_implémentations_généralistes_de_map">8.3.6. Les implémentations généralistes de <code>Map</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>Situation analogue à <code>Set</code></p>
</li>
</ul>
</div>
<div class="admonitionblock tip">
<table>
<tr>
<td class="icon">
<i class="fa icon-tip" title="Tip"></i>
</td>
<td class="content">
on choisit <code>HashMap</code> sauf si on a besoin d&#8217;un ordre sur les éléments
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_les_implémentations_de_list"><a class="anchor" href="#_les_implémentations_de_list"></a><a class="link" href="#_les_implémentations_de_list">8.3.7. Les implémentations de <code>List</code></a></h4>
<div class="ulist">
<ul>
<li>
<p><code>ArrayList</code> est plus rapide</p>
<div class="ulist">
<ul>
<li>
<p>permet un accès par position en temps constant</p>
</li>
<li>
<p>pas d&#8217;allocation à chaque ajout</p>
</li>
<li>
<p>on peut passer une <em>capacité</em> au constructeur de <code>ArrayList</code></p>
</li>
<li>
<p>possède les opérations <code>ensureCapacity</code> et <code>trimToSize</code> en plus de celle de l&#8217;interface <code>List</code></p>
</li>
</ul>
</div>
</li>
<li>
<p><code>LinkedList</code> est linéaire pour l&#8217;accès par position</p>
<div class="ulist">
<ul>
<li>
<p>adaptée si on fait beaucoup d&#8217;insertions/suppressions en milieu de liste (opérations en temps constant mais le facteur constant est élevé)</p>
</li>
<li>
<p>possède les opérations <code>addFirst</code>, <code>getFirst</code>, <code>removeFirst</code>, <code>addLast</code>, <code>getLast</code>, et <code>removeLast</code></p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="admonitionblock tip">
<table>
<tr>
<td class="icon">
<i class="fa icon-tip" title="Tip"></i>
</td>
<td class="content">
on choisit <code>ArrayList</code> sauf si on a beaucoup de modifications en milieu de liste
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_implémentations_spécialisées"><a class="anchor" href="#_quelques_implémentations_spécialisées"></a><a class="link" href="#_quelques_implémentations_spécialisées">8.3.8. Quelques implémentations spécialisées</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>EnumSet</code> (<code>Set</code>) est une implémentation efficace (vecteur de bits) pour les énumérations</p>
</li>
<li>
<p><code>CopyOnWriteArraySet</code> (<code>Set</code>) effectue une copie de l&#8217;ensemble pour chaque modification</p>
</li>
<li>
<p><code>CopyOnWriteArrayList</code> (<code>List</code>) effectue une copie de la liste pour chaque modification</p>
</li>
<li>
<p><code>EnumMap</code> (<code>Map</code>) permet d&#8217;associer une instance d&#8217;énumération à une valeur</p>
</li>
<li>
<p><code>WeakHashMap</code> (<code>Map</code>) autorise la libération de la mémoire d&#8217;une paire (clé, valeur) dès que la clé n&#8217;est plus référencée</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_implémentations_décorations"><a class="anchor" href="#_implémentations_décorations"></a><a class="link" href="#_implémentations_décorations">8.3.9. Implémentations "décorations"</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une telle implémentation délégue les traitements principaux à une collection particulière mais y ajoute un certain nombre de fonctionnalités</p>
<div class="ulist">
<ul>
<li>
<p>modèle de conception <em>Décorateur</em></p>
</li>
</ul>
</div>
</li>
<li>
<p>Ces implémentations sont <em>anonymes</em></p>
<div class="ulist">
<ul>
<li>
<p>pas de classe publique mais une méthode de fabrication statique</p>
</li>
<li>
<p>on les obtient par des méthodes de classe (<em>static factory method</em>) de la classe <code>Collections</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Plusieurs catégories sont disponibles :</p>
<div class="ulist">
<ul>
<li>
<p>avec synchronisation pour rendre les collections "tolérantes aux threads"</p>
</li>
<li>
<p>non modifiables pour supprimer toute possibilité de modification d&#8217;une collection</p>
</li>
<li>
<p>vérifiant le type dynamiquement</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; list = Collections.synchronizedList(new ArrayList&lt;Integer&gt;());
Collection&lt;String&gt; collec = Collections.unmodifiableCollection(uneCollection);
Set&lt;String&gt; set = Collections.checkedSet(new HashSet&lt;String&gt;(), String.class);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_les_implémentations_simples"><a class="anchor" href="#_les_implémentations_simples"></a><a class="link" href="#_les_implémentations_simples">8.3.10. Les implémentations "simples"</a></h4>
<div class="ulist">
<ul>
<li>
<p>Ces implémentations sont des "mini" implémentations plus pratiques et généralement plus performantes que les implémentations généralistes</p>
<div class="ulist">
<ul>
<li>
<p><code>Arrays.asList</code> permet de manipuler un tableau comme une liste</p>
</li>
<li>
<p><code>Collections.nCopies</code> génère une liste non modifiable contenant de multiples copies du même élément</p>
</li>
<li>
<p><code>Collections.singleton</code> génère un ensemble non modifiable contenant un unique élément</p>
</li>
<li>
<p><code>emptySet</code>, <code>emptyList</code> et <code>emptyMap</code> de la classe <code>Collections</code> représentent l&#8217;ensemble, la liste et le tableau associatif vides</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_utiliser_des_implémentations_simples"><a class="anchor" href="#_utiliser_des_implémentations_simples"></a><a class="link" href="#_utiliser_des_implémentations_simples">8.3.11. Utiliser des implémentations "simples"</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Créer une liste de taille fixe
List&lt;String&gt; list = Arrays.asList(new String[size]);

// Créer une liste de 1000 éléments initialisés à null
List&lt;Type&gt; l = new ArrayList&lt;&gt;(Collections.nCopies(1000, (Type)null));

// Ajouter 10 fois la chaîne "element" à une collection
uneCollection.addAll(Collections.nCopies(10, "element"));

// Supprimer toutes les occurences de e dans la collection
c.removeAll(Collections.singleton(e));

// Supprimer tous les juristes d'une map
profession.values().removeAll(Collections.singleton(JURISTE));

// Récupérer une liste vide
List&lt;String&gt; s = Collections.emptyList();</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_écrire_une_implémentation"><a class="anchor" href="#_écrire_une_implémentation"></a><a class="link" href="#_écrire_une_implémentation">8.3.12. Écrire une implémentation</a></h4>
<div class="ulist">
<ul>
<li>
<p>La notion d'<em>implémentation abstraite</em> simplifie l&#8217;écriture d&#8217;une implémentation</p>
</li>
<li>
<p>Une <em>implémentation abstraite</em> est un squelette d&#8217;implémentation d&#8217;une collection</p>
</li>
<li>
<p>Processus pour écrire son implémentation</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>choisir une implémentation abstraite appropriée</p>
</li>
<li>
<p>implémenter les méthodes abstraites (et éventuellement certaines méthodes concrêtes)</p>
</li>
<li>
<p>tester l&#8217;implémentation obtenue</p>
</li>
<li>
<p>si les performances sont importantes, étudier les caractéristiques des méthodes héritées et les redéfinir si nécessaire</p>
</li>
</ol>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_principales_implémentations_abstraites"><a class="anchor" href="#_principales_implémentations_abstraites"></a><a class="link" href="#_principales_implémentations_abstraites">8.3.13. Principales implémentations abstraites</a></h4>
<div class="ulist">
<ul>
<li>
<p><code>AbstractCollection</code> pour une collection quelconque</p>
<div class="ulist">
<ul>
<li>
<p>les méthodes <code>iterator</code> et <code>size</code> doivent être fournies</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>AbstractSet</code> pour un ensemble (même utilisation que <code>AbstractCollection</code>)</p>
</li>
<li>
<p><code>AbstractList</code> pour une liste basée sur une structure à accès aléatoire (comme un tableau)</p>
<div class="ulist">
<ul>
<li>
<p>les méthodes <code>get(int)</code> et <code>size</code> doivent être fournies</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>AbstractSequentialList</code> pour une liste basée sur une structure à accès séquentiel (comme une liste chaînée)</p>
<div class="ulist">
<ul>
<li>
<p>les méthodes <code>listIterator</code> et <code>size</code> doivent être fournies</p>
</li>
</ul>
</div>
</li>
<li>
<p><code>AbstractQueue</code> nécessite de fournir les méthodes <code>offer</code>, <code>peek</code>, <code>poll</code> et <code>size</code> ainsi qu&#8217;un itérateur supportant <code>remove</code></p>
</li>
<li>
<p><code>AbstractMap</code> pour un tableau associatif</p>
<div class="ulist">
<ul>
<li>
<p>la vue <code>entrySet</code> doit être fournie</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_algorithmes"><a class="anchor" href="#_algorithmes"></a><a class="link" href="#_algorithmes">8.4. Algorithmes</a></h3>
<div class="sect3">
<h4 id="_les_algorithmes"><a class="anchor" href="#_les_algorithmes"></a><a class="link" href="#_les_algorithmes">8.4.1. Les algorithmes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les algorithmes sont des méthodes de classe de la classe <a href="https://docs.oracle.com/javase/8/docs/api/java/util/Collections.html"><code>Collections</code></a></p>
</li>
<li>
<p>Le premier paramètre de ces algorithmes est la collection traitée</p>
</li>
<li>
<p>La plupart opèrent sur des listes</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_algorithmes_disponibles"><a class="anchor" href="#_quelques_algorithmes_disponibles"></a><a class="link" href="#_quelques_algorithmes_disponibles">8.4.2. Quelques algorithmes disponibles</a></h4>
<div class="ulist">
<ul>
<li>
<p>tri : <code>sort</code> (complexité en \$n log(n)\$, stable)</p>
</li>
<li>
<p>mélange : <code>shuffle</code></p>
</li>
<li>
<p>manipulation des données : <code>reverse</code>, <code>fill</code>, <code>copy</code>, <code>swap</code>, <code>addAll</code></p>
</li>
<li>
<p>recherche dans une collection triée : <code>binarySearch</code></p>
</li>
<li>
<p>composition : <code>frequency</code>, <code>disjoint</code></p>
</li>
<li>
<p>extremum : <code>min</code>, <code>max</code></p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; l = new ArrayList&lt;Integer&gt;();
// ...
Collections.sort(l);
int pos = Collections.binarySearch(l, key);</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_mise_en_uvre"><a class="anchor" href="#_mise_en_uvre"></a><a class="link" href="#_mise_en_uvre">8.5. Mise en &oelig;uvre</a></h3>
<div class="sect3">
<h4 id="_exercice_sur_les_listes"><a class="anchor" href="#_exercice_sur_les_listes"></a><a class="link" href="#_exercice_sur_les_listes">8.5.1. Exercice sur les listes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Créer une liste (basée sur <code>ArrayList</code>) contenant les 10 premiers entiers</p>
</li>
<li>
<p>Mélanger aléatoirement les éléments</p>
<div class="ulist">
<ul>
<li>
<p>utiliser la méthode de classe <code>void shuffle(List&lt;?&gt; list)</code> de la classe <code>Collections</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Afficher la liste à l&#8217;endroit puis à l&#8217;envers</p>
</li>
<li>
<p>Trier la liste selon l&#8217;ordre naturel (croissant) puis selon l&#8217;ordre inverse (décroissant)</p>
<div class="ulist">
<ul>
<li>
<p>utiliser les méthodes de classe <code>void sort(List&lt;?&gt; list)</code> et <code>void sort(List&lt;?&gt; list, Comparator&lt;? super T&gt; c)</code> de la classe <code>Collections</code></p>
</li>
</ul>
</div>
</li>
<li>
<p>Que doit-on changer pour utiliser une <code>LinkedList</code> à la place d&#8217;une <code>ArrayList</code> ?</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_créer_une_liste_contenant_les_10_premiers_entiers"><a class="anchor" href="#_créer_une_liste_contenant_les_10_premiers_entiers"></a><a class="link" href="#_créer_une_liste_contenant_les_10_premiers_entiers">8.5.2. Créer une liste contenant les 10 premiers entiers</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; uneListe = new ArrayList&lt;&gt;();
for (int i = 0; i &lt; MAX; ++i) uneListe.add(i);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_mélanger_aléatoirement_les_éléments"><a class="anchor" href="#_mélanger_aléatoirement_les_éléments"></a><a class="link" href="#_mélanger_aléatoirement_les_éléments">8.5.3. Mélanger aléatoirement les éléments</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Collections.shuffle(uneListe);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_afficher_la_liste_à_lendroit_puis_à_lenvers"><a class="anchor" href="#_afficher_la_liste_à_lendroit_puis_à_lenvers"></a><a class="link" href="#_afficher_la_liste_à_lendroit_puis_à_lenvers">8.5.4. Afficher la liste à l&#8217;endroit puis à l&#8217;envers</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">System.out.println(uneListe);
for (ListIterator&lt;Integer&gt; it = uneListe.listIterator(uneListe.size());
     it.hasPrevious(); ) {
    System.out.print(it.previous());
    System.out.print(", ");
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_trier_la_liste_selon_lordre_naturel_croissant_puis_selon_lordre_inverse_décroissant"><a class="anchor" href="#_trier_la_liste_selon_lordre_naturel_croissant_puis_selon_lordre_inverse_décroissant"></a><a class="link" href="#_trier_la_liste_selon_lordre_naturel_croissant_puis_selon_lordre_inverse_décroissant">8.5.5. Trier la liste selon l&#8217;ordre naturel (croissant) puis selon l&#8217;ordre inverse (décroissant)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Collections.sort(uneListe);</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">uneListe.sort((i1, i2) -&gt; i2 - i1);</code></pre>
</div>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">uneListe.sort(Collections.reverseOrder());</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_que_doit_on_changer_pour_utiliser_une_linkedlist_à_la_place_dune_arraylist"><a class="anchor" href="#_que_doit_on_changer_pour_utiliser_une_linkedlist_à_la_place_dune_arraylist"></a><a class="link" href="#_que_doit_on_changer_pour_utiliser_une_linkedlist_à_la_place_dune_arraylist">8.5.6. Que doit-on changer pour utiliser une <code>LinkedList</code> à la place d&#8217;une <code>ArrayList</code> ?</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// Remplacer
List&lt;Integer&gt; uneListe = new ArrayList&lt;&gt;();
// Par
List&lt;Integer&gt; uneListe = new LinkedList&lt;&gt;();
//
// Le reste du programme ne change pas !
//</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exercice_sur_les_tableaux_associatifs"><a class="anchor" href="#_exercice_sur_les_tableaux_associatifs"></a><a class="link" href="#_exercice_sur_les_tableaux_associatifs">8.5.7. Exercice sur les tableaux associatifs</a></h4>
<div class="ulist">
<ul>
<li>
<p>Créer un tableau associatif (<code>HashMap</code>) contenant les 10 premiers entiers associés à leur cube</p>
</li>
<li>
<p>Afficher les valeurs des cubes triées par ordre croissant</p>
</li>
<li>
<p>Afficher les nombres pairs et leur cube</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_créer_un_tableau_associatif_contenant_les_10_premiers_entiers_associés_à_leur_cube"><a class="anchor" href="#_créer_un_tableau_associatif_contenant_les_10_premiers_entiers_associés_à_leur_cube"></a><a class="link" href="#_créer_un_tableau_associatif_contenant_les_10_premiers_entiers_associés_à_leur_cube">8.5.8. Créer un tableau associatif contenant les 10 premiers entiers associés à leur cube</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Map&lt;Integer, Integer&gt; uneMap = new HashMap&lt;&gt;();
for (int i = 0; i &lt; MAX; ++i) uneMap.put(i, i * i * i);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_afficher_les_valeurs_des_cubes_triées_par_ordre_croissant"><a class="anchor" href="#_afficher_les_valeurs_des_cubes_triées_par_ordre_croissant"></a><a class="link" href="#_afficher_les_valeurs_des_cubes_triées_par_ordre_croissant">8.5.9. Afficher les valeurs des cubes triées par ordre croissant</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; lesCubes = new ArrayList&lt;&gt;(uneMap.values());
Collections.sort(lesCubes);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_afficher_les_nombres_pairs_et_leur_cube"><a class="anchor" href="#_afficher_les_nombres_pairs_et_leur_cube"></a><a class="link" href="#_afficher_les_nombres_pairs_et_leur_cube">8.5.10. Afficher les nombres pairs et leur cube</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">for (Map.Entry&lt;Integer, Integer&gt; elt : uneMap.entrySet()) {
    if (elt.getKey() % 2 == 0) {
        System.out.println(elt.getKey() + " -&gt; " + elt.getValue());
    }
}</code></pre>
</div>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_3"><a class="anchor" href="#_exercices_3"></a><a class="link" href="#_exercices_3">8.6. Exercices</a></h3>
<div class="sect3">
<h4 id="_utilisation_des_collections"><a class="anchor" href="#_utilisation_des_collections"></a><a class="link" href="#_utilisation_des_collections">8.6.1. Utilisation des collections</a></h4>
<div class="paragraph">
<p>L&#8217;objet de cet exercice est de simuler l&#8217;interrogation d&#8217;un DNS (<em>Domain Name Server</em>).
Un DNS convertit une adresse IP (<code>192.168.0.1</code> par exemple) en un nom qualifié de machine (<code>machine.domaine.local</code> par exemple) et inversement.
Un nom qualifié comporte le nom de la machine (avant le premier <code>'.'</code>) et un nom de domaine (après le premier <code>'.'</code>).</p>
</div>
<div class="paragraph">
<p>L&#8217;interface proposera une ligne de commande à partir de laquelle les commandes suivantes devront être interprétées:</p>
</div>
<div class="ulist">
<ul>
<li>
<p><code>nom.qualifié.machine</code> : l&#8217;adresse IP de la machine est affichée;</p>
</li>
<li>
<p><code>adr.es.se.ip</code> : le nom qualifié de cette machine est affiché;</p>
</li>
<li>
<p><code>ls [-a]</code> <em>domaine</em> : la liste des machines du domaine <em>domaine</em> sera affichée triée selon le nom des machines ou selon les adresses IP (si <code>-a</code> est présent).</p>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>La base de données du serveur sera conservée dans un fichier texte (une ligne par machine au format &#8220;un_nom_de_machine une.adresse.IP&#8221;) chargé au lancement du programme.</p>
</li>
<li>
<p>Le nom du fichier devra être stocké dans un fichier de propriétés (cf. <a href="http://docs.oracle.com/javase/tutorial/essential/environment/properties.html">Tutoriel sur les propriétés</a>).</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Réaliser les classes <code>AdresseIP</code>, <code>NomMachine</code> et <code>DnsItem</code> qui représentent respectivement une adresse IP, un nom qualifié de machine et une entrée du DNS.</p>
</li>
<li>
<p>Réaliser la classe <code>Dns</code> qui proposera les opérations suivantes:</p>
<div class="ulist">
<ul>
<li>
<p>un constructeur qui chargera la base de données,</p>
</li>
<li>
<p>deux méthodes <code>getItem</code> qui retourneront une instance de <code>DnsItem</code> soit à partir d&#8217;une adresse IP, soit à partir d&#8217;un nom de machine,</p>
</li>
<li>
<p>une méthode <code>getItems</code> qui retournera une liste d&#8217;items à partir d&#8217;un nom de domaine.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Réaliser la classe <code>DnsTUI</code> qui se chargera des interactions avec l&#8217;utilisateur.
Cette classe fournira une méthode <code>nextCommande</code> qui analysera le texte saisi par l&#8217;utilisateur et retournera un objet implémentant l&#8217;interface <code>Commande</code> (cf. question suivante) et une méthode <code>affiche</code> qui affichera un résultat.</p>
</li>
<li>
<p>Les commandes DNS seront implémentées à l&#8217;aide du modèle de conception <a href="http://en.wikipedia.org/wiki/Command_pattern">Commande</a>.</p>
<div class="ulist">
<ul>
<li>
<p>créer l&#8217;interface <code>Commande</code> comportant une seule méthode <code>execute</code>,</p>
</li>
<li>
<p>créer une classe implémentant cette interface pour chaque action (rechercher une IP, rechercher un nom, rechercher les machines d&#8217;un domaine, quitter l&#8217;application).</p>
</li>
</ul>
</div>
</li>
<li>
<p>Réaliser la classe principale <code>DnsApp</code>.
La méthode <code>run</code> de cette classe interagira avec l&#8217;interface utilisateur pour récupérer la prochaine commande, l&#8217;exécutera puis affichera la résultat.</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_écriture_dalgorithmes"><a class="anchor" href="#_écriture_dalgorithmes"></a><a class="link" href="#_écriture_dalgorithmes">8.6.2. Écriture d&#8217;algorithmes</a></h4>
<div class="paragraph">
<p>Le but de cet exercice est d&#8217;écrire des algorithmes pouvant s&#8217;appliquer à toute collection respectant l&#8217;interface <code>List</code>.</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Ecrire un algorithme <code>bubbleSort</code> implémentant le tri à bulle.
Deux versions de l&#8217;algorithme seront proposées:
la première basée sur l&#8217;interface <code>Comparable</code>, la deuxième sur l&#8217;interface <code>Comparator</code> pour les comparaisons.</p>
</li>
<li>
<p>Ecrire un algorithme <code>copyIf</code> créant une copie d&#8217;une collection contenant uniquement les éléments vérifiant une condition passée en paramètre</p>
</li>
</ol>
</div>
</div>
<div class="sect3">
<h4 id="_exercice_de_synthèse"><a class="anchor" href="#_exercice_de_synthèse"></a><a class="link" href="#_exercice_de_synthèse">8.6.3. Exercice de synthèse</a></h4>
<div class="paragraph">
<p>Le but de cet exercice est de réaliser un logiciel de dessin 2D.
On se limitera ici à un affichage textuel, i.e. seule une description des figures sera affichée.</p>
</div>
<div class="paragraph">
<p>Le logiciel devra offrir les fonctionnalités suivantes:</p>
</div>
<div class="ulist">
<ul>
<li>
<p>manipulation (affichage et déplacement) des formes comme des rectangles et des cercles,</p>
</li>
<li>
<p>regroupement d&#8217;objets afin de leur faire subir un traitement global
(par exemple, déplacer ensemble un cercle et un rectangle),</p>
</li>
<li>
<p>sauvegarde/chargement d&#8217;un dessin à l&#8217;aide de la sérialisation.</p>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p>Les erreurs devront être gérées en utilisant les exceptions,</p>
</li>
<li>
<p>les ensembles de formes avec la librairie de collections.</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Proposer une hiérarchie de classe modélisant ce problème et un découpage en module du logiciel</p>
</li>
<li>
<p>Réaliser une implémentation du logiciel de dessin</p>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_la_bibliothèques_streams_et_la_programmation_fonctionnelle_en_java"><a class="anchor" href="#_la_bibliothèques_streams_et_la_programmation_fonctionnelle_en_java"></a><a class="link" href="#_la_bibliothèques_streams_et_la_programmation_fonctionnelle_en_java">9. La bibliothèques <em>streams</em> et la programmation fonctionnelle en Java</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_introduction_3"><a class="anchor" href="#_introduction_3"></a><a class="link" href="#_introduction_3">9.1. Introduction</a></h3>
<div class="sect3">
<h4 id="_programmation_impérative"><a class="anchor" href="#_programmation_impérative"></a><a class="link" href="#_programmation_impérative">9.1.1. Programmation impérative</a></h4>
<div class="ulist">
<ul>
<li>
<p>En <em>programmation impérative</em>, un programme est</p>
<div class="ulist">
<ul>
<li>
<p>une <strong>séquence d&#8217;instructions</strong></p>
</li>
<li>
<p>qui <strong>modifie l&#8217;état</strong> du programme</p>
</li>
</ul>
</div>
</li>
<li>
<p>Repose sur la séquence d&#8217;instructions, l'<strong>affectation</strong>, les structures de contrôle</p>
</li>
<li>
<p>Permet les <em>effets de bord</em></p>
<div class="ulist">
<ul>
<li>
<p>modifications de zones "partagées"</p>
</li>
</ul>
</div>
</li>
<li>
<p>Suit le <em>paradigme</em> utilisé au niveau du processeur (langage machine)</p>
</li>
<li>
<p>Basée sur la <em>machine de Turing</em> et l'<em>architecture de von Neumann</em></p>
</li>
<li>
<p>De nombreux langages supportent ce paradigme</p>
<div class="ulist">
<ul>
<li>
<p>C, Java, Python, &#8230;&#8203;</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_programmation_fonctionnelle"><a class="anchor" href="#_programmation_fonctionnelle"></a><a class="link" href="#_programmation_fonctionnelle">9.1.2. Programmation fonctionnelle</a></h4>
<div class="ulist">
<ul>
<li>
<p>En <em>programmation fonctionnelle</em>, un programme est</p>
<div class="ulist">
<ul>
<li>
<p>un ensemble de fonctions (au sens mathématique) emboîtées</p>
</li>
<li>
<p>sans effets de bord</p>
</li>
</ul>
</div>
</li>
<li>
<p>Repose sur une approche déclarative, l&#8217;évaluation de fonctions</p>
</li>
<li>
<p>Basée sur le \$lambda\$-calcul</p>
</li>
<li>
<p>De plus en plus de langages supportent ce paradigme</p>
<div class="ulist">
<ul>
<li>
<p>Haskell, F#, ML, Clojure, Lisp, &#8230;&#8203;</p>
</li>
<li>
<p>Java, Scala, Python, &#8230;&#8203;</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_fonctions"><a class="anchor" href="#_fonctions"></a><a class="link" href="#_fonctions">9.1.3. Fonctions</a></h4>
<div class="dlist">
<dl>
<dt class="hdlist1">Fonction <em>pure</em></dt>
<dd>
<p>fonction sans effet de bord</p>
</dd>
<dt class="hdlist1">Fonction d&#8217;ordre supérieur</dt>
<dd>
<p>une fonction peut être passée en paramètre ou retournée par une
fonctione</p>
</dd>
<dt class="hdlist1">Fonction de première classe</dt>
<dd>
<p>les fonctions sont traitées comme les autres données</p>
</dd>
<dt class="hdlist1">Fonction lambda</dt>
<dd>
<p>fonction anonyme créée "à la volée"</p>
</dd>
<dt class="hdlist1">Fermeture</dt>
<dd>
<p>fonction lambda avec son contexte</p>
</dd>
</dl>
</div>
</div>
<div class="sect3">
<h4 id="_transparence_référentielle"><a class="anchor" href="#_transparence_référentielle"></a><a class="link" href="#_transparence_référentielle">9.1.4. Transparence référentielle</a></h4>
<div class="ulist">
<ul>
<li>
<p>Remplacer une expression par sa valeur ne change pas le résultat</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">Le programme suivant ne respecte pas la transparence référentielle</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="C" class="language-C hljs">int globalValue = 2;
int inc(int k) {
  globalValue += k;
  return globalValue;
}
int result = inc(1) + inc(1)); // result = 3 + 4 = 7
globalValue = 2;
result = 2 * inc(1); // result = 2 * 3 = 6</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_avantages"><a class="anchor" href="#_avantages"></a><a class="link" href="#_avantages">9.1.5. Avantages</a></h4>
<div class="ulist">
<ul>
<li>
<p>Certains programmes s&#8217;expriment plus simplement</p>
</li>
<li>
<p>Permet un raisonnement sur le programme (preuve de programmes)</p>
</li>
<li>
<p>Facilite la programmation parallèle et concurrente</p>
<div class="ulist">
<ul>
<li>
<p>tire parti des processeurs multi-c&oelig;urs</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_programmation_fonctionnelle_en_java"><a class="anchor" href="#_programmation_fonctionnelle_en_java"></a><a class="link" href="#_programmation_fonctionnelle_en_java">9.2. Programmation fonctionnelle en Java</a></h3>
<div class="sect3">
<h4 id="_fonction_lambda"><a class="anchor" href="#_fonction_lambda"></a><a class="link" href="#_fonction_lambda">9.2.1. Fonction lambda</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>fonction lambda</em> est une fonction anonyme</p>
</li>
<li>
<p>En Java, la syntaxe est composée</p>
<div class="ulist">
<ul>
<li>
<p>d&#8217;une liste de paramètres formels entre parenthèses</p>
</li>
<li>
<p>d&#8217;une flèche &#8594;</p>
</li>
<li>
<p>d&#8217;une expression ou d&#8217;un bloc d&#8217;instructions</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">// En précisant le type et avec un bloc
(Person p1, Person p2) -&gt; {
    return p1.getAge() - p2.getAge()
}
// Avec une expression (sans return)
(Person p1, Person p2) -&gt; p1.getAge() - p2.getAge()
// Le type des paramètres est optionnel
(person1, person2) -&gt; person1.getAge() - person2.getAge()
// Avec un seul paramètres, les parenthèses sont optionnelles
person -&gt; person.getAge()</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_fonction_lambda_et_interface"><a class="anchor" href="#_fonction_lambda_et_interface"></a><a class="link" href="#_fonction_lambda_et_interface">9.2.2. Fonction lambda et interface</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une fonction lambda peut être utilisée quand une <em>interface fonctionnelle</em> est attendue</p>
</li>
<li>
<p>Une interface fonctionnelle (<em>functional interface</em>) ne doit comporter qu&#8217;une unique méthode abstraite</p>
</li>
<li>
<p>L&#8217;annotation <code>@FunctionalInterface</code> permet de marquer de telle interface</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">En utilisant l&#8217;interface et une classe anonyme</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">uneliste.sort(new Comparator&lt;Person&gt; {
    public int compare(Person p1, Person p2) {
        return p1.getAge() - p2.getAge();
    }
});</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">En utilisant une fonction lambda</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">uneliste.sort((person1, person2) -&gt; person1.getAge() - person2.getAge());</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_fermeture"><a class="anchor" href="#_fermeture"></a><a class="link" href="#_fermeture">9.2.3. Fermeture</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>fermeture</em> est une fonction lamda avec son contexte</p>
</li>
</ul>
</div>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public class ClosureDemo {
    public static Function&lt;Integer, Integer&gt; ajouteur(int n1) {
        return n2 -&gt; n1 + n2;
    }
    public static void main(String[] args) {
        Function&lt;Integer, Integer&gt; ajouteur10 = ajouteur(10);
        assert ajouteur10(1) == 11;
    }
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>En Java, une fermeture ne peut pas modifier les variables de son contexte</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_référence_de_méthode"><a class="anchor" href="#_référence_de_méthode"></a><a class="link" href="#_référence_de_méthode">9.2.4. Référence de méthode</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une <em>référence de méthode</em> permet d&#8217;utiliser une méthode comme fonction lambda</p>
</li>
<li>
<p>Quatre types de référence de méthode existent</p>
</li>
</ul>
</div>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 50%;">
<col style="width: 50%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Catégorie</th>
<th class="tableblock halign-left valign-top">Exemple</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Référence à une méthode de classe</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>ContainingClass::staticMethodName</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Référence à une méthode d&#8217;un objet précis</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>containingObject::instanceMethodName</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Référence à une méthode d&#8217;un objet quelconque</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>ContainingType::methodName</code></p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Référence à un constructeur</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>ClassName::new</code></p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_référence_de_méthode_exemples"><a class="anchor" href="#_référence_de_méthode_exemples"></a><a class="link" href="#_référence_de_méthode_exemples">9.2.5. Référence de méthode (exemples)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

numbers.forEach(e -&gt; System.out.println(e)); // lambda
numbers.forEach(System.out::println); // référence de méthode (objet précis)

numbers.stream()
       // .map(e -&gt; String.valueOf(e)) // lambda
       .map(String::valueOf) // référence de méthode (méthode de classe)
       .forEach(System.out::println);

numbers.stream()
       .map(String::valueOf(e))
       // .map(e -&gt; e.toString()) // lambda
       .map(String::toString) // référence de méthode (objet quelconque)
       .forEach(System.out::println);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_collection_de_litératif_au_fonctionnel_15"><a class="anchor" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_15"></a><a class="link" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_15">9.2.6. Parcourir une collection (de l&#8217;itératif au fonctionnel) 1/5</a></h4>
<div class="listingblock">
<div class="title">Itérateur externe avec une boucle classique</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

for(int i = 0; i &lt; numbers.size(); i++) {
    System.out.println(numbers.get(i));
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Beaucoup de "détails" sont visibles</p>
<div class="ulist">
<ul>
<li>
<p>indices limites</p>
</li>
<li>
<p>test d&#8217;arrêt</p>
</li>
<li>
<p>accès aux éléments</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_collection_de_litératif_au_fonctionnel_25"><a class="anchor" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_25"></a><a class="link" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_25">9.2.7. Parcourir une collection (de l&#8217;itératif au fonctionnel) 2/5</a></h4>
<div class="listingblock">
<div class="title">Itérateur externe avec une boucle foreach</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

for(int e : numbers) {
    System.out.println(e);
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Masque les détails mais demeure impératif</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_collection_de_litératif_au_fonctionnel_35"><a class="anchor" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_35"></a><a class="link" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_35">9.2.8. Parcourir une collection (de l&#8217;itératif au fonctionnel) 3/5</a></h4>
<div class="listingblock">
<div class="title">Itérateur interne</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

numbers.forEach(new Consumer&lt;Integer&gt;() {
    public void accept(Integer value) {
        System.out.println(value);
    }
});</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Syntaxe plus déclarative</p>
</li>
<li>
<p>L&#8217;argument de <code>forEach</code> est ici une <a href="https://docs.oracle.com/javase/tutorial/java/javaOO/anonymousclasses.htmlhttps://docs.oracle.com/javase/tutorial/java/javaOO/anonymousclasses.html"><em>classe anonyme</em></a></p>
</li>
<li>
<p><a href="https://docs.oracle.com/javase/8/docs/api/java/util/function/Consumer.html"><code>java.util.function.Consumer&lt;T&gt;</code></a> est une interface fonctionnelle</p>
</li>
<li>
<p><code>Consumer</code> opère par effet de bord</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_collection_de_litératif_au_fonctionnel_45"><a class="anchor" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_45"></a><a class="link" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_45">9.2.9. Parcourir une collection (de l&#8217;itératif au fonctionnel) 4/5</a></h4>
<div class="listingblock">
<div class="title">Itérateur interne avec lambda</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

numbers.forEach(value -&gt; System.out.println(value));</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Beaucoup plus concis et lisible</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_parcourir_une_collection_de_litératif_au_fonctionnel_55"><a class="anchor" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_55"></a><a class="link" href="#_parcourir_une_collection_de_litératif_au_fonctionnel_55">9.2.10. Parcourir une collection (de l&#8217;itératif au fonctionnel) 5/5</a></h4>
<div class="listingblock">
<div class="title">Itérateur interne avec référence de méthode</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

numbers.forEach(System.out::println);</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le plus lisible</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_la_bibliothèque_streams"><a class="anchor" href="#_la_bibliothèque_streams"></a><a class="link" href="#_la_bibliothèque_streams">9.3. La bibliothèque streams</a></h3>
<div class="sect3">
<h4 id="_streams"><a class="anchor" href="#_streams"></a><a class="link" href="#_streams">9.3.1. Streams</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>flux</em> (<em>stream</em>) est une séquence d&#8217;éléments</p>
</li>
<li>
<p>Il véhicule des éléments à partir d&#8217;une source à travers un <em>pipeline</em></p>
</li>
<li>
<p>Un flux ne stocke aucune donnée</p>
<div class="ulist">
<ul>
<li>
<p>ce n&#8217;est pas une structure de données</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_pipeline"><a class="anchor" href="#_pipeline"></a><a class="link" href="#_pipeline">9.3.2. Pipeline</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un pipeline est une séquence d&#8217;opérations applicables sur un flux</p>
</li>
<li>
<p>Il comporte</p>
<div class="ulist">
<ul>
<li>
<p>une source (collection, tableau, fonction génératrice, flux I/O)</p>
</li>
<li>
<p>une séquence d&#8217;opérations intermédiaires (chacune produit un nouveau stream)</p>
</li>
<li>
<p>une opération terminal qui calcule un résultat</p>
</li>
</ul>
</div>
</li>
<li>
<p>Une opération ne modifie pas le flux d&#8217;origine</p>
</li>
<li>
<p>L&#8217;évaluation est <em>paresseuse</em></p>
</li>
<li>
<p>Peut être exécuté séquentiellement ou en parallèle</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_opération_terminale"><a class="anchor" href="#_opération_terminale"></a><a class="link" href="#_opération_terminale">9.3.3. Opération terminale</a></h4>
<div class="ulist">
<ul>
<li>
<p>Une opération terminal traverse le flux pour produire un résultat ou un effet de bord</p>
</li>
<li>
<p>Après exécution, le flux est considéré comme consommé et ne peut pas être réutilisé</p>
</li>
<li>
<p>Une opération terminale est également nommée <em>réduction</em></p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_un_exemple_de_stream"><a class="anchor" href="#_un_exemple_de_stream"></a><a class="link" href="#_un_exemple_de_stream">9.3.4. Un exemple de stream</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

// Calcul le total des doubles des nombres pairs
System.out.println(
    numbers.stream()
           .filter(e -&gt; e % 2 == 0)
           .mapToInt(e -&gt; e * 2)
           .sum());</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_linterface_stream"><a class="anchor" href="#_linterface_stream"></a><a class="link" href="#_linterface_stream">9.3.5. L&#8217;interface <code>Stream</code></a></h4>
<div class="ulist">
<ul>
<li>
<p>L&#8217;interface <a href="https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html"><code>java.util.stream.Stream</code></a> regroupe l&#8217;ensemble des opérations applicables aux pipelines</p>
</li>
<li>
<p>Les interfaces <code>IntStream</code>, <code>LongStream</code> et <code>DoubleStream</code> sont spécialisés pour les types primitifs</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_création_dun_flux"><a class="anchor" href="#_création_dun_flux"></a><a class="link" href="#_création_dun_flux">9.3.6. Création d&#8217;un flux</a></h4>
<div class="ulist">
<ul>
<li>
<p>À partir d&#8217;une collection</p>
<div class="ulist">
<ul>
<li>
<p><code>Collection.stream</code>, <code>Collection.parallelStream</code> (flux parallèle)</p>
</li>
</ul>
</div>
</li>
<li>
<p>À partir d&#8217;un tableau (<code>Arrays.stream</code>)</p>
</li>
<li>
<p>À partir d&#8217;un intervalle</p>
<div class="ulist">
<ul>
<li>
<p><code>IntStream.range</code>, <code>IntStream.rangeClosed</code> (aussi avec <code>LongStream</code>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>À partir de valeurs</p>
<div class="ulist">
<ul>
<li>
<p><code>Stream.of</code> (aussi dans <code>IntStream</code>, <code>LongStream</code> et <code>DoubleStream</code>)</p>
</li>
</ul>
</div>
</li>
<li>
<p>À partir des méthodes de classe de <code>Stream</code></p>
<div class="ulist">
<ul>
<li>
<p><code>concat</code>, <code>empty</code>, <code>generate</code>/<code>iterate</code> (flux infini)</p>
</li>
</ul>
</div>
</li>
<li>
<p>À partir de nombres aléatoires (<code>doubles</code>, <code>ints</code> et <code>longs</code> de la classe <code>Random</code>)</p>
</li>
<li>
<p>À partir d&#8217;un fichier (<code>Files.lines</code>, <code>BufferedReader.lines</code>)</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_opérations_intermédiaires"><a class="anchor" href="#_quelques_opérations_intermédiaires"></a><a class="link" href="#_quelques_opérations_intermédiaires">9.3.7. Quelques opérations intermédiaires</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 50%;">
<col style="width: 50%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Opération</th>
<th class="tableblock halign-left valign-top">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>filter</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">retourne les éléments respectant un prédicat</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>map</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">applique une fonction à chaque élément</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>flatMap</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">désimbrique des flux</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>limit</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">tronque un flux</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>skip</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">ignore les premiers éléments</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>distinct</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">élimine les doublons (avec état)</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>sorted</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">retourne un flux trié (avec état)</p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_opérations_intermédiaires_exemples"><a class="anchor" href="#_opérations_intermédiaires_exemples"></a><a class="link" href="#_opérations_intermédiaires_exemples">9.3.8. Opérations intermédiaires (exemples)</a></h4>
<div class="listingblock">
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

numbers.stream()
       .filter(e -&gt; e % 2 == 0)
       .forEach(System.out::println)); // 2 4 6 8 10

numbers.stream()
       .filter(e -&gt; e % 2 == 0)
       .map(e -&gt; e * 2)
       .forEach(System.out::println)); // 4 8 12 16 20</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_quelques_opérations_terminales"><a class="anchor" href="#_quelques_opérations_terminales"></a><a class="link" href="#_quelques_opérations_terminales">9.3.9. Quelques opérations terminales</a></h4>
<table class="tableblock frame-all grid-all stretch">
<colgroup>
<col style="width: 50%;">
<col style="width: 50%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Opération</th>
<th class="tableblock halign-left valign-top">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>reduce</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">applique une réduction avec une fonction d&#8217;accumulation</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>count</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">compte les éléments</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>sum</code>, &#8230;&#8203;</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">réduction spécialisée sur les flux de types primitifs</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>collect</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">réalise une réduction par modification</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>allMatch</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">teste si tous les éléments respectent un prédicat</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock"><code>forEach</code></p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">exécute une action pour chaque élément</p></td>
</tr>
</tbody>
</table>
</div>
<div class="sect3">
<h4 id="_opérations_terminales_exemple_13"><a class="anchor" href="#_opérations_terminales_exemple_13"></a><a class="link" href="#_opérations_terminales_exemple_13">9.3.10. Opérations terminales (exemple) 1/3</a></h4>
<div class="listingblock">
<div class="title">Calculer une somme avec <code>reduce</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

System.out.println(
    numbers.stream()
           .filter(e -&gt; e % 2 == 0)
           .map(e -&gt; e * 2.0)
           .reduce(0.0, (carry, e) -&gt; carry + e));</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Calculer une somme avec <code>sum</code> et <code>DoubleStream</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">System.out.println(
    numbers.stream()
           .filter(e -&gt; e % 2 == 0)
           .mapToDouble(e -&gt; e * 2.0)
           .sum());</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_opérations_terminales_exemple_23"><a class="anchor" href="#_opérations_terminales_exemple_23"></a><a class="link" href="#_opérations_terminales_exemple_23">9.3.11. Opérations terminales (exemple) 2/3</a></h4>
<div class="listingblock">
<div class="title">Les doubles des nombres pairs dans une liste avec <code>collect</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Integer&gt; numbers = Arrays.asList(1, 2, 3, 4, 5, 1, 2, 3, 4, 5);

List&lt;Integer&gt; doubleOfEven =
    numbers.stream()
           .filter(e -&gt; e % 2 == 0)
           .map(e -&gt; e * 2)
           .collect(Collectors.toList());
System.out.println(doubleOfEven);</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Les doubles des nombres pairs dans un dictionnaire avec <code>collect</code></div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Map&lt;Integer, Integer&gt; doubleOfEven =
    numbers.stream()
           .filter(e -&gt; e % 2 == 0)
           .collect(Collectors.toMap(
               Function.identity(),
               i -&gt; i * 2));
System.out.println(doubleOfEven);</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_opérations_terminales_exemple_33"><a class="anchor" href="#_opérations_terminales_exemple_33"></a><a class="link" href="#_opérations_terminales_exemple_33">9.3.12. Opérations terminales (exemple) 3/3</a></h4>
<div class="listingblock">
<div class="title">Un dictionnaire des personnes regroupées par nom</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">List&lt;Person&gt; persons = //...

Map&lt;Person, List&lt;Person&gt;&gt; personsByName =
    persons.stream()
           .collect(Collectors.groupingBy(Person::getName));
System.out.println(personsByName);</code></pre>
</div>
</div>
<div class="listingblock">
<div class="title">Un dictionnaire des noms de personnes regroupés par sexe</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Map&lt;Person.Gender, List&lt;String&gt;&gt; namesByGender =
    persons.stream()
           .collect(Collectors.groupingBy(
               Person::getGender,
               Collectors.mapping(
                   Person::getName,
                   Collectors.toList())));</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_flux_infinis"><a class="anchor" href="#_flux_infinis"></a><a class="link" href="#_flux_infinis">9.3.13. Flux infinis</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les méthodes de classe <code>Stream.generate</code> et <code>Stream.iterate</code> créent un flux infini</p>
</li>
<li>
<p>Ce type de flux peut exister grâce à l'<em>évaluation paresseuse</em></p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;application d&#8217;opérations élémentaires ne provoque pas la traversée du pipeline</p>
</li>
<li>
<p>seules les opérations terminales déclenchent le traitement</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
<div class="listingblock">
<div class="title">Un dictionnaire des noms de personnes regroupés par sexe</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Stream&lt;Integer&gt; integers = Stream.iterate(0, i -&gt; i + 1);
integers.limit(10)
        .forEach(System.out::println);</code></pre>
</div>
</div>
<div class="admonitionblock warning">
<table>
<tr>
<td class="icon">
<i class="fa icon-warning" title="Warning"></i>
</td>
<td class="content">
Il ne faut jamais réduire l&#8217;intégralité d&#8217;un flux infini.
</td>
</tr>
</table>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_exercices_4"><a class="anchor" href="#_exercices_4"></a><a class="link" href="#_exercices_4">9.4. Exercices</a></h3>
<div class="sect3">
<h4 id="_requêtes_en_utilisant_les_streams"><a class="anchor" href="#_requêtes_en_utilisant_les_streams"></a><a class="link" href="#_requêtes_en_utilisant_les_streams">9.4.1. Requêtes en utilisant les <code>streams</code></a></h4>
<div class="paragraph">
<p>Le but de cette exercice est d&#8217;exprimer un ensemble de requêtes en utilisant la bibliothèque stream.</p>
</div>
<div class="paragraph">
<p>Un employé possède les attributs suivants :
nom (<code>String</code>), age (<code>int</code>), sexe (<code>enum</code>), salaire (<code>BigDecimal</code>),
date d&#8217;embauche (<code>LocalDate</code>) et service de rattachement (<code>Service</code>).
Un service comporte un nom (<code>String</code>) et une adresse (<code>String</code>).</p>
</div>
<div class="olist arabic">
<ol class="arabic">
<li>
<p>Implémentez la classe <code>Employe</code> et l&#8217;énumération <code>Service</code></p>
</li>
<li>
<p>Créez un jeu de données de test</p>
</li>
<li>
<p>Implémentez les requêtes suivantes (faites afficher le résultat)</p>
<div class="olist loweralpha">
<ol class="loweralpha" type="a">
<li>
<p>les employés (avec toutes leurs caractéristiques)</p>
</li>
<li>
<p>les employés de moins de 30 ans</p>
</li>
<li>
<p>le nom des hommes</p>
</li>
<li>
<p>le nom et le salaire trié par salaire décroissant</p>
</li>
<li>
<p>la moyenne des salaires</p>
</li>
<li>
<p>les employés regroupés selon leur sexe</p>
</li>
<li>
<p>la moyenne des salaires par sexe</p>
</li>
<li>
<p>le nom et la date d&#8217;embauche par services</p>
</li>
</ol>
</div>
</li>
</ol>
</div>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_conclusion"><a class="anchor" href="#_conclusion"></a><a class="link" href="#_conclusion">10. Conclusion</a></h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_bilan"><a class="anchor" href="#_bilan"></a><a class="link" href="#_bilan">10.1. Bilan</a></h3>
<div class="sect3">
<h4 id="_principaux_concepts_abordés"><a class="anchor" href="#_principaux_concepts_abordés"></a><a class="link" href="#_principaux_concepts_abordés">10.1.1. Principaux concepts abordés</a></h4>
<div class="ulist">
<ul>
<li>
<p>Objet et messages</p>
</li>
<li>
<p>Type et classe, métaclasse, généricité</p>
</li>
<li>
<p>Sous-type, héritage, polymorphisme, classe abstraite, héritage multiple et à répétition</p>
</li>
<li>
<p>Relations entre classes (dépendance, association/agrégation/composition, héritage)</p>
</li>
<li>
<p>Modules</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_autres_notions_abordées"><a class="anchor" href="#_autres_notions_abordées"></a><a class="link" href="#_autres_notions_abordées">10.1.2. Autres notions abordées</a></h4>
<div class="ulist">
<ul>
<li>
<p>Gestion d&#8217;erreurs et exceptions</p>
</li>
<li>
<p>Entrées/sorties et persistance</p>
</li>
<li>
<p>Gestion des collections</p>
</li>
<li>
<p>Bibliothèques <code>stream</code> et notion de programmation fonctionnelle</p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_conception_orientée_objet"><a class="anchor" href="#_conception_orientée_objet"></a><a class="link" href="#_conception_orientée_objet">10.2. Conception orientée-objet</a></h3>
<div class="sect3">
<h4 id="_quest_ce_que_la_conception_orientée_objet"><a class="anchor" href="#_quest_ce_que_la_conception_orientée_objet"></a><a class="link" href="#_quest_ce_que_la_conception_orientée_objet">10.2.1. Qu&#8217;est-ce que la conception orientée-objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>Lors de son exécution, un <em>système OO</em> est <strong>un ensemble d&#8217;objets qui interagissent</strong></p>
</li>
<li>
<p>La <em>conception orientée-objet</em> (COO) consiste donc à créer un <em>modèle</em> qui respecte les concepts objet</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_difficultés_de_la_conception_orientée_objet"><a class="anchor" href="#_difficultés_de_la_conception_orientée_objet"></a><a class="link" href="#_difficultés_de_la_conception_orientée_objet">10.2.2. Difficultés de la conception orientée-objet</a></h4>
<div class="ulist">
<ul>
<li>
<p>Les concepts objets sont nombreux et complexes (attribut, méthode, objet, classe, héritage, &#8230;&#8203;)</p>
<div class="ulist">
<ul>
<li>
<p>&#8658; plusieurs solutions sont en général envisageables</p>
</li>
</ul>
</div>
</li>
<li>
<p>Identifier la bonne solution est difficile</p>
</li>
<li>
<p>Plusieurs symptômes voire métriques de qualité peuvent guider les choix</p>
</li>
</ul>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
<div class="ulist">
<ul>
<li>
<p><strong>Programmer en Java ou en C# n&#8217;est pas concevoir objet !</strong></p>
</li>
<li>
<p>Seule une analyse objet conduit à une solution objet, i.e. qui respecte les concepts objet</p>
</li>
<li>
<p>Le langage de programmation est un moyen d&#8217;implémentation qui ne garantit pas le respect des concepts objet</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_principes_patterns_et_idiomes"><a class="anchor" href="#_principes_patterns_et_idiomes"></a><a class="link" href="#_principes_patterns_et_idiomes">10.2.3. Principes, patterns et idiomes</a></h4>
<div class="ulist">
<ul>
<li>
<p>Un <em>principe</em> donne des directives générales</p>
<div class="ulist">
<ul>
<li>
<p>souvent indépendant des paradigmes et des langages</p>
</li>
<li>
<p>par exemple <em>KISS</em>, <em>YAGNI</em>, <em>DRY</em>, <em>Law of Demeter</em>/<em>Tell, don&#8217;t ask</em>, &#8230;&#8203;</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un <em>pattern</em> propose une solution reconnue à un problème récurrent</p>
<div class="ulist">
<ul>
<li>
<p>en général indépendant des langages</p>
</li>
<li>
<p>par exemple le design pattern <em>Composite</em></p>
</li>
</ul>
</div>
</li>
<li>
<p>Un <em>idiome</em> est une construction spécifique d&#8217;un langage pour implémenter une situation courante</p>
<div class="ulist">
<ul>
<li>
<p><code>uneListe.forEach(System.out::println);</code> (afficher une liste en Java 8)</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_kiss_keep_it_simple_stupid"><a class="anchor" href="#_kiss_keep_it_simple_stupid"></a><a class="link" href="#_kiss_keep_it_simple_stupid">10.2.4. KISS (Keep It Simple, Stupid)</a></h4>
<div class="ulist">
<ul>
<li>
<p>"<em>Simplicity should be a key goal in design and unnecessary complexity should be avoided</em>", Kelly Johnson, ingénieur chez Lockheed</p>
</li>
<li>
<p>Le code le plus simple est aussi le plus simple à maintenir</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_yagni_you_arent_gonna_need_it"><a class="anchor" href="#_yagni_you_arent_gonna_need_it"></a><a class="link" href="#_yagni_you_arent_gonna_need_it">10.2.5. YAGNI (You Aren’t Gonna Need It)</a></h4>
<div class="ulist">
<ul>
<li>
<p>"<em>Do the Simplest Thing That Could Possibly Work</em>"</p>
</li>
<li>
<p>Ne pas ajouter une fonctionnalité avant que cela soit nécessaire</p>
</li>
<li>
<p>Principe issu d&#8217;eXtreme Programming</p>
</li>
<li>
<p>Nécessite de s&#8217;appuyer sur du <em>refactoring</em> pour être efficace</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_dry_dont_repeat_yourself"><a class="anchor" href="#_dry_dont_repeat_yourself"></a><a class="link" href="#_dry_dont_repeat_yourself">10.2.6. DRY (Don’t Repeat Yourself)</a></h4>
<div class="ulist">
<ul>
<li>
<p>"<em>Every piece of knowledge must have a single, unambiguous, authoritative representation within a system</em>", <em>The Pragmatic Programmer</em>, Andrew Hunt and David Thomas</p>
</li>
<li>
<p>Chaque fonctionnalité doit être réalisée à un seul endroit du code</p>
</li>
<li>
<p>Une modification d&#8217;un élément ne nécessite pas de changer un autre élément non relié logiquement</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_law_of_demeter"><a class="anchor" href="#_law_of_demeter"></a><a class="link" href="#_law_of_demeter">10.2.7. Law of Demeter</a></h4>
<div class="admonitionblock note">
<table>
<tr>
<td class="icon">
<i class="fa icon-note" title="Note"></i>
</td>
<td class="content">
<div class="title">Law of Demeter or principle of least knowledge</div>
<div class="ulist">
<ul>
<li>
<p>Each unit should have only limited knowledge about other units: only units "closely" related to the current unit.</p>
</li>
<li>
<p>Each unit should only talk to its friends; don&#8217;t talk to strangers.</p>
</li>
<li>
<p>Only talk to your immediate friends.</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p>Une méthode d&#8217;un objet devrait invoquer uniquement les méthodes de</p>
<div class="ulist">
<ul>
<li>
<p>l&#8217;objet lui-même,</p>
</li>
<li>
<p>ses paramètres,</p>
</li>
<li>
<p>tout objet qu&#8217;elle instancie,</p>
</li>
<li>
<p>ses composants directs.</p>
</li>
</ul>
</div>
</li>
<li>
<p>Un objet connaît le minimum de la structure de ses voisins</p>
</li>
<li>
<p>Cela limite les dépendances avec les autres objets</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_la_loi_de_demeter_15"><a class="anchor" href="#_exemple_de_la_loi_de_demeter_15"></a><a class="link" href="#_exemple_de_la_loi_de_demeter_15">10.2.8. Exemple de la Loi de Demeter 1/5</a></h4>
<div class="listingblock">
<div class="title">Un client paye (<strong>version incorrecte</strong>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">Wallet theWallet = theCustomer.getWallet();
double totalMoney = theWallet.getTotalMoney();
if (totalMoney &gt; AMOUNT_TO_PAY_IN_EUROS) {
    theWallet.subtractMoney(AMOUNT_TO_PAY_IN_EUROS);
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Cet exemple est extrait de <a href="http://www.ccs.neu.edu/research/demeter/demeter-method/LawOfDemeter/paper-boy/demeter.pdf">The Paperboy, The Wallet, and The Law Of Demeter</a>, David Bock</p>
</li>
<li>
<p>Le créancier connaît la structure du client et manipule lui-même le portefeuille</p>
</li>
<li>
<p>Il dispose de plus d&#8217;informations que nécessaire</p>
</li>
<li>
<p>La validité du portefeuille n&#8217;est pas garantie</p>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_la_loi_de_demeter_25"><a class="anchor" href="#_exemple_de_la_loi_de_demeter_25"></a><a class="link" href="#_exemple_de_la_loi_de_demeter_25">10.2.9. Exemple de la Loi de Demeter 2/5</a></h4>
<div class="listingblock">
<div class="title">La classe <code>Customer</code> (<strong>version incorrecte</strong>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public class Customer {
  private String name;
  private Wallet wallet;

  public Customer(String name, double fortune) {
    this.name = name;
    wallet = new Wallet(fortune);
  }

  public Wallet getWallet() {
    return wallet;
  }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_la_loi_de_demeter_35"><a class="anchor" href="#_exemple_de_la_loi_de_demeter_35"></a><a class="link" href="#_exemple_de_la_loi_de_demeter_35">10.2.10. Exemple de la Loi de Demeter 3/5</a></h4>
<div class="listingblock">
<div class="title">La classe <code>Wallet</code> (<strong>version incorrecte</strong>)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public class Wallet {
  private double totalMoney;

  public Wallet(double fortune) {
    totalMoney = fortune;
  }

  public double getTotalMoney() {
    return totalMoney;
  }

  public void subtractMoney(double amountToPayInEuros) {
    totalMoney -= amountToPayInEuros;
  }
}</code></pre>
</div>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_la_loi_de_demeter_45"><a class="anchor" href="#_exemple_de_la_loi_de_demeter_45"></a><a class="link" href="#_exemple_de_la_loi_de_demeter_45">10.2.11. Exemple de la Loi de Demeter 4/5</a></h4>
<div class="listingblock">
<div class="title">Un client paye (version corrigée)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">double paidAmount = theCustomer.getPayment(AMOUNT_TO_PAY_IN_EUROS);</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>Le créancier doit demander le paiement</p>
</li>
<li>
<p>La classe <code>Wallet</code> est isolée (diminue le couplage)</p>
</li>
<li>
<p>La méthode <code>getPayment</code> encapsule la logique du paiement (améliore la cohésion)</p>
</li>
<li>
<p>La classe <code>Customer</code> est plus complexe</p>
<div class="ulist">
<ul>
<li>
<p>mais la complexité a été transférée depuis le code de l&#8217;application</p>
</li>
</ul>
</div>
</li>
</ul>
</div>
</div>
<div class="sect3">
<h4 id="_exemple_de_la_loi_de_demeter_55"><a class="anchor" href="#_exemple_de_la_loi_de_demeter_55"></a><a class="link" href="#_exemple_de_la_loi_de_demeter_55">10.2.12. Exemple de la Loi de Demeter 5/5</a></h4>
<div class="listingblock">
<div class="title">La classe <code>Customer</code> (version corrigée)</div>
<div class="content">
<pre class="highlightjs highlight"><code data-lang="java" class="language-java hljs">public class Customer {
  private String name;
  private Wallet wallet;

  public Customer(String name, double fortune) {
    this.name = name;
    wallet = new Wallet(fortune);
  }

  public double getPayment(double amountToPayInEuros) {
    double totalMoney = wallet.getTotalMoney();
    double paidAmount = 0.0;
    if (totalMoney &gt; amountToPayInEuros) {
      paidAmount = amountToPayInEuros;
      wallet.subtractMoney(paidAmount);
    }
   return paidAmount;
  }
}</code></pre>
</div>
</div>
<div class="ulist">
<ul>
<li>
<p>La classe <code>Customer</code> ne publie plus la méthode <code>getWallet()</code></p>
</li>
</ul>
</div>
</div>
</div>
<div class="sect2">
<h3 id="_pour_aller_plus_loin"><a class="anchor" href="#_pour_aller_plus_loin"></a><a class="link" href="#_pour_aller_plus_loin">10.3. Pour aller plus loin&#8230;&#8203;</a></h3>
<div class="sect3">
<h4 id="_lisez"><a class="anchor" href="#_lisez"></a><a class="link" href="#_lisez">10.3.1. Lisez !</a></h4>
<div class="ulist">
<ul>
<li>
<p>Des livres (cf. la bibliographie en début de cours)</p>
</li>
<li>
<p>Des blogs (<a href="https://dzone.com/">DZone</a>, <a href="https://www.infoq.com/">InfoQ</a>, <a href="https://blog.jetbrains.com/idea/tag/java-annotated/">Java Annotated Monthly</a>), wiki (<a href="http://wiki.c2.com/">C2 wiki</a>), flux, &#8230;&#8203;</p>
</li>
<li>
<p>Des questions/réponses (<a href="https://stackoverflow.com/">Stack Overflow</a>)</p>
</li>
<li>
<p><strong>Du code</strong> (<a href="http://wiki.c2.com/?TipsForReadingCode">Tips For Reading Code</a>, <a href="https://github.com/explore">github</a>, <a href="http://wiki.c2.com/?ProgramsToRead">Programs To Read</a>)</p>
</li>
</ul>
</div>
<div class="admonitionblock caution">
<table>
<tr>
<td class="icon">
<i class="fa icon-caution" title="Caution"></i>
</td>
<td class="content">
pour les langages, attention aux versions (Java &gt;= 8)
</td>
</tr>
</table>
</div>
<div class="admonitionblock important">
<table>
<tr>
<td class="icon">
<i class="fa icon-important" title="Important"></i>
</td>
<td class="content">
Ayez l&#8217;esprit critique (toutes les pages ne se valent pas)
</td>
</tr>
</table>
</div>
</div>
<div class="sect3">
<h4 id="_pratiquez"><a class="anchor" href="#_pratiquez"></a><a class="link" href="#_pratiquez">10.3.2. Pratiquez !</a></h4>
<div class="ulist">
<ul>
<li>
<p><a href="http://codekata.com/">Kata</a>, Koans, <a href="https://fr.wikipedia.org/wiki/Coding_dojo">Coding Dojo</a></p>
</li>
</ul>
</div>
<div class="admonitionblock tip">
<table>
<tr>
<td class="icon">
<i class="fa icon-tip" title="Tip"></i>
</td>
<td class="content">
<div class="title">Ajoutez des contraintes</div>
<div class="ulist">
<ul>
<li>
<p>les types primitifs doivent systématiquement être encapsulés</p>
</li>
<li>
<p>pas de méthodes de plus de 4 lignes</p>
</li>
<li>
<p>un seul niveau d&#8217;indentation par méthode</p>
</li>
<li>
<p>pas plus de 2 paramètres par méthode</p>
</li>
<li>
<p>pas d&#8217;utilisation de la souris</p>
</li>
<li>
<p>&#8230;&#8203;</p>
</li>
</ul>
</div>
</td>
</tr>
</table>
</div>
<div class="ulist">
<ul>
<li>
<p><a href="https://www.codewars.com/">Codewars</a>, <a href="https://www.codingame.com/start">CodinGame</a></p>
</li>
<li>
<p>Participez à un projet Open Source</p>
</li>
</ul>
</div>
</div>
</div>
</div>
</div>
</div>
<div id="footer">
<div id="footer-text">
Version 2022-2023<br>
Last updated 2023-07-02 17:30:21
</div>
</div>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/styles/github.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.6/highlight.min.js"></script>
<script>hljs.initHighlighting()</script>
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  messageStyle: "none",
  tex2jax: {
    inlineMath: [["\\(", "\\)"]],
    displayMath: [["\\[", "\\]"]],
    ignoreClass: "nostem|nolatexmath"
  },
  asciimath2jax: {
    delimiters: [["\\$", "\\$"]],
    ignoreClass: "nostem|noasciimath"
  },
  TeX: { equationNumbers: { autoNumber: "none" } }
})
MathJax.Hub.Register.StartupHook("AsciiMath Jax Ready", function () {
  MathJax.InputJax.AsciiMath.postfilterHooks.Add(function (data, node) {
    if ((node = data.script.parentNode) && (node = node.parentNode) && node.classList.contains('stemblock')) {
      data.math.root.display = "block"
    }
    return data
  })
})
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_HTMLorMML"></script>
</body>
</html>
