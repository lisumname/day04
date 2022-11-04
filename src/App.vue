<template>
  <div>
    <MySchool :name='msg' :sex='xing' :age='number'/>
    <hr>
    <MySchool name='李四' sex='女' :age='30'/>
  </div>
</template>

<script>
import MySchool from "./components/School.vue";
export default {
  name: "App",
  data() {
    return {
      msg:'张三',
      number:19,
      xing:'男'
    }
  },
  components: { MySchool }
}
</script>
