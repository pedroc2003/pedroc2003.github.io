<!DOCTYPE html>
<html lang="pt-br">

<head>
    <link rel="icon" href="favicon.ico">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/js/bootstrap.bundle.min.js" integrity="sha384-JEW9xMcG8R+pH31jmWH6WWP0WintQrMb4s7ZOdauHnUtxwoG2vI5DkLtS3qm9Ekf" crossorigin="anonymous"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.11.3/jquery-ui.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment.min.js" integrity="sha512-qTXRIMyZIFb8iQcfjXWCO8+M5Tbc38Qi5WzdPOYZHIlZpzBHG3L3by84BBBOiRGiEb7KKtAOAs5qYdUiZiQNNQ==" crossorigin="anonymous"></script>
    <title>Objetivo</title>
</head>
<style>
  table {
    text-align: center;
  }

  #aula{
    cursor: pointer;
  }

  th, td {
    vertical-align: middle;
  }

  #disciplina:hover {
    background-color: #ececec;
    cursor: pointer;
  }

/*
  #botao {
    position: relative;
    animation-name: shake;
    animation-duration: 5s;
    animation-timing-function: ease-in;
  }
  #botao:active {
    animation-name: shakeAnim;
  }

  @keyframes shakeAnim {
    0% {left: 0}
    1% {left: -3px}
    2% {left: 5px}
    3% {left: -8px}
    4% {left: 8px}
    5% {left: -5px}
    6% {left: 3px}
    7% {left: 0}
  }

  @keyframes shake {
    0% {left: 0}
    1% {left: -3px}
    2% {left: 5px}
    3% {left: -8px}
    4% {left: 8px}
    5% {left: -5px}
    6% {left: 3px}
    7% {left: 0}
  }
*/
</style>

<body class="px-4 pt-4">
  <div class="alert alert-primary alert-dismissible fade show" role="alert">
    <h4>Link e informações importantes <span class="badge bg-secondary" id="horario"></span></h4>
    <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
  </div>
  <div class="accordion" id="accordionExample">
    <div class="accordion-item">
        <h2 class="accordion-header" id="headingOne">
          <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
            Horário Aulas
          </button>
        </h2>
        <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            <table class="table table-striped table-bordered" id="aula" onclick="meet('rrq-pucg-oqo')">
              <thead>
                <tr>
                  <th scope="col">Horário</th>
                  <th scope="col">Segunda</th>
                  <th scope="col">Terça</th>
                  <th scope="col">Quarta</th>
                  <th scope="col">Quinta</th>
                  <th scope="col">Sexta</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <th scope="row">18:45 - 19:30</th>
                  <td>História I</td>
                  <td>Geografia</td>
                  <td>Redação</td>
                  <td>Biologia</td>
                  <td>Química I-II</td>
                </tr>
                <tr>
                  <th scope="row">19:30 - 20:15</th>
                  <td>História I</td>
                  <td>Geografia</td>
                  <td>Literatura</td>
                  <td>Biologia</td>
                  <td>Matemática</td>
                </tr>
                <tr>
                  <th scope="row">20:15 - 21:00</th>
                  <td>Química I-II</td>
                  <td>Geografia</td>
                  <td>Literatura</td>
                  <td>Física I-III</td>
                  <td>Matemática</td>
                </tr>
                <tr>
                  <th scope="row">21:00 - 21:20</th>
                  <td>Intervalo</td>
                  <td>Intervalo</td>
                  <td>Intervalo</td>
                  <td>Intervalo</td>
                  <td>Intervalo</td>
                </tr>
                <tr>
                  <th scope="row">21:20 - 22:05</th>
                  <td>Física II</td>
                  <td>História II</td>
                  <td>Matemática</td>
                  <td>Biologia</td>
                  <td>Química III</td>
                </tr>
                <tr>
                  <th scope="row">22:05 - 22:50</th>
                  <td>Gramática</td>
                  <td>Inglês</td>
                  <td>Matemática</td>
                  <td>Física I-III</td>
                  <td>Filosofia/Sociologia</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
    </div>
    <div class="accordion-item">
        <h2 class="accordion-header" id="headingTwo">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
            Horário Plantões
          </button>
        </h2>
        <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            <table class="table table-sm table-striped table-bordered">
              <thead>
                <tr>
                  <th scope="col">Disciplina</th>
                  <th scope="col">Segunda</th>
                  <th scope="col">Terça</th>
                  <th scope="col">Quarta</th>
                  <th scope="col">Quinta</th>
                  <th scope="col">Sexta</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('rwj-dgoj-kii')">Linguagens</th>
                  <td>----</td>
                  <td>----</td>
                  <td><p>18:00 - 18:45</p></td>
                  <td>----</td>
                  <td>----</td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('ukv-hpzd-tua')">Biologia</th>
                  <td>----</td>
                  <td>18:00 - 18:50</td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td>----</td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('idj-stfb-zaz')">Física</th>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p></td>
                  <td>----</td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p></td>
                  <td>----</td>
                  <td>16:00 - 18:50</td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('bme-tojn-ukh')">Geografia</th>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td>----</td>
                  <td>----</td>
                  <td>----</td>
                  <td>----</td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('qtt-fwgz-wiy')">História</th>
                  <td>----</td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td>----</td>
                  <td>----</td>
                  <td>----</td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('ref-ozbk-ifh')">Matemática</th>
                  <td><p>18:00 - 18:50</p></td>
                  <td>----</td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p><p>18:00 - 18:50</p></td>
                </tr>
                <tr>
                  <th id="disciplina" scope="row" onclick="meet('dcq-hvzf-qar')">Química</th>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                  <td><p>14:00 - 15:40</p></td>
                  <td><p>14:00 - 15:40</p><p>16:00 - 17:40</p><p>18:00 - 18:50</p></td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Simulados
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          <img src="simulados.PNG" class="img-fluid mx-auto d-block" width="70%" alt="algo de errado não está certo :/">
        </div>
      </div>
    </div>
  </div>
</body>

<script>
  moment.updateLocale('en', {
    weekdays : [
      "Domingo", "Segunda", "Terça", "Quarta", "Quinta", "Sexta", "Sábado"
    ],
    months: [
      "Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho", "Julho",
      "Agosto", "Setembro", "Outubro", "Novembro", "Dezembro"
    ]
});
  console.log(moment.locale());
  let renderClock = function() {
    var localLocale = moment();
    document.getElementById('horario').innerText = localLocale.format('D [de] MMMM, dddd, HH:mm:ss');
  }
  renderClock();
  setInterval(renderClock, 1000);

  function meet(codigo){
    window.open('https://meet.google.com/'+ codigo + '?pli=1&authuser=1', '_blank');
  }
</script>

</html>