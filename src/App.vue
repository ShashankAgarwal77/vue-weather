<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="Search..." />
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location"> Bulandshahr, UP</div>
          <div class="date"> Monday 10 May 2021</div>
        </div>

        <div class="weather-box">
          <div class="temp">9°c</div>
          <div class="weather">Rain</div>
        </div>

      </div>

    </main>
  </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      api_key: '6566ae56a04003829471d7a03f4040cb'
      }
  }
}
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: 'Avenir', sans-serif;
  }

  #app {
    background-image: url('assets/cold-bg.jpg');
    background-size: cover;
    background-position: bottom;
    transition: 0.4s;
  }

  main {
    height: 100vh;
    padding: 25px;

    background-image: linear-gradient(to bottom, rgba(0,0,0,0.25), rgba(0,0,0,0.75));
  }

  .search-box {
    width: 100%;
    margin-bottom: 30px;
  }

  .search-box .search-bar {
    display: block;
    width: 100%;
    padding: 15px;

    color: #313131;
    font-size: 1.25rem;
    
    appearance: none;
    border: none;
    outline: none;
    background: none;

    background-color: rgba(255, 255, 255, 0.5);
    border-radius: 0px 16px 0px 16px;
    transition: 0.4s;
  }

  .search-box .search-bar:focus {
    box-shadow: 0px 0px 16px rgba(0,0,0, 0.25);
    background-color: rgba(255, 255, 255, 0.75);
    border-radius: 16px 0px 16px 0px;
  }

  .location-box .location {
    color: #fff;
    font-size: 32px;
    font-weight: 500;
    text-align: center;
    text-shadow: 1px 3px rgba(0,0,0,0.25);
  }

  .location-box .date {
    color: #fff;
    font-size: 20px;
    font-weight: 300;
    font-style: italic;
    text-align: center;
  }

  .weather-box {
    text-align: center;
  }

  .weather-box .temp {
    display: inline-block;
    padding: 10px 25px;
    color: #fff;
    font-size: 102px;
    font-weight: 900;

    text-shadow: 3px 6px rgba(0,0,0,0.25);
    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 1rem;
    margin: 2rem 0rem;

    box-shadow: 3px 6px rgba(0,0,0,0.25);
  }


</style>
