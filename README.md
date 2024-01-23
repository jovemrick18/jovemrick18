<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Câmera Web</title>
</head>
<body>

<input type="file" accept="image/*,video/*" capture="camera" id="fileInput">
<button onclick="enviarArquivo()">Enviar</button>

<script>
  function enviarArquivo() {
    var fileInput = document.getElementById('fileInput');
    var arquivo = fileInput.files[0];

    if (arquivo) {
      // Aqui você pode implementar a lógica para enviar o arquivo para a dashboard.
      // Por exemplo, você pode usar AJAX para enviar o arquivo para o servidor.
      console.log('Arquivo selecionado:', arquivo);
    } else {
      console.log('Nenhum arquivo selecionado.');
    }
  }
</script>

</body>
</html>
