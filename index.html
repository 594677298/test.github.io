
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>DbMusic Search</title>
<link href="http://cdn.static.runoob.com/libs/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<link href="http://www.zhangxinxu.com/jq/pagination_zh/lib/pagination.css" rel="stylesheet">
<style>
html, body, div, input, p, a, img, h1, h2, h3, h4, h5, h6 {
	padding: 0;
	margin: 0;
}
.clearfix:befor, .clearfix:after {
 content: " ",  display:table;
}
.clearfix:after {
	clear: both;
}
.clearfix {
 *zoom:1;
}
.search_main {
	min-height: 100%;
	width: 70%;
	margin-left: auto;
	margin-right: auto;
	padding-top: 30px;
	padding-bottom: 20px;
	position: relative;
}
.search_main h1 {
	text-align: center;
}
.search_input {
	margin-top: 20px;
	width: 70%;
	height: 30px;
	margin-left: auto;
	margin-right: auto;
}
.search_input input, .search_input button {
	height: 100%;
}
.search_input input {
	width: 70%;
}
.search_input button {
	width: 28%;
	color: #fff;
	font-size: 15px;
	letter-spacing: 1px;
	background: #3385ff;
	border: none;
	border-bottom: 1px solid #2d78f4;
	outline: medium;
	cursor: pointer;
	-webkit-appearance: none;
	-webkit-border-radius: 0;
}
.search_input button:hover {
	background: #317ef3;
	border-bottom: 1px solid #2868c8;
}
.totle {
	width: 70%;
	margin: 0 auto;
	margin-top: 10px;
	margin-bottom: 10px;
}
.img, .content {
	float: left;
}
.content {
	padding-left: 10px;
}
.table {
	margin-top: 10px;
}
#display {
	width: 70%;
	margin: 0 auto;
}
.page {
	width: 50%;
	margin: 0 auto;
	display: none;
}
/*鍔犺浇鍔ㄧ敾鐗规晥*/
.spinner {
	display: none;
	/*visibility: hidden;*/
	width: 80%;
	margin-top: 10px;
	height: 60px;
	text-align: center;
	font-size: 10px;
}
.spinner > div {
	background-color: #67CF22;
	height: 100%;
	width: 6px;
	display: inline-block;
	-webkit-animation: stretchdelay 1.2s infinite ease-in-out;
	animation: stretchdelay 1.2s infinite ease-in-out;
}
.spinner .rect2 {
	-webkit-animation-delay: -1.1s;
	animation-delay: -1.1s;
}
.spinner .rect3 {
	-webkit-animation-delay: -1.0s;
	animation-delay: -1.0s;
}
.spinner .rect4 {
	-webkit-animation-delay: -0.9s;
	animation-delay: -0.9s;
}
.spinner .rect5 {
	-webkit-animation-delay: -0.8s;
	animation-delay: -0.8s;
}
 @-webkit-keyframes stretchdelay {
 0%, 40%, 100% {
-webkit-transform: scaleY(0.4)
}
 20% {
-webkit-transform: scaleY(1.0)
}
}
 @keyframes stretchdelay {
 0%, 40%, 100% {
 transform: scaleY(0.4);
 -webkit-transform: scaleY(0.4);
}
20% {
 transform: scaleY(1.0);
 -webkit-transform: scaleY(1.0);
}
}
</style>
</head>
<body>
<section class="search_main">
  <h1>jsonp解决跨越demo  --音乐数据来自豆瓣api</h1>
  <div class="search_input">
    <input id="keyworlds" type="text" placeholder="搜索歌名，歌手">
    <button id="toSearch">搜索</button>
  </div>
  <div class="spinner">
    <div class="rect1"></div>
    <div class="rect2"></div>
    <div class="rect3"></div>
    <div class="rect4"></div>
    <div class="rect5"></div>
  </div>
  <div class="totle"></div>
  <div id="display" class="clearfix"> </div>
</section>
<div class="page">
  <ul class="pagination">
  </ul>
</div>
<div class="M-box"></div>
<script src="https://apps.bdimg.com/libs/jquery/2.1.4/jquery.min.js">
</script> 
<script src="https://cdn.static.runoob.com/libs/bootstrap/3.3.7/js/bootstrap.min.js"></script> 
<script src="http://www.zhangxinxu.com/jq/pagination_zh/lib/jquery.pagination.js"></script>
<script>
		$(document).ready(function(){
	var musicContent = null;
	var start = 0;
	function musicSearch(){
		var keyworld = $("#keyworlds").val();
		if(keyworld){
			$(".spinner").show();
			$.ajax({
			type:"get",
			async:true,
			url:"https://api.douban.com/v2/music/search?q="+keyworld+"&start="+start+"&count=10",
			dataType:"jsonp",
			jsonp:"callback",
			jsonpCallback:"ms",
			success:function(json){
				//alert(json.musics);
				$(".spinner").hide();
				$("#display").children().remove();
				$(".pagination").children().remove();
				$(".totle").html("共有"+json.total+"条数据，当前第"+(start+1)+"页");
				displayMusic(json.musics);
				pagecount(json.total,start);
				$(".page").show();
				},
			error:function(){
				alert("查询失败");
			}
			})
		}
		else{
			alert("请输入查询内容！");
		}
	};
	//点击查询
	$("#toSearch").click(function(){
		start = 0;
		musicSearch();
	});
	//输入框绑定回车事件ß
	$("#keyworlds").keypress(function(event){
		if(event.keyCode == "13"){
			start = 0;
			musicSearch();
		}
	});
	//焦点获取
	$("#keyworlds").focus();
	//音乐查询结果
	function displayMusic(music){
		for(var i=0;i<10;i++){
			var imgshow = "<div class='img'><img src="+music[i].image+"></div>";
			var title = "<div><a href="+music[i].alt+" title="+music[i].title+" alt="+music[i].alt_title+">"+music[i].title+"</a></div>";
			var ratings = "<div>豆瓣评分:"+music[i].rating.average+"</div>";
			var authors = "<div>"+music[i].attrs.singer+"</div>";
			var content = "<div class='content'>"+title+ratings+authors+"</div>";
			$("<div class='table clearfix'>"+imgshow+content+"</div>").appendTo("#display");
		}
	}

	//分页判断
	function pagecount(pagetotle,curretpage){
		var count=Math.ceil(pagetotle/10);
		curretpage+=1;
		var pages="";
		//分页显示页码判定
		if(curretpage<4){
			for(var i=1;i<7;i++){
				pages+="<li><a href='#'>"+i+"</a></li>";
			}
			
		}
		else if(curretpage>(count-4)){
			for(var i=(count-4);i<count;i++){
				pages+="<li><a href='#'>"+i+"</a></li>";
			}
		}
		else{
			pages="<li><a href='#'>"+(curretpage-3)+"</a></li>"+"<li><a href='#'>"+(curretpage-2)+"</a></li>"+"<li><a href='#'>"+(curretpage-1)+"</a></li>"+"<li><a href='#'>"+curretpage+"</a></li>"+"<li><a href='#'>"+(curretpage+1)+"</a></li>"+"<li><a href='#'>"+(curretpage+2)+"</a></li>";
		}
		$(pages).appendTo(".pagination");
	}
	//分页点击
	$(function(){
		$(".pagination").on("click","li",function(){
			var pagenum = $(this).text();
			start = pagenum - 1;
			musicSearch();
		})
	})
})
		
		
		
if (window.console) {
    var cons = console;
    if (cons) {
        cons.log("%c\n       ", "font-size:41px;background:url('http://www.lagou.com/image1/M00/02/76/Cgo8PFTUaQmANERoAAJOmBSMRyU785.jpg') no-repeat -135px -1px");
        cons.log('想和我们共同打造世界最大中文互动问答平台吗？\n想让自己的成就在亿万用户面前展现吗？想让世界看得你的光芒吗？\n加入我们，在这里不仅是工作，投入你的时间和热情，滴滴汗水终会汇聚成不平凡的成果。\n期待你的加盟。（投简历地址被我砍了）');
        cons.log("请在邮件中注明%c来自:console", "color:red;font-weight:bold;");
    }
}
	</script>
</body>
</html>
