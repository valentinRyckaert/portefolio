<script>

    export let listSentences = [
        [
            "Je suis là pour vous tenir compagnie.",
            "Je ne mords pas... sauf quand je le fais."
        ],
        [

        ]
    ]

    export let page = '/';
    let rand = -1;

    function setRand(){
      if(rand > 0)
        rand = Math.round(Math.random() * 3);
    }

    function getSentence(){
      	if(rand == -1){
        	return "Bonjour ! Je m'appelle Bill. Je suis là pour vous tenir compagnie.";
      	}
      	switch(page){
          	case "/":
            	return listSentences[0][rand];
          	case "/formation":
            	return listSentences[1][rand];
          	case "/competences":
            	return listSentences[2][rand];
          	case "/projets":
            	return listSentences[3][rand];
          	case "/a_propos":
            	return listSentences[4][rand];
    	}
    }
    
</script>

<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal" on:click={() => setRand()}>
    Appeller Bill
  </button>

  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h1 class="modal-title fs-5" id="exampleModalLabel">Bill</h1>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          <p class="m-3">{getSentence()}</p>
        </div>
      </div>
    </div>
  </div>
  