
<!DOCTYPE html>
<!--[if IE 7]>
<html class="ie ie7" lang="en-US" prefix="og: http://ogp.me/ns#">
<![endif]-->
<!--[if IE 8]>
<html class="ie ie8" lang="en-US" prefix="og: http://ogp.me/ns#">
<![endif]-->
<!--[if !(IE 7) | !(IE 8)  ]><!-->
<html lang="en-US" prefix="og: http://ogp.me/ns#">
<!--<![endif]-->
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width" />
<meta name="description" content="A Computer Science portal for geeks. It contains well written, well thought and well explained computer science and programming articles, quizzes and practice/competitive programming/company interview Questions.">
<link rel="shortcut icon" href="/gfg.png" type="image/x-icon" />

<meta property="og:image" content="https://www.geeksforgeeks.org/wp-content/uploads/gfg_200X200.png">
<meta property="og:image:type" content="image/png">
<meta property="og:image:width" content="200">
<meta property="og:image:height" content="200">

<title>Scanner Class in Java - GeeksforGeeks</title>
<link rel="profile" href="http://gmpg.org/xfn/11" />
<link rel="pingback" href="" />
<!--[if lt IE 9]>
<script src="https://www.geeksforgeeks.org/wp-content/themes/iconic-one/js/html5.js" type="text/javascript"></script>
<![endif]-->

<script type="application/ld+json">
    {
        "@context" : "http://schema.org",
        "@type" : "Organization",
        "name" : "GeeksforGeeks",
        "url" : "https://www.geeksforgeeks.org/",
        "logo" : "https://www.geeksforgeeks.org/gfgLogo.png",
        "description" : "A computer science portal for geeks. It contains well written, well thought and well explained computer science and programming articles, quizzes and practice/competitive programming/company interview Questions.",
        "founder": [
            {
                "@type" : "Person",
                "name" : "Sandeep Jain",
                "url" : "https://in.linkedin.com/in/sandeep-jain-b3940815"
            }
        ],
        "sameAs" : [ "https://www.facebook.com/geeksforgeeks.org/",
            "https://twitter.com/geeksforgeeks",
            "https://www.linkedin.com/company/1299009",
            "https://www.youtube.com/geeksforgeeksvideos/"
        ]
    }
</script>
<script>

    var arrPostCat = new Array();
            arrPostCat.push('2058');
            arrPostCat.push('2078');
        var domain = 1;
    var arrPost = new Array();
    var post_id = "136904";
    var post_type = "post";
    var post_slug = window.location.href;
    var ip = "13.59.250.5";
    var post_title = "Scanner Class in Java";
    var post_status = "publish";
                            var isAdminLoggedIn = 0;
        </script>

<!-- This site is optimized with the Yoast SEO plugin v3.7.1 - https://yoast.com/wordpress/plugins/seo/ -->
<link rel="canonical" href="https://www.geeksforgeeks.org/scanner-class-in-java/" />
<meta property="og:locale" content="en_US" />
<meta property="og:type" content="article" />
<meta property="og:title" content="Scanner Class in Java - GeeksforGeeks" />
<meta property="og:description" content="Scanner is a class in java.util package used for obtaining the input of the primitive types like int, double etc. and strings. It is the… Read More &raquo;" />
<meta property="og:url" content="https://www.geeksforgeeks.org/scanner-class-in-java/" />
<meta property="og:site_name" content="GeeksforGeeks" />
<meta property="article:tag" content="Java-I/O" />
<meta property="article:section" content="Java" />
<meta property="article:published_time" content="2016-02-09T22:01:38+00:00" />
<meta property="article:modified_time" content="2017-05-27T11:31:38+00:00" />
<meta property="og:updated_time" content="2017-05-27T11:31:38+00:00" />
<!-- / Yoast SEO plugin. -->

<link rel='dns-prefetch' href='//www.geeksforgeeks.org' />
<link rel='dns-prefetch' href='//fonts.googleapis.com' />
<link rel='dns-prefetch' href='//s.w.org' />
<link rel="alternate" type="application/rss+xml" title="GeeksforGeeks &raquo; Feed" href="https://www.geeksforgeeks.org/feed/" />
<link rel="alternate" type="application/rss+xml" title="GeeksforGeeks &raquo; Comments Feed" href="https://www.geeksforgeeks.org/comments/feed/" />
		<script type="text/javascript">
			window._wpemojiSettings = {"baseUrl":"https:\/\/s.w.org\/images\/core\/emoji\/2\/72x72\/","ext":".png","svgUrl":"https:\/\/s.w.org\/images\/core\/emoji\/2\/svg\/","svgExt":".svg","source":{"concatemoji":"https:\/\/www.geeksforgeeks.org\/wp-includes\/js\/wp-emoji-release.min.js"}};
			!function(a,b,c){function d(a){var c,d,e,f,g,h=b.createElement("canvas"),i=h.getContext&&h.getContext("2d"),j=String.fromCharCode;if(!i||!i.fillText)return!1;switch(i.textBaseline="top",i.font="600 32px Arial",a){case"flag":return i.fillText(j(55356,56806,55356,56826),0,0),!(h.toDataURL().length<3e3)&&(i.clearRect(0,0,h.width,h.height),i.fillText(j(55356,57331,65039,8205,55356,57096),0,0),c=h.toDataURL(),i.clearRect(0,0,h.width,h.height),i.fillText(j(55356,57331,55356,57096),0,0),d=h.toDataURL(),c!==d);case"diversity":return i.fillText(j(55356,57221),0,0),e=i.getImageData(16,16,1,1).data,f=e[0]+","+e[1]+","+e[2]+","+e[3],i.fillText(j(55356,57221,55356,57343),0,0),e=i.getImageData(16,16,1,1).data,g=e[0]+","+e[1]+","+e[2]+","+e[3],f!==g;case"simple":return i.fillText(j(55357,56835),0,0),0!==i.getImageData(16,16,1,1).data[0];case"unicode8":return i.fillText(j(55356,57135),0,0),0!==i.getImageData(16,16,1,1).data[0];case"unicode9":return i.fillText(j(55358,56631),0,0),0!==i.getImageData(16,16,1,1).data[0]}return!1}function e(a){var c=b.createElement("script");c.src=a,c.type="text/javascript",b.getElementsByTagName("head")[0].appendChild(c)}var f,g,h,i;for(i=Array("simple","flag","unicode8","diversity","unicode9"),c.supports={everything:!0,everythingExceptFlag:!0},h=0;h<i.length;h++)c.supports[i[h]]=d(i[h]),c.supports.everything=c.supports.everything&&c.supports[i[h]],"flag"!==i[h]&&(c.supports.everythingExceptFlag=c.supports.everythingExceptFlag&&c.supports[i[h]]);c.supports.everythingExceptFlag=c.supports.everythingExceptFlag&&!c.supports.flag,c.DOMReady=!1,c.readyCallback=function(){c.DOMReady=!0},c.supports.everything||(g=function(){c.readyCallback()},b.addEventListener?(b.addEventListener("DOMContentLoaded",g,!1),a.addEventListener("load",g,!1)):(a.attachEvent("onload",g),b.attachEvent("onreadystatechange",function(){"complete"===b.readyState&&c.readyCallback()})),f=c.source||{},f.concatemoji?e(f.concatemoji):f.wpemoji&&f.twemoji&&(e(f.twemoji),e(f.wpemoji)))}(window,document,window._wpemojiSettings);
		</script>
		<style type="text/css">
img.wp-smiley,
img.emoji {
	display: inline !important;
	border: none !important;
	box-shadow: none !important;
	height: 1em !important;
	width: 1em !important;
	margin: 0 .07em !important;
	vertical-align: -0.1em !important;
	background: none !important;
	padding: 0 !important;
}
</style>
<link rel='stylesheet' id='mtq_CoreStyleSheets-css'  href='https://www.geeksforgeeks.org/wp-content/plugins/mtouch-quiz/mtq_core_style.min.css' type='text/css' media='all' />
<link rel='stylesheet' id='mtq_ThemeStyleSheets-css'  href='https://www.geeksforgeeks.org/wp-content/plugins/mtouch-quiz/mtq_theme_style.min.css' type='text/css' media='all' />
<link rel='stylesheet' id='wp-quicklatex-format-css'  href='https://www.geeksforgeeks.org/wp-content/plugins/wp-quicklatex/css/quicklatex-format.css' type='text/css' media='all' />
<link rel='stylesheet' id='themonic-fonts-css'  href='https://fonts.googleapis.com/css?family=Ubuntu:400,700&#038;subset=latin,latin-ext' type='text/css' media='all' />
<link rel='stylesheet' id='custom-style-css'  href='https://www.geeksforgeeks.org/wp-content/themes/iconic-one/css/gfg-1.7.css' type='text/css' media='all' />
<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-includes/js/jquery/jquery.js'></script>
<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-includes/js/jquery/jquery-migrate.min.js'></script>
<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-content/themes/iconic-one/js/gfg-7.0.js'></script>
<link rel='https://api.w.org/' href='https://www.geeksforgeeks.org/wp-json/' />
<link rel="EditURI" type="application/rsd+xml" title="RSD" href="https://www.cdn.geeksforgeeks.org/xmlrpc.php?rsd" />
<link rel="wlwmanifest" type="application/wlwmanifest+xml" href="https://www.geeksforgeeks.org/wp-includes/wlwmanifest.xml" /> 
<meta name="generator" content="WordPress 4.6.9" />
<link rel='shortlink' href='https://www.geeksforgeeks.org/?p=136904' />
<link rel="alternate" type="application/json+oembed" href="https://www.geeksforgeeks.org/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.geeksforgeeks.org%2Fscanner-class-in-java%2F" />
<link rel="alternate" type="text/xml+oembed" href="https://www.geeksforgeeks.org/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.geeksforgeeks.org%2Fscanner-class-in-java%2F&#038;format=xml" />
<style>
#wpadminbar{
background: #ff0000 !important;
}
</style>
<style type="text/css" id="custom-background-css">
body.custom-background { background-color: #ffffff; }
</style>
<style type="text/css" id="syntaxhighlighteranchor"></style>
<link rel="icon" href="https://www.geeksforgeeks.org/wp-content/uploads/gfg_200X200-100x100.png" sizes="32x32" />
<link rel="icon" href="https://www.geeksforgeeks.org/wp-content/uploads/gfg_200X200.png" sizes="192x192" />
<link rel="apple-touch-icon-precomposed" href="https://www.geeksforgeeks.org/wp-content/uploads/gfg_200X200.png" />
<meta name="msapplication-TileImage" content="https://www.geeksforgeeks.org/wp-content/uploads/gfg_200X200.png" />

<script type='text/javascript'>
  var googletag = googletag || {};
  googletag.cmd = googletag.cmd || [];
  (function() {
    var gads = document.createElement('script');
    gads.async = true;
    gads.type = 'text/javascript';
    var useSSL = 'https:' == document.location.protocol;
    gads.src = (useSSL ? 'https:' : 'http:') +
      '//www.googletagservices.com/tag/js/gpt.js';
    var node = document.getElementsByTagName('script')[0];
    node.parentNode.insertBefore(gads, node);
  })();
</script>

<script type='text/javascript'>
  googletag.cmd.push(function() {
    googletag.defineSlot('/27823234/SP', [300, 250], 'div-gpt-ad-1458112424022-0').addService(googletag.pubads());
    googletag.pubads().enableSingleRequest();
    googletag.enableServices();
  });
</script>
</head>

<body class="single single-post postid-136904 single-format-standard custom-background custom-background-white custom-font-enabled">

<!-- BuySellAds Ad Code -->
<script type="text/javascript">
(function(){
  var bsa = document.createElement('script');
     bsa.type = 'text/javascript';
     bsa.async = true;
     bsa.src = '//s3.buysellads.com/ac/bsa.js';
  (document.getElementsByTagName('head')[0]||document.getElementsByTagName('body')[0]).appendChild(bsa);
})();
</script>
<!-- End BuySellAds Ad Code -->

<div id="page" style="position:relative;" class="hfeed site">
	<header id="masthead" class="site-header" role="banner">
		<div style="margin-bottom: 5px;">	
				<hgroup class="main_gfg_title">
			<a href="https://www.geeksforgeeks.org/" title="GeeksforGeeks" rel="home">GeeksforGeeks</a>
				<br .../> <a class="site-description">A computer science portal for geeks</a>
		</hgroup>
		<span class="responsive-custom-search">
<script>
  (function() {
    var cx = '009682134359037907028:tj6eafkv_be';
    var gcse = document.createElement('script');
    gcse.type = 'text/javascript';
    gcse.async = true;
    gcse.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') +
        '//cse.google.com/cse.js?cx=' + cx;
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(gcse, s);
  })();
</script>
		
		<gcse:search></gcse:search>  
		</span>

<div class="top-button-div">
<hgroup style="float:right;display:inline-block;margin-top:5px;">   


<a class="products" href="https://practice.geeksforgeeks.org/">Practice</a>

<a class="products" href="http://quiz.geeksforgeeks.org/gate-corner-2/">GATE CS</a>

<a class="products" href="http://quiz.geeksforgeeks.org/placements/">Placements</a>

<a class="products" href="https://www.youtube.com/geeksforgeeksvideos/">Videos</a>

<a class="products" href="https://www.geeksforgeeks.org/contribute/">Contribute</a>
</hgroup><br></br>


<div id="profile" style="float: right; margin-top: -1%;margin-right:1%;"></div>
</div>
</div>

		
		
		<nav id="site-navigation" class="themonic-nav" role="navigation">
			<a class="assistive-text" href="#content" title="Skip to content">Skip to content</a>
			<div class="menu-iconic-container"><ul id="menu-top" class="nav-menu"><li id="menu-item-147519" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147519"><a href="/"><img style="width: 30px;vertical-align: middle;" src="https://www.geeksforgeeks.org/wp-content/uploads/gfg_transparent_white_small.png"></a></li>
<li id="menu-item-141975" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-141975"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/">Algo ▼</a>
<ul class="sub-menu">
	<li id="menu-item-135030" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135030"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/#AnalysisofAlgorithms">Analysis of Algorithms</a></li>
	<li id="menu-item-146823" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146823"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/">Topicwise ►</a>
	<ul class="sub-menu">
		<li id="menu-item-147774" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147774"><a href="http://www.geeksforgeeks.org/searching-algorithms/">Searching Algorithms</a></li>
		<li id="menu-item-147773" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147773"><a href="http://www.geeksforgeeks.org/sorting-algorithms/">Sorting Algorithms</a></li>
		<li id="menu-item-135041" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135041"><a href="http://www.geeksforgeeks.org/graph-data-structure-and-algorithms/">Graph Algorithms</a></li>
		<li id="menu-item-135040" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135040"><a href="http://www.geeksforgeeks.org/bitwise-algorithms/">Bit Algorithms</a></li>
		<li id="menu-item-135034" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135034"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/#PatternSearching">Pattern Searching</a></li>
		<li id="menu-item-135038" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135038"><a href="http://www.geeksforgeeks.org/geometric-algorithms/">Geometric Algorithms</a></li>
		<li id="menu-item-135039" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135039"><a href="http://www.geeksforgeeks.org/mathematical-algorithms/">Mathematical Algorithms</a></li>
		<li id="menu-item-135042" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135042"><a href="http://www.geeksforgeeks.org/randomized-algorithms/">Randomized Algorithms</a></li>
		<li id="menu-item-156520" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-156520"><a href="http://www.geeksforgeeks.org/category/algorithm/game-theory/">Game Theory</a></li>
	</ul>
</li>
	<li id="menu-item-146824" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146824"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/">Algorithm Paradigms ►</a>
	<ul class="sub-menu">
		<li id="menu-item-135032" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135032"><a href="http://www.geeksforgeeks.org/greedy-algorithms/">Greedy Algorithms</a></li>
		<li id="menu-item-135033" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135033"><a href="http://www.geeksforgeeks.org/dynamic-programming/">Dynamic Programming</a></li>
		<li id="menu-item-135037" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135037"><a href="http://www.geeksforgeeks.org/divide-and-conquer/">Divide and Conquer</a></li>
		<li id="menu-item-135036" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135036"><a href="http://www.geeksforgeeks.org/backtracking-algorithms/">Backtracking</a></li>
		<li id="menu-item-137933" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137933"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/#BranchandBound">Branch &#038; Bound</a></li>
	</ul>
</li>
	<li id="menu-item-146911" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146911"><a href="http://www.geeksforgeeks.org/fundamentals-of-algorithms/">All Algorithms</a></li>
</ul>
</li>
<li id="menu-item-142016" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-142016"><a href="http://www.geeksforgeeks.org/data-structures/">DS  ▼</a>
<ul class="sub-menu">
	<li id="menu-item-135054" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135054"><a href="http://www.geeksforgeeks.org/array-data-structure/">Array</a></li>
	<li id="menu-item-135045" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135045"><a href="http://www.geeksforgeeks.org/data-structures/linked-list/">LinkedList</a></li>
	<li id="menu-item-135046" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135046"><a href="http://www.geeksforgeeks.org/stack-data-structure/">Stack</a></li>
	<li id="menu-item-135047" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135047"><a href="http://www.geeksforgeeks.org/queue-data-structure/">Queue</a></li>
	<li id="menu-item-146827" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146827"><a href="http://www.geeksforgeeks.org/data-structures/">Tree based DS ►</a>
	<ul class="sub-menu">
		<li id="menu-item-135048" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135048"><a href="http://www.geeksforgeeks.org/binary-tree-data-structure/">Binary Tree</a></li>
		<li id="menu-item-135049" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135049"><a href="http://www.geeksforgeeks.org/binary-search-tree-data-structure/">Binary Search Tree</a></li>
		<li id="menu-item-135050" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135050"><a href="http://www.geeksforgeeks.org/heap-data-structure/">Heap</a></li>
	</ul>
</li>
	<li id="menu-item-135051" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135051"><a href="http://www.geeksforgeeks.org/hashing-data-structure/">Hashing</a></li>
	<li id="menu-item-135052" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135052"><a href="http://www.geeksforgeeks.org/graph-data-structure-and-algorithms/">Graph</a></li>
	<li id="menu-item-135053" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135053"><a href="http://www.geeksforgeeks.org/advanced-data-structures/">Advanced Data Structure</a></li>
	<li id="menu-item-135055" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135055"><a href="http://www.geeksforgeeks.org/matrix/">Matrix</a></li>
	<li id="menu-item-147716" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147716"><a href="http://www.geeksforgeeks.org/string-data-structure/">Strings</a></li>
	<li id="menu-item-135056" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135056"><a href="http://www.geeksforgeeks.org/data-structures/">All Data Structures</a></li>
</ul>
</li>
<li id="menu-item-147478" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-147478"><a href="http://www.geeksforgeeks.org/category/program-output/">Languages ▼</a>
<ul class="sub-menu">
	<li id="menu-item-135006" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-135006"><a href="https://www.geeksforgeeks.org/c/">C</a></li>
	<li id="menu-item-135007" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-135007"><a href="https://www.geeksforgeeks.org/c-plus-plus/">C++</a></li>
	<li id="menu-item-135012" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-135012"><a href="https://www.geeksforgeeks.org/java/">Java</a></li>
	<li id="menu-item-137004" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-137004"><a href="https://www.geeksforgeeks.org/python/">Python</a></li>
	<li id="menu-item-135016" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-135016"><a href="http://www.geeksforgeeks.org/sql-tutorial/">SQL</a></li>
	<li id="menu-item-140854" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-140854"><a title="http://www.geeksforgeeks.org/category/program-output/" href="https://www.geeksforgeeks.org/category/program-output/">Program Output</a></li>
</ul>
</li>
<li id="menu-item-142017" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-142017"><a href="http://www.geeksforgeeks.org/about/interview-corner/">Interview  ▼</a>
<ul class="sub-menu">
	<li id="menu-item-141326" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-141326"><a href="https://www.geeksforgeeks.org/company-preparation/">Company Prep</a></li>
	<li id="menu-item-137171" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137171"><a href="http://www.geeksforgeeks.org/interview-preparation-for-software-developer/">Top Topics</a></li>
	<li id="menu-item-137172" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137172"><a href="https://practice.geeksforgeeks.org/company-tags">Practice Company Questions</a></li>
	<li id="menu-item-137173" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137173"><a href="http://www.geeksforgeeks.org/about/interview-corner/">Interview Experiences</a></li>
	<li id="menu-item-137174" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137174"><a href="http://www.geeksforgeeks.org/category/interview-experiences/experienced-interview-experiences/">Experienced Interviews</a></li>
	<li id="menu-item-137175" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137175"><a href="http://www.geeksforgeeks.org/category/interview-experiences/internship-interview-experiences/">Internship Interviews</a></li>
	<li id="menu-item-137176" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137176"><a href="http://www.geeksforgeeks.org/category/competitive-programming/">Competitive Programming</a></li>
	<li id="menu-item-147581" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147581"><a href="http://www.geeksforgeeks.org/software-design-patterns/">Design Patterns</a></li>
	<li id="menu-item-137186" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137186"><a href="http://geeksquiz.com/quiz-corner/">Multiple Choice Quizzes</a></li>
</ul>
</li>
<li id="menu-item-137178" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-137178"><a href="http://www.geeksforgeeks.org/student-corner/">Students  ▼</a>
<ul class="sub-menu">
	<li id="menu-item-137183" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137183"><a href="http://www.geeksforgeeks.org/campus-ambassador-program-by-geeksforgeeks/">Campus Ambassador Program</a></li>
	<li id="menu-item-137179" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137179"><a href="http://www.geeksforgeeks.org/geek-of-the-month/">Geek of the Month</a></li>
	<li id="menu-item-137570" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137570"><a href="http://geeksquiz.com/placements/">Placement Course</a></li>
	<li id="menu-item-136004" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-136004"><a href="https://www.geeksforgeeks.org/category/project/">Project</a></li>
	<li id="menu-item-137180" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137180"><a href="http://www.geeksforgeeks.org/category/competitive-programming/">Competitive Programming</a></li>
	<li id="menu-item-137181" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137181"><a href="http://www.geeksforgeeks.org/testimonials/">Testimonials</a></li>
	<li id="menu-item-138863" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-138863"><a href="http://www.geeksforgeeks.org/category/geek-on-the-top/">Geek on the Top</a></li>
	<li id="menu-item-141974" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-141974"><a href="http://www.geeksforgeeks.org/careers/">Careers</a></li>
	<li id="menu-item-137378" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-137378"><a href="http://www.geeksforgeeks.org/internship/">Internship</a></li>
	<li id="menu-item-147457" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147457"><a href="http://www.geeksforgeeks.org/school-programming/">School Programming</a></li>
</ul>
</li>
<li id="menu-item-146712" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146712"><a href="http://www.geeksforgeeks.org/gate-corner-2-gq/">GATE ▼</a>
<ul class="sub-menu">
	<li id="menu-item-146713" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146713"><a href="http://www.geeksforgeeks.org/gate-corner-2-gq/">GATE CS Corner</a></li>
	<li id="menu-item-146714" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146714"><a href="http://www.geeksforgeeks.org/gate-cs-notes-gq/">GATE Notes</a></li>
	<li id="menu-item-146715" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146715"><a href="http://www.geeksforgeeks.org/lmns-gq/">Last Minute Notes</a></li>
	<li id="menu-item-146716" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146716"><a href="http://www.geeksforgeeks.org/original-gate-previous-year-question-papers-cse-and-it-gq/">Official Papers</a></li>
	<li id="menu-item-146717" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146717"><a href="http://www.geeksforgeeks.org/gate-cs-2018-important-dates/">Gate 2018 Important Dates and Links</a></li>
</ul>
</li>
<li id="menu-item-146718" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146718"><a href="http://www.geeksforgeeks.org/articles-on-computer-science-subjects-gq/">CS Subjects ▼</a>
<ul class="sub-menu">
	<li id="menu-item-146729" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146729"><a href="http://www.geeksforgeeks.org/operating-systems/">Operating Systems</a></li>
	<li id="menu-item-146724" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146724"><a href="http://www.geeksforgeeks.org/dbms/">DBMS</a></li>
	<li id="menu-item-146721" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146721"><a href="http://www.geeksforgeeks.org/computer-network-tutorials/">Computer Networks</a></li>
	<li id="menu-item-146720" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146720"><a href="http://www.geeksforgeeks.org/compiler-design-tutorials/">Compiler Design</a></li>
	<li id="menu-item-147831" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147831"><a href="http://www.geeksforgeeks.org/web-technology/">Web Technology</a></li>
	<li id="menu-item-146722" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146722"><a href="http://www.geeksforgeeks.org/computer-organization-and-architecture-tutorials/">Computer Organization &#038; Architecture</a></li>
	<li id="menu-item-146726" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146726"><a href="http://www.geeksforgeeks.org/digital-electronics-logic-design-tutorials/">Digital Electronics</a></li>
	<li id="menu-item-146727" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146727"><a href="http://www.geeksforgeeks.org/engineering-mathematics-tutorials/">Engg. Mathematics</a></li>
	<li id="menu-item-146730" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146730"><a href="http://www.geeksforgeeks.org/theory-of-computation-automata-tutorials/">Theory of Computation</a></li>
	<li id="menu-item-147512" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-147512"><a href="http://www.geeksforgeeks.org/advanced-computer-subjects-tutorials/">Advanced Topics</a></li>
	<li id="menu-item-146725" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146725"><a href="http://www.geeksforgeeks.org/category/geeksquiz/articles-gq/difference-gq/">What&#8217;s Difference?</a></li>
</ul>
</li>
<li id="menu-item-140855" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-140855"><a href="http://quiz.geeksforgeeks.org/quiz-corner/">Quizzes ▼</a>
<ul class="sub-menu">
	<li id="menu-item-146748" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146748"><a href="http://www.geeksforgeeks.org/quizzes-on-programming-languages-gq/">Languages ►</a>
	<ul class="sub-menu">
		<li id="menu-item-146743" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146743"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#C%20Programming%20Mock%20Tests">C</a></li>
		<li id="menu-item-146745" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146745"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#C++%20Programming%20Mock%20Tests">C++</a></li>
		<li id="menu-item-146746" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146746"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Java%20Programming%20Mock%20Tests">Java</a></li>
		<li id="menu-item-146747" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146747"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Python%20Programming%20Mock%20Tests">Python</a></li>
	</ul>
</li>
	<li id="menu-item-146825" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-has-children menu-item-146825"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Data%20Structures%20Mock%20Tests">CS Subjectwise ►</a>
	<ul class="sub-menu">
		<li id="menu-item-146731" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146731"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Data%20Structures%20Mock%20Tests">Data Structures</a></li>
		<li id="menu-item-146732" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146732"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Algorithms%20Mock%20Tests">Algorithms</a></li>
		<li id="menu-item-146733" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146733"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Operating%20Systems%20Mock%20Tests">Operating Systems</a></li>
		<li id="menu-item-146734" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146734"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#DBMS%20Mock%20Tests">DBMS</a></li>
		<li id="menu-item-146735" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146735"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Compiler%20Design%20Mock%20Tests">Compiler Design</a></li>
		<li id="menu-item-146736" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146736"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Computer%20Networks%20Mock%20Tests">Computer Networks</a></li>
		<li id="menu-item-146737" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146737"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Theory%20of%20Computation%20Mock%20Tests">Theory of Computation</a></li>
		<li id="menu-item-146738" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146738"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Computer%20Organization%20and%20Architecture">Computer Organization</a></li>
		<li id="menu-item-146739" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146739"><a href="http://www.geeksforgeeks.org/software-engineering-gq/">Software Engineering</a></li>
	</ul>
</li>
	<li id="menu-item-146740" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146740"><a href="http://www.geeksforgeeks.org/html-and-xml-gq/">HTML &#038; XML</a></li>
	<li id="menu-item-146741" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146741"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Engineering%20Mathematics">Engg. Mathematics</a></li>
	<li id="menu-item-146742" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-146742"><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Aptitude%20Mock%20Tests">Aptitude</a></li>
</ul>
</li>
<li id="menu-item-135367" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-135367"><a href="https://www.geeksforgeeks.org/category/guestblogs/">GBlog</a></li>
<li id="menu-item-141885" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-141885"><a href="http://www.geeksforgeeks.org/puzzles/">Puzzles</a></li>
<li id="menu-item-141816" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-141816"><a href="https://www.geeksforgeeks.org/gate-cs-2018-mock-tests/">What&#8217;s New?</a></li>
</ul></div>		</nav><!-- #site-navigation -->
		<div class="clear"></div>
	</header><!-- #masthead -->
<button id="scrollTopBtn" title="Scroll to Top" type="button" class="btn btn-success">&#x25B2;</button>
	<div id="main" class="wrapper">
<div class="leftSideBarParent">
    <div class="leftSideBar">
        <div class="menuDivForLeftbar"><div class="bar1"></div><div class="bar2"></div><div class="bar3"></div></div><span class="leftbarDataSpan" data-pid="136904" data-lid="7" data-type="post" data-termid="2058"></span><div class="quickLink_S" data-termid="-30" >
<div class="quickLink-header_S">Quick Links for Java


</div>

<table>
<tbody>
<tr>
<td><a href="http://www.geeksforgeeks.org/category/java/">Recent Articles</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/quiz-corner-gq/#Java%20Programming%20Mock%20Tests">MCQ / Quizzes</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java/#Collection%20in%20Java">Java Collections</a></td>
</tr>
<tr>
<td><a href="https://practice.geeksforgeeks.org/topics/Java/?ref=home">Practice Problems</a></td>
</tr>
<tr>
<td>Commonly Asked Questions <a href="http://www.geeksforgeeks.org/commonly-asked-java-programming-interview-questions-set-1/">Set 1</a> & <a href="http://www.geeksforgeeks.org/commonly-asked-java-programming-interview-questions-set-2/">Set 2</a></td>
</tr>
</tbody>
</table>


</div>

<br><br>


<div class="quickLink_S">
<table>
<tbody>

<tr>
<td class="quickLink-header_S"><b>Basics</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/java-identifiers/">Identifiers</a>, <a href="http://www.geeksforgeeks.org/data-types-in-java/">Data types</a> & <a href="http://www.geeksforgeeks.org/variables-in-java/">Variables</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/variable-scope-in-java/">Scope of Variables</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/operators-in-java/">Operators</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/loops-in-java/">Loops</a> and <a href="http://www.geeksforgeeks.org/decision-making-javaif-else-switch-break-continue-jump/">Decision Making</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-basics/">Explore More...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Input / Output</td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/ways-to-read-input-from-console-in-java/">Ways to read Input from Console</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/difference-between-scanner-and-bufferreader-class-in-java/"> Scanner VS BufferReader Class</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/formatted-output-in-java/">Formatted output</a></td>
<tr>
<td><a href="http://www.geeksforgeeks.org/fast-io-in-java-in-competitive-programming/">Fast I/O in Java in Competitive Programming</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/command-line-arguments-in-java/">Command Line arguments</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-io/">Explore More...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Arrays</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/g-fact-65/">Arrays in Java</a></td> 
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/default-array-values-in-java/">Default array values in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/compare-two-arrays-java/">Compare two arrays</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/final-arrays-in-java/">Final Arrays</a> & <a href="http://www.geeksforgeeks.org/jagged-array-in-java/">Jagged Arrays</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/understanding-array-indexoutofbounds-exception-in-java/">Array IndexOutofbounds Exception</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-arrays/">Explore More...</a></td>
</tr>


<tr>
<td class="quickLink-header_S"><b>Strings</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/string-class-in-java/">String Class in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/stringbuffer-class-in-java/">StringBuffer </a>, <a href="http://www.geeksforgeeks.org/stringtokenizer-class-java-example-set-1-constructors/">StringTokenizer</a> & <a href="http://www.geeksforgeeks.org/java-util-stringjoiner-java8/">StringJoiner</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/how-to-initialize-and-compare-strings-in-java/">Initialize and Compare Strings</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/g-fact-27-string-vs-stringbuilder-vs-stringbuffer/">String vs StringBuilder vs StringBuffer</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/different-ways-for-integer-to-string-conversions-in-java/">Integer to String</a> & <a href="http://www.geeksforgeeks.org/string-to-integer-in-java-parseint/">String to Integer</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/searching-for-character-and-substring-in-a-string/">Search</a>, <a href="http://www.geeksforgeeks.org/reverse-a-string-in-java-5-different-ways/">Reverse</a> and <a href="http://www.geeksforgeeks.org/split-string-java-examples/">Split()</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-strings/">Explore More...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>OOP in Java</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/classes-objects-java/">Classes and Objects in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/different-ways-create-objects-java/">Different ways to create objects</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/access-modifiers-java/">Access Modifiers in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/object-class-in-java/">Object class in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/encapsulation-in-java/">Encapsulation</a> & <a href="http://www.geeksforgeeks.org/inheritance-in-java/">Inheritance</a></td>

<tr>
<td><a href="http://www.geeksforgeeks.org/overloading-in-java/">Method Overloading</a> & <a href="http://www.geeksforgeeks.org/overriding-in-java/">Overriding</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-class-and-object/">Explore More...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Constructors</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/constructors-in-java/">Constructors</a> & <a href="http://www.geeksforgeeks.org/constructor-chaining-java-examples/">Constructor Chaining</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/constructor-overloading-java/">Constructor Overloading</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/private-constructors-and-singleton-classes-in-java/">Private Constructors and Singleton Classes</a></td>
</tr>
<tr>
<td><a href="http://www.cdn.geeksforgeeks.org/tag/java-constructors/">Explore More...</a></td>
</tr>


<tr>
<td class="quickLink-header_S"><b>Methods</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/g-fact-45/">Parameter Passing</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/returning-multiple-values-in-java/">Returning Multiple Values</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/private-and-final-methods-in-java/">Private and Final Methods</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/default-methods-java/">Default Methods</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java/#Methods%20in%20Java">Explore More...</a></td>
</tr>



<tr>
<td class="quickLink-header_S"><b>Exception Handling</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/exceptions-in-java/">Exceptions</a> & <a href="http://www.geeksforgeeks.org/types-of-exception-in-java-with-examples/">Types of Exceptions</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/flow-control-in-try-catch-finally-in-java/">Flow control in try-catch</a> & <a href="http://www.geeksforgeeks.org/multicatch-in-java/">Multicatch</a</td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/throw-throws-java/">throw and throws</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-exception-handling/">Explore More...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Multithreading</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/multithreading-in-java/">Multithreading</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/lifecycle-and-states-of-a-thread-in-java/">Lifecycle and States of a Thread</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/main-thread-java/">Main Thread</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/synchronized-in-java/">Synchronization</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/inter-thread-communication-java/">Inter-thread Communication</a> & <a href="http://www.geeksforgeeks.org/java-concurrency-yield-sleep-and-join-methods/">Java Concurrency</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-multithreading/">Explore More...</a></td>
</tr>



<tr>
<td class="quickLink-header_S"><b>File Handling</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/file-class-in-java/">File Class</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/file-permissions-java/">File Permissions</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/different-ways-reading-text-file-java/">Different ways of Reading a text file</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/delete-file-using-java/">Delete a File</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java/#File%20Handling">Explore more...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Garbage Collection</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/garbage-collection-java/">Garbage Collection</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/mark-and-sweep-garbage-collection-algorithm/">Mark and Sweep</a></td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/java/#Garbage%20Collection">Explore more...</a></td>
</tr>

<tr>
<td class="quickLink-header_S"><b>Java Packages</td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/packages-in-java/">Packages</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java-io-packag/">Java.io Package</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java-lang-package-java/">Java.lang package</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/java-util-package-java/">Java.util Package</a></td>
</tr>


<tr>
<td class="quickLink-header_S"><b>Networking</td>
</tr>

<tr>
<td><a href="http://www.geeksforgeeks.org/socket-programming-in-java/">Socket Programming</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/url-class-java-examples/">URL class in Java</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/reading-url-using-urlconnection-class/">Reading from a URL</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/networking-class-in-java/">Inet Address Class</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/a-group-chat-application-in-java/">A Group Chat Application</a></td>
</tr>
<tr>
<td><a href="http://www.geeksforgeeks.org/tag/java-networking/">Explore more...</a></td>
</tr>

</tbody>
</table>
</div>

    </div>
</div>
	<div id="primary" class="site-content">
		<div id="content" role="main">
                        							 	<article id="post-136904" class="post-136904 post type-post status-publish format-standard hentry category-java category-school-programming tag-java-io">
				<header class="entry-header">
						<h1 class="entry-title">Scanner Class in Java</h1>
				
							<div class="divclass"> 
					<a href="https://www.geeksforgeeks.org/basic/" title="Basic"><span class="articleRating alignright level-1">1.6</span></a>
					</div>
								</header><!-- .entry-header -->

				<div class="entry-content">
			<p style="text-align: justify;">Scanner is a class in java.util package used for obtaining the input of the primitive types like int, double etc. and strings. It is the easiest way to read input in a Java program, though not very efficient if you want an input method for scenarios where time is a constraint like in competitive programming.</p>
<ul>
<li style="text-align: justify;">To create an object of Scanner class, we usually pass the predefined object System.in, which represents the standard input stream. We may pass an object of class File if we want to read input from a file.</li>
<li style="text-align: justify;">To read numerical values of a certain data type XYZ, the function to use is nextXYZ(). For example, to read a value of type short, we can use nextShort()</li>
<li style="text-align: justify;">To read strings, we use nextLine().</li>
<li style="text-align: justify;">To read a single character, we use next().charAt(0). next() function returns the next token/word in the input as a string and charAt(0) funtion returns the first character in that string.</li>
</ul>
<p>Let us look at the code snippet to read data of various data types.</p>
<pre class="brush: java; title: ; notranslate" title="">
// Java program to read data of various types using Scanner class.
import java.util.Scanner;
public class ScannerDemo1
{
    public static void main(String[] args)
    {
        // Declare the object and initialize with
        // predefined standard input object
        Scanner sc = new Scanner(System.in);

        // String input
        String name = sc.nextLine();

        // Character input
        char gender = sc.next().charAt(0);

        // Numerical data input
        // byte, short and float can be read
        // using similar-named functions.
        int age = sc.nextInt();
        long mobileNo = sc.nextLong();
        double cgpa = sc.nextDouble();

        // Print the values to check if input was correctly obtained.
        System.out.println(&quot;Name: &quot;+name);
        System.out.println(&quot;Gender: &quot;+gender);
        System.out.println(&quot;Age: &quot;+age);
        System.out.println(&quot;Mobile Number: &quot;+mobileNo);
        System.out.println(&quot;CGPA: &quot;+cgpa);
    }
}
</pre>
<p>Input :</p>
<pre class="gb wf">Geek
F
40
9876543210
9.9
</pre>
<p>Output :</p>
<pre class="gb wf">Name: Geek
Gender: F
Age: 40
Mobile Number: 9876543210
CGPA: 9.9</pre>
<p style="text-align: justify;">Sometimes, we have to check if the next value we read is of a certain type or if the input has ended (EOF marker encountered).</p>
<p style="text-align: justify;">Then, we check if the scanner&#8217;s input is of the type we want with the help of hasNextXYZ() functions where XYZ is the type we are interested in. The function returns true if the scanner has a token of that type, otherwise false. For example, in the above code, we have used hasNextInt().To check for a string, we use hasNextLine(). Similarly, to check for a single character, we use hasNext().charAt(0).</p>
<p>Let us look at the code snippet to read some numbers from console and print their mean.</p>
<pre class="brush: java; highlight: [17]; title: ; notranslate" title="">
// Java program to read some values using Scanner
// class and print their mean.
import java.util.Scanner;

public class ScannerDemo2
{
    public static void main(String[] args)
    {
        // Declare an object and initialize with
        // predefined standard input object
        Scanner sc = new Scanner(System.in);

        // Initialize sum and count of input elements
        int sum = 0, count = 0;

        // Check if an int value is available
        while (sc.hasNextInt())
        {
            // Read an int value
            int num = sc.nextInt();
            sum += num;
            count++;
        }
        int mean = sum / count;
        System.out.println(&quot;Mean: &quot; + mean);
    }
}
</pre>
<p>Input:</p>
<pre class="gb wf">101
223
238
892
99
500
728
</pre>
<p>Output:</p>
<pre class="gb wf">Mean: 397</pre>
<p>This article is contributed by <strong>Sukrit Bhatnagar</strong>. If you like GeeksforGeeks and would like to contribute, you can also write an article and mail your article to contribute@geeksforgeeks.org. See your article appearing on the GeeksforGeeks main page and help other Geeks.</p>
<p>Please write comments if you find anything incorrect, or you want to share more information about the topic discussed above</p>

			 <div class="AdsParent" style="width:100%;">
<span class="rectangleAd">
<!--
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
 Big Rectangle Blog Bottom 
<ins class="adsbygoogle"
     style="display:inline-block;width:336px;height:280px"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="4061219431"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
-->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- GfGDownLeftNew -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="5794942435"
     data-ad-format="auto"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
</span>
<span class="responsiveAd">
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- newMobile2 -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="1950485631"
     data-ad-format="auto"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
</span>
</div>
<h1><strong><a href="http://quiz.geeksforgeeks.org/gate-corner-2/">GATE CS Corner</a>
&nbsp;&nbsp;&nbsp;<a href="https://practice.geeksforgeeks.org/company-tags">Company Wise Coding Practice</a></strong></h1>

		</div><!-- .entry-content -->
				
		

		<footer class="entry-meta">
		<span><div class="categoryButton"><a href="https://www.geeksforgeeks.org/category/programming-language/java/" rel="category tag">Java</a></div><div class="categoryButton"><a href="https://www.geeksforgeeks.org/category/school-programming/" rel="category tag">School Programming</a></div></span> <span><div class="tagButton"><a href="https://www.geeksforgeeks.org/tag/java-io/" rel="tag">Java-I/O</a></div></span>
           	<div id="improveArticle" style="float: right;cursor: pointer;"></div><div class="common-bottom">Please write to us at contribute@geeksforgeeks.org to report any issue with the above content.</div>          	
					</footer><!-- .entry-meta -->
	</article><!-- #post -->


<div style="font-size:15px; line-height:22px; margin-left:20px; color:green">

<h2 style='font-size:20px; color: #838383'>Recommended Posts:</h2><br/><ul><li><a href='https://www.geeksforgeeks.org/ways-to-read-input-from-console-in-java/'>Ways to read input from console in Java</a></li><li><a href='https://www.geeksforgeeks.org/gfact-51-java-scanner-nextchar/'>Scanner and nextChar() in Java</a></li><li><a href='https://www.geeksforgeeks.org/difference-between-scanner-and-bufferreader-class-in-java/'>Difference between  Scanner and BufferReader Class in Java</a></li><li><a href='https://www.geeksforgeeks.org/arrays-in-java/'>Arrays in Java</a></li><li><a href='https://www.geeksforgeeks.org/fast-io-in-java-in-competitive-programming/'>Fast I/O in Java in Competitive Programming</a></li><li><a href='https://www.geeksforgeeks.org/java-helperclass/'>Java | How to create your own Helper Class?</a></li><li><a href='https://www.geeksforgeeks.org/writing-clean-else-statements/'>Writing clean if else statements</a></li><li><a href='https://www.geeksforgeeks.org/size-of-file-on-the-internet-using-java/'>Size of file on the Internet using Java</a></li><li><a href='https://www.geeksforgeeks.org/java-class-file/'>Java Class File</a></li><li><a href='https://www.geeksforgeeks.org/classnotfoundexception-vs-noclassdeffounderror-java/'>ClassNotFoundException Vs NoClassDefFoundError in Java</a></li></ul><br/></div>


<!-- Added on 29 Oct 2015 for next and previous from same category -->
<nav class="nav-single">
					<div class="assistive-text">Post navigation</div>
					<span class="nav-previous"><a href="https://www.geeksforgeeks.org/python-set-4-dictionary-keywords-python/" rel="prev"><< Previous Post</a></span>
					<span class="nav-next"><a href="https://www.geeksforgeeks.org/python-list-comprehension-and-slicing/" rel="next">Next Post >></a></span>
				</nav><!-- .nav-single -->
<!--
<script type="text/javascript">
	
				arrPost.push('');
	
		   <?php// } ?>

</script>
-->



<div class="plugins">
<div pid="136904" ptitle="Scanner Class in Java" id="ratePlugin"><div class="login">
            (<a href="https://auth.geeksforgeeks.org/?to=https://www.geeksforgeeks.org/scanner-class-in-java/">Login</a> to Rate)
            <br><br>
            </div>
            <div class="techno">
            <span id="rating_box" class="avg-rating level-1">1.6</span>
            <span class="rating-desc"> Average Difficulty : <b id="diff-rating">1.6/5.0</b><br><span id="vote_count">Based on <b>46</b> vote(s)</span></span><br/><br/>
        <input rating="1" type="button" class="box basic"  value="Basic"/>
        <input rating="2" type="button" class="box easy"   value="Easy"/>
        <input rating="3" type="button" class="box medium" value="Medium"/>
        <input rating="4" type="button" class="box hard"   value="Hard"/>
        <input rating="5" type="button" class="box expert" value="Expert"/>
        <br><span class="process"></span></div></div><div pid="136904" ptitle="Scanner Class in Java" id="markPlugin"><br><br><div class="lists">
        <input id="todo" type="checkbox" class="mark">
        <label class="checkbox" for="todo"> Add to TODO List </label>
        <br>
        <input id="done" type="checkbox" class="mark">
        <label class="checkbox" for="done"> Mark as DONE </label>
        </div></div></div>
<div id="author" name="Sandeep Jain"></div>
<br></br>

<style type="text/css">
 
#share-buttons img {
width: 35px;
padding: 5px;
border: 0;
box-shadow: 0;
display: inline;
}
#share-buttons a:hover {
	text-decoration: none;
}
</style>


<div id="share-buttons" style="display:none">
   
    <!-- Facebook -->
    <a href="http://www.facebook.com/sharer.php?u=https://www.geeksforgeeks.org/scanner-class-in-java/" target="_blank" title="Share on Facebook">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/facebook.png" alt="Facebook" />
    </a>
    
    <!-- Google+ -->
    <a href="https://plus.google.com/share?url=https://www.geeksforgeeks.org/scanner-class-in-java/" target="_blank" title="Share on Google">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/google.png" alt="Google" />
    </a>
    
    <!-- LinkedIn -->
    <a href="http://www.linkedin.com/shareArticle?mini=true&amp;url=https://www.geeksforgeeks.org/scanner-class-in-java/" target="_blank" title="Share on LinkedIn">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/linkedin.png" alt="LinkedIn" />
    </a>
    
    <!-- Twitter -->
    <a href="https://twitter.com/share?url=https://www.geeksforgeeks.org/scanner-class-in-java/&amp;text=Scanner Class in Java&amp;hashtags=GeeksforGeeks" target="_blank" title="Share on Twitter">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/twitter.png" alt="Twitter" />
    </a>

    <!-- Pinterest -->
    <a href="javascript:void((function()%7Bvar%20e=document.createElement('script');e.setAttribute('type','text/javascript');e.setAttribute('charset','UTF-8');e.setAttribute('src','http://assets.pinterest.com/js/pinmarklet.js?r='+Math.random()*99999999);document.body.appendChild(e)%7D)());" title="Share on Pinterest">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/pinterest.png" alt="Pinterest" />
    </a>
    
    <!-- Reddit -->
    <a href="http://reddit.com/submit?url=https://www.geeksforgeeks.org/scanner-class-in-java/&amp;title=Scanner Class in Java" target="_blank" title="Share on Reddit">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/reddit.png" alt="Reddit" />
    </a>
    
    <!-- StumbleUpon-->
    <a href="http://www.stumbleupon.com/submit?url=https://www.geeksforgeeks.org/scanner-class-in-java/&amp;title=Scanner Class in Java" target="_blank" title="Share on StumbleUpon">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/stumbleupon.png" alt="StumbleUpon" />
    </a>
    
    <!-- Tumblr-->
    <a href="http://www.tumblr.com/share/link?url=https://www.geeksforgeeks.org/scanner-class-in-java/&amp;title=Scanner Class in Java" target="_blank" title="Share on Tumblr">
        <img src="https://www.geeksforgeeks.org/wp-content/uploads/tumblr.png" alt="Tumblr" />
    </a>
   
</div>

<br></br>
<div id="ide_link">
<p>Writing code in comment? Please use <a href="https://ide.geeksforgeeks.org/">ide.geeksforgeeks.org</a>, generate link and share the link here.</a></p>
</div>
<br/>
<div style="display:flex">
<button id="comment" class="action-button" style="width:45%;cursor: pointer;margin-right:10%;box-shadow: 0 2px 5px 0 rgba(0,0,0,0.4), 0 6px 20px 0 rgba(0,0,0,0);border-color: #4cb96b;border-radius: 4px;">Load Comments</button>
<button id="share" class="action-button" onclick="document.getElementById('share-buttons').style.display='block';this.style.display='none';" style="width:45%;cursor: pointer;margin-right:10%;box-shadow: 0 2px 5px 0 rgba(0,0,0,0.4), 0 6px 20px 0 rgba(0,0,0,0);border-color: #4cb96b;border-radius: 4px;">Share this post!</button>

</div>

<div id="disqus_thread"></div>

					</div><!-- #content -->
	</div><!-- #primary -->


			<div id="secondary" class="widget-area" role="complementary">
			<aside id="text-2" class="widget widget_text">			<div class="textwidget"><script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- Big 300x600 Sidebar -->
<ins class="adsbygoogle"
     style="display:inline-block;width:300px;height:600px"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="4402736037"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script></div>
		</aside><aside id="text-3" class="widget widget_text">			<div class="textwidget"><div class="trendings_gfg">
					<table width="100%" align="center">
						<thead>
							<tr>
								<th style="border:1px solid #6AA84F;background-color:#4CB96B;color:#fff;text-align: center;font-size: 16px;">Trending Content</th>
							</tr>
						</thead>
						<tbody>

<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">


							<a href="http://www.geeksforgeeks.org/longest-common-subsequence/">Longest Common Subsequence</a>

						</td>
					</tr>			
												<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">


							<a href="http://www.geeksforgeeks.org/breadth-first-traversal-for-a-graph/">Breadth First Traversal or BFS</a>

						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">

							<a href="http://www.geeksforgeeks.org/school-programming/">School Programming</a>

						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/longest-repeated-subsequence/">Longest Repeated Subsequence</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/dynamic-programming-set-12-longest-palindromic-subsequence/">Longest Palindromic Subsequence</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/detect-negative-cycle-graph-bellman-ford/">Detect a negative cycle in a Graph | (Bellman Ford)</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/knapsack-problem/">0-1 Knapsack Problem</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/gate-cs-notes-gq/">GATE CS Notes</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/depth-first-traversal-for-a-graph/">Depth First Traversal or DFS for a Graph</a>
						</td>
					</tr>					<tr>
						<td style="border:1px solid #6AA84F;padding:2px;">
							<a href="http://www.geeksforgeeks.org/reverse-a-linked-list/">Reverse a linked list</a>

						</td>
					</tr>
						</tbody>
					</table>
				</div></div>
		</aside><aside id="text-4" class="widget widget_text">			<div class="textwidget"><script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- ResponsiveRightBarMay16 -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="7089558833"
     data-ad-format="auto"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script></div>
		</aside><aside id="text-5" class="widget widget_text">			<div class="textwidget"><table align="center" width="100%">
    <thead>
        <tr>
            <th style="border:1px solid #6AA84F;background-color:#4CB96B;color:#fff;text-align: center;font-size: 16px;line-height:1.7;">
                Most Visited Posts
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/top-algorithms-and-data-structures-for-competitive-programming/">Top 10 Algorithms and Data Structures for Competitive Programming</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/top-10-algorithms-in-interview-questions/">Top 10 algorithms in Interview Questions</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/how-to-begin-with-competitive-programming/">How to begin with Competitive Programming?</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/a-complete-step-by-step-guide-for-placement-preparation-by-geeksforgeeks/">Step by Step Guide for Placement Preparation</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/how-to-prepare-for-acm-icpc/">How to prepare for ACM-ICPC?</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://quiz.geeksforgeeks.org/insertion-sort/">Insertion Sort</a>,
                <a href="http://geeksquiz.com/binary-search/">Binary Search</a>,
                <a href="http://geeksquiz.com/quick-sort/">QuickSort</a>,
                <a href="http://geeksquiz.com/merge-sort/">MergeSort</a>,
                <a href="http://geeksquiz.com/heap-sort/">HeapSort</a>
            </td>
        </tr>
    </tbody>
</table></div>
		</aside><aside id="text-7" class="widget widget_text">			<div class="textwidget"><script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- GfGSideBottomResponsive -->
<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-9465609616171866"
     data-ad-slot="5749413230"
     data-ad-format="auto"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script></div>
		</aside><aside id="text-6" class="widget widget_text">			<div class="textwidget"><table align="center" width="100%">
    <thead>
        <tr>
            <th style="border:1px solid #6AA84F;background-color:#4CB96B;color:#fff;text-align: center;font-size: 16px;line-height:1.7;">
                Popular Categories
            </th>
        </tr>
    </thead>
    <tbody>

        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/interview-experiences/">Interview Experiences</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/advanced-data-structures/">Advanced Data Structures</a>
            </td>
        </tr>

        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/dynamic-programming/">Dynamic Programming</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/greedy/">Greedy Algorithms</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/backtracking/">Backtracking</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/pattern-searching/">Pattern Searching</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/divide-and-conquer/">Divide &amp; Conquer</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/algorithm/geometric/">Geometric Algorithms</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/searching/">Searching</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/sorting/">Sorting</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/algorithm/analysis/">Analysis of Algorithms</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/algorithm/mathematical/">Mathematical Algorithms</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/algorithm/randomized/">Randomized Algorithms</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/tag/recursion">Recursion</a>
            </td>
        </tr>
        <tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">
                <a href="http://www.geeksforgeeks.org/category/algorithm/game-theory/">Game Theory</a>
            </td>
<tr>
            <td style="border:1px solid #6AA84F;padding:2px;line-height:1.7;font-size:13px;">							<a href="http://www.geeksforgeeks.org/tag/statistical-algorithms/">Statistical Algorithms</a>            </td>

        </tr>

    </tbody>
</table></div>
		</aside><aside id="text-8" class="widget widget_text">			<div class="textwidget"><!-- BuySellAds Zone Code -->
<div id="bsap_1306934" class="bsarocks bsap_785bf45b162de1c5511e8baa02854e5c"></div>
<!-- End BuySellAds Zone Code --></div>
		</aside><aside id="tag_cloud-3" class="widget widget_tag_cloud"><p class="widget-title">Tags</p><div class="tagcloud"><a href='https://www.geeksforgeeks.org/category/advanced-data-structure/' class='tag-link-1762 tag-link-position-1' title='168 topics' style='font-size: 9.5806451612903pt;'>Advanced Data Structure</a>
<a href='https://www.geeksforgeeks.org/tag/amazon/' class='tag-link-1942 tag-link-position-2' title='477 topics' style='font-size: 14.661290322581pt;'>Amazon</a>
<a href='https://www.geeksforgeeks.org/tag/aptitude/' class='tag-link-2159 tag-link-position-3' title='288 topics' style='font-size: 12.177419354839pt;'>Aptitude</a>
<a href='https://www.geeksforgeeks.org/category/quizzes-gq/aptitude-gq/' class='tag-link-2200 tag-link-position-4' title='283 topics' style='font-size: 12.064516129032pt;'>Aptitude</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/c-arrays/' class='tag-link-3 tag-link-position-5' title='710 topics' style='font-size: 16.58064516129pt;'>Arrays</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/bit-magic/' class='tag-link-17 tag-link-position-6' title='239 topics' style='font-size: 11.274193548387pt;'>Bit Magic</a>
<a href='https://www.geeksforgeeks.org/category/programming-language/c/' class='tag-link-2064 tag-link-position-7' title='621 topics' style='font-size: 15.903225806452pt;'>C</a>
<a href='https://www.geeksforgeeks.org/tag/c/' class='tag-link-2138 tag-link-position-8' title='397 topics' style='font-size: 13.758064516129pt;'>C</a>
<a href='https://www.geeksforgeeks.org/category/programming-language/cpp/' class='tag-link-2065 tag-link-position-9' title='791 topics' style='font-size: 17.145161290323pt;'>C++</a>
<a href='https://www.geeksforgeeks.org/category/quizzes-gq/computer-science-quizzes-gq/cpp-gq/' class='tag-link-2207 tag-link-position-10' title='130 topics' style='font-size: 8.3387096774194pt;'>C++ Quiz</a>
<a href='https://www.geeksforgeeks.org/category/computer-subject/computer-networks/' class='tag-link-2051 tag-link-position-11' title='121 topics' style='font-size: 8pt;'>Computer Networks</a>
<a href='https://www.geeksforgeeks.org/tag/cpp-library/' class='tag-link-1964 tag-link-position-12' title='152 topics' style='font-size: 9.0161290322581pt;'>CPP-Library</a>
<a href='https://www.geeksforgeeks.org/category/quizzes-gq/computer-science-quizzes-gq/c-gq/' class='tag-link-2206 tag-link-position-13' title='275 topics' style='font-size: 11.951612903226pt;'>C Quiz</a>
<a href='https://www.geeksforgeeks.org/tag/data-structures/' class='tag-link-2142 tag-link-position-14' title='129 topics' style='font-size: 8.2258064516129pt;'>Data Structures</a>
<a href='https://www.geeksforgeeks.org/category/quizzes-gq/computer-science-quizzes-gq/data-structures-gate-gq/' class='tag-link-2213 tag-link-position-15' title='131 topics' style='font-size: 8.3387096774194pt;'>Data Structures</a>
<a href='https://www.geeksforgeeks.org/category/computer-subject/dbms/' class='tag-link-2053 tag-link-position-16' title='121 topics' style='font-size: 8pt;'>DBMS</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/dynamic-programming/' class='tag-link-1746 tag-link-position-17' title='309 topics' style='font-size: 12.516129032258pt;'>Dynamic Programming</a>
<a href='https://www.geeksforgeeks.org/category/interview-experiences/experienced-interview-experiences/' class='tag-link-1795 tag-link-position-18' title='140 topics' style='font-size: 8.6774193548387pt;'>Experienced</a>
<a href='https://www.geeksforgeeks.org/category/guestblogs/' class='tag-link-1710 tag-link-position-19' title='301 topics' style='font-size: 12.403225806452pt;'>GBlog</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/geometric/' class='tag-link-1754 tag-link-position-20' title='138 topics' style='font-size: 8.5645161290323pt;'>Geometric</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/graph/' class='tag-link-2068 tag-link-position-21' title='197 topics' style='font-size: 10.370967741935pt;'>Graph</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/hash/' class='tag-link-1756 tag-link-position-22' title='171 topics' style='font-size: 9.6935483870968pt;'>Hash</a>
<a href='https://www.geeksforgeeks.org/category/interview-experiences/internship-interview-experiences/' class='tag-link-1794 tag-link-position-23' title='183 topics' style='font-size: 9.9193548387097pt;'>Internship</a>
<a href='https://www.geeksforgeeks.org/category/interview-experiences/' class='tag-link-1140 tag-link-position-24' title='2,139 topics' style='font-size: 22pt;'>Interview Experiences</a>
<a href='https://www.geeksforgeeks.org/category/programming-language/java/' class='tag-link-2058 tag-link-position-25' title='741 topics' style='font-size: 16.806451612903pt;'>Java</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/linked-list/' class='tag-link-8 tag-link-position-26' title='207 topics' style='font-size: 10.596774193548pt;'>Linked Lists</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/mathematical/' class='tag-link-1753 tag-link-position-27' title='927 topics' style='font-size: 17.935483870968pt;'>Mathematical</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/matrix/' class='tag-link-1760 tag-link-position-28' title='248 topics' style='font-size: 11.5pt;'>Matrix</a>
<a href='https://www.geeksforgeeks.org/tag/microsoft/' class='tag-link-104 tag-link-position-29' title='195 topics' style='font-size: 10.258064516129pt;'>Microsoft</a>
<a href='https://www.geeksforgeeks.org/tag/number-digits/' class='tag-link-1911 tag-link-position-30' title='147 topics' style='font-size: 8.9032258064516pt;'>number-digits</a>
<a href='https://www.geeksforgeeks.org/category/program-output/' class='tag-link-5 tag-link-position-31' title='195 topics' style='font-size: 10.258064516129pt;'>Program Output</a>
<a href='https://www.geeksforgeeks.org/category/project/' class='tag-link-1767 tag-link-position-32' title='129 topics' style='font-size: 8.2258064516129pt;'>Project</a>
<a href='https://www.geeksforgeeks.org/category/puzzles/' class='tag-link-2063 tag-link-position-33' title='177 topics' style='font-size: 9.8064516129032pt;'>Puzzles</a>
<a href='https://www.geeksforgeeks.org/category/programming-language/python/' class='tag-link-1789 tag-link-position-34' title='760 topics' style='font-size: 16.91935483871pt;'>Python</a>
<a href='https://www.geeksforgeeks.org/category/quizzes-gq/qa-placement-quizzes-gq/' class='tag-link-2204 tag-link-position-35' title='274 topics' style='font-size: 11.951612903226pt;'>QA - Placement Quizzes</a>
<a href='https://www.geeksforgeeks.org/tag/qa-placement-quizzes/' class='tag-link-2187 tag-link-position-36' title='274 topics' style='font-size: 11.951612903226pt;'>QA - Placement Quizzes</a>
<a href='https://www.geeksforgeeks.org/category/school-programming/' class='tag-link-2078 tag-link-position-37' title='461 topics' style='font-size: 14.435483870968pt;'>School Programming</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/searching/' class='tag-link-1751 tag-link-position-38' title='155 topics' style='font-size: 9.1290322580645pt;'>Searching</a>
<a href='https://www.geeksforgeeks.org/tag/series/' class='tag-link-1919 tag-link-position-39' title='174 topics' style='font-size: 9.6935483870968pt;'>series</a>
<a href='https://www.geeksforgeeks.org/category/algorithm/sorting/' class='tag-link-1752 tag-link-position-40' title='282 topics' style='font-size: 12.064516129032pt;'>Sorting</a>
<a href='https://www.geeksforgeeks.org/tag/stl/' class='tag-link-1797 tag-link-position-41' title='333 topics' style='font-size: 12.854838709677pt;'>STL</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/c-strings/' class='tag-link-7 tag-link-position-42' title='566 topics' style='font-size: 15.451612903226pt;'>Strings</a>
<a href='https://www.geeksforgeeks.org/category/technical-scripter/' class='tag-link-1788 tag-link-position-43' title='200 topics' style='font-size: 10.370967741935pt;'>Technical Scripter</a>
<a href='https://www.geeksforgeeks.org/category/data-structures/tree/' class='tag-link-19 tag-link-position-44' title='319 topics' style='font-size: 12.741935483871pt;'>Trees</a>
<a href='https://www.geeksforgeeks.org/category/web-technologies/' class='tag-link-2628 tag-link-position-45' title='203 topics' style='font-size: 10.483870967742pt;'>Web Technologies</a></div>
</aside><aside id="text-9" class="widget widget_text">			<div class="textwidget"><!-- BuySellAds Zone Code -->
<div id="bsap_1304848" class="bsarocks bsap_785bf45b162de1c5511e8baa02854e5c"></div>
<!-- End BuySellAds Zone Code --></div>
		</aside><aside id="text-10" class="widget widget_text">			<div class="textwidget"><a href="http://www.geeksforgeeks.org/recent-comments/" style="margin-right: 0px !important;">
  <center>
    <input type="button" value="Recent Comments" style="background-color: #4cb96b; color:white; width:100%; font-size:large; cursor:pointer;font-weight:bold;">
  </center>
</a></div>
		</aside>		</div><!-- #secondary -->
		</div><!-- #main .wrapper -->
	<footer id="colophon" role="contentinfo" style="padding:0; ">
		<div class="site-info">
		<div class="clear"></div>
		</div><!-- .site-info -->
		</footer><!-- #colophon -->
<center>
  <div class="iconic-footer" style="min-height:40px;font-size:14px;padding-bottom: 0px;line-height: 1.5;">
    @geeksforgeeks, 
    <a href="http://creativecommons.org/licenses/by-nc-nd/2.5/in/deed.en_US" title="Valid XHTML Strict 1.0">Some rights reserved</a><a href="https://www.geeksforgeeks.org/about/contact-us/"> &nbsp; &nbsp; &nbsp; &nbsp;Contact Us!</a>
    <a href="https://www.geeksforgeeks.org/about/"> &nbsp; &nbsp; &nbsp; &nbsp;About Us!&nbsp; &nbsp; &nbsp;</a>
    <a href="https://www.geeksforgeeks.org/careers/"> &nbsp; &nbsp; &nbsp;Careers!&nbsp; &nbsp; </a>
    <a href="https://www.geeksforgeeks.org/privacy-policy/">&nbsp; &nbsp; &nbsp; Privacy Policy&nbsp; &nbsp;&nbsp; </a>
    <!-- adding social buttons on 07 April, 2017 -->
    <a href="https://www.facebook.com/GeeksforGeeks-316764689022/timeline/" style="display: inline-block;margin-left: 10px;border:1px solid #fff;border-radius: 2px;" title="facebook">
      <img src="https://www.geeksforgeeks.org/wp-content/uploads/square_facebook_green.png" style="width:30px;vertical-align: middle;" />
    </a>
    <a href="https://twitter.com/geeksforgeeks" style="display: inline-block;margin-left: 10px;border:1px solid #fff;border-radius: 2px;" title="twitter">
      <img src="https://www.geeksforgeeks.org/wp-content/uploads/square_twitter_green.png" style="width:30px;vertical-align: middle;" />
    </a>
    <a href="https://www.linkedin.com/company-beta/1299009" style="display: inline-block;margin-left: 10px;border:1px solid #fff;border-radius: 2px;" title="linkedin">
      <img src="https://www.geeksforgeeks.org/wp-content/uploads/square_linkedin_green.png" style="width:30px;vertical-align: middle;" />
    </a>
    <a href="https://play.google.com/store/apps/details?id=free.programming.programming" style="display: inline-block;margin-left: 10px;border:1px solid #fff;border-radius: 2px;" title="play store">
      <img src="https://www.geeksforgeeks.org/wp-content/uploads/square_play_store_green.png" style="width:30px;vertical-align: middle;" />
    </a>
    <a href="https://www.microsoft.com/en-us/store/apps/geeksforgeeks-official/9nblggh4rh30" style="display: inline-block;margin-left: 10px;border:1px solid #fff;border-radius: 2px;" title="windows store">
      <img src="https://www.geeksforgeeks.org/wp-content/uploads/square_windows_store_green.png" style="width:30px;vertical-align: middle;" />
    </a>
  </div>
</center><!-- .site-info -->

				<div class="clear"></div>
</div><!-- #page -->

<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-content/plugins/syntaxhighlighter/syntaxhighlighter3/scripts/shCore-1.1.js'></script>
<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-content/plugins/syntaxhighlighter/syntaxhighlighter3/scripts/shBrushJava.js'></script>
<script type='text/javascript'>
	(function(){
		var corecss = document.createElement('link');
		var themecss = document.createElement('link');
		var corecssurl = "https://www.geeksforgeeks.org/wp-content/plugins/syntaxhighlighter/syntaxhighlighter3/styles/shCore.css?ver=3.0.9b";
		if ( corecss.setAttribute ) {
				corecss.setAttribute( "rel", "stylesheet" );
				corecss.setAttribute( "type", "text/css" );
				corecss.setAttribute( "href", corecssurl );
		} else {
				corecss.rel = "stylesheet";
				corecss.href = corecssurl;
		}
		document.getElementsByTagName("head")[0].insertBefore( corecss, document.getElementById("syntaxhighlighteranchor") );
		var themecssurl = "https://www.geeksforgeeks.org/wp-content/plugins/syntaxhighlighter/syntaxhighlighter3/styles/shThemeDefault.css?ver=3.0.9b";
		if ( themecss.setAttribute ) {
				themecss.setAttribute( "rel", "stylesheet" );
				themecss.setAttribute( "type", "text/css" );
				themecss.setAttribute( "href", themecssurl );
		} else {
				themecss.rel = "stylesheet";
				themecss.href = themecssurl;
		}
		//document.getElementById("syntaxhighlighteranchor").appendChild(themecss);
		document.getElementsByTagName("head")[0].insertBefore( themecss, document.getElementById("syntaxhighlighteranchor") );
	})();
	SyntaxHighlighter.config.strings.expandSource = '+ expand source';
	SyntaxHighlighter.config.strings.help = '?';
	SyntaxHighlighter.config.strings.alert = 'SyntaxHighlighter\n\n';
	SyntaxHighlighter.config.strings.noBrush = 'Can\'t find brush for: ';
	SyntaxHighlighter.config.strings.brushNotHtmlScript = 'Brush wasn\'t configured for html-script option: ';
	SyntaxHighlighter.defaults['gutter'] = false;
	SyntaxHighlighter.defaults['pad-line-numbers'] = true;
	SyntaxHighlighter.defaults['toolbar'] = false;
	SyntaxHighlighter.all();
</script>
<script type='text/javascript' src='https://www.geeksforgeeks.org/wp-includes/js/wp-embed.min.js'></script>

<style>
.eventLink{
border: 1px solid #868686;
background-color: #e0e0e0;
padding: 10px;
box-shadow: none;
display: block;
text-align: center;
color: #555 !important;
font-size: 14px;
font-weight: bold;
}
</style>

<script type="text/javascript">
// below changes to be added in gfg.js in future.
// load comment button click when page scroll to it and positioned ad in mobile view.
flag=0;jQuery(window).scroll(function(){if(jQuery('#comment').length !=0 ){var hT=jQuery('#comment').offset().top,hH=jQuery('#comment').outerHeight(),wH=jQuery(window).height(),wS=jQuery(this).scrollTop();if(wS>(hT+hH-wH-70)&&!flag){jQuery('#comment').click();flag=1}}});var temp_width=jQuery(window).width();if(temp_width<468){if(jQuery('article').length>1){jQuery(jQuery('.responsiveAd')).insertAfter('article:eq(2)');jQuery('.rectangleAd').hide()}
else if(jQuery('#practiceLinkDiv').length>0){jQuery(jQuery('.responsiveAd')).insertAfter('#practiceLinkDiv');jQuery('.rectangleAd').css('width','')}else{jQuery('.responsiveAd').hide();jQuery('.rectangleAd').css('width','')}}


  var _gaq = _gaq || [];
  _gaq.push(['_setAccount', 'UA-12148232-1']);
  _gaq.push(['_trackPageview']);

  (function() {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
  })();

</script>  
<script async type="text/javascript" src="//cdn.fancybar.net/ac/fancybar.js?zoneid=1502&serve=C6ADVKE&placement=geeksforgeeks" id="_fancybar_js"></script>
</body>
</html>

<!-- Dynamic page generated in 0.227 seconds. -->
<!-- Cached page generated by WP-Super-Cache on 2018-02-12 12:27:51 -->

<!-- Compression = gzip -->