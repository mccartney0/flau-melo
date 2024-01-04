<template>
  <header>
    <nav class="flex items-center justify-evenly pt-4">
      <div class="logo">
        <img src="@/assets/logo.png" alt="Logo">
      </div>

      <div class="links flex items-center justify-evenly">
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/mentorias" class="nav-link">Mentorias</RouterLink>
        <RouterLink to="/clientes" class="nav-link">Clientes</RouterLink>
        <RouterLink to="/sobre" class="nav-link">Sobre</RouterLink>
        <a href="/whatsapp" class="nav-link contact-us-button p-3 rounded-lg">FALE COM ESPECIALISTA</a>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
  nav {
    .links {
      color: var(--vt-c-black-mute);
      width: 70%;

      .nav-link {
        &:not(:last-child) {
          width: 20px;
          transition: font-size 0.3s ease;

          &:hover {
            font-weight: 600;
            font-size: .97rem;
          }
        }
      }

      .contact-us-button {
        background-color: var(--vt-c-white);
        text-align: center;

        &:hover {
          color: var(--vt-c-white);
          background-color: var(--vt-c-white-mute);

          animation: shake 0.82s cubic-bezier(.36,.07,.19,.97) both;
          transform: translate3d(0, 0, 0);
          perspective: 1000px;
        }

        @keyframes shake {
          10%, 100% {
            transform: translate3d(-1px, 0, 0);
          }
          20%, 80% {
            transform: translate3d(1px, 0, 0);
          }
          50%, 70% {
            transform: translate3d(-1px, 0, 0);
          }
          40%, 60% {
            transform: translate3d(1px, 0, 0);
          }
        }
      }
    }
  }
</style>