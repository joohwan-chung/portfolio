<template>
  <section id="about" class="container">
    <h1>About</h1>
    <div class="row gx-5">
      <figure class="col-md-6">
        <img src="../assets/images/profile.jpg" alt="profile" />
        <figcaption>About JooHwan</figcaption>
      </figure>
      <p class="col-md-6">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos.
      </p>
    </div>

    <article class="row mt-5">
      <h2>Skills</h2>
      <dl v-for="skill in skills" :key="skill.name">
        <dt class="lead">
          {{ skill.name }}
        </dt>
        <dd>
          <div class="progress" role="progressbar">
            <div class="progress-bar" :style="{ width: skill.percent }"></div>
          </div>
        </dd>
      </dl>
    </article>
  </section>
</template>

<script setup>
  const skills = [
    {
      name: 'HTML',
      percent: '90%'
    },
    {
      name: 'CSS',
      percent: '80%'
    },
    {
      name: 'JavaScript',
      percent: '85%'
    },
    {
      name: 'Vue',
      percent: '95%'
    }
  ]
</script>

<style lang="scss">
figure img {
  width: 100%;
}
</style>