# anima-o

<canvas id="tela" width="600" height="400"> </canvas>
<script>
var tela = document.getElementById("tela");
var c = tela.getContext ("2d");


function circulo(x, y, raio) {
	c.fillStyle = "blue";
	c.beginPath();
	c.arc(x, y, raio, 0, 2*Math.PI);
	c.fill();
	
}

function limpaTela() {
	c.clearRect(0, 0, 600, 400);
}   
var x = 1;

function desenha() {
   limpaTela ();
   circulo (x, 100, 100);
  x = x + 1; 
}  
  
setInterval (desenha, 30);
</script>
