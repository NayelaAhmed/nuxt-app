<template>
    <div>
        <div class="card">
         <!-- displaying the card data    -->
            
            <img :src="movieData.Poster" class="card-img-top">
            <div class="card-body">
                <h2 class="card-text">Title: {{movieData.Title}}</h2>
                  <p class="card-text">Year: {{ movieData.Year }}</p>
                  <p class="card-text">Plot: {{ movieData.Plot }}</p>  
            </div>
        </div>
    </div>
</template>



<script>


// setting up the props for the attributes and prop validation
export default {
    props: {
        movieData: {
            type: Object,
            required: true,
            default: () => {}
        }
    },

    
}
</script>