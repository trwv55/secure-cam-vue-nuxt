<template>
<div class="container d-flex flex-column min-vh-100">
  <header>
    <slot name="header"></slot>
  </header>
  <main class="container main flex-fill">
    <slot></slot>
  </main>
  <footer>
    <slot name="footer"></slot>
  </footer>
</div>
</template>