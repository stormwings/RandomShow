<script>
  const goToBuy = () => console.log('Go buy!')
  const goToDownload = () => console.log('Go pirate!')
  const imageProfile = 'https://i1.wp.com/culturageek.com.ar/wp-content/uploads/2020/03/Culturageek.com_.ar-Resident-Evil-3-Review-1.jpg'

</script>

<main>
  <div class="card">
    <div class="card--header">
      <div class="card--header__title">
        Resident Evil 3 Remake
      </div>
    </div>
    <div class="card--body">
      <div class="card--body__image">
        <img src={imageProfile} alt="Resident evil 3 banner">
      </div>
      <div class="card--body__description">
        El Juego aún no ha sido crackeado 💔
      </div>
    </div>
    <div class="card--footer">
      <button class="card--footer__button" on:click={goToBuy}>
        Ir a comprar
      </button>
      <button class="card--footer__button" on:click={goToDownload}>
        Descargar Pirata
      </button>
    </div>
  </div>
</main>

<style>
  .card {
    width: 100%;
    max-width: 600px;
    border-radius: 15px;
    background-color: var(--background-color__card);
  }

  .card--header {
    padding-top: 15px;
    padding-bottom: 10px;
    min-height: 20px;
  }

  .card--header__title {
    font-size: 1.2em;
  }

  .card--body__image {
    border-radius: 15px;
    overflow: hidden;
    margin-bottom: 5px;
  }

  .card--body__image img {
    width: 100%;
  }

  .card--body {
    padding: 5px 10px;
    min-height: 20px;
  }

  .card--body__description {
    font-size: 0.9em;
  }

  .card--footer {
    padding: 15px 0;
  }
  .card--footer__button {
    border: none;
    border-radius: 5px;
    background-color: var(--text-info);
    color: var(--text-primary);
    font-size: 15px;
    margin: 0px 2px;
  }


</style>