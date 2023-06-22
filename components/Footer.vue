<script setup lang="ts"></script>

<template>
  <footer>
    <div class="pattern">
      <div class="pattern__wave pattern__wave--footer"></div>
    </div>
    <div class="pattern">
      <div class="pattern__square pattern__square--left"></div>
    </div>
    <div class="container relative mx-auto lg:max-w-[1280px]">
      <div class="block d-flex">
        <div class="block__logo">
          <img
            src="@/assets/images/logo-white.svg"
            alt="Logo singgih saputro"
          />
        </div>
        <div class="block__copyright ml-auto align-self-center">
          <i class="far fa-copyright"></i>2023 Singgih Saputro. Made with<i
            class="fas fa-heart"
          ></i>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="postcss" scoped>
footer {
  @apply relative bg-[#4951A8] overflow-hidden p-[39px] pt-[150px] mt-5;

  .pattern__square--left {
    @apply z-0 bg-[#2b75bf] w-[281px] h-[281px];
    left: -32px;
    bottom: -204px;
    transform: rotate(35deg);
  }

  .block {
    &__logo {
      @apply z-1;
    }

    &__copyright {
      @apply z-1 text-sm text-base-white;
    }
  }
}
.pattern {
  &__wave {
    @apply z-0 absolute left-0 bg-no-repeat bg-auto w-full h-[100px] min-[1282px]:bg-[length:101%];

    &--top {
      @apply bottom-0 bg-[url(/assets/images/pattern-top-1.svg)];
    }

    &--footer {
      @apply top-0 bg-[url('/assets/images/pattern-bottom.svg')];
    }
  }

  &__square {
    @apply absolute rounded-[30px];
  }
}
</style>
