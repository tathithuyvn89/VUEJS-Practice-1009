<template>
  <div>
    <!-- <Header/>
    <ProgressSteps/> -->
    <QuizzList/>
    <router-view></router-view>
  </div>
</template>

<script>

// import Header from './components/layout/Header'
// import ProgressSteps from './components/layout/ProgressSteps'
 import QuizzList from './components/quizz/QizzList'
export default {

 nam: 'App',
 components: {
  //  Header,
  //  ProgressSteps
   QuizzList
 }

}
</script>

<style>

</style>