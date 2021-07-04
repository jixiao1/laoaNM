vue开始学习

1. vue的双向绑定原理
2. v-text和v-for的使用
3. v-html的使用
4. v-bind的使用
5. v-bind:class中的使用
      <div class="box" :class="value"></div>
    <div :class="'box '+ value"></div>
    <div :title="value" title="box"></div>
    <hr>
    <div class="box" :class="obj"></div>
    <div class="box" :class="{red: true, yellow: false, blue: isActive}"></div>
    <div class="box" :class="arr"></div>
    <div class="box" :class="[{blue: true}, {green: false}, 'red']"></div>

     var vm = new Vue({
      el: '#app',
      data: {
        value: 'red',
        obj: {
          red: false,
          blue: true,
          yellow: true
        },
        isActive: true,
        arr: ['red', 'blue', 'yellow']
      }
    })
7. style的绑定
8. v-show 和v-if以及v-else-if的使用