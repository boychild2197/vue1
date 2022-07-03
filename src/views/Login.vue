<template>
  <v-img src="../assets/images/payment-methods.webp">
    <v-container>
      <v-row>
        <v-col cols="4"></v-col>
        <v-col cols="4" class="align-center justify-center">
          <v-card class="my-5">
            <form class="mx-3 my-3">
              <v-subheader
                class="
                  align-center
                  justify-center
                  primary--text
                  font-weight-bold
                  display-1
                "
                style=""
                >Login</v-subheader
              >

              <v-text-field
                v-model="email"
                :error-messages="emailErrors"
                label="E-mail"
                required
                @input="$v.email.$touch()"
                @blur="$v.email.$touch()"
              ></v-text-field>
              <v-text-field
                v-model="name"
                :error-messages="nameErrors"
                :counter="8"
                label="Password"
                required
                @input="$v.name.$touch()"
                @blur="$v.name.$touch()"
              ></v-text-field>

              <v-btn class="my-3" @click="submit"> submit </v-btn>
        
            </form>
          </v-card>
        </v-col>
        <v-col cols="4"></v-col>
      </v-row>
    </v-container>
  </v-img>
</template>

<script>
export default {
  name: "Login",

  data: () => ({}),
};
</script>
