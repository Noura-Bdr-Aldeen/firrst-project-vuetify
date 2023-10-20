    <template>
  <v-container >
    <div class="text-h3 ma-8">OUR TEAM</div>
    <v-divider class="border-opacity-75 mb-6" color="secondary"></v-divider>
    <v-row align="center" justify="center">
    
      <v-col
        v-for="(variant, i) in variants"
        :key="i"
        cols="auto"
      >
      
        <v-card
          class="mx-auto"
          max-width="344"
          :color="color"
          :variant="variant"
        >
          <v-card-item>
        
                                
                  <div class="text-h6 mb-1 bg-brown">
            employee
              </div>
              <div >Lorem ipsum dolor sit amet consectetur sit amet consectetur </div>
           
          </v-card-item>

          <v-card-actions>
           <v-btn>
            <v-icon icon="mdi-phone" color="secondary"></v-icon>connect</v-btn>
           
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
  import { ref } from 'vue'
const variants = ['outlined', 'outlined', 'outlined', 'outlined','outlined', 'outlined']
  
</script>
