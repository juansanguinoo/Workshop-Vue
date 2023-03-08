<template>
  <div class="form-container">
    <form>
      <input
        type="text"
        placeholder="Search by role, salary, location or company"
      />
      <button type="submit">
        <i class="fas fa-search" style="color: #495057"></i>
      </button>
    </form>
  </div>
</template>

<script>
export default {
  name: "SearchBar",
};
</script>

<style scoped>
.form-container {
  width: 100%;
  height: 80px;

  display: flex;
  justify-content: center;
  align-items: center;

  background-color: #3a8ced;
}

form {
  width: 40%;
  height: 45px;

  display: flex;
  justify-content: space-between;
  align-items: center;
}

input {
  width: 90%;
  height: 100%;

  padding: 0 10px;

  border: 1px solid #dee2e6;
  border-radius: 5px 0 0 5px;
  outline: none;
}

button {
  width: 10%;
  height: 100%;

  border: 1px solid #dee2e6;
  border-radius: 0 5px 5px 0;
  outline: none;
  cursor: pointer;
}

@media screen and (max-width: 1000px) {
  form {
    width: 80%;
  }

  input {
    width: 80%;
  }

  button {
    width: 20%;
  }
}
</style>
