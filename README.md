# Prof.-Paulo-exemploJS.html
Modelo com JavaScript

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo JS</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
    <style>
        #olho{
            position: relative;
            left: 10px;
            top: 8px;
            cursor: pointer;
        }
        
</style>
</head>
<body>
    <form action="#" method="get">
        <label for="nome">Senha:</label>
        <input type="password" id="senha" name="senha" required> 
        <span id="olho" class="material-symbols-outlined" onclick="mostraSenha()">
            visibility_off
            </span>
        <br>
        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required onmouseenter="mudaNome()" onmouseleave="mudaNome2()" 
         required>
        <br>
        <br>
        <input type="submit" value="Enviar">
    </form>
</body>
</html>
<script>
    function mudaNome() {
        document.getElementById('nome').value = "Louis"
    }
    function mudaNome2() {
        document.getElementById('nome').value = ""
    }
    function mostraSenha() {
        if(document.getElementById("senha").type == "text"){
            document.getElementById("senha").type = "password"
            document.getElementById("olho").innerHTML = "visibility_off"
        }
        else{
        document.getElementById("senha").type = "text"
        document.getElementById("olho").innerHTML = "visibility"
    }
}
</script>
