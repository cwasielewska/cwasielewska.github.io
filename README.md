/* 	Begin Modified Meyer Reset */
html, body, div, span, applet, object, iframe, h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code, del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var, b, u, i, center, dl, dt, dd, ol, ul, li,
fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary, time, mark, audio, video {
	margin:0; padding:0; border:0; font-size:100%; font:inherit; vertical-align:baseline;
}
/* HTML5 reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display:block;
}
body { line-height:1; letter-spacing:-0.25px; overscroll-behavior:contain;}
#container:not([style*="zoom"]) { -webkit-text-size-adjust:none;}
table { border-collapse:collapse; border-spacing:0; }
th { font-weight:normal; text-align:left; }
ul { list-style-type:none; }
.page ol { list-style-position:outside; margin-left:1em; }
/*.page ol > li, .page  ul > li { text-indent:-1em; padding-left:1em; }*/
.page .singleline li, .page .singleline li { text-indent:inherit; padding:0; }
.page ol > li > *, .page ul > li > * { text-indent:initial; padding-left:initial; }
button { background:transparent;border:none; }
/*General styles*/
html, body, #container-wrap, #container { height:100%; }
#container-wrap { position:absolute; top:0; left:0; }
#container-wrap, #container { min-height:100%; width:100%; background-color:transparent; z-index:0;}
b { font-weight:bold; }
i { font-style:italic; }
a { color:inherit; text-decoration:inherit; }
input,select,textarea { font-size:inherit; }
p:first-child { margin-top:inherit !important; }
*{ outline:none; animation-fill-mode:both !important; -webkit-animation-fill-mode:both !important; }
[data-onclick],[onclick],[onrollover],[data-fixed-action],[aria-details],button,.flipwrap{ cursor:pointer; pointer-events:auto; }

body[class^='scaled-none'],body[class*=' scaled-none']{ overflow:auto; }
body[class^='scaled-width'],body[class*=' scaled-width']{ overflow-x:hidden; }
body[class^='scaled-height'],body[class*=' scaled-height']{ overflow-y:hidden; }
body[class^='scaled-best'],body[class*=' scaled-best']{ overflow:hidden; }
body[class^='scaled-best'][data-page-mode^='c'],body[class*=' scaled-best'][data-page-mode^='c']{ overflow:auto; }
body[class^='scaled-width'][data-page-mode^='csh'],body[class*=' scaled-width'][data-page-mode^='csh']{ overflow-x:auto; }
body[class^='scaled-height'][data-page-mode^='csv'],body[class*=' scaled-height'][data-page-mode^='csv']{ overflow-y:auto; }
body[data-scaled-to='w'] #container{ height:auto; min-height:auto; }
body[data-scaled-to='w'][data-page-mode^='cs'] #container{ position:absolute; }
body[data-scaled-to='w'][data-page-mode^='csv'] .pages { padding:0;}
body.zoomed:not([class*='scaled-']) #container { position:absolute; }
body[class*='scaled-'] .pages.paper-vertical{ margin:0; }
body[class^='zoomed'],body[class*=' zoomed']{ overflow-x:auto;overflow-y:auto; }
body[data-scaled-to] .anythingSlider-in5, body[data-scaled-to] #container > .page {padding:0;margin:0;}
body[data-scaled-to] #in5footer { position:fixed; bottom:0;}
/*body[data-scaled-to] * { -webkit-backface-visibility: hidden; }*/ /*fix blurry imgs*/
html.ios body[class*='scaled-'] #container { position:absolute; top:0; left:0; }
body.tall-page {overflow-y:auto;}
.liquid .page.tall-page {height:auto;}

.paper-vertical:after {
    position:relative;
    content:' ';
    display:block;
    height:50px;
    clear:both;
}
body[data-scaled-to="h"] .paper-vertical:after { display:none; }
body[data-scaled-to='h'] .paper-horizontal { margin:0; }
body[data-scaled-to='h'] .paper-horizontal .page { margin-top:0; }

#loadIndicator{
	width:100%; padding:6px; position:fixed;
	top:0; left:0; margin:auto;
    transition:all 1s ease-in .5s;
    opacity:1; z-index:99;
}
body.loaded #loadIndicator {
	opacity:0;
	transform:translateY(-36px);
	-webkit-transform:translateY(-36px);
	display:none\9;/*old IE*/
}
#loadIndicator img {
	vertical-align:text-bottom; width:18px;
}
html.local #loadIndicator, html.dps #loadIndicator, html.baker #loadIndicator { display:none; }

#in5footer{
	height:26px; line-height:26px; clear:both; position:relative; margin-top:-26px;
}

#demoNote {
    right:0; bottom:0; margin:auto;
    height:96px !important;
    padding:36px 10px;
}

#in5footer a, #demoNote a {
	text-decoration:none; color:#99ccff;
}
svg-img{display:block;position:absolute;}
.win-safari svg-img{width:100%;}
svg-img{width:100%\9;}
.spread-shift { position:absolute; }
.pageItem, svg { position:absolute; top:0; left:0; }
svg { overflow:visible; }
.pageItem {
	display:block;
	width:auto !important; height:auto !important;
	box-sizing:border-box; 
	-moz-box-sizing:border-box;
	-webkit-tap-highlight-color:transparent;
	padding:0;
}
.pageItem.hd/*, .pageItem img.hd*/  {
	-ms-transform:scale(.5);
    -ms-transform-origin:0 0 0;
    -webkit-transform:scale(.5);
    -webkit-transform-origin:0 0 0;
    transform:scale(.5);
    transform-origin:0 0 0;
}
@media screen and (-webkit-min-device-pixel-ratio:0) and (min-resolution:.001dpcm) {
    .pageItem { image-rendering: -webkit-optimize-contrast; }
}
@media not all and (min-resolution:.001dpcm)
{ @supports (-webkit-appearance:none) and (stroke-color:transparent) {
    .pageItem { image-rendering: optimizeSpeed; }
}}
@-moz-document url-prefix() {
  .pageItem { image-rendering: optimizeQuality; }
}
.svg-wrap { width:inherit !important; height:inherit !important; }
.pageItem p img { vertical-align:text-top; }
.pageItem p input, .pageItem p button {display:inline;}
.pageItem p .hidden, .details {visibility:hidden; }
.pageItem.group[data-ani] { will-change: transform; }
#colorbox .details { visibility:visible; }
.details {max-width:550px;font-size:18px;font-family:sans-serif;padding:0 24px;line-height:150%;left:0;right:0;margin:auto;}
.details p {margin-top:.5em;}
.details h1,.details h2,.details h3,.details h4,.details h5, .details strong {font-weight:bold;margin:.7em 0;}
.details em { font-style:italic; }
.details h1{font-size:150%;} .details h2{font-size:140%;} .details h3{font-size:130%;}
.details a {color:#0099ff;text-decoration:underline}
.details a:hover {text-decoration:none;}
@media (max-device-width:812px){ .details { font-size:32px; } }
html.ios .iframe-container { overflow:auto; -webkit-overflow-scrolling:touch; }
iframe[scrolling="auto"] { overflow:auto; }
iframe[scrolling="yes"] { overflow:scroll; }
iframe[scrolling="no"] { overflow:hidden; }
.page-scale-wrap { transform:translateZ(0); }
.page, .page-scale-wrap {
	position:relative; float:left; overflow:hidden;
}
.pages {
	list-style:none outside none;
	padding:0; margin:0 auto ;
}	
#container > .page { /*center single page baker*/
    position:absolute; bottom:0;
    left:0; right:0; top:0; margin:0 auto;
}
body:not(.zoomed,.responsive) #container/*, .page-scale-wrap*/ {/*desktop scaling transitions*/
	-webkit-transition:-webkit-transform .5s;
	transition:transform .5s;
}
html.multifile body #container { opacity:0; }
html.multifile body.loaded #container {/*do show scaling of multi-page*/
	opacity:1;
	-ms-transition:opacity .1s step-start .1s !important;
	-webkit-transition:opacity .1s step-start .1s !important;
	transition:opacity .1s step-start .1s !important;
}
html.multifile.fade body.loaded #container {
	-ms-transition:opacity .6s !important;
	-webkit-transition:opacity .6s !important;
	transition:opacity .6s !important;
}

.textColumn { float:left; }
.singleline p { line-height:1em !important; position:absolute;width:100%;/*fix webkit display issue*/ }
p.col-break-before::before {
	content:'';
    height:0px; width:100%;
    display:block; margin-bottom:100%;
}
.scroll, .scroll-vert, .scroll-horiz { -webkit-overflow-scrolling:touch; }/*was broken in iOS, turn off if scroll not working*/
.scroll { overflow:auto; }
.scroll-vert { overflow-y:auto; overflow-x:hidden; }
.scroll-horiz { overflow-x:auto; overflow-y:hidden; }
.scroll-vert::-webkit-scrollbar { -webkit-appearance:none; width:7px; } /*add back scrollbar for webkit*/
.scroll-vert::-webkit-scrollbar-thumb { border-radius:4px; background-color:rgba(0,0,0,.5); }
.hidescroll::-webkit-scrollbar { display:none; }
.hidescroll { -ms-overflow-style:none; overflow:-moz-scrollbars-none;/*old FF*/ }
.pulltab-left, .pulltab-left > * {
	-moz-transform:scaleX(-1);
    -webkit-transform:scaleX(-1);
    -o-transform:scaleX(-1);
    transform:scaleX(-1);
}
.pulltab-top, .pulltab-top > * {
	-moz-transform:scaleY(-1);
    -webkit-transform:scaleY(-1);
    -o-transform:scaleY(-1);
    transform:scaleY(-1);
}
object, embed, img, a { outline:0; }
.liquid svg, .liquid .page-scale-wrap { height:100%; width:100%; }
.noPlugin {
	width:100%; height:100%; padding:6px;
	background:#ccc; border:1px solid #666;
}

.paper-vertical, .paper-horizontal { padding:0 8px; }
.flip { 
	overflow:hidden; 
	-webkit-transition:transform 0.3s ease-in-out;
	-ms-transition:transform 0.3s ease-in-out;
	transition:transform 0.3s ease-in-out;
}
.turn-page-wrapper{
	will-change:transform;
}
.turn-page {
	-moz-box-shadow:0px 0px 20px rgba(0,0,0,.7);
	-webkit-box-shadow:0px 0px 20px rgba(0,0,0,.7);
    box-shadow:0px 0px 20px rgba(0,0,0,.7);
}
.turn-page:not(.activePage) .pageItem[data-ani] { /*fix 2x animation*/
  	opacity:0;
  	animation:none !important;
}
.paper-horizontal {
	position:absolute; overflow-y:visible; overflow-x:hidden;
	margin-top:auto; margin-bottom:auto;
    top:0; bottom:0;
}

.paper-vertical .page, .paper-horizontal .page {
	border:1px solid #bbb;	
	margin:4px 4px 4px 0;
	-moz-box-shadow:0px 0px 0px #999;
	-webkit-box-shadow:0px 0px 5px #999;
	box-shadow:0px 0px 5px #999;
}

html[data-dir="rtl"] .paper-horizontal .page { float:right; }

.one-page-scroll .page {
	border:none;
	margin:0;
	-moz-box-shadow:none;
	-webkit-box-shadow:none;
	box-shadow:none;
}

.mejs-mediaelement { overflow:hidden; }
.mejs-container{position:relative;background:none;}
.mejs-none .mejs-overlay-loading, .mejs-none .mejs-overlay-button, .mejs-none .mejs-controls, .mejs-bigplay .mejs-controls {display:none !important;}
.mejs-uncon video { object-fit:fill; }
.mejs-coverfit video { object-fit:cover; }
.mejs-ccsize-large .mejs-captions-layer {font-size:20px;}
.mejs-ccsize-xlarge .mejs-captions-layer {font-size:26px;}
.mejs-video .mejs-controls { transform:translateZ(0); }

.mejs-no-controls { display:none; }
.vid-scaled .mejs-layers, .vid-scaled .mejs-controls {
	-webkit-transform:translateZ(0);
	transform:translateZ(0);
}

.liquid .page, .page.liquid {
	position:absolute; width:100%; height:100%;
	overflow:hidden; display:none;
}

.page.liquid { /*for multi-file*/
    display:block;
}
.liquid .page.activePage {display:block; }
.liquid video {width:100%; height:100%; }
.liquid .slideshow img { object-fit:contain; }

.in5-highlight {
	background:rgba(255,255,0,.6);
	mix-blend-mode:multiply;
	pointer-events:none;
	animation-name:in5-highlight-in,in5-highlight-in;
	animation-direction:normal,reverse;
	animation-delay:3s,3s;
	animation-duration:.5s,1s;
	animation-iteration-count:1,1;
}
@keyframes in5-highlight-in{ from{ opacity:0 } to { opacity: 1} }
.hidden { display:none !important; }
.skip-link-wrap { z-index: 1; position: fixed; }
[data-reader-only="1"]{
	transform: translateY(-100vh) !important;
	z-index:-1;
}
[data-reader-only="1"]:focus, [data-reader-only="1"]:active {
	transform: translateY(0%) !important;
	z-index:1;
}
.mso, .group, .mso > .state { pointer-events:none; }
.mso > .state * { pointer-events: inherit; }
.mso > .state.active * { pointer-events:auto; }
[data-tapstart="1"], [data-useswipe="1"], .group > * { pointer-events:auto; }
.mso > .state { display:block; opacity:0; width:100% !important; height:inherit !important; position:absolute; z-index:-1; }
.liquid .mso > .state { height:100% !important; }
.liquid label > .state {
    width:100% !important;
    height:100% !important;
}
.mso > .state.active, .mso > .state.transition { display:block; opacity:1; z-index:0; }
.mso.slideshow.seq, .panzoom, .fauxgroup { overflow:hidden; }
.panzoom { cursor:move; cursor:-moz-grab; cursor:-webkit-grab; }
.panzoom > .content {
	-ms-transform:none;
    -ms-transform-origin:auto;
    -webkit-transform:none;
    -webkit-transform-origin:auto;
    transform:none;
    transform-origin:auto;
}
.panzoom:not(.dragging) > .content {
	transition:all .3s;
}

button .state {width:100% !important; height:100% !important;}
button .state.btn-on, button .state.btn-down { display:none; }
html:not(.ios) button.has-on:hover .state.btn-on { display:block; }
html:not(.ios) button.has-on:hover .state.btn-off, html:not(.ios) button.has-on:hover .state.btn-down { display:none; }
html:not(.zz) button.has-down .state { pointer-events:none; }
html:not(.zz) button.has-down:active .state.btn-down { display:block; }
html:not(.zz) button.has-down:active .state.btn-off, html:not(.zz) button.has-down:active .state.btn-on { display:none; }

.align-vert { display:table; }
[class^="valign"] {
	position:relative;
	display:table-cell;
	vertical-align:middle;
	columns:inherit;
}
.valign-bottom { vertical-align:bottom; }
[class^="valign"] > p { position:relative; }

.flex-image, .fill-image { background-repeat:no-repeat; }
.flex-image { background-size:contain; background-position:center; }
.fill-image { background-size:cover; }

/*tabs*/
p.tabs, p.tabs > a { 
	display:-webkit-box;
	display:-moz-box;
	display:-ms-flexbox;
	display:-webkit-flex;
	display:flex;
	flex-wrap:wrap;
}
p.tabs > a {
	width:100%;
	width:-moz-available;
	width:-webkit-fill-available;
}
p.tabs span.tabbed-right { 
	-ms-flex-grow:1; 
	-webkit-flex-grow:1; 
	flex-grow:1; 
	text-align:right; 
}
p.tabs span.tabbed-center { 
	-ms-flex-grow:50; 
	-webkit-flex-grow:50; 
	flex-grow:50; 
	text-align:center; 
}
span.tabbed-standard { text-indent:2ex;padding-left:2ex; }
p.no-start-indent { text-indent:0px !important; }

/*anchor object styles*/
.ao-noTextWrap { position:absolute; }
.ao-alignLeft, .ao-leftFullWidth { float:left; position:relative; }
.ao-alignRight, .ao-rightFullWidth { float:right; transform-origin:90% 50%; -webkit-transform:90% 50%; /*fix for anchored animation*/ }
.ao-alignCenter {display:block; margin-left:auto; margin-right:auto;}
.ao-inlineTable { display:block; }
.ao-leftFullWidth { padding-right:100%; }
.ao-rightFullWidth { padding-left:100%; }
.anchorGroup { position:relative; };
div.ao-alignLeft:before, div.ao-leftFullWidth:before { content:''; float:left; display:none; }
div.ao-alignRight:before, div.ao-leftFullRight:before { content:''; float:right; display:none; }
.anchorGroup > .mso, .anchorGroup > .group { position:relative; }

ul.thumbs {
	padding:20px; white-space:nowrap; width:1px;
}

ul.thumbs li { /*Baker index thumbnails*/
    display:inline; list-style-type:none;
    margin:0 4px; outline:none;
    vertical-align:top;
}
ul.thumbs > li img { box-shadow:0 0 4px rgba(0, 0, 0, 0.5); }
.baker audio[controls] {min-width:400px;} /*fix progress bar*/

@media print { 
	#container,.page-scale-wrap{transform:none !important;}
	[class*=" btn-form-"]{display:none;}
}

:-ms-fullscreen .paper-horizontal { width:auto;height:auto;position:initial;margin:auto; }
:-moz-full-screen .paper-horizontal { width:auto;height:auto;position:initial;margin:auto; }
:-webkit-full-screen .paper-horizontal { width:auto;height:auto;position:initial;margin:auto; }

:-ms-fullscreen .paper-vertical .page { display:none; }
:-moz-full-screen .paper-vertical .page { display:none; }
:-webkit-full-screen .paper-vertical .page { display:none; }

:-ms-fullscreen .paper-horizontal .page { display:none; }
:-moz-full-screen .paper-horizontal .page { display:none; }
:-webkit-full-screen .paper-horizontal .page { display:none; }

:-ms-fullscreen .page.activePage { display:block; }
:-moz-full-screen .page.activePage { display:block; }
:-webkit-full-screen .page.activePage { display:block; }

:-webkit-full-screen .hideFS { display:none; }
:-ms-fullscreen .hideFS { display:none; }
:-moz-full-screen .hideFS { display:none; }

/*CSS Generated from InDesign Styles*/

body, #container-wrap { background:#ededed; }
:-webkit-full-screen { background:#ededed; }
#loadIndicator span:after { padding-left:1ex; content:'loading content...'; }
.page-scale-wrap { width:612px; height:651px; background: #fff !important; }
.paper-vertical { width:612px; height:100%; }
.paper-horizontal { width:1244px; height:663px; }
@media all and (max-height:651px) {
	.paper-horizontal { margin:0;top:0;}
	#container > .page { margin:0 auto;}/*pos top for webkit+baker*/
}
@media all and (max-width:612px) {
	.paper-vertical .page, .paper-horizontal .page, .anythingSlider-in5 { padding:0;top:0;border:0; }
	.paper-vertical, .paper-horizontal { padding:0; }
}

#item243 {
	width:468px !important;
	height:264px !important;
	left:72px !important;
	top:70px !important;
}

#item569 {
	width:509px !important;
	height:307px !important;
	left:-19px !important;
	top:581px !important;
}

p.Basic-Paragraph {
	font-family:"Minion Pro","Times New Roman", Times, serif;
	font-size:12px;
	line-height:14.4px;
	color:#000;
	hyphens:auto;
	-moz-hyphens:auto;
	-ms-hyphens:auto;
	-webkit-hyphens:auto;
	hyphenate-after:2;
	-ms-hyphenate-after:2;
	-moz-hyphenate-after:2;
	-webkit-hyphenate-after:2;
	hyphenate-before:2;
	-ms-hyphenate-before:2;
	-moz-hyphenate-before:2;
	-webkit-hyphenate-before:2;
	text-align:left;
}

p.No-Paragraph-Style {
	font-family:"Minion Pro","Times New Roman", Times, serif;
	font-size:12px;
	line-height:14.4px;
	color:#000;
	hyphens:auto;
	-moz-hyphens:auto;
	-ms-hyphens:auto;
	-webkit-hyphens:auto;
	hyphenate-after:2;
	-ms-hyphenate-after:2;
	-moz-hyphenate-after:2;
	-webkit-hyphenate-after:2;
	hyphenate-before:2;
	-ms-hyphenate-before:2;
	-moz-hyphenate-before:2;
	-webkit-hyphenate-before:2;
	text-align:left;
}

span.None {
}
