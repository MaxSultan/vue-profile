<template>
    <div>
        <section class="frame">
            <h1>Max Sultan</h1>
        </section>
        <section class='frame'>
            <h1>Projects</h1>
            <div v-for="project in projects" :key="project.name" @click="selectProject(project)"> {{ project.name }} </div>
            <div v-if="selectedProject" class="selectedProject">
                <h1>{{ selectedProject.name }}</h1>
                <img :src="img"/>
                <p>{{ selectedProject.description }}</p>
                <a :href="selectedProject.github" target="_blank">Github Link</a>
                <a :href="selectedProject.heroku" target="_blank">Heroku Link</a>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            projects: [
                {
                    name: "Sticky", 
                    img: '', 
                    github:'https://github.com/MaxSultan/sticky-bugtracker', 
                    heroku:'https://sticky-bugtracker.herokuapp.com/', 
                    description:'An app that lets members of a company track their bugs. It allows teams share descriptions of the bugs, times the bugs were created, who the bugs are assigned to, and when work began on a bug. The bug tracker allows members to archive bugs and projects. It also allows team members to collabate and add additional information on the bugs through chats. Information about the bugs is visually represented through charts that can be downloaded for easy use offline.'
                },
                {
                    name: "Digital Glovebox", 
                    img: '', 
                    github:'https://github.com/devpointlabs/glove_box', 
                    heroku:'', 
                    description:'An app that tracks documents for your vehicle including drivers liscence, registration, maintainence records, etc. It allows you to add vehicles and add images of records.'
                },
                {
                    name: "Chicken Tinder", 
                    img: '', 
                    github:'https://github.com/MaxSultan/Chicken-Tinder', 
                    heroku:'', 
                    description:''
                }
            ],
            selectedProject: undefined,
        }
    },
    methods: {
        selectProject(project) {
            this.selectedProject = project
        }
    },
}
</script>

<style scoped>
.selectedProject{
    float:right;
    max-width: 65%;
    background-color: #c4c4c4;
    margin: 2em;
    padding: 2em;
    border-radius: 10px;
}
</style>