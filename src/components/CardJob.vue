<template>
  <div class="card-container">
    <div class="card-job">
      <div class="card-logo">
        <img v-bind:src="logo" v-bind:alt="company" />
      </div>
      <div class="card-info">
        <div class="card-row-1">
          <div class="title">
            <h5>{{ name }}</h5>
          </div>
          <div class="skills">
            <ul>
              <li v-for="(skill, index) in skills" :key="index">{{ skill }}</li>
            </ul>
          </div>
        </div>
        <div class="card-details">
          <div class="details">
            <button>
              <i class="fas fa-building"></i>
            </button>
            <p>{{ company }}</p>
          </div>
          <div class="details">
            <button>
              <i class="fa-sharp fa-solid fa-location-dot"></i>
            </button>
            <p>{{ location }}</p>
          </div>
          <div class="details">
            <button>
              <i class="fa-solid fa-money-bill"></i>
            </button>
            <p>${{ salary }}</p>
          </div>
          <div class="details">
            <button>
              <i class="fa-solid fa-user"></i>
            </button>
            <p>{{ vacant }} Job</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardJob",
  props: {
    name: String,
    company: String,
    logo: String,
    location: String,
    salary: String,
    skills: Array,
    vacant: Number,
  },
};
</script>

<style scoped>
.card-container {
  width: 100%;
  height: auto;

  display: flex;
  justify-content: center;
}

.card-job {
  width: 100%;
  height: 100px;
  margin-top: 10px;
  margin-bottom: 4px;

  display: flex;

  background-color: #fff;

  border: 1px solid #dee2e6;
  padding: 5px;
  cursor: pointer;
}

.card-job:hover {
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
}

.card-logo {
  width: 150px;
  height: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
}

.card-info {
  width: calc(100% - 150px);
  height: 100%;

  display: flex;
  flex-direction: column;
}

.card-row-1 {
  width: 100%;
  height: 50%;

  display: flex;
  align-items: center;
}

ul {
  list-style: none;
  display: flex;
  margin-top: 12px;
}

li {
  margin-right: 14px;
  padding: 0 10px;
  border-radius: 10px;
  border: 1px solid #343a40;
}

.card-details {
  width: 100%;
  height: 50%;

  display: flex;
  align-items: center;
}

.details {
  width: 20%;
  height: 100%;

  display: flex;
}

.details button {
  border: none;
  background-color: transparent;
  color: #343a40;
}

.details p {
  margin-top: 10px;
  margin-left: 5px;
}

@media screen and (max-width: 1100px) {
  .card-job {
    height: 150px;
  }

  .card-logo {
    width: 100px;
  }

  .card-info {
    width: calc(100% - 100px);
  }

  .details {
    width: 25%;

    display: flex;
    align-items: center;
  }
}

@media screen and (max-width: 700px) {
  .card-job {
    height: 250px;
  }

  .card-row-1 {
    flex-direction: column;
  }

  .card-details {
    flex-direction: column;
  }

  .details {
    width: 100%;
    height: 20%;
  }
}

@media screen and (max-width: 500px) {
  .card-job {
    height: 300px;
  }

  .skills {
    width: 100%;
    height: 100%;

    display: flex;
    justify-content: flex-start;

    margin-bottom: 5px;
  }

  ul {
    margin-top: 0;
    flex-direction: column;
  }

  li {
    margin-bottom: 5px;
    margin-right: 5px;
  }

  .card-details {
    margin-top: 14px;
  }
}
</style>
