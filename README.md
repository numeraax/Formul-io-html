<!doctype html>
<html>

<head>
    <!-- Metadados -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- CSS -->
    <link rel="stylesheet" type="text/css" href="formulario.css" media="screen">
    <style>
        /* Estilo do modo escuro */
        :root {
            --bg-color: #121212; /* Fundo escuro */
            --text-color: #87cefa; /* Azul claro para o texto */
            --field-bg: #1e1e1e; /* Fundo dos campos de entrada */
            --field-text: #ffffff; /* Texto dos campos de entrada */
            --field-border: #87cefa; /* Borda azul claro */
            --button-bg: #6200ea; /* Fundo do botão */
            --button-text: #ffffff; /* Texto do botão */
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            text-align: center;
        }

        .campo input, .campo select, .campo textarea {
            background-color: var(--field-bg);
            color: var(--field-text);
            border: 1px solid var(--field-border);
            padding: 0.5em;
            border-radius: 4px;
            width: 100%;
            max-width: 300px;
            margin: 0.5em auto;
        }

        .grupo {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1em;
        }

        .grupo .campo {
            flex: 1;
            min-width: 150px;
        }

        button {
            background-color: var(--button-bg);
            color: var(--button-text);
            border: none;
            padding: 0.7em 1.5em;
            cursor: pointer;
            border-radius: 4px;
            margin-top: 1em;
        }

        button:hover {
            opacity: 0.9;
        }

        #titulo {
            margin-bottom: 0.5em;
        }

        #subtitulo {
            margin-bottom: 1em;
            font-size: 1.1em;
        }
    </style>

    <!-- Título da página -->
    <title>Cadastro</title>
</head>

<body>

    <!-- Cabeçalho -->
    <div>
        <h1 id="titulo">Cadastro de DEVs</h1>
        <p id="subtitulo">Complete suas informações</p>
    </div>

    <!-- Formulário -->
    <form>
        <fieldset class="grupo">
            <div class="campo">
                <label for="nome"><strong>Nome</strong></label>
                <input type="text" name="nome" id="nome" required>
            </div>

            <div class="campo">
                <label for="sobrenome"><strong>Sobrenome</strong></label>
                <input type="text" name="sobrenome" id="sobrenome" required>
            </div>
        </fieldset>

        <div class="campo">
            <label for="email"><strong>Email</strong></label>
            <input type="email" name="email" id="email" required>
        </div>

        <div class="campo campo-radio">
            <label><strong>De qual lado da aplicação você desenvolve?</strong></label>
            <label>
                <input type="radio" name="devweb" value="frontend" checked> Front-end
            </label>
            <label>
                <input type="radio" name="devweb" value="backend"> Back-end
            </label>
            <label>
                <input type="radio" name="devweb" value="fullstack"> Fullstack
            </label>
        </div>
    
        

        <div class="campo">
            <label for="senioridade"><strong>Senioridade</strong></label>
            <select id="senioridade" required>
                <option selected disabled value="">Selecione</option>
                <option>Júnior</option>
                <option>Pleno</option>
                <option>Sênior</option>
            </select>
        </div>

        <fieldset class="grupo">
            <div id="check">
                <label><strong>Selecione as tecnologias que utiliza:</strong></label><br><br>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label for="tecnologia1"> HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia2" value="CSS">
                <label for="tecnologia2"> CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="JavaScript">
                <label for="tecnologia3"> JavaScript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="PHP">
                <label for="tecnologia4"> PHP</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia5" value="C#">
                <label for="tecnologia5"> C#</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia6" value="Python">
                <label for="tecnologia6"> Python</label>
                <input type="checkbox" id="tecnologia7" name="tecnologia7" value="Java">
                <label for="tecnologia7"> Java</label>
            </div>
        </fieldset>

        <div class="campo">
            <br>
            <label for="experiencia"><strong>Conte um pouco mais da sua experiência: </strong></label>
            <textarea rows="6" id="experiencia" name="experiencia"></textarea>
        </div>

        <button class="botao" type="submit">Concluído</button>
    </form>

</body>

</html># Formul-io-html
