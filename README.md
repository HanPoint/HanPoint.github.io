<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>언제든 사라질 수 있는</title>
    <link rel="stylesheet" href="style.css">
    <script src="script.js"></script>
    <link href="npm/bootstrap%405.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">
    <script src="jquery-latest.min.js"></script>
    <script src="npm/axios/dist/axios.min.js"></script>
</head>
<body>
    <div id="mainblock">
        <div id="title">언제든 사라질 수 있는 실시간 지하철</div>
        <div id="body">
            <select id="selbox" class="form-select">
		<option value="none" disabled="" selected="">노선 선택</option>
        	<option value="1">1호선</option>
                <option value="2">2호선</option>
                <option value="3">3호선</option>
                <option value="4">4호선</option>
                <option value="5">5호선</option>
                <option value="6">6호선</option>
                <option value="7">7호선</option>
                <option value="8">8호선</option>
                <option value="9">9호선</option>
		<option value="KK">경강선</option>
                <option value="G">경춘선</option>
                <option value="SH">서해선</option>
                <option value="A">공항철도</option>
                <option value="SI">신분당선</option>
                <option value="K">경의중앙선</option>
                <option value="SU">수인분당선</option>
                <option value="UI">우이신설선</option>
		<option value="YE">용인 에버라인</option>
		<option value="XA">GTX-A</option>
	    </select>
        </div>
    </div>
    <div id="viewTrain" style="width: calc(100% - 50px); margin: auto;">
    </div>
</body>
</html>
<script>
    $(document).ready(function(){
        $("#selbox").change(function(){
            selectLine(this.value)
        })
    })
</script>
