<template>
  <div class="card">
    <div class="card__top">
        <svg class="" width="34" height="34" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"></path></svg>
        <div class="card__links">
            <a :href="item.source" target="_blank" class="icon">
                <svg class="source-code" fill="currentColor" width="24" height="24" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12.316 3.051a1 1 0 01.633 1.265l-4 12a1 1 0 11-1.898-.632l4-12a1 1 0 011.265-.633zM5.707 6.293a1 1 0 010 1.414L3.414 10l2.293 2.293a1 1 0 11-1.414 1.414l-3-3a1 1 0 010-1.414l3-3a1 1 0 011.414 0zm8.586 0a1 1 0 011.414 0l3 3a1 1 0 010 1.414l-3 3a1 1 0 11-1.414-1.414L16.586 10l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
            </a>
            <a :href="item.link" target="_blank" class="icon">
                <svg class="external-link" fill="currentColor" width="24" height="24" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M11 3a1 1 0 100 2h2.586l-6.293 6.293a1 1 0 101.414 1.414L15 6.414V9a1 1 0 102 0V4a1 1 0 00-1-1h-5z"></path><path d="M5 5a2 2 0 00-2 2v8a2 2 0 002 2h8a2 2 0 002-2v-3a1 1 0 10-2 0v3H5V7h3a1 1 0 000-2H5z"></path></svg>
            </a>
        </div>
    </div>
    <div class="card__content">
        <h3 class="card__title">{{ item.title }}</h3>
        <p class="card__description">{{ item.description }}</p>
    </div>
    <div class="card__bottom">
        <p class="card__bottom-tech">{{ item.tech }}</p>
    </div>
  </div>
</template>

<script>
export default {
props: {
    item: Object
}
}
</script>

<style lang="scss" scoped>
.card {
   background: $light;
   color: $white;
   padding: 2rem 1.75rem;
   border-radius: 8px;
   transition: all 0.2s ease;

   &:hover {
       transform: translateY(-2px);
       transform-origin: center;
       box-shadow: 0px 4px 20px rgba(0,0,0,0.4);
   }
}

.card__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;

    .card__links {
        display: flex;

        & > .icon:first-child {
            margin-right: 1rem;
        }
    }
}

.card__content {
    line-height: 1.6rem;

    & > * {
        margin-bottom: 0.75rem;
    }

    .card__title {
        font-size: clamp(1.5rem, 2vw, 2rem);
        font-weight: 500;
        
    }

    .card__description {

    }
}

.card__bottom {
    font-size: 0.85rem;
    opacity: 0.4;
}
</style>