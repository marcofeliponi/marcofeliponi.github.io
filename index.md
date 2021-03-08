<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrinnk-to-fit=no">
    
    <link rel="stylesheet" type="text/css" href="formulario.css" media="screen"
    
    <title>Cadastro</title>
</head>
<body>
    
    <div>
        <h1 id="titulo">Cadastro de DEVs</h1><br>
        <p id="subtitulo">Complete suas informações</p><br>
        <br>
    </div>

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
        
        <div class="campo">
            <label><strong>De qual lado da aplicação você desenvolve?</strong></label>
            <label> 
                <input type="radio" name="devweb" value="frontend">Front-end
            </label>
            <label>
                <input type="radio" name="devweb" value="backend">Back-end
            </label>
            <label>
                <input type="radio" name="devweb" valeu="fullstack">Fullstack
            </label>
        </div>

        <div class="campo">
            <label for="senioridade"><strong>Senioridade</strong></label>
            <select id="senioridade">
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
                <label for="tecnologia1">HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia1" value="CSS">
                <label for="tecnologia2">CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia1" value="JavaScript">
                <label for="tecnologia3">JavaScript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia1" value="PHP">
                <label for="tecnologia4">PHP</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia1" value="C#">
                <label for="tecnologia5">C#</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia1" value="Python">
                <label for="tecnologia6">Python</label>
                <input type="checkbox" id="tecnologia7" name="tecnologia1" value="Java">
                <label for="tecnologia7">Java</label>
            </div>
        </fieldset>

        <div class="campo">
            <br>
            <label><strong>Conte um pouco da sua experiência:</strong></label>
            <textarea row="6" style="width: 26em" id="experiencia" name="experiencia"></textarea>
        </div>

        <button class="botao" type="submit" onsubmit="">Concluído</button>

        </form>

    </body>

</html>

*{
    margin: 0;
    padding: 0;
}

#titulo{
    font-family: sans-serif;
    color: #00BFFF;
    margin-left: 7%;
}

#subtitulo {
    font-family: sans-serif;
    color: #00BFFF;
    margin-left: 10%;
}

#check{
    display: : inline-block;
}

fieldset {
    border: 0;
}

body{
    background-color: #F0FFFF;
    font-family: sans-serif;
    font-size: 1em;
    color: #00BFFF;
    margin-left: 36%;
    margin-top: 2%;
    justify-content: center;
}

input, select, textarea, button {
    font-family: sans-serif;
    font-size: 1em;
    color: #00BFFF;
    border-radius: 5px;
}

.grupo:before, .grupo:after {
    display: table;
}

.grupo:after {
    clear: both;
}

.campo {
    margin-bottom: 1em;
}

.campo label {
    margin-bottom: 0.2em;
    color: #00BFFF;
    display: block;
}

fieldset grupo .campo{
    float: left;
    margin-right: 1em;
}

.campo input[type="text"], .campo input[type="email"], .campo select, .campo textarea {
    padding: 0.2em;
    border: 1px solid #00BFFF;
    box-shadow: 2px 2px 2px rgba(0,0,0,0.2)
    display block;
}

.campo select option{
    padding-right: 1em;
}

.campo input:focus, .campo select:focus, .campo textarea:focus{
    background: #ffffff;
}

.botao {
    font-size: 1.2em;
    background: #00BFFF;
    border: 0;
    margin-bottom: 1em;
    color: #ffffff;
    padding: 0.2em 0.6em;
    box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow: 1px 1px 1px rgba(0,0,0,0.5);
    position: absolute;
    top: 90%;
    left: 50%;
    margin-right: -50%;
    transform: traslate(-50%, -50%);
}

.botao:hover {
    background: #00BFFF;
    box-shadow: inset 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow: none;
}

.botao, select{
    cursor: pointer;
}
