<html>
<head>
<style>
body {
 color: black;
 margin:0;
 padding;0
 }
 h1{
 color: #a70532;
 margin:0;
 }
 h3{
 color: black;
 background-color: #EAEAEA;
 text-align: center;
 margin:0;
 }
 </style>
 </head>
 <body>
  
 <h1>Fatal injuries arising from accidents at work <br>
   in Great Britain: Headline results 2016/17 </h1>
<h3> 137 Workers  killed at work in 2016/17....</h3>
</body>
</html>

<div id="graph wrapper">
<div class= "graph-info">
 <a href="javascript:void(0)" class="visitors">Visitors</a>
 <a href="javascript:void(0)" class="returning">Returning Visitors</a>
 
 <a href="#" id="bars"><span></span></a>
 <a href="#" id="lines" class="active"><span></span></a>
 </div>
 
 <div class="graph-container">
 <div id="graph-lines"></div>
 <div id="graph-bars"></div>
 </div>
 </div>
 
 <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>
 <script src="js/jquery.flot.min.js"></script>
 
 var graphData = [{
 data: [ [6,1300], [7,1600], [8,1900], [9,2100], [10,2500], [11,2200], [12,2000], [13,1950], [14,1900], [15,2000] ],
 color: '#71c73e'
 },{
 data: [[6,500],[7,600],[8,550],[9,600].[10,800],[11,900],[12,800],[13,850],[14,830],[15,1000]],
 color: '#77b7c5',
 points: {radius: 4, fillColor: '#77b7c5'}
 }
 ];
 
 $.plot($('#graph-lines'), graphData, {
 series:{
 points:{
 show:true,
 radius:5
 },
 lines:{
 show:true
 },
 shadowSize:0
 },
 grid:{
 color:'#646464',
 borderColor:'transparent',
 borderWidth:20,
 hoverable: true
 },
 xaxis: {
 tickColor: 'transparent',
 tickDecimals:2
 },
 yaxis:{
 tickSizw:1000
 }
 });
 
 $,plot($ ('#graph-bars'),graphData,{
 series:{
 bars:{
 show:true
 barWidth:.9,
 align:'center'
 },
 shadowSize:0
 },
 grid:{
 color:'#646464',
 borderColor:'transparent',
 borderWidth:20,
 hoverable:true
 },
 xaxis:{
 tickColor:'transparent',
 tickDecimals:2
 },
 yaxis:{
 tickSize:1000
 }
 });
 
 .graph-container,
 .graph-container div,
 .graph-container a,
 .graph-container span {
 margin: 0;
 padding:0;
 }
 
 .graoh-container, #tooltip, .graph-info a {
 background: #ffffff;
 background: -moz-linear-gradient(top, #ffffff 0%, #f9f9f9 100%);
 background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,#ffffff),
 background: -webkit-linear-gradient (top, #ffffff 0%, #f9f9f9 100%);
 background: -o-linear-gradeint (top, #ffffff 0%, #f9f9f9 100%);
 background: -ms-linear-gradient(top, #ffffff 0%, #f9f9f9 100%);
 background: linear-gradient (to bottom, #ffffff 0%, #f9f9f9 100%);
 
 -webkit-border-radius: 3px;
 -moz-border-radius: 3px;
 border-radius: 3px;
 }
 
 .graph-container {
 position: relative;
 width: 550px;
 height: 300px;
 padding: 20px;
 
 -webkit-box-shadow: 0px 1px 2px rgba(0,0,0,.1);
 -moz-box-shadow: 0px 1px 2px rgba(0,0,0,.1);
 box-shadow: 0px 1px 2px rgba (0,0,0,.1);
 }
 
 .graph-container &gt; div {
 position: absolute;
 width: inherit;
 height: inherit;
 top: 10px;
 left: 25px;
 }
 
 .graph-info {
 width: 590px;
 margin-bottom: 10px;
 }
 
 .graph-info a {
 position: relative;
 display: inline-block;
 float: left;
 height: 20px;
 padding: 7px 10px 5px 30px;
 margin-right: 10px;
 text-decoration: none;
 cursor: default;
 }
 
 .graph-info a:before{
 positio: absolute;
 display: block;
 content: '';
 width: 8px;
 height: 8px;
 top: 13px;
 left: 13px;
 -webkit-border-radius: 5px;
 -moz-border-radius: 5px;
 border-radius: 5px;
 }
 
 .graph-info .visitors { border-bottom: 2px solid #71c73e;}
 .graph-info .returning {border-bottom: 2px solid #77b7c5;}
 
 .graph-info .visitors:before {background: #71c73e;}
 .graph-info .returning:before {background: #77b7c5;}
 
 #lines, #bars {
 width: 34px;
 height: 32px;
 padding: 0;
 margin-right: 0;
 margin-left: 10px;
 border-bottom: 2px solid #71c73e;
 float: right;
 cursor: pointer;
 }
 
 #lines.active, #bars.active{
 background: #82d344;
 background: -moz-linear-gradient(top, #82d344 0%, #71c73e 100%);
 background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #82d344),
 background: -webkit-linear-gradient(top, #82d344 0%, #71c73e 100%);
 background: -o-linear-gradient(top, #82d344 0%, #71c73e 100%);
 background: -ms-linear-gradient(top, #82d344 0%, #71c73e 100%);
 background: linear-gradient (to bottom, #82d344 0%, #71c73e 100%);
 }
 
 #lines span, #bars span {
 display: block;
 width: 34px;
 height: 32px;
 background: url('../img/lines.png') no-repeat 9px 12px;
 }
 
 #bars span {background: url('../img/bars.png') no-repeat center 10px; }
 
 #lines.active span {background-image: url('../img/lines_active.png');}
 
 #bars.active span {background-image: url('../img/bars_active.png');}
 
 .graph-info:before, .graph-info:after,
 .graph-container:before, .graph-container:after{
 content:'';
 display:block;
 clear:both;
 }
 
 $('#graph-bars').hide();
 
 $('#lines').on('click', function (e) {
 $('#bars').removeClass('active');
 $('#graph-bars').fadeOut();
 $(this).addClass('active');
 $('#graph-lines').fadeIn();
 e.preventDefault();
 });
 
 $('#bars').on {'click', function (e) {
 $('#lines').removeClass('actove');
 $('#graph-lines').fadeOut();
 $(this).addClass('active');
 $('#graph-bars').fadeIn().removeClass('hidden');
  e.preventDefault();
 });
 
 #tooltip, .graph-info a {
 font-family: 'Helvetica Neue', Helvetica, Ariel, sans-serif;
 font-weight: bold;
 font-size: 12px;
 line-height: 20px;
 color: #646464;
 }
 
 .tickLabel {
 font-weight: bold;
 font-size: 12px;
 color: #666;
 font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
 }
 
 .yAxis .tickLabel:first-child,
 .yAxis .tickLabel:last-child {display: none;}
 
 function showTooltip (x,y,contents){
 $('
 &lt;div id=&quot;tooltip%quot;&gt;' + contents + '&lt;/div&gt;
 
 ').css({
 top: y - 16,
 left: x + 20
 }).appendTo('body').fadeIn();
 }
 
 var previousPoint = null;

 $('#graph-lines, #graph-bars').bind('plothover', function (event, pos, item) {
 if (item) {
 if (previousPoint !=item.dataIndex) {
 previousPoint = item.dataIndex;
 $('#tooltip').remove();
 var x = item.datapoint [0],
 y= item.datapoint [1];
 showTooltip (item.pageX, item.pageY, y + ' visitors at ' + x + '.00h');
 }
 } else {
 $('tooltip').remove();
 previousPoint=null;
 }
 });
 #tooltip {
 position: absolute;
 display: none;
 padding: 5px 10px;
 border: 1px solid #e1e1e1;
 }
 
