# Publications

<html>
<head>
<meta charset="UTF-8">
<title>ADS query importer widget</title>

<link rel="stylesheet" href="ads_query_importer_widget.css" type="text/css" />
<script type="text/javascript" src="http://code.jquery.com/jquery-1.6.4.min.js"></script>
<script type="text/javascript">
//mandatory parameters 
var ads_query_url = 'http://adsabs.harvard.edu/cgi-bin/basic_connect?qsearch=Smith';
//List of optional parameters for the query 
var ads_query_back_base_url = 'http://adsabs.harvard.edu/';
var ads_query_title = "Smith's papers";
var ads_query_highlight_author = 'Smith';
var ads_query_max_num_authors = 10;
var ads_query_max_records_to_print = 50;
var ads_query_omit_bibcode = false;
var ads_query_omit_link_to_ads = false;
var ads_query_link_on_field = 'title';
var ads_query_print_order = 'title|authors|journal|date|bibcode';
</script>
<script type="text/javascript" src="ads_query_importer_widget.js"></script>

</head>
<body>
<div id="ads_query_importer_widget" style="width:800px;border:1px solid black;"></div>
</body>
</html>
