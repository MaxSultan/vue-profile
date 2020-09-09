<template>
    <div class="frame">
        <h1>Tech</h1>
        <div v-for="tech in techList" :key="tech.name" @click="selectTech(tech)">{{ tech.name }}</div>
        <div v-if="selectedTech">
            <h1> {{ selectedTech.name }} </h1>
            <p>Projects displaying this technology: {{ selectedTech.projects }}</p>
            <h3>Key concepts Familiar with:
                <ul>
                    <li v-for="concept in selectedTech.concepts" :key="concept">{{ concept }}</li>
                </ul>
            </h3>
        </div>
    </div>
</template> 
 
<script>
export default {
    data() {
        return {
            techList: [
                {name: "React", projects: "Sticky, Digital GloveBox, Chicken Tinder", concepts: ['Redux','React Router', 'React Hooks', 'Functional Components', 'Lifecycle Methods']},
                {name: "Ruby on Rails", projects: "Sticky, Digital GloveBox, Chicken Tinder", concepts: ["ActionCable","MVC architecture","ActiveRecord Associations","Custom Routing","Bundling and Gems"]},
                {name: "PosgreSQL", projects: "Sticky, Digital GloveBox, Chicken Tinder", concepts:["Custom SQL statements"," Joins","Limits", "Ordering"] },
                {name: "Django", projects: "Movies App", concepts: ["ORM", "Routing","Admin Pannel",]},
                {name: "Jest", projects: "", concepts: ["Unit Testing", "Snapshot testing", "Suites and Tests"]},
                {name: "Docker", projects: "", concepts: ""},
                {name: "AWS", projects: "", concepts: ""},
                
            ],
            selectedTech: undefined,
        }
    },
    methods: {
        selectTech(tech) {
            this.selectedTech = tech
        }
    }
}
</script>