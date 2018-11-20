<template>
  <div>
    <h1>Bio</h1>
    <div class="row">
      <div class="col col-6">
        <h4>Education</h4>
        <div v-for="course in courseList" :key="course.name">
          <p>{{ course.name }}</p>
          <p>{{ course.type}}</p>
          <p>{{ course.duration }}</p>
          <p>{{ course.institution }}</p>
        </div>
      </div>
      <div class="col col-6">
        <h4>Accomplishments</h4>
        <div v-for="acc in accList" :key="acc.name">
          <p>{{ acc.name }}</p>
          <p>{{ acc.type}}</p>
          <p>{{ acc.date }}</p>
        </div>
      </div>
      <div class="col col-6">
        <h4>Professional</h4>
        <div v-for="job in jobList" :key="job.position">
          <p>{{ job.position }}</p>
          <p>{{ job.company}}</p>
          <p>{{ job.duration }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Bio extends Vue {
    public courseList = [
    {
      name: 'Computer Sciences',
      type: 'Bachelor\'s Degree',
      duration: '2018-2022',
      institution: 'Universidade Estadual de Campinas',
    },
  ];
    public accList = [
    {
      name: 'EOS Hackathon',
      type: '1st Place',
      date: 'Brazil - 2018',
    },
  ];
  public jobList = [
    {
      position: 'Blockchain Developer',
      company: 'Bluchain',
      duration: '2018 - today',
    },
  ];

  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
