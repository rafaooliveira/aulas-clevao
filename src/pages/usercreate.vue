<template lang="pug">
  q-page(
    padding
  )
    div.row.justify-center
      q-card.col-xs-12.col-sm-6.col-lg-6
        q-card-section.text-white
          div.text-h6 Novo Usuário
        q-separator
        q-card-section
          q-form
            q-input(
              label="E-mail"
              v-model="email"
            )
            q-input(
              type="password"
              label="Senha"
              v-model="password"
            )
            q-input(
              type="password"
              label="Confirmar Senha"
              v-model="password_confirm"
            )
        q-card-actions(
          align="around"
        )
          q-btn(
            flat
            @click.prevent="submit"
          ) Criar
          q-btn(
            flat
            @click.prevent="cancel"
          ) Cancelar
</template>

<script>
export default {
  data () {
    return {
      email: '',
      password: '',
      password_confirm: ''
    }
  }
}
</script>

<style>

</style>
