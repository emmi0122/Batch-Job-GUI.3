<template>
  <header>
    <div id="top-part">
      <div class="format">
        <button>Vecka</button>
        <button id="selected">Månad</button>
      </div>

      <div class="month-nav-container">
        <div id="month-nav">
          <img src="../assets/arrow-right.png" alt="arrow-left" id="arrow-left" />
          <h3>Januari</h3>
          <img src="../assets/arrow-right.png" alt="arrow-right" id="arrow-right" />
        </div>
      </div>
    </div>

    <div id="color-info">
      <div class="color-info">
        <img src="../assets/green-circle.png" />
        Ledig
      </div>

      <div class="colors">
        <img src="../assets/green-striped-circle.png" alt="green-striped-circle.png" />
        Preliminärt bokad
      </div>

      <div class="colors">
        <img src="../assets/blue-circle.png" alt="blue-circle" />
        Bokad
      </div>

      <div class="colors">
        <img src="../assets/grey-circle.png" alt="grey-circle" />
        Frånvaro
      </div>
    </div>

    <div id="weeks">
      <h3 id="vecka1">Vecka 1</h3>

      <h3 id="vecka2">Vecka 2</h3>

      <h3 id="vecka3">Vecka 3</h3>

      <h3 id="vecka4">Vecka 4</h3>
    </div>
    <div id="date">
      <div>
        <h4 class="numbers">1</h4>
        Mån
      </div>
      <div>
        <h4 class="numbers">2</h4>
        Tis
      </div>
      <div>
        <h4 class="numbers">3</h4>
        Ons
      </div>
      <div>
        <h4 class="numbers">4</h4>
        Tors
      </div>
      <div>
        <h4 class="numbers">5</h4>
        Fre
      </div>
      <div>
        <h4 class="numbers">6</h4>
        Lör
      </div>
      <div>
        <h4 class="numbers">7</h4>
        Sön
      </div>
      <div>
        <h4 class="numbers">8</h4>
        Mån
      </div>
      <div>
        <h4 class="numbers">9</h4>
        Tis
      </div>
      <div>
        <h4 class="numbers">10</h4>
        Ons
      </div>
      <div>
        <h4 class="numbers">11</h4>
        Tors
      </div>
      <div>
        <h4 class="numbers">12</h4>
        Fre
      </div>
      <div>
        <h4 class="numbers">13</h4>
        Lör
      </div>
      <div>
        <h4 class="numbers">14</h4>
        Sön
      </div>
      <div>
        <h4 class="numbers">15</h4>
        Mån
      </div>
      <div>
        <h4 class="numbers">16</h4>
        Tis
      </div>
      <div>
        <h4 class="numbers">17</h4>
        Ons
      </div>
      <div>
        <h4 class="numbers">18</h4>
        Tors
      </div>
      <div>
        <h4 class="numbers">19</h4>
        Fre
      </div>
      <div>
        <h4 class="numbers">20</h4>
        Lör
      </div>
      <div>
        <h4 class="numbers">21</h4>
        Sön
      </div>
      <div>
        <h4 class="numbers">22</h4>
        Mån
      </div>
      <div>
        <h4 class="numbers">23</h4>
        Tis
      </div>
      <div>
        <h4 class="numbers">24</h4>
        Ons
      </div>
      <div>
        <h4 class="numbers">25</h4>
        Tors
      </div>
      <div>
        <h4 class="numbers">26</h4>
        Fre
      </div>
      <div>
        <h4 class="numbers">27</h4>
        Lör
      </div>
      <div>
        <h4 class="numbers">28</h4>
        Sön
      </div>
      <div>
        <h4 class="numbers">29</h4>
        Mån
      </div>
      <div>
        <h4 class="numbers">30</h4>
        Tis
      </div>
    </div>
    <!-- ✅ Close #date -->
  </header>
</template>

<style scoped>
* {
  padding: 0;
  box-sizing: border-box;
}

button {
  all: unset;
}

header {
  padding: 2rem;
  background-color: #ffffff;
}

#top-part {
  display: flex;
  gap: 1rem;
}

#month-nav {
  display: flex;
}

#month-nav h3 {
  font-size: 1.1rem;
  margin: 0;
}

#date {
  display: flex;
  text-align: center;
}

#date div {
  font-size: 0.95rem;
}

#color-info {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
  margin-bottom: 2rem;
}

.numbers {
  margin: 1rem 1rem 0rem 1rem;
  font-size: 1rem;
}

.month-nav-container {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  width: 90%;
}

.format {
  display: flex;
  justify-content: center;
  gap: 1.2rem;
  font-size: large;
}

#selected {
  border-bottom: 3px solid black;
}

#arrow-left {
  margin-right: 1rem;
  width: 20px;
  height: 20px;
  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
}

#arrow-right {
  margin-left: 1rem;
  width: 20px;
  height: 20px;
}

#weeks {
  display: flex;
  gap: 14.5rem;
  border-bottom: 3px solid rgb(192, 191, 191);
  padding-bottom: 0.7rem;
}

#vecka3 {
  margin-left: 2rem;
}

#vecka4 {
  margin-left: 2.6rem;
}
</style>
