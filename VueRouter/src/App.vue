<template>
  <div id="app">
    <div class="ui fixed inverted menu">
      <div class="ui container">
        <router-link :to="{name: 'root'}" class="header item">Accueil</router-link>
        <router-link :to="{name: 'a'}" class="item">Page A</router-link>
        <router-link :to="{name: 'post', params: {id: 1}}" class="item">Article</router-link>
      </div>
    </div>
    <div class="sidebar">
      <h1>Sidebar</h1>
      <transition>
        <router-view name="sidebar"></router-view>
      </transition>
    </div>
    <div class="main">
      <h1>Main</h1>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
}
</script>
