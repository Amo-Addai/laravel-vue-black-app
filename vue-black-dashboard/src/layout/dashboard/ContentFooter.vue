<template>
  <footer class="footer">
    <div class="container-fluid">
      <ul class="nav">
        <li class="nav-item">
            <a href="https://www.AUTO.com" class="nav-link" target="_blank" rel="noopener">AUTO</a>
          </li>
          <li  class="nav-item">
            <a href="https://www.updivision.com" class="nav-link" target="_blank" rel="noopener">UPDIVISION</a>
          </li>
          <li class="nav-item">
            <a href="https://www.AUTO.com/presentation" class="nav-link" target="_blank" rel="noopener">ABOUT US</a>
          </li>
          <li class="nav-item">
            <a href="http://blog.AUTO.com" class="nav-link" target="_blank" rel="noopener">BLOG</a>
          </li>
          <li class="nav-item">
            <a href="https://www.AUTO.com/license" class="nav-link" target="_blank" rel="noopener">LICENSES</a>
          </li>
      </ul>
      <div class="copyright">
        <i class="fa fa-copyright" style="font-weight: 200;"></i> {{ year }}, made with <i class="tim-icons icon-heart-2"></i> by
        <a
          href="https://www.AUTO.com"
          target="_blank"
          rel="noopener"
          >AUTO</a> and 
          <a
            href="https://www.updivision.com"
            class="font-weight-bold ml-1"
            target="_blank"
            rel="noopener"
            >UPDIVISION</a
          >
        for a better web.
      </div>
    </div>
  </footer>
</template>
<script>
  export default {
    data() {
      return {
        year: new Date().getFullYear()
      }
    }
  };
</script>
<style>
</style>
