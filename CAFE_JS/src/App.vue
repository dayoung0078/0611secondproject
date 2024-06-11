<script setup>
// import { RouterLink, RouterView } from 'vue-router';

// 영수증 컴포넌트를 가져옵니다.
import OrderReceipt from "./components/OrderReceipt.vue";
</script>


<template>

  <OrderReceipt>
    <Bar>
      <ReceiptBox>
    </ReceiptBox>
    </Bar>
      <ReceiptFix>
        <BigNumber>
        </BigNumber>
      </ReceiptFix>
  </OrderReceipt>



    <!-- <RouterLink to="/OrderReceipt">영수증</RouterLink>
    <br>
    <RouterLink to="/">home</RouterLink>
  </div>  
    <RouterView /> -->

</template>



<style scoped>

</style>

