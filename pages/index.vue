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
      <div >
        <Card :contact="contact" v-for='contact of contacts.reverse()' :key="contact.id"/>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data () {
    return {
      contacts: [
        {
          id: 1,
          name: '生菜',
          email: 'v61265@gmail.com',
          job: '工程師',
          characteristic: ['貓貓', '話癆', '有待開發']
        },
        {
          id: 2,
          name: '電次',
          email: 'chianman@gmail.com',
          job: '記者',
          characteristic: ['貓貓', '美食']
        },
        {
          id: 3,
          name: '瑪琪瑪',
          email: 'makima@gmail.com',
          job: 'PM',
          characteristic: ['貓貓', '喝茶', '有待開發']
        },
        {
          id: 4,
          name: '秋',
          email: 'asakawa@gmail.com',
          job: '記者',
          characteristic: ['喝茶', '音樂',]
        },
        {
          id: 5,
          name: '帕瑪',
          email: 'pama@gmail.com',
          job: '設計師',
          characteristic: ['貓貓', '美食', '話癆']
        }
      ]
    }
  }
}
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
