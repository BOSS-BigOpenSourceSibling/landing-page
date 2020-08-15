<template>
    <v-app>
        <v-main>
            <v-container class="fill-height pa-0">
                <v-row justify="center" align="center" no-gutters>
                    <v-col
                            cols="12"
                            sm="12"
                            md="6"
                    >
                        <v-img  @click="goToProject" class="text-center main-logo clickable"
                               src="@/assets/logo-nome-alternativo.png"></v-img>
                        <v-row no-gutters>
                            <v-col md="6" sm="12" align-self="center">
                                <div class="action-button clickable" @click="goToProject">Sou Mentora</div>
                            </v-col>
                            <v-col md="6" sm="12" align-self="center">
                                <div class="action-button clickable" @click="goToProject">Sou Participante</div>
                            </v-col>
                        </v-row>
                    </v-col>
                    <v-col
                            cols="12"
                            sm="12"
                            md="6"
                    >
                        <v-img @click="goToGnome" src="@/assets/gnome.png" class="clickable"></v-img>
                    </v-col>
                </v-row>
            </v-container>
        </v-main>
    </v-app>
</template>

<script>

    export default {
        name: 'App',

        methods: {
            goToProject() {
                window.location = 'https://github.com/BOSS-BigOpenSourceSister/BigSister';
            },
            goToGnome() {
                window.location = 'https://www.gnome.org/challenge/phase-one-winners/';
            }
        }
    }
</script>

<style scoped lang="scss">
    #app {
        background: white;
        margin: 0;
        text-align: center;
    }

    .clickable {
        cursor: pointer;
    }

    .main-logo {
        margin-bottom: 20px;
        margin: 20px;
        max-height: 50vh;
    }

    .google-badge {
        height: auto;
        width: auto;
        max-height: 100%;
        max-width: 100%;
    }

    .phone-frame {
        height: 95vh;
    }

    .action-button {
        margin: 30px 30px 10px 10px;
        border: 1px solid purple;
        padding: 10px;
        border-radius: 20px;
        font-size: 1.5em;
        color: purple;

        &:hover {
            background-color: purple;
            color: white;
        }

    }
</style>
