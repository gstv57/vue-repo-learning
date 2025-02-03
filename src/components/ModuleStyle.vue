<template>
  <h1 :class="myClasses['m-class']">Using Module CSS with $ syntax (kebab-case)</h1>
  <h1 :class="myClasses.anotherClass">Using Module CSS with $ syntax (camelCase)</h1>
</template>

<style module="myClasses">
/* kebab-case */
.m-class {
  background: firebrick;
  color: white;
}
.anotherClass {
  background: seagreen;
  color: white;
}
</style>
