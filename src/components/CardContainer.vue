<template>
  <div class="container-fluid">
    <CardJob
      v-for="job in jobs"
      :key="job.id"
      :name="job.name"
      :company="job.company"
      :logo="job.logo"
      :location="job.location"
      :salary="job.salary"
      :skills="job.skills"
      :vacant="job.vacant"
    />
  </div>
</template>

<script>
import CardJob from "./CardJob.vue";

export default {
  name: "CardContainer",
  components: {
    CardJob,
  },
  data() {
    return {
      jobs: [
        {
          id: 1,
          name: "Full Stack Developer",
          company: "Be Bolder",
          logo: "https://i.postimg.cc/Gm0ggNgz/be-bolder.png",
          location: "Remote in",
          salary: "5M - 8.4 COP",
          skills: ["React", "Javascript", "Java"],
          vacant: 1,
        },
        {
          id: 2,
          name: "DevOps",
          company: "Bankuish",
          logo: "https://i.postimg.cc/hGcycmBd/dev-ops.png",
          location: "Remote - Anywhere",
          salary: "50K - 70k USD",
          skills: ["Gcp", "CI/CD", "Contenedores"],
          vacant: 1,
        },
        {
          id: 3,
          name: "Nursing assistant",
          company: "Confidential",
          logo: "https://i.postimg.cc/TwHCVHWV/no-logo.png",
          location: "Antioquia",
          salary: "1M - 1.5M COP",
          skills: ["Trabajo en equipo", "Buen desempeño", "Autogestionado"],
          vacant: 1,
        },
        {
          id: 4,
          name: "IT Infrastructure Engineer Medellín",
          company: "Confidential",
          logo: "https://i.postimg.cc/TwHCVHWV/no-logo.png",
          location: "Hybrid",
          salary: "4.5M - 5M COP",
          skills: ["Administración de servidores", "Administración de redes"],
          vacant: 1,
        },
        {
          id: 5,
          name: "Fullstack Developer (.NET - Javascript) Sr.",
          company: "VICHARA TECHN",
          logo: "https://i.postimg.cc/25t0vKW4/vichara.png",
          location: "Remote in Colombia",
          salary: "8M - 11M COP",
          skills: ["Sql Server", "Javascript", ".NET"],
          vacant: 1,
        },
        {
          id: 6,
          name: "Machine Learning Intern",
          company: "VICHARA TECH",
          logo: "https://i.postimg.cc/25t0vKW4/vichara.png",
          location: "Remote in Colombia",
          salary: "2M - 3M COP",
          skills: ["Ingles", "Sql", "Python"],
          vacant: 1,
        },
        {
          id: 7,
          name: "Customer Desktop Support",
          company: "Aventior Inc",
          logo: "https://i.postimg.cc/bNNLCnhC/aventior.png",
          location: "Remote in Colombia",
          salary: "12.5M - 17.5M COP",
          skills: ["Seguridad informática", "Soporte IT", "Jira"],
          vacant: 1,
        },
        {
          id: 8,
          name: "React Architect",
          company: "Nisum Colombia",
          logo: "https://i.postimg.cc/4NVt1NKL/nisum.png",
          location: "Remote in Colombia",
          salary: "12.5M - 16.5M COP",
          skills: ["Metodologías Ágiles (Scrum)", "Unit Testing", "React"],
          vacant: 1,
        },
        {
          id: 9,
          name: "Senior Java Backend Developer",
          company: "Nisum Colombia",
          logo: "https://i.postimg.cc/4NVt1NKL/nisum.png",
          location: "Remote in Chile",
          salary: "2.8M - 3.1M CLP",
          skills: ["Java (Springboot)", "Kubernetes", "Microservices"],
          vacant: 1,
        },
        {
          id: 10,
          name: "Android Developer",
          company: "Bankuish",
          logo: "https://i.postimg.cc/hGcycmBd/dev-ops.png",
          location: "Remote",
          salary: "2K - 3.5k USD",
          skills: ["Android (Kotlin)", "Android"],
          vacant: 2,
        },
      ],
    };
  },
};
</script>

<style scoped></style>
