

1. Resolution

* provided PDF wireframe is made with 300dpi resolution and 2480 pixels width. maybe for Retina display.

* standard screen resolution is 72dpi

* resizing 300dpi to 72dpi gives 595px width

* resizing 300dpi to 150dpi gives 1240px width (that tells me maybe Retina display as it 2@x)


2. Responsive

* used Fluid responsive just in case adaptive to many screen sizes 

* Mobile responsive is added


3. SASS

* folder /sass/style.scss

* max 3rd level

* custom reset added

* no need to add general full reset.css or normalize.css if project doesn't require elements such as audio,
canvas, details, hgroup, progress, table, ol etc 


4. Responsive navigation menu for mobile

* no JS used as required

* brief : On mobile , clicking on the “menu” link should display the menu entries to the user.

click "menu" link can mean to add small script such as JQuery

		$(".menu-link").click(function() {
			$(".menu").slideToggle("fast");
			return false;
		});

but use of JS is discouraged and I came with below solution


* click "menu" link works such as hover of #nav:hover .menu {display:block} or .menu-link:hover .menu

* bonus but not required - structure can be also presented in diffrent way such as below

	<!-- Navigation -->
	<nav id="nav">
		<ul class="navbar">
			<li>
				<a href="" title="menu link" class="menu-link">menu</a>
				<ul class="menu">
					<li><a href="#" title="link title">Home</a></li>
					<li><a href="#" title="link title">eBooks</a></li>
					<li><a href="#" title="link title">Magazines</a></li>
					<li><a href="#" title="link title">Movies</a></li>
					<li><a href="#" title="link title">Help</a></li>
					<li><a href="#" title="link title">Login</a></li>
				</ul>
			</li>
		</ul>    
	</nav><!-- /#nav -->

	#nav li:hover .menu {display:block}




5. CSS 3

* added a few small things for hovers



6. Scripts

* no scripts added

* no bug fix scripts for IE 6, 7, 8 added 

* IE doesnt support CSS 3 shadows, rounded corners etc


7. font-face

* PDF document used Droid Serif and Droid Sans

* Droid Sans added to the test work


8. social icons

* added as a sprite image

* smaller icons with Mobile version

* PNG transparency for IE6 can be solved if bug fix added or add below line onto CSS

it can also go like this _filter:progid:DXImageTransform.Microsoft.AlphaImageLoader (src='',sizingMethod='crop');


9. Testing

* Chrome 

* Firefox

* Opera

* IE 7+

* Safari

* iPhone

* IPad