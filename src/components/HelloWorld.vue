<template>
  hello world
  <!-- ref、reactive -->
  <!-- {{ a }}- {{ b }} -{{ a1 }} - {{ b1.dataB2 }} -->
  <!-- <button @click="handleClick">click me</button> -->

  <!-- toRefs、 toRef -->
  <ul>
    <li>obj1: {{ obj1 }}</li>
    <li>attrA: {{ attrA }}</li>
    <li>obj2: {{ obj2 }}</li>
    <li>attrB: {{ attrB }}</li>
  </ul>
  <button @click="func1">addA</button>
  <button @click="func2">addB</button>
</template>

<script>
import { reactive, ref, toRefs, toRef, watch } from "vue";
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  setup() {
    // ref、reactive
    // const a = ref(1);
    // const b = ref({ a: 1 });
    // const a1 = reactive(1);
    // const b1 = reactive({ dataB2: 1 });
    // console.log("a:", a);
    // console.log("b:", b);
    // // console.log("a1:", a1);
    // console.log("b1:", b1);

    // const handleClick = () => {
    //   a.value++;
    //   b.value.a++;
    //   // a1++; reactive无法实现基本类型响应式
    //   b1.dataB2++;
    // };

    // return {
    //   a,
    //   b,
    //   a1,
    //   b1,
    //   handleClick,
    //   // ...toRefs(b1),
    // };

    // toRefs、 toRef
    const obj1 = { a: 1 };
    const attrA = toRef(obj1, "a");
    const obj2 = reactive({ b: 1 });
    const attrB = toRef(obj2, "b");
    console.log("obj1", obj1);
    console.log("attrA", attrA);
    console.log("obj2", obj2);
    console.log("attrB", attrB);
    function func1() {
      attrA.value++;
      console.log("---111", obj1, attrA.value);
    }
    function func2() {
      // attrB.value++;
      obj2.b++;
      console.log("---222", obj2, attrB.value);
    }
    return { obj1, obj2, attrA, attrB, func1, func2 };
  },
};
</script>
