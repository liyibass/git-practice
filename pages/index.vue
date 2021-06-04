<template>
  <div class="container">
    <div>
      <div class="title">
        好耶
      </div>
      <div class="subtitle">
        「所有理解一切的人，只能思考萬聖節直至死亡。」- 《電鋸人》
      </div>
      <InputGroup />
      <Card />
      <Card />
    </div>
  </div>
</template>

<script>

export default {}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  margin-top: 32px;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
  text-align: center;
}

.subtitle {
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
  text-align: center;
}

.links {
  padding-top: 15px;
}
</style>
