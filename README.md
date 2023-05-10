<!DOCTYPE html>
<html>
<head>
	<title>Random Quote Generator</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
	<h1>Random Quote Generator</h1>
	<p>Click the button to generate a random quote:</p>
	<button onclick="generateQuote()">Generate</button>
	<p id="result"></p>

	<script>
		function generateQuote() {
			var quotes = [
				"The greatest glory in living lies not in never falling, but in rising every time we fall. -Nelson Mandela",
				"The way to get started is to quit talking and begin doing. -Walt Disney",
				"If life were predictable it would cease to be life, and be without flavor. -Eleanor Roosevelt",
				"If you look at what you have in life, you'll always have more. If you look at what you don't have in life, you'll never have enough. -Oprah Winfrey",
				"If you set your goals ridiculously high and it's a failure, you will fail above everyone else's success. -James Cameron"
			];
			var quote = quotes[Math.floor(Math.random() * quotes.length)];
			document.getElementById("result").innerHTML = quote;
		}
	</script>
</body>
</html>
