<script>
  import LogoFooter from "../LogoFooter.svelte";
  import Atendimento from "./footer-list/Atendimento.svelte";
  import Contatos from "./footer-list/Contatos.svelte";
  import Produtos from "./footer-list/Produtos.svelte";
  import Siganos from "./footer-list/Siganos.svelte";

  const year = new Date().getFullYear();
</script>

<footer class="bg-sky-950">
  <div class="container p-6 mx-auto">
    <div class="lg:flex">
      <div class="w-full -mx-6 lg:w-2/5">
        <div class="px-6">
          <LogoFooter />

          <p class="max-w-sm mt-2 text-gray-400">
            Nosso papel é dar uma ótima impressão.
          </p>
        </div>
      </div>

      <div class="mt-6 lg:mt-0 lg:flex-1">
        <div
          class="grid grid-cols-1 gap-6 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4"
        >
          <Siganos />

          <Atendimento />

          <Produtos />

          <Contatos />
        </div>
      </div>
    </div>

    <hr class="h-px my-6 border-none bg-gray-700" />

    <div>
      <p class="text-center text-gray-400">
        © Gráfica Plantão {year} - Todos os direitos reservados
      </p>
    </div>
  </div>
</footer>
