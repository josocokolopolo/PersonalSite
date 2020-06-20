<template>
  <div class="about">
    <h1>Jhon Solier Collazos</h1>
    <about-item
      imageUrl="professional.jpg"
      imageAlt="Professional"
      text="Soy ingeniero de software, especializado en aplicaciones web, con
      conocimientos de desarrollo front-end y back-end, además de bases de datos
      y conocimientos iniciales de manejo de ciclo de vida de aplicaciones."
    />
    <about-item
      imageUrl="sports.jpg"
      imageAlt="Sports"
      text="También me gusta hacer deporte, especialmente patinaje urbano y artes
      marciales, es importante buscar el equilibrio entre la vida profesional y
      la personal."
    />
    <about-item
      imageUrl="photography.jpg"
      imageAlt="Photography"
      text="Últimamente también he encontrado una curiosidad por la fotografía, la
      panadería y respostería, es muy posible que pronto tenga una página
      individual para cada una de estas aficiones"
    />
  </div>
</template>

<script>
import AboutItem from "@/components/AboutItem";
export default {
  name: "About",
  components: { AboutItem }
};
</script>

<style lang="scss" scoped></style>
