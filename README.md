<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');
  
body {
   line-height: 1.4;
   background-image: linear-gradient( 90deg,
      rgba(58, 58, 158, 0.8),
      rgba(136, 136, 206, 0.7)
    ),
    url(https://images.unsplash.com/photo-1498050108023-c5249f4df085?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=872&q=80);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  font-family: 'Open Sans', sans-serif;
  font-weight: bold;
  text-align: center;
  }
  
  #title {
    margin-top: 20px;
    color: white;
    font-family: 'Roboto', sans-serif;;
    font-size: 40px;
  }
  
  #survey-form{
    background-color: rgba(198, 204, 178, 0.8);
    width: 60%;
    margin: auto;
    padding: 30px;
    border-radius: 8px;
    color: #2E282A;
    text-align: left;
    line-heigth: 10px;   
  }
  
  .bloco{
    padding: 5px; 
  }
  
  .barra{
    display: flex;
    flex-direction: column;
    width: 80%;
    heigth: 25px;
    border-radius: 5px;
    border: 0px solid;
    padding: 8px;
    margin-top: 10px;
  }
  
  
  #submit{
    padding: 5px;
    border-radius: 5px;
    font-weight: bold;
  }
  
  #submit:hover{
    background-color: rgb(84, 84, 211);
    color: white;
    
  }
  
  textarea {
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
  
</style>

<head></head>
<body>
  <h1 id="title">Formulário de Pesquisa</h1>
  <p id="description">Obrigado(a) pela sua colaboração!</p>
  
  <form id="survey-form">
    <div id="container">
      <div class="bloco">
      <!--Nome-->
      <label id="name-label" for="name"> Nome </label><input class="barra" id="name" type="text" name="name" required placeholder="Qual é o seu nome?"><br>
      </div> 

      <div class="bloco">
      <!--Email-->
      <label id="email-label" for="email">Email </label><input class="barra" id="email" type="email" required placeholder="Qual é o seu email?"><br>
      </div> 

      <div class="bloco">
      <!--Idade-->
      <label  id="number-label" for="number">Idade (opcional) </label>
      <input class="barra" id="number"  type="number" min="16" max="90" placeholder="0">
      </div> 

      <div class="bloco">
      <!--lista suspensa-->
       <p>Qual é a sua escolaridade ?</p>
        <select class="barra" id="dropdown" name="role" class="form-control" required>
          <option disabled selected value>Selecione entre as opções </option>
          <option value="Fundamental">Ensino Fundamental</option>
          <option value="Médio">Ensino Médio</option>
          <option value="Superiorincompleto">Ensino Superior incompleto</option>
          <option value="Superiorcompleto">Ensino Superior completo</option>
          <option value="Pós">Pós Graduação incompleta</option>
          <option value="Póscompleta">Pós Graduação completa</option>
          <option value="outro">Outro</option>
        </select>
      </div> 

      <div class="bloco">
      <!--botão rádio-->
      <p>Você já sabe programar ?</p>
      <label for="sim">
      <input type="radio" id="sim" name="programacao" value="sim" checked>Sim</label><br>

      <label for="incerto">
      <input type="radio" id="incerto" name="programacao" value="NaoTemCerteza">Não tenho certeza</label><br>

      <label for="não">
      <input type="radio" id="não" name="programacao" value="Não">Não</label><br>
      </div> 

      <div class="bloco">
      <!--checkbox-->
      <p>Qual linguaguem de programação você deseja conhecer? <p>
       <label for="php"><input id="php" type="checkbox" name="linguagens" value="php">PHP </label><br> 

       <label for="javascript"> <input id="javascript" type="checkbox" name="linguagens" value="javascript"> JavaScript </label><br> 

       <label for="c#"> <input id="c#" type="checkbox" name="linguagens" value="c#">C#  </label><br> 

       <label for="python"> <input id="python" type="checkbox" name="linguagens" value="python"> Python </label><br>

       <label for="outra"> <input id="outra" type="checkbox" name="linguagens" value="outra">Outra</label><br> 
       </div> 

      <div class="bloco">
      <!--campo p/ comentários-->
        <p>Conte por que deseja se tornar um programador?</p>
      <textarea class="barra" id="comentario" name="comentario" placeholder="Escreva aqui..." ></textarea><br>
        </div> 

      <div class="bloco">
      <!--Botão Submit-->
      <button id="submit" type="submit">Enviar</button>
       </div> 
    </div>
  </form>
<body> Html5-CSS3
Projetos freeCodeCamp
