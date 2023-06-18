<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teste</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            font-size: 24px;
            background-image: url('https://bit.ly/coraçãopng');
            background-size: cover;
        }

        h1 {
            font-size: 40px;
            color: white;
            text-shadow: 2px 2px 4px #000;
        }

        .mensagem {
            color: white;
            text-shadow: 2px 2px 4px #000;
            font-weight: bold;
            margin-top: 20px;
            font-size: 28px;
        }

        #sim {
            background-color: green;
            color: white;
            font-size: 20px;
            padding: 10px 20px;
            font-weight: bold;
        }

        #nao {
            background-color: red;
            color: white;
            font-size: 20px;
            padding: 10px 20px;
            font-weight: bold;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const mensagemElement = document.getElementById("mensagem");

            function exibirMensagem(mensagem) {
                mensagemElement.textContent = mensagem;
            }

            document.getElementById("sim").addEventListener("click", function() {
                exibirMensagem("Isso é maravilhoso! Eu estou tão feliz!");
            });

            document.getElementById("nao").addEventListener("click", function() {
                exibirMensagem("Oh, eu entendo... Talvez em outra oportunidade.");
            });
        });
    </script>
</head>
<body>
    <h1>Teste?</h1>
    <div>
        <button id="sim">Sim</button>
        <button id="nao">Não</button>
    </div>
    <p id="mensagem" class="mensagem"></p>
</body>
</html>
