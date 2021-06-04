<template>
  <div class="input__container">
    <h2>新朋友！</h2>
    <form>
      <div class="input-area">
          姓名：<input placeholder="請輸入姓名" type="text"/>
      </div>
      <div class='input-area'>
          信箱：<input placeholder="請輸入信箱" type="email"/>
      </div>
      <div class='input-area'>
          職位：<br>
          <label><input  type="radio" name="job" value="PM"> PM</label>
          <label><input  type="radio" name="job" value="工程師"> 工程師</label>
          <label><input  type="radio" name="job" value="記者"> 記者</label>
          <label><input  type="radio" name="job" value="設計師"> 設計師</label>
      </div>
      <div class='input-area'>
          屬性：<br>
          <label><input  type="checkbox" name="attribute" value="貓貓"> 貓貓</label>
          <label><input  type="checkbox" name="attribute" value="喝茶"> 喝茶</label>
          <label><input  type="checkbox" name="attribute" value="音樂"> 音樂</label>
          <br>
          <label><input  type="checkbox" name="attribute" value="美食"> 美食</label>
          <label><input  type="checkbox" name="attribute" value="話癆"> 話癆</label>
          <label><input  type="checkbox" name="attribute" value="有待開發"> 有待開發</label>
      </div>
      <button type="submit" class="button--grey button--submit">送出</button>
    </form>
  </div>
</template>

<script>
export default {}
</script>

<style scope>
  .input__container {
    margin: 24px 0;
    padding: 20px;
    color: #35495e;
    background-color: #ccd1d1;
  }

  input[type = 'text'], input[type = 'email'] {
    width: 100%;
    height: 32px;
    padding: 10px;
    font-size: 16px;
    border-radius: 5px;
    border: 0px;
    margin-top: 5px;
  }

  input:focus-visible {
    outline: 0px;
  }

  .input-area {
    margin-top: 10px;
  }

  .button--submit {
    width: 100%;
  }
</style>
