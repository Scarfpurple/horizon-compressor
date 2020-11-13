<template>
<v-app id="inspire">
    <v-card elevation="24" style="max-width:50%;left:50%;transform:translate(-50%, -50%);top:50%;">
        <v-card-text>
            <v-form ref="form" v-model="valid" lazy-validation>
                <v-text-field style="" v-model="name" label="Usuario"></v-text-field>
                <v-text-field style="" v-model="password" :append-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'" :type="show1 ? 'text' : 'password'" name="input-10-1" label="Contraseña" hint="Min 8 caracteres" counter @click:append="show1 = !show1" @keyup.enter="enviar"></v-text-field>
                <v-checkbox v-model="checkbox" :label="`Recordar datos`"></v-checkbox>
                <v-btn color="success" class="mr-4" @click="enviar"> Enviar </v-btn>
                <v-btn color="error" class="mr-4" @click="reset">
                    Vaciar Campos
                </v-btn>
            </v-form>
        </v-card-text>
    </v-card>
</v-app>
</template>

<script>
export default {
    name: "login",
    data() {
        return {
            name: "",
            valid: true,
            checkbox: false,
            show1: false,
            show2: true,
            password: "",

        }
    },
}
</script>

<style scoped>
.login-window {

    max-width: 40%;
}
</style>
