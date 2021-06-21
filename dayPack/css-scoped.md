## css-style标签<style scoped>
### 用法
#### 当 <style> 标签有 scoped 属性时，它的 CSS 只作用于当前组件中的元素。
### scoped与无scoped属性的，可混用
#### 作用
#### scoped标签应用后，父组件样式不会渗透到子组件，如若想影响更深（可使用>>>【sass没法设别】，可换成/deep/或：：v-deep）
