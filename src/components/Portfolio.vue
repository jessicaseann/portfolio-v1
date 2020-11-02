<template>
  <div class="homepage" :style="{'background-color':'#FBF0ED'}">
    <v-container class="ma-0 pa-0">
      <div class="section fp-auto-height-responsive" :style="{'background-color':'#FBF0ED', 'background-image': `url(${require(`@/assets/profilepic.png`)})`, 'background-size': 'auto 768px' }">
          <v-container fill-height fluid>
            <v-row style="height: 768px; min-height:768px">
                <v-col class="ma-0 pa-0" cols="1" md="6" lg="5"/>
                <v-col class="ma-0 pa-0" cols="11" md="6" lg="7">
                    <v-row class="ma-0 pa-0" style="height: 65%; " >
                        <v-col cols="12" sm="4" md="4">
                          <v-container style="padding-top: 50px">
                            <template v-for="(item, index) in navOption">
                                <p :key="index"><span class="font-weight-medium" style="font-size:18px">{{item}}</span></p>
                            </template>
                          </v-container> 
                            
                        </v-col>
                        <v-col class="hidden-sm-and-down" cols="0" sm="" md="8" fill-height> 
                          <v-container style="padding-top: 50px;">
                            <p style="font-size:16px"> Hello, I'm Jessica based in Jakarta, Indonesia. A one-part coder, one part traveller and an analog film enthusiasts. I really really enjoy taking flights, eat and taking random photos. Since, I can't sit still in my long holiday and I stuck at home because of the COVID-19 stuff, so I gather all my free-time to build my own portfolio website. <br> <br> Welcome here!</p>
                          </v-container>
                        </v-col>
                    </v-row>
                    <v-row class="ma-0 pa-0" style="height: 35%; padding-right=36px;">
                        <p text-align: right style="margin: 0"><span class="font-weight-bold"
                            style="font-size:100px; line-height: 1em; letter-spacing: 6px; ">Jessica Sean</span></p>
                    </v-row>
                </v-col>
            </v-row>
          </v-container>
      </div>


    </v-container>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  components: {},
  props: {
    msg: String,
  },
  data () {
        return {
            navOption: [
                'Home',
                'About Me',
                'Projects',
                'Contacts'
            ]
        }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
