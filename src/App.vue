<template>
  <div id="app">
    <div class="row">
      <div class="card">
        <img :src="cardimg" alt="Imagen de la tarjeta" />
        <div class="card-body">
          <h3>{{ cardtitle }}</h3>
          <p>{{ cardbody }}</p>
          <button>{{ cardbtn }}</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      cardimg: "https://picsum.photos/200/300",
      cardtitle: "Card title",
      cardbody:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, voluptatem.",
      cardbtn: "Go somewhere",
    };
  },
};
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  width: 300px;
  align-items: center;
  justify-content: center;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
  text-align: center;
  background-color: #fff;
}

.card img {
  width: 300px;
  margin: 0 auto;
  height: 200px;
  border-radius: 5%;
  object-fit: cover;
}

.card h3 {
  font-size: 24px;
  margin-bottom: 10px;
}

.card p {
  font-size: 16px;
  margin-bottom: 20px;
}

.card button {
  background-color: #007bff;
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}
</style>
