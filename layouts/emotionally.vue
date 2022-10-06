<template>
  <div class="emotionallyFont">
    <slot></slot>
    <!-- <Menu /> -->
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Ledger&family=Montserrat:wght@400;500;600;700&display=swap");
.emotionallyFont {
  font-family: "Ledger", serif;
}
.page-enter-from {
  @apply opacity-0;
}

.page-enter-active,
.page-leave-active {
  @apply transition-all;
}
.page-enter,
.page-leave-to {
  @apply opacity-0;
}
</style>
