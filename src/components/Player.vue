<template>
    <v-container fluid>
        <v-layout style='height: 450px'>
            <v-flex xs3>
                <v-toolbar dense>
                    <v-btn icon>
                        <v-icon>arrow_back_ios</v-icon>
                    </v-btn>
                    <v-toolbar-title>Nome do curso</v-toolbar-title>
                </v-toolbar>
                <div class='scroll-lessons scroll-y'>
                <v-expansion-panel expand>
                    <v-expansion-panel-content
                        v-for="(item, i) in 9"
                        :key="i"
                        class='pa-2'
                    >
                    <div slot='header' class='subheading'>Módulo {{i+1}}</div>
                    <v-card href='#'>
                        <v-card-text>
                            Aula {{i+1}}
                        </v-card-text>
                    </v-card>
                    </v-expansion-panel-content>
                </v-expansion-panel>
                </div>
            </v-flex>
            <v-flex xs9>
                <v-toolbar flat dense class='toolbar-lesson'>
                    <v-toolbar-title>Nome da aula</v-toolbar-title>
                    <v-spacer></v-spacer>
                    <v-btn flat>
                        <v-icon>arrow_back_ios</v-icon>
                        Anterior
                    </v-btn>
                    <div class="btn"></div>
                    <v-btn flat>
                        Próximo
                        <v-icon>arrow_forward_ios</v-icon>
                    </v-btn>
                </v-toolbar>
                <iframe width="100%" height="400" src="https://www.youtube.com/embed/Eg-0hJx8b0g" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <v-layout justify-center>
                    <v-btn 
                        flat
                        v-for="(item, i) in 4"
                        :key="i"
                        class='mx-3'
                        @click.stop = "files = !files"  
                    >
                        <v-icon>folder</v-icon>
                        Arquivos
                    </v-btn>
                    <v-navigation-drawer
                        v-model="files"
                        absolute
                        temporary
                        right
                    >
                        <v-card>
                            <v-card-title>teste</v-card-title>
                            <v-card-text>
                                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laudantium, facilis nesciunt omnis, vitae facere tempore eaque libero nulla distinctio eos quos at fugiat! Recusandae, iste non obcaecati debitis voluptates quas.
                            </v-card-text>
                        </v-card>
                    </v-navigation-drawer>
                </v-layout>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    data() {
        return {
            files: null
        }
    }
}
</script>

<style>
.toolbar-lesson {
    border-left: 5px solid grey;
}
.btn {
    width: 2px;
    height: 70%;
    background-color: black;
}
.scroll-lessons {
    max-height: 100%;
}
</style>
