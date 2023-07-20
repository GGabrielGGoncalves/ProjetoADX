<template>
<v-container>
  <v-layout row wrap>


    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/faleconosco">
      Cartão de Crédito em 12x
    </v-btn>

    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/carrinho">
      10% OFF no boleto ou PIX
    </v-btn>

    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/carrinho">
      Frete grátis para Sul eSudeste
    </v-btn>

    <v-btn prepend-icon="$vuetify" stacked variant="text" color="indigo-darken-3" router to = "/carrinho">
      Cartão de crédito em 12x
    </v-btn>

  </v-layout>


  <v-layout row wrap>
    <v-col cols="1"></v-col>
    <v-col cols="5">
 
  <v-carousel :show-arrows="false">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>

</v-col>

<v-col cols="6">
  <h1>Bicicleta de aluminio aro 29 KSW Shimazo TZ Vel Ltx</h1>
  <b>Tamanho do Quadro</b>

  
  <v-layout row wrap>
    <v-btn variant="outlined">
      15,5"
    </v-btn>
    <v-btn variant="outlined">
      17"
    </v-btn>
    <v-btn variant="outlined">
      19"
    </v-btn>
    <v-btn variant="outlined">
      21"
    </v-btn>
  </v-layout>
  <b>Escolha a cor</b>
  <v-layout row wrap>
     <v-btn variant="outlined">
      Vermelho
    </v-btn>
    <v-btn variant="outlined">
      Azul
    </v-btn>
    <v-btn variant="outlined">
      Verde
    </v-btn>
    <v-btn variant="outlined">
      Amarela
    </v-btn>
  </v-layout>
  <h3>R$2.999,00</h3>
  <h4>A vista no Pix ou Boleto ou ate 12x de R$259,91 com juros</h4>

  <v-container>
    <v-expansion-panels>
      <v-expansion-panel>
      <v-expansion-panel-title v-slot="{ open }">
        <v-row no-gutters>
          <v-col cols="4" class="d-flex justify-start">
            Crédito
          </v-col>
          <v-col
            cols="8"
            class="text--secondary"
          >
            <v-fade-transition leave-absolute>
              <span
                v-if="open"
                key="0"
              >
                Select cred
              </span>
              <span
                v-else
                key="1"
              >
                {{ cred.pay }}
              </span>
            </v-fade-transition>
          </v-col>
        </v-row>
      </v-expansion-panel-title>
      <v-expansion-panel-text>
        <v-row no-gutters>
          <v-spacer></v-spacer>
          <v-col cols="5">
            <v-select
              v-model="cred.pay"
              :items="pays"
              chips
              flat
              variant="solo"
            ></v-select>
          </v-col>

          <v-divider
            vertical
            class="mx-4"
          ></v-divider>

          <v-col cols="3">
            Selecione sua forma de pagamento
          </v-col>
        </v-row>
      </v-expansion-panel-text>
    </v-expansion-panel>
</v-expansion-panels>


  </v-container>
  <v-container>
    <v-expansion-panels>
      <v-expansion-panel>
      <v-expansion-panel-title v-slot="{ open }">
        <v-row no-gutters>
          <v-col cols="4" class="d-flex justify-start">
            Pix
          </v-col>
          <v-col
            cols="8"
            class="text--secondary">
            <v-fade-transition leave-absolute>
              <span
                v-if="open"
                key="0"
              >
                Select cred
              </span>
              <span
                v-else
                key="1"
              >
                {{ cred.pay }}
              </span>
            </v-fade-transition>
          </v-col>
        </v-row>
      </v-expansion-panel-title>
      <v-expansion-panel-text>
        <v-col cols="3">
            QRcode
          </v-col>
      </v-expansion-panel-text>
    </v-expansion-panel>
</v-expansion-panels>
  </v-container>

  <v-container>

  </v-container>

  <v-container>

  </v-container>
<v-btn  variant="elevated"  color="black" large router to = "/carrinho" class ="info">COMPRE AGORA</v-btn>

</v-col>
  
  </v-layout>
</v-container>


</template>

<script>
export default {
    data: () => ({
      cred: {
        name: '',
        pay: null,
        start: null,
        end: null,
      },
      pays: ['1x de 2.999', '2x valor', '3x valor', '4x valor', '5x valor', '6x valor', '7x valor', '8x valor', '9x valor', '10x valor', '11x valor','12x 259,91'],
      items: [
          {
            src: './src/assets/bike.png',
          },
          {
            src: './src/assets/bike.png',
          },
          {
            src: './src/assets/bike.png',
          },
          {
            src: './src/assets/bike.png',
          },
        ],
    }),
  }
</script>