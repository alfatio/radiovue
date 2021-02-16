<template>
  <div id="page">
      <label> radio buttons</label>
      <div id="main">
        <Radio name="label">
          <label>name label</label>
        </Radio>
        <Radio name="label">
          <input type="text" placeholder="additional input">
          <div id="sub">
            <Radio name="label2">
              <input type="date" placeholder="another sub component date">
              <div id="sub">
                <Radio name="label3">
                  <input type="text" placeholder="another another sub component">
                </Radio>
                <Radio name="label3">
                  <input type="text" placeholder="another another sub component">
                </Radio>
              </div>
            </Radio>
            <Radio name="label2">
              <input type="text" placeholder="another sub component">
            </Radio>
          </div>
        </Radio>
        <Radio name="label">
          <label>name label3</label>
        </Radio>
      </div>
  </div>
</template>

<script>
import Radio from './components/Radio'
export default {
  name: 'App',
  components: {
    Radio
  }
}
</script>

<style>
#page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  gap: 1rem;
}
#main {
  display: flex;
  flex-direction: row;
}
#sub {
  margin-left: 2rem;
}
</style>
