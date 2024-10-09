<!-- <script>
import axios from 'axios';
axios.defaults.baseURL = `http://localhost:3005`;

export default {
	data() {
		return {
			maps:[],
		};
	},
  mounted() {
		this.card();
  },
  methods: {
  async card(){
    let response = await axios.get(`/card`);
    this.maps = response.data
    }
  },
  
}

</script> -->

<template>
  
        <h1 id="text_main">Best Sekling Plants</h1>
        <p class="text_pob">
          Easist way to healthy life by buying your favorite plants
        </p>
  
    <div class="bloc_flex" id="Products">

    <!-- <div class="Bloc_img_card">
      <div class="bloc_in_bloc" v-for="(card,index) in maps">
        <div class="bloc_img_main">
          <img :src="'src/assets/'+ card.image + '.png' "  title="" alt="" id="img_main" />
        </div>
        <div class="bloc_text_img">
          <p class="text_img">{{ card.title }}</p>
        </div>
        <div class="bloc_number">
          <p class="Number">$ {{ card.gold }}</p>
        </div>
      </div>
    </div> -->

    <div class="Bloc_img_card">
      <div class="bloc_in_bloc">
        <div class="bloc_img_main">
          <img src="../assets/Res3.png"  title="" alt="" id="img_main" />
        </div>
        <div class="bloc_text_img">
          <p class="text_img">Natural Plants</p>
        </div>
        <div class="bloc_number">
          <p class="Number">$ 1400</p>
        </div>
      </div>
    </div>

    <div class="Bloc_img_card">
      <div class="bloc_in_bloc">
        <div class="bloc_img_main">
          <img src="../assets/Res2.png"  title="" alt="" id="img_main" />
        </div>
        <div class="bloc_text_img">
          <p class="text_img">Artificial Plants</p>
        </div>
        <div class="bloc_number">
          <p class="Number">$ 900</p>
        </div>
      </div>
    </div>

    <div class="Bloc_img_card">
      <div class="bloc_in_bloc">
        <div class="bloc_img_main">
          <img src="../assets/Res1.png"  title="" alt="" id="img_main" />
        </div>
        <div class="bloc_text_img">
          <p class="text_img">Artificial Plants</p>
        </div>
        <div class="bloc_number">
          <p class="Number">$ 3500</p>
        </div>
      </div>
    </div>
  </div>

  <div class="raz"></div>
</template>
 
<style scoped>
.raz {
  margin: 120px;
}

.bloc_flex {
  display: flex;
  margin: 0 auto;
  max-width: 1200px;
}

.Bloc_img_card {
  display: flex;
}


.bloc_in_bloc {
  display: block;
  margin: 20px 75px 0px 35px;
}

.bloc_text_main {
  width: 350px;
  height: 100px;
}

#text_main {
  font-weight: 650;
  font-size: 46px;
  text-align: center;
}

.bloc_text_pob {
  margin: 15px 0px;
  width: 255px;
}

.text_pob {
  font-size: 23px;
  text-align: center;
}

.bloc_text_img {
  margin: 10px 0px;
}

.text_img {
  font-weight: 600;
  font-size: 23px;
  margin: 0px;
}

/* .bloc_number{
  
} */

.Number {
  font-size: 18px;
  color: rgb(144, 138, 138);
}

img {
  height: 436px;
  width: 300px;
  border-radius: 15px;
}
</style>