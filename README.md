# BOTAOZAO

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Botão para Aumentar/Diminuir Fonte</title>
    <style>
        #texto {
            font-size: 16px; /* Tamanho inicial da fonte */
        }
    </style>
</head>
<body>

    <div>
        <button onclick="aumentarFonte()">Aumentar Fonte</button>
        <button onclick="diminuirFonte()">Diminuir Fonte</button>
    </div>

    <p id="texto">Este é um texto de exemplo. Clique nos botões para alterar o tamanho da fonte.</p>

    <script>
        function aumentarFonte() {
            var texto = document.getElementById('texto');
            var tamanhoAtual = parseInt(window.getComputedStyle(texto).fontSize);
            texto.style.fontSize = (tamanhoAtual + 2) + 'px'; // Aumenta a fonte em 2px
        }

        function diminuirFonte() {
            var texto = document.getElementById('texto');
            var tamanhoAtual = parseInt(window.getComputedStyle(texto).fontSize);
            texto.style.fontSize = (tamanhoAtual - 2) + 'px'; // Diminui a fonte em 2px
        }
    </script>

</body>
</html>
