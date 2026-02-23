<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="Alrededor de la Nómina y prestaciones sociales donde encontramos: -Documento para diligenciar los pagos realizados a los empleados, por la contraprestación laboral. -Devengos que se compone del salario, auxilio de transporte, horas extras, bonificaciones, comisiones, entre otras. -Deducciones donde se encuentra, la salud, pensión, libranzas, embargos. -Contratos de trabajo donde se abarcan los escritos, verbales, indefinidos, transitorios y dan origen a prestaciones sociales como, primas, liquidación, licencias, entre otros. -Por otro lado, encontramos el salario que se compone por los elementos como, salario, subordinación y prestación del servicio. Terminación como muerte, renuncia o despido. -Retribución por el servicio prestado. -Salario mínimo, salario integral, salario variable, salario a destajo. Por último, se encuentran las hojas de cálculo y software para la generación de informes financieros. Ciclo contable como libro diario, mayor, auxiliares, balances, informes financieros. ")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
