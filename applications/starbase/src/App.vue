<<template>
<div id="app">
    <h3>{{title}}</h3>
    <div class="col-md-12">
        <character 
        v-for="(id,index) in initial_ids"
        :id="1" 
        key="index"
        />
    </div>
</div>
</template>
<<script>
import Character from './components/Character.vue'
export default{
    name: 'app',
    data(){
        return {
            title: 'Genearate Your Team',
            initial_ids:[1,13,14]
        }
    },
    components:{
      Character
    }
}
</script>
