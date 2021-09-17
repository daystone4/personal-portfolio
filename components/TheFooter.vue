<template>
   <footer class="footer">
    <div class="footer__links">
        <a href="https://github.com/daystone4" target="_blank" class="github">
          <svg xmlns="http://www.w3.org/2000/svg" role="img" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#4f5d75" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github"><title>GitHub</title><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
        </a>
        <a href="https://codepen.io/d-stone" target="_blank" class="codepen">
          <svg xmlns="http://www.w3.org/2000/svg"  aria-label="codepen" role="img" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#4f5d75" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-codepen"><title>CodePen</title><polygon points="12 2 22 8.5 22 15.5 12 22 2 15.5 2 8.5 12 2"></polygon><line x1="12" y1="22" x2="12" y2="15.5"></line><polyline points="22 8.5 12 15.5 2 8.5"></polyline><polyline points="2 15.5 12 8.5 22 15.5"></polyline><line x1="12" y1="2" x2="12" y2="8.5"></line></svg>
        </a>
        <a href="" target="_blank" class="twitter">
            <svg xmlns="http://www.w3.org/2000/svg"  aria-label="twitter" width="24" height="24" fill="none" stroke="#4f5d75" stroke-width="2" viewBox="0 0 24 24"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"/></svg>
        </a>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.footer {

  margin: 4rem 0 1rem 0;

  &__links {
    display: flex;
    justify-content: center;

    & > a > svg {
      margin: 0 1rem;
      transition: all 0.2s ease;


      &:hover {
        stroke: $accent;
        transform: translateY(-2px);
      }
    }
  }
}
</style>