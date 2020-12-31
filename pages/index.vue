<template>
  <div class="container mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-2">
      <div>
        <title-and-text title="Desenvolvimento de Software" text="Nós ajudamos você a gerenciar e criar o software que contribuirá com o sucesso da sua empresa. Somos profissionais altamente qualificados focados em entregar o melhor software para sua empresa."/>
      </div>
      <div>
        <card :text-card-options="textCard" title="Criamos o software para atender com as suas aspectativas:" subtitle="Estamos sempre em constante contato para entregarmos o melhor sistema, para garantir o sucesso do nosso cliente." />
      </div>
    </div>
  </div>
</template>

<script>
import Card from '../components/show-text/Card.vue';
export default {
  components: { Card },
  data() {
    return {
      textCard: [
        {
          text: "Layout personalizado, criando com um forte estudo de design gráfico."
        },
        {
          text: "É feita toda uma documentação de funcionamento do seu projeto."
        },
        {
          text: "Temos nosso próprio sistema para acompanhamento do andamento do projeto e das entregas a serem feitas para nosso cliente."
        }
      ]
    }
  },
};
</script>


