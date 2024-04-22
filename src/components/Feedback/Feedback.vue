<template>
  <section class="feedback feedback__wrapper">
   <div class="container feedback__container">
     <div class="feedback__preview-wrapper">
       <img src="@/assets/images/feedback/customer_block.png" alt="Feedback" class="feedback__preview-image">
     </div>
     <div>
       <h2 class="feedback__title title">What do customers say about us?</h2>
       <article class="feedback__article">
         <div class="feedback__article-wrapper">
           <div class="feedback__customer-image-wrapper">
             <img src="@/assets/images/feedback/customer_profile.png" alt="Customer" class="feedback__customer-image">
           </div>
           <div>
             <p class="feedback__customer-name">Hiroshi</p>
             <div class="feedback__customer-location description">Tokyo, Japan</div>
           </div>
         </div>
         <p class="feedback__text description">Very satisfying service makes it comfortable, a beautiful place in the world.</p>
         <div class="feedback__rating">
           <img src="@/assets/images/feedback/rating_star.svg" alt="Rating" class="feedback__rating-img">
           <img src="@/assets/images/feedback/rating_star.svg" alt="Rating" class="feedback__rating-img">
           <img src="@/assets/images/feedback/rating_star.svg" alt="Rating" class="feedback__rating-img">
           <img src="@/assets/images/feedback/rating_star.svg" alt="Rating" class="feedback__rating-img">
           <img src="@/assets/images/feedback/rating_star.svg" alt="Rating" class="feedback__rating-img">
         </div>
       </article>
     </div>
   </div>
  </section>
</template>

<style lang="scss">
  @import "@/assets/styles/feedback.scss";
</style>
<script setup lang="ts">
</script>
