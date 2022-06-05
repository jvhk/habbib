<template>
  <div id="main-div">
		<v-app id="app">
		<v-container>
					<v-row>
						<v-col>

								<v-switch  v-model="switch1" color="brown" label="Habbibizar" @click="habbibiza()"> eu sou o switch</v-switch>

						</v-col>
					</v-row>
					<v-row>
						<v-card >
							<template>
								<v-img v-show="habbibizar" max-height="500" max-width="500" src="https://pbs.twimg.com/media/FUVxbPvXoAA5Asn?format=jpg&name=small"/>
								<v-img v-show="!habbibizar" max-height="500" max-width="800" src="https://pbs.twimg.com/media/FQa8osLWYAYQaNi?format=jpg&name=small"/>
							</template>
						</v-card>
					</v-row>
		</v-container>
		</v-app>
	</div>
</template>

<script>

export default {
  name: 'Habbib',
  props: {

  },
	data() {
		return {
			switch1: false,
			habbibizar: false,
		}
	},
	methods:{
		habbibiza(){
			this.habbibizar = !this.habbibizar;
		}
	}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >

body{
	background-color: antiquewhite;
}

#main-div{
	display: flex;
	justify-content: center;
  margin-left: auto;
  margin-right: auto;
  width: 40%;
}

#app{
	background-color: antiquewhite;
}

.row{
	display: flex;
	justify-content: center;
	margin: 0px;
}

.col{
	display: contents;
}

.v-input{
	display: flex;
	justify-content: center;
}

.container{
	max-width: fit-content;
	background-color: none;
}

</style>
