<template>
    <div class="shimmer-wrapper">
        <div class="shimmer shimmer_heading"></div>
        <div class="shimmer shimmer_small_para"></div>
        <div class="shimmer shimmer_small_para"></div>
        <div class="shimmer shimmer_small_para"></div>
        <div class="shimmer shimmer_small_para"></div>
        <div class="shimmer shimmer_small_para"></div>
        <div class="shimmer shimmer_small_para"></div>
    </div>
</template>

<script>
export default {
  name: 'Shimmer'
}
</script>


<style>
    .shimmer-wrapper {
        bottom: 0;
        left: 0;
        position: absolute;
        right: 0;
        top: 0;
        align-items: center;
        display: block;
        justify-content: center;
        overflow: hidden;
        z-index: 9999;
    }
    .shimmer {
        margin-top:12px;
        background: #f6f7f8;
        /* fallback
        background-image: linear-gradient(to right, #f6f7f8 0%, #edeef1 20%, #f6f7f8 40%, #f6f7f8 100%);
        background-repeat: no-repeat;
        */
        animation : shim infinite 1.2s linear;
    }
    @keyframes shim {
        0% { background-position: -468px 0;}
        100% { background-position: 468px 0;}
    }
    .shimmer_circle {
        width:80px;
        height:80px;
        border-radius:80px;
    }
    .shimmer_circle_heading .shimmer_heading{
        width : 90%;
        margin-left:3%
    }
    .shimmer_circle_heading {
        display: flex;
        align-items : center
    }
    .shimmer_heading {
        width:50%;
        height:20px;
        margin-top : 18px;
    }
    .shimmer_small_para {
        height:24px;

    }
    .shimmer_large_para {
        height:48px;
    }

</style>