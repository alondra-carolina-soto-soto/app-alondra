<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
   
   <div class="spinner-border" role="status">
  <span class="visually-hidden">Loading...</span>
  
</div>
  </div>
  <nav aria-label="Page navigation example">
  <ul class="pagination justify-content-end">
    <li class="page-item disabled">
      <a class="page-link">Previous</a>
    </li>
    <li class="page-item"><a class="page-link" href="#">1</a></li>
    <li class="page-item"><a class="page-link" href="#">2</a></li>
    <li class="page-item"><a class="page-link" href="#">3</a></li>
    <li class="page-item">
      <a class="page-link" href="#">Next</a>
    </li>
  </ul>
</nav>
 <footer class="footer">
  <div class="footer-center">alondra carolina soto soto</div>

</footer>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
 .container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  padding: 20px;
}

/* responsivilidad para pantallas */
@media (max-width: 600px) {
  .container {
    flex-direction: column;
    padding: 10px;
  }

  .container > * {
    margin-bottom: 10px;
  }
}
.footer {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f0f0f0;
  padding: 10px 20px;
  font-size: 14px;
  border-top: 1px solid #ccc;
}



.footer-center {
  text-align: center;
  flex: 1;
}


</style>
