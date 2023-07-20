<template>
  <v-col>
 <v-col>

  <v-layout row wrap>
    <img src="./src/assets/logo.png">


    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/faleconosco">
      Fale Conosco
    </v-btn>
    <v-flex cols="6"  class="text-xs-center">
      <v-text-field label="Pesquisar" variant="outlined"></v-text-field>
    </v-flex>
    

    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/carrinho">
      Carrinho
    </v-btn>
    
    <v-container>
      Olá, Daniel, temos novidades pra você
    </v-container>
  </v-layout>
    

      <v-layout row wrap>
    <v-flex xs12 sm6 class="text-xs-center">
      <v-btn variant="text" color="indigo-darken-3" large router to = "/bicicletaskrw" class ="info">Bicicleta KRW</v-btn>
    </v-flex>
    <v-flex xs12 sm6 class="text-xs-center ">
      <v-btn variant="text" color="indigo-darken-3" large router to = "/quadros KRW" class ="info">Quadros KRW</v-btn>
    </v-flex>
    <v-flex xs12 sm6 class="text-xs-center">
      <v-btn variant="text" color="indigo-darken-3" large router to = "/bicicletas" class ="info">Bicicletas</v-btn>
    </v-flex>
    <v-flex xs12 sm6 class="text-xs-center">
      <v-btn variant="text" color="indigo-darken-3" large router to = "/ofertas" class ="info">Ofertas</v-btn>
    </v-flex>
    <v-flex xs12 sm6 class="text-xs-center ">
      <v-btn variant="text" color="indigo-darken-3"  large router to = "/categoria" class ="info">Categoria</v-btn>
    </v-flex>
    <v-spacer></v-spacer>
    <v-flex xs12 sm1 class="text-xs-center">
      <v-btn  variant="elevated"  color="indigo-darken-2" large router to = "/ofertas" class ="info">OFERTAS IMPERDIVEIS</v-btn>
    </v-flex>
  </v-layout>
</v-col>
  </v-col>

</template>


