<template>
  <div class="header">
    <img src="../assets/logo_transparent.png" alt="" />
    <nav>
      <ul>
        <li>
          <router-link :to="{ name: 'home' }">Home</router-link>
        </li>
        <li>
          <router-link :to="{ name: 'about' }">About</router-link>
        </li>
        <li>
          <router-link :to="{ name: '' }">Contact</router-link>
        </li>
        <li>
          <router-link :to="{ name: '' }">Shop</router-link>
        </li>
      </ul>
    </nav>
    <button>Register</button>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5px;
  box-shadow: 0.5px 0.5px 4px rgba(128, 128, 128, 0.443);

  img {
    width: 70px;
    margin-left: 30px;
  }

  ul {
    display: flex;
    list-style-type: none;
  }
  li a {
    display: inline;
    margin: 50px;
    padding: 5px;
    text-decoration: none;
    color: black;
    font-size: 1.1rem;
    margin-left: 20px;
  }
  a:hover {
    background-color: rgba(0, 0, 0, 0.39);
    color: white;
    border-radius: 5px;
    font-style: italic;
  }

  button {
    align-items: center;
    margin-right: 70px;
    padding: 10px;
    border-radius: 15px;
    background-color: rgb(41, 96, 126);
    color: white;
    cursor: pointer;
    border: none;
  }
  button:hover {
    background-color: rgba(41, 96, 126, 0.786);
    font-weight: 600;
  }
}
</style>
