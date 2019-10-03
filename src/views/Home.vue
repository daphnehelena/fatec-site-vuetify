<template>
  <div>
  

     <v-parallax
         dark
        src="../assets/universe-hackathon.png"
       >
      <v-row
      align="center"
      justify="center"
      
       >
      
      <h4 class="subheading display-3 text-center font-weight-black">Venha fazer parte do nosso time!</h4>
   
      </v-row>
       <div class="text-center">
          <v-btn class="ma-5" outlined color="white">saiba mais</v-btn>
      </div>
        </v-parallax>

       
  

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
  <body>
      <section>
        <h2>{O que fazemos}</h2>
        <p class="texto">
          Damos vida a suas ideias, criamos soluções eficientes e profissionais para suas necessidades.
        </p>
         
      
        <hr/>
        <div class="card-position">
          <div class="card">
            <v-icon x-large color="pink">mdi-brain</v-icon>
            <h3>Inteligência Artificial</h3>
            <p class="texto-card txt-responsivo">Aplicações que lidam com grandes volumes de informações, seja por texto, voz, vídeo ou fotos.</p>
            <!-- <p>Criamos aplicações que aprendem com bases de dados e podem ser treinadas para lidarem com grandes volumes de informações de variadas situações, seja por comando de texto, voz, vídeo ou fotos.</p> -->
          </div>
        
            <div class="card">
          <!-- ícone com links -->
              <v-icon x-large color="red">mdi-code-tags</v-icon>
              <h3>Sites</h3>
              <p class="texto-card txt-responsivo">Manutenção e criação de sites responsivos utilizando HTML5+CSS3, planejamento em Marketing Digital e SEO e paineis administrativos.</p>
              <!-- <p>Oferecemos serviçoes de criação e manutençã de sites, planejamento em marketing digital e SEO, técnicas que garantem deixar seu website no topo das buscas.</p> -->
            </div>

          <div class="card">
              <v-icon x-large color="orange">mdi-code-braces</v-icon>
              <h3>Softwares e Apps</h3>
              <p class="texto-card txt-responsivo">Softwares de gerenciamento de empresas para Windows, Linux e macOS. Aplicativos para smartphones para as plataformas iOs e Android.</p>
              
         </div>
        </div>
      

      </section>
        <section>
        <h2>{Projetos do ano}</h2>
        <p class="texto">
          Spoiler: nossos projetos são reconhecidos mundialmente!
        </p>
        <hr/>

      <div class="hestia">
        <template>
  <v-container class="pa-4 text-center">
    <v-row class="fill-height" align="center" justify="center">
      <template v-for="(item, i) in items">
        <v-col
          :key="i"
          cols="12"
          md="4"
        >
          <v-hover v-slot:default="{ hover }">
            <v-card
              :elevation="hover ? 12 : 2"
              :class="{ 'on-hover': hover }"
            >
              <v-img
                src="../assets/hestia-ai.jpg"
                height="225px"
              >
                <v-card-title class="title white--text">
                  <v-row
                    class="fill-height flex-column"
                    justify="space-between"
                  >
                    <p class="mt-4 subheading text-left">{{ item.title }}</p>

                    <div>
                      <p class="ma-0 body-1 font-weight-bold font-italic text-left">
                        {{ item.text }}
                      </p>
                      <p class="caption font-weight-medium font-italic text-left">
                        {{ item.subtext }}
                      </p>
                    </div>

                   
                  </v-row>
                </v-card-title>
              </v-img>
            </v-card>
          </v-hover>
        </v-col>
      </template>
    </v-row>
  </v-container>
</template>
      </div>


       
      </section>

      <section>
        <h2>{Clientes}</h2>
        <p class="texto">
          Serviços de qualidades atraem e conquistam clientes incríveis!
        </p>
        <hr/>
        <div class="card-position">
        <div class="card2">
          <v-icon x-large color="green">mdi-paw</v-icon>
          <h3>ExoticPets</h3>
          <p class="texto-card">A ExoticPets é a maior rede de petshop de animais exóticos do Brasil, além de oferecer serviços de adoções tanto para animais exóticos quanto domésticos a ExoticPets foi a primiera rede de petshop a ganhar reconhecimento legal do IBAMA.</p>
       
        </div>
        
          <div class="card2">
        <v-icon x-large color="yellow">mdi-flag-variant</v-icon> 
        <h3>1944</h3>
           <p class="texto-card">A equipe de historiadores da 1944 é responsável por propagar conhecimento sobre a Segunda Guerra Mundial por todo o cenário da América do Sul. Responsável pela divulgação de documentos históricos e pela venda de livros e produtos da época.</p>
        
        </div>
          <div class="card2">
        <v-icon x-large color="purple">mdi-orbit</v-icon> 
        <h3>Empresa</h3>
           <p class="texto-card">Lorem ipsum dolor sit, amet consectetur Lorem ipsum dolor sit amet consectetur, adipisicing elit. Earum dolorum accusamus rerum fugit reprehenderit excepturi, aliquid tenetur veritatis quaerat aspernatur sit, impedit perferendis quia.</p>
       
        </div>
        </div>
      </section>            
        
      
  </body>

  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          title: 'Héstia 4.2.1-F',
          text: "Home Assistent 100% brasileira! ",
          subtext: 'Ganhadora de inúmeros prêmios.',
          img: '',
        },
      
      ],
      transparent: 'rgba(255, 255, 255, 0)',
    }),
  }
</script>

<style scoped>
.v-parallax{
  background-size: cover;
}
body{
font-family: 'Courier New', Courier, monospace;
padding: 0;
margin: 0;
}

section{
  margin: 80px 0px 90px 0px;
}
section>hr{
  margin:0 auto;
  width: 20%;
}

section > h2{
  text-align: center;
}

.texto{
  text-align:center; 
}

.card-position{
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: space-around;

}
.card, .card2 {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  margin: 50px 0px  10px 20px;
  text-align: center;
  background-color: white;
 
}
.texto-card{
  text-align: unset;
  padding: 0 15px;

}

.card{
  width:330px;
  height: 200px;
}
.card2{
  width: 300px;
  height: 400px;
}

.card2 button {
  border: none;
  outline: 0;
  padding: 12px;
  color: white;
  background-color: #000;
  text-align: center;
  cursor: pointer;
  width: 50%;
  font-size: 18px;
}

.card2 button:hover {
  opacity: 0.7;
}

@media(min-width:934px){
  .card-position{
  flex-direction: row;
  justify-content: center;
}
.txt-responsivo{
padding: 0 5px;
}


}


</style>