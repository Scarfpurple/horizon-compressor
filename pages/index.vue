<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <h1>Horizon-Compressor</h1>
      </div>
      <v-card>
        <v-card-title class="headline">
          Bienvenido a Horizon-Compressor
        </v-card-title>
        <v-card-text>
          <p>Horizon-Compressor, esta pensado para facilitarte el manejo de tus archivos mas importantes, soportando distintos formatos, para que los tengas cuando quieras!.</p>
          <p>
            Visita nuestra cuenta de Facebook <a
              href="https://fb.com"
              target="_blank"
              rel="noopener noreferrer"
            >
              Horizon-Compressor
            </a>.
          </p>
          <p>
            Si tienes alguna duda, no duces en escribirnos... <a
              href="horizoncompressor@gmailcom"
              target="_blank"
              rel="noopener noreferrer"
              title="chat"
            >
              e-mail
            </a>.
          </p>
          <p>Gracias por visitarnos, tus archivos estan a salvo.</p>
          <div class="text-xs-right">
            <em><small>&mdash; Horizon-Compressor S.A</small></em>
          </div>
          <hr class="my-3">
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/login"
          >
            Eres nuevo? Registrate!
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>


export default {
  name: "inicio"
}
</script>
