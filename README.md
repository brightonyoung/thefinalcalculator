<html>
<head>
<meta charset="utf-8">
<title>Calculator | Brighton Young</title>
	<link rel="stylesheet" href="style.css">
</head>
 
<body>
	<script>
	function calcNumbers(result){
		form.displayResult.value=form.displayResult.value+result;
			
	}
	</script>
	<div class="container">
		<form name="form">
		<div class="display">
			<input type="text" placeholder="0" name="displayResult">
		</div>
			<div class="buttons">
			  <div class="row">
				<input type="button" name="b7" value="7" onClick="calcNumbers(b7.value)">
				  <input type="button" name="b8" value="8" onClick="calcNumbers(b8.value)">
				  <input type="button" name="b9" value="9" onClick="calcNumbers(b9.value)">
				  <input type="button" name="addb" value="+" onClick="calcNumbers(addb.value)">
				</div>
				
				<div class="row">
				<input type="button" name="b4" value="4" onClick="calcNumbers(b4.value)">
				  <input type="button" name="b5" value="5" onClick="calcNumbers(b5.value)">
				  <input type="button" name="b6" value="6" onClick="calcNumbers(b6.value)">
				  <input type="button" name="subb" value="-" onClick="calcNumbers(subb.value)">
				</div>
				
				<div class="row">
				<input type="button" name="b1" value="1" onClick="calcNumbers(b1.value)">
				  <input type="button" name="b2" value="2" onClick="calcNumbers(b2.value)">
				  <input type="button" name="b3" value="3" onClick="calcNumbers(b3.value)">
				  <input type="button" name="mulb" value="*" onClick="calcNumbers(mulb.value)">
				</div>
				
				<div class="row">
				<input type="button" name="b0" value="0" onClick="calcNumbers(b0.value)">
				  <input type="button" name="potb" value="." onClick="calcNumbers(potb.value)">
				  <input type="button" name="divb" value="/" onClick="calcNumbers(divb.value)">
				  <input type="button" class="red" value="=" onClick="displayResult.value=eval(displayResult.value)">
				</div>
			</div>
		
		</form>
	</div>
	<script type="text/javascript"> == $0
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
	</script>
</body>
	
</html>