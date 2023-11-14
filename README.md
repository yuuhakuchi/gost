# gost

@charset "UTF-8";
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script&family=Noto+Sans+TC&display=swap');

/* http://meyerweb.com/eric/tools/css/reset/ 
	v2.0 | 20110126
	License: none (public domain)
*/
@font-face {
	font-family: coolvetica;
	src: url(../webfonts/coolvetica\ rg.otf);
}

/* 咒語 - 消除所有預設 */
html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
	display: block;
}

body {
	line-height: 1;
}

ol,
ul {
	list-style: none;
}

blockquote,
q {
	quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
	content: '';
	content: none;
}

table {
	border-collapse: collapse;
	border-spacing: 0;
}

* {
	box-sizing: border-box;
}

body {
	font-family:
		-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, "Helvetica Neue", Helvetica, Arial,
		"PingFang TC", "Heiti TC", "Microsoft JhengHei", "Noto Sans TC", sans-serif;
}

:root {
	--light_grey: #ccc;
	--grey: #999;
	--deep_grey: #444;
	--major-color: #f2edf0;
	--major-color2: #e6ece5;
	--major-color3: #ecf0f4;
	--lesser-color1: #bf9899;
}


a {
	display: block;
	color: var(--deep_grey);
	text-decoration: none;
}

/* 咒語 - 消除所有預設 */

body {
	font-family: 'Arial', sans-serif;
	margin: 0;
	padding: 0;
	background-color: black;
}

#section-1 {
	height: 100vh;
}

.index_banner img {
	width: 100%;
	padding: 0px 0 0px 0;

}

.mobile_banner {
	display: none;
}

/* 導覽頁 */

/* 頁首區 */
#topbar {
	/* position預設寬度為內容的寬度 */
	position: absolute;
	/* 固定定位 */
	left: 0px;
	top: 0px;
	/* 座標位置 */
	width: 100%;
	/* 補position移除的寬度 */
	display: flex;
	justify-content: space-between;
	padding: 40px 24px 0 24px;
	background-color: #000;
	/* background-color: cadetblue; */
	z-index: 999;
}

#topbar .desktop_logo {
	width: 20%;
	display: flex;
	align-items: center;
}

#topbar .desktop_logo img {
	width: 100%;
	margin-bottom: 32px;
}

.mobile-logo {
	display: none;
	/* 隱藏手機版 logo */
}


#topbar nav {
	display: flex;
	flex-direction: column;
	/* 主軸:垂直 */
	align-items: flex-end;
	/* 副軸:水平/齊底 */
}

#topbar ul {
	display: flex;
}

.menu {
	margin: 0px 0;
	padding: 10px 20px 0px 20px;
	background-color: #000;
}

.menu a {
	color: aliceblue;
	font-size: 15px;
	font-weight: 700;
	padding: 10px 0 10px 0px;
	margin: 0 20px;
	transition: background-color 0.3s ease-out, color 0.5s ease-out;
	box-sizing: border-box;
	/* 要固定 a 的總尺寸，增加的內距會會從內容的空間扣除 */
}

.menu a:hover {
	font-weight: bolder;
	color: black;
	background-color: rgba(232, 61, 24, 0.8);
	position: relative;
	padding: 60px 15px 60px 15px;
	margin: -50px 5px;
	/* 要讓元素位置保留和原本一樣的地方 */
}

.has-dropdown {
	position: relative;
}

.dropdown-content {
	display: none;
	position: absolute;
	top: 243%;
	/* 使下拉內容在上方 */
	left: -14%;
}

.has-dropdown .dropdown-content :hover {
    position:absolute;
	display: flex;
	flex-direction: column;
}

.has-dropdown:hover .dropdown-content {
	display: block;
	position: absolute;
}

.dropdown-content a{
	font-size: 15px; 
	width: 80%;
    padding: 15px 10px 10px 10px;
	color: #E73D18;
	background-color: #000;
}




@media (min-width:821px) {
	.hamburger {
		display: none;
	}
}

@media (max-width:821px) {

	/* 平板 選單列樣式 */
	.menu {
		display: flex;
		flex-direction: column;
		padding: 10px 20px;
		border-radius: 20px;
		background-color: rgba(255, 255, 255, 0.4);
	}

	.menu li {
		margin-bottom: 20px;
	}

	.menu a {
		font-family: Jost, sans-serif;
		position: relative;
		text-decoration: none;
		color: black;
		padding: 10px;
	}

	.icon {
		display: flex;
		justify-content: space-between;
		width: 100%;
	}

	.icon a {
		width: 35px;
		margin: 0 5px;
	}

	/* 漢堡按鈕  */
	.nav_box {
		position: relative;
		display: flex;
		flex-direction: column;
		align-items: flex-end;
	}

	.hamburger {
		display: inline-block;
		cursor: pointer;
		background-color: transparent;
		border: none;
		padding: 0;
	}

	.bar {
		display: block;
		width: 25px;
		height: 3px;
		background-color: #333;
		margin: 5px auto;
		transition: all 0.3s ease-in-out;
	}

	/* 三 變換為 X */
	.hamburger.is-active .bar:nth-child(1) {
		transform: translateY(8px) rotate(45deg);
	}

	.hamburger.is-active .bar:nth-child(2) {
		opacity: 0;
	}

	.hamburger.is-active .bar:nth-child(3) {
		transform: translateY(-8px) rotate(-45deg);
	}

	.navigation {
		display: none;

		position: absolute;
		top: 40px;
		right: 0px;
		/* background-color: rgba(255, 255, 255, 0.3); */
		animation: navigation 0.35s both;
	}

	@keyframes navigation {
		from {
			opacity: 1;
		}

		to {
			opacity: 0;
		}
	}

	.navigation.show {
		display: block;
		animation: show 0.35s both;
	}

	@keyframes show {
		from {
			opacity: 0;
		}

		to {
			opacity: 1;
		}
	}

}





/* chat 輔助 相對位置 */


#carouselExampleAutoplaying {
	margin: 100px 0 125px 0;
}

/* Section-1 Styles
#section-1 {
	height: 100vh;
	color: #fff;
	background-color: #222;
}

#section-1 .content-slider {
	position: relative;
	width: 100%;
	height: 100%;
}

#section-1 .content-slider input {
	display: none;
}

#section-1 .content-slider .slider {
	position: relative;
	width: inherit;
	height: inherit;
	overflow: hidden;
}

#section-1 .content-slider .slider .banner {
	position: absolute;
	top: 0;
	left: 0;
	opacity: 0;
	z-index: 0;
	width: inherit;
	height: inherit;
	text-align: center;
	background-repeat: no-repeat;
	background-position: 50% 50%;
	transition: all 0.5s ease;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper {
	height: 100%;
	padding-top: 6em;
	background-image: linear-gradient(rgba(243, 129, 129, 0.9), rgba(252, 227, 138, 0.9));
	box-sizing: border-box;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper h2 {
	padding-bottom: 0.3em;
	font-family: "Kaushan Script", cursive;
	font-weight: 400;
	font-size: 2.5em;
	text-transform: none;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper h1 {
	font-size: 6em;
	line-height: 95%;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper .line {
	display: block;
	width: 4em;
	height: 0.1875em;
	margin: 2.5em auto;
	background: #fff;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper .learn-more-button {
	padding-bottom: 5em;
	z-index: 15 !important;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper .learn-more-button a {
	padding: 0.5em 2em;
	text-align: center;
	font-family: Montserrat, sans-serif;
	font-size: 0.875em;
	color: #fff;
	text-transform: uppercase;
	border: 0.1875em solid #fff;
}

#section-1 .content-slider .slider .banner .banner-inner-wrapper .learn-more-button a:hover {
	color: #e88382;
	border-color: #e88382;
	transition: 0.3s;
}

#section-1 .content-slider .slider #top-banner-1 {
	background: url("https://checkboxes-demo.webdevs.co.ua/images/mogo/banner-1.png") no-repeat center center;
	background-size: cover;
}

#section-1 .content-slider .slider #top-banner-2 {
	background: url("https://checkboxes-demo.webdevs.co.ua/images/mogo/banner-2.png") no-repeat center center;
	background-size: cover;
}

#section-1 .content-slider .slider #top-banner-3 {
	background: url("https://checkboxes-demo.webdevs.co.ua/images/mogo/banner-3.png") no-repeat center center;
	background-size: cover;
}

#section-1 .content-slider .slider #top-banner-4 {
	background: url("https://checkboxes-demo.webdevs.co.ua/images/mogo/banner-4.png") no-repeat center center;
	background-size: cover;
}

#section-1 .content-slider nav {
	position: absolute;
	bottom: 0.5em;
	width: 100%;
	z-index: 10;
	text-align: center;
}

#section-1 .content-slider nav .controls {
	display: block;
	width: 70%;
	margin: 0 auto;
	font-family: Montserrat, sans-serif;
	color: #fff;
}

#section-1 .content-slider nav .controls label {
	position: relative;
	display: inline-block;
	width: 20%;
	height: 3.1em;
	overflow: hidden;
	margin: 0 1em;
	padding-top: 1em;
	text-align: left;
	text-transform: uppercase;
	font-family: Montserrat, sans-serif;
	font-size: 1em;
	color: #f6eac5;
	font-weight: 400;
	cursor: pointer;
	transition: all 0.3s;
}

#section-1 .content-slider nav .controls label .progressbar {
	position: absolute;
	top: 0;
	left: 0;
	height: 3px;
	width: 100%;
	background: #f6eac5;
	z-index: 100;
}

#section-1 .content-slider nav .controls label .progressbar .progressbar-fill {
	position: inherit;
	width: inherit;
	height: inherit;
	margin-left: -100%;
	background: #e88382;
}

#section-1 .content-slider nav .controls label span {
	font-size: 1.4em;
	font-weight: 700;
}

#section-1 .content-slider nav .controls label:hover {
	color: #e88382;
}

#section-1 .content-slider #banner1:checked~.slider #top-banner-1,
#section-1 .content-slider #banner2:checked~.slider #top-banner-2,
#section-1 .content-slider #banner3:checked~.slider #top-banner-3,
#section-1 .content-slider #banner4:checked~.slider #top-banner-4 {
	opacity: 1;
	z-index: 1;
}

#section-1 .content-slider #banner1:checked~nav label:nth-of-type(1),
#section-1 .content-slider #banner2:checked~nav label:nth-of-type(2),
#section-1 .content-slider #banner3:checked~nav label:nth-of-type(3),
#section-1 .content-slider #banner4:checked~nav label:nth-of-type(4) {
	cursor: default;
	color: #fff;
	transition: all 0.5s;
}

#section-1 .content-slider #banner1:checked~nav label:nth-of-type(1) .progressbar,
#section-1 .content-slider #banner2:checked~nav label:nth-of-type(2) .progressbar,
#section-1 .content-slider #banner3:checked~nav label:nth-of-type(3) .progressbar,
#section-1 .content-slider #banner4:checked~nav label:nth-of-type(4) .progressbar {
	background: #fff;
}

#section-1 .content-slider #banner1:checked~nav label:nth-of-type(1) .progressbar-fill,
#section-1 .content-slider #banner2:checked~nav label:nth-of-type(2) .progressbar-fill,
#section-1 .content-slider #banner3:checked~nav label:nth-of-type(3) .progressbar-fill,
#section-1 .content-slider #banner4:checked~nav label:nth-of-type(4) .progressbar-fill {
	animation: progressBarFill 5s linear;
}

/* Animations */
@keyframes progressBarFill {
	from {
		margin-left: -100%;
	}

	to {
		margin-left: 0;
	}
}

*/ .left_icon,
.right_icon,
.autopoint {
	position: absolute;
	/*能置於 main banner上層*/
	width: 50px;
	/* 設定圖標的寬度，根據需求調整 */
	cursor: pointer;
}

.left_icon {
	left: 10px;
	/* 設定圖標離左邊的距離 */
}

.right_icon {
	right: 10px;
	/* 設定圖標離右邊的距離 */
}

.autopoint {
	bottom: 20px;
	/* 設定autopoint離底部的距離 */
	left: 50%;
	/* 設定autopoint水平居中 */
	width: 75px;
	transform: translateX(-50%);
	/* 修正水平居中的位置 */
}

/* main_banner 下方 */

/*設定鬼鬼的相對位置*/
.animate_g {
	background-color: #000;
	position: absolute;
	display: flex;
	align-items: center;
	/* 水平置中 */
	justify-content: space-between;
	width: 100%;
	/* 控制兩個圖片之間的距離 */
	z-index: 1;
}

/*設定鬼鬼的詳細位置*/
#Lanimate {
	margin-left: 220px;
	margin-top: -10px;
	padding: 50px;
	width: 20%;
}

#Ranimate {
	margin-right: 220px;
	margin-top: -10px;
	padding: 50px;
	width: 20%;
}

@media(max-width:820px) {
	#Lanimate {
		margin-left: 100px;
		width: 25%;
	}

	#Ranimate {
		margin-right: 100px;
		width: 25%;
	}
}

/*設定標準字的相對位置*/
.group1 {
	position: relative;
	display: flex;
	align-items: center;
	justify-content: center;
	flex-direction: column;
	z-index: 2;
}



/*設定標準字的詳細位置*/
.ch-stander {
	position: relative;
	padding: 50px 0px 20px 0;
	width: 30%;
}

.en-stander {
	position: relative;
	padding: 0px;
	width: 30%;
}

.slogan {
	position: relative;
	padding: 20px 0;
	width: 32%;
}

@media(max-width:820px) {
	.ch-stander {
		width: 35%;
	}

	.en-stander {
		width: 35%;
	}

	.slogan {
		width: 43%;
	}
}

/* 設定 index02 的相對位置 */

.gost {
	position: relative;
	top: -125px;

}

.gost .L {
	position: relative;
	width: 255%;
	right: 385px;
	top: 87px;
}

.gost .R {
	position: absolute;
	width: 255%;
	top: 87px;
	left: 260px;
}

.slogan {
	position: relative;
	width: 35%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	top: -250px;
	right: 15px;
	margin: 0 0 -10% 0;
}

.slogan .T {
	position: relative;
	left: 20px;
	top: -40px;
}

.slogan div img {
	width: 34%;
}

.slogan .two {
	width: 52%;
}

.slogan .sec {
	position: relative;
	width: 80%;
	top: -20px;
	left: 40px
}


.slogan .third {
	position: relative;
	width: 100%;
	left: 0px;
}

.historyphoto {
	background-color: #000;
	position: relative;
	display: flex;
	flex-direction: column;
	/*轉換垂直排列*/
	align-items: center;
	justify-content: center;
	width: 100%;
}

.album {
	display: flex;
	justify-content: center;
	width: 100%;
	margin: 0px 0 0px 0;
}

.ph_album {
	display: flex;
	justify-content: center;
	align-content: center;
	width: 80%;
	margin: 60px 0 0px 0;
}

.iphone-ph,
.iphone-ph2,
.iphone-ph3 {
	display: none;
}

.more_btn {
	display: flex;
	padding: 10px 0 10px 0;
}

/*  票區  */
.ticket {
	background-color: #000;
	position: relative;
	display: flex;
	flex-direction: column;
	/*轉換垂直排列*/
	align-items: center;
	justify-content: center;
	width: 100%;
}

.tilte {
	margin: 68px 0 11px 0;
}

.ph_ticket {
	margin: 23px 0;
	width: 80%;
}

.wo_ticket {
	width: 50%;
}

.iphone_ticket {
	display: none;
}

.iphone_ticket_p {
	display: none;
}

.iphone_ticket_p1 {
	display: none;
}

.iphone_ticket_p2 {
	display: none;
}

/* RWD尺寸 */
@media(max-width:820px) {
	.ticket {
		height: 100%;
		width: auto;
		padding: 0px 15px;

	}
}


/*  藝人區  */
.artist {
	background-color: #000;
	position: relative;
	display: flex;
	flex-direction: column;
	/*轉換垂直排列*/
	align-items: center;
	justify-content: center;
	width: 100%;
}

.ph_artist {
	margin: 23px 0;
	width: 80%;
}

.wo_artist {
	width: 50%;
}


.iphone_artist {
	display: none;
}


.iphone_artist_p {
	display: none;
}

.iphone_artist_p1 {
	display: none;
}


/* 新聞區 */
.news {
	background-color: #000;
	position: relative;
	display: flex;
	flex-direction: column;
	/*轉換垂直排列*/
	align-items: center;
	justify-content: center;
	width: 100%;
	padding-bottom: 94px;
}

.ph_news {
	margin: 23px 0;
	width: 80%;
}

.wo_news {
	width: 50%;
}

.iphone_news {
	display: none;
}

.iphone_news_p {
	display: none;
}

.iphone_news_p1 {
	display: none;
}

.more_btn_ne {
	display: none;
}

/* footer區 */

footer {
	position: relative;
	background-color: #87C122;
	width: 100%;
	height: 75vh;
}

.iphone-footer {
	display: none;
}

.footer_wrapper {
	position: absolute;
	top: 9%;
	left: 12.5%;
	right: 12.5%;
	bottom: 9%;

	display: flex;
	flex-direction: column;
}

.word img {
	width: 28%;
	margin: 7px 0px;
}

.iphone_footer_word {
	display: none;
}

.iphone_icon {
	display: none;
}

.social_links {
	display: flex;
}


.social_links img {
	margin: 0px 15px 100px 0px;
}



.web_map {
	position: absolute;
	display: flex;
	font-weight: bolder;
	font-size: 100%;
	right: 0px;
	top: 2%;
}

.web_map h3 {
	margin: 0px 0px 0px 40px;
}


.web_map p {
	margin: 32px 0px 0px 40px;
	font-size: 80%;
	font-weight: 400;
}

.iphone_map {
	display: none;
}

.rights_reserved {
	display: flex;
	flex-direction: column;
}

.rights_reserved .line {
	color: #000;
	border-bottom: 1px solid #000;
	/* 這裡指定了寬度為1px，樣式為solid，和顏色 */
	padding: 16px 0;
	margin: 0px 0px 32px 0px;
}

.iphone_res {
	display: none;
}

.rights {
	width: 30%;
}

.late_line {
	display: flex;
	flex-direction: row;
}


.late_line p {
	margin: 0px 330px 0 0px;
}

.late_line a {
	color: #000;
	border-bottom: 1px solid #000;
	font-size: 80%;
	font-weight: 400;
	margin: 0px 0 0 150px;

}

/*	Gotop 列 */
#gotop {
	position: fixed;
	right: 40px;
	bottom: 40px;
	width: 50px;
	height: 50px;
	padding: 14px;
	background-color: rgba(255, 255, 255, 0.7);
	border-radius: 100%;
}

#gotop:hover {
	animation: bounce 1s;
}

@keyframes bounce {

	0%,
	50%,
	80%,
	100% {
		transform: translateY(0);
	}

	20% {
		transform: translateY(10px);
	}

	40% {
		transform: translateY(-5px);
	}

	60% {
		transform: translateY(2px);
	}
}

@media (max-width:576px) {


	/* banner */
	.mobile_banner {
		display: block;
		position: absolute;
		z-index: 999;
		top: 0px;
	}

	.d-block {
		display: none !important;
	}

	/* nav-bar */
	#topbar {
		width: 100%;
		position: sticky;
		/* 将导航栏固定在屏幕上 */
		top: 530px;
		height: 40px;
		background-color: #E73D18;
		padding: 0px 15px;
		/* 调整内边距 */
		justify-content: space-between;
		z-index: 999;
	}

	#topbar h1 {
		width: 50%;
	}

	#topbar .desktop_logo {
		display: none;
		/* 隱藏手機版 logo */
		margin-bottom: 0px;
	}

	.mobile-logo {
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
		width: 70%;
		padding: 4px 0px;
	}



	.navigation {
		display: none;
		/* 隐藏导航栏 */
	}

	.hamburger {
		display: flex;
		/* 显示汉堡按钮 */
		flex-direction: column;
		padding: 8px 0px;
	}

	.hamburger .bar {
		background-color: #040404;
		/* 汉堡按钮的颜色 */
		height: 3px;
		/* 汉堡按钮条的高度 */
		margin: 2px 0;
	}

	/* G O S T  */


	.gost .L {
		width: 100%;
		top: 427px;
		right: 143px;
	}

	.gost .R {
		width: 100%;
		top: 427px;
		left: 125px;
	}

	.slogan {
		position: relative;
		width: 35%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		top: 230px
	}

	.slogan .T {
		position: relative;
		left: -27px;
		top: -38px;
		width: 170%;
	}

	.slogan div img {
		width: 34%;
	}

	.slogan .two {
		width: 52%;
	}

	.slogan .sec {
		position: relative;
		width: 140%;
		top: -36px;
		left: -20px;
	}


	.slogan .third {
		position: relative;
		width: 155%;
		left: -30px;
		top: -30px;
		bottom: 25px;
	}

	/* photo */

	.historyphoto {
		position: relative;
		display: flex;
		flex-direction: column;
		/*轉換垂直排列*/
		align-items: center;
		justify-content: center;
		width: 100%;
	}

	.album {
		position: relative;
		display: flex;
		flex-direction: column;
		flex-wrap: wrap;
		align-items: center;
	}

	.album .iphone-ph {
		position: relative;
		width: 100%;
		top: 230px;
		padding: 0px 15px;
		z-index: 99;
		;
	}

	.iphone-ph,
	.iphone-ph2,
	.iphone-ph3 {
		display: flex;
	}

	.ph_album {
		display: none;
	}


	.more_btn {
		display: flex;
		padding: 103px 40px 5px 55px;
		width: 85%;
	}

	.wo_ticket {
		display: none;
	}

	.ph_ticket {
		display: none;
	}

	/*  票區  */
	.tilte {
		display: none;
	}

	.iphone_ticket {
		display: flex;
		position: relative;
		margin-top: 32px;

	}

	.iphone_ticket_p {
		position: relative;
		display: flex;
		margin: 8px 0px;
	}

	.iphone_p {
		display: flex;
	}

	.iphone_ticket_p1 {
		display: flex;
		position: relative;
	}

	.iphone_ticket_p2 {
		display: flex;
		position: relative;
		left: 12px;
	}

	.more_btn_ti {
		position: relative;
		display: flex;
		padding: 5px 26px 5px 47px;
		width: 80%;
	}

	/*  人區  */

	.iphone_artist {
		margin-top: 32px;
		display: flex;
		position: relative;
	}


	.iphone_artist_p {
		padding: 8px 0px;
		display: flex;
		position: relative;
	}

	.iphone_artist_p1 {
		display: flex;
		position: relative;
	}

	.more_btn_ar {
		position: relative;
		display: flex;
		padding: 0px 26px 5px 47px;
		top: -87px;
		width: 80%;
	}

	/* 消息區 */

	.iphone_news {
		margin-top: -64px;
		display: flex;
		position: relative;
	}


	.iphone_news_p {
		padding: 8px 0px;
		display: flex;
		position: relative;
	}

	.iphone_news_p1 {
		display: flex;
		position: relative;
	}

	.more_btn_ne {
		position: relative;
		display: flex;
		padding: 0px 26px 5px 47px;
		margin-bottom: -30px;
		top: 8px;
		width: 75%;
	}

	/* footer  */

	footer {
		display: flex;
		position: absolute;
		background-color: #87C122;
		height: 180vh;
	}

	.footer_wrapper {
		top: 7%;
		left: 7%;
		right: 7%;
	}

	.iphone-footer {
		display: flex;
	}

	.web_footer {
		display: none;
	}

	.iphone_footer_word {
		display: flex;
		flex-direction: column;
		align-content: center;
		flex-wrap: wrap;
		margin: 10px 0px;
	}

	.social_links {
		display: flex;
		flex-direction: row;
		justify-content: center;
		margin: 14px 0px -76px 0px;
	}

	.iphone_icon {
		display: flex;
	}

	.web_icon {
		display: none;
	}

	.iphone_map {
		display: flex;
		flex-direction: column;
		font-size: 24px;
		font-weight: 800;
	}

	.iphone_map h2 {
		color: #000;
	}

	.iphone_map .tri {
		border-bottom: #000 1px solid;
		padding: 32px 0;

	}

	.iphone_map {
		border-top: #000 1px solid;
		padding: 0px 0px 32px;

	}

	.triangle {
		width: 0;
		height: 0;
		border-left: 10px solid transparent;
		/* 左边的边框透明 */
		border-right: 10px solid transparent;
		/* 右边的边框透明 */
		border-bottom: 20px solid rgb(0, 0, 0);
		/* 底部的边框设置为三角形的颜色 */
		rotate: 90deg;
		transition: transform 0.3s;
	}

	.triangle:hover {
		transform: rotate(90deg);
	}

	.triangle:hover::after {
		content: "Hi";
		position: absolute;
		top: 100%;
		left: 0px;
		padding: 0 30px;

	}

	.iphone_map .tri {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-items: center;
		justify-content: space-between;
	}


	.iphone_res {
		display: flex;
		flex-direction: column;
		align-items: center;
		bottom: 32px;
	}

	.iphone_res img {
		padding: 16px 0px;
	}

	.iphone_i {
		display: flex;
		margin: 16px 0;
		font-weight: 800;
	}

	.iphone_i a {
		color: #000;
		border-bottom: #000 1px solid;
		margin: 0px 28px;
	}

	.iphone_res p {
		color: #000;
		font-size: 14px;
		font-weight: 700;
	}














	/*   desktop - 系列         */

	/*  藝人區  */

	.ph_artist {
		display: none;
		margin: 23px 0;
		width: 80%;
	}

	.wo_artist {
		display: none;
		width: 50%;
	}






	.ph_news {
		display: none;
		margin: 23px 0;
		width: 80%;
	}

	.wo_news {
		display: none;
	}



	.word img {
		display: none;
		width: 28%;
		margin: 7px 0px;
	}




	.social_links img {
		display: flex;
		margin: 0px 15px 100px 0px;
	}

	.web_map {
		display: none;

	}

	.web_map h3 {
		display: none;
		margin: 0px 0px 0px 40px;
	}


	.web_map p {
		display: none;
		margin: 32px 0px 0px 40px;
		font-size: 80%;
		font-weight: 400;
	}

	.rights_reserved {
		display: none;

	}

	.rights_reserved .line {
		display: none;

	}


	.rights {
		display: none;
		width: 30%;
	}

	.late_line {
		display: none;
		display: flex;
		flex-direction: row;
	}


	.late_line p {
		display: none;
		margin: 0px 330px 0 0px;
	}

	.late_line a {
		display: none;

	}

}
