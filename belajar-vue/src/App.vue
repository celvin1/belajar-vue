<script setup>
import { ref } from 'vue'

const nama = prompt("masukan nama")
const umur = prompt("masukan umur")
const kelas = prompt("masukan kelas")
const msg = "hello word"
const rawhtml = "<li>baju</li> <li>benget</li> <li>celana</li>"
const link = "https://www.youtube.com"
var a = 2;
var b = 98;
var c = a + b;
</script>

<template>
  <p>biodata diri</p>
  <p>nama : <span v-html= "nama" style="color: violet;"></span></p><br>
  <p>umur : <span v-html= "umur" style="color: violet;"></span></p><br>
  <p>kelas : <span v-html= "kelas" style="color: violet;"></span></p><br>
<div id="app">
  <h1>{{ msg }}</h1>
  <span v-html= "rawhtml"></span>
  </div>
  <div :id="dynamicId" style="color: blue;">WAW</div><br>
  <button :disabled="isButtonDisabled"><a :href="link">pencet</a></button>
  <br>
  <span v-on:[event]="dosomething"> hasisll {{ c }}</span>


  </template> 