          <script setup>

          import { ref, onMounted, computed } from 'vue';
          // import { getOrderNumber, getCurrentDate, getOrders, calculateTotalPrice } from 'vue';
          // 데이터 파일을 가져옵니다.
          import ReceiptBox from "../components/Receipt/ReceiptBox.vue";
          import BigNumber from "../components/Receipt/BigNumber.vue";
          import ReceiptFix from "../components/Receipt/ReceiptFix.vue";


          // const OrderNumber = ref('');
          // const CurrentDate = ref('');
          // const Orders = ref([]);


          // 데이터로드

          // onMounted(async () => {
          //   orderNumber.value = await getOrderNumber();
          //   currentDate.value = await getCurrentDate();
          //   orders.value = await getOrders();
          // });

          //총 가격 계산
          // const totalPrice = computed(() => calculateTotalPrice(orders.value));


</script>

  <template>
    <div class="container">
      <ReceiptBox>
    <div class="Receipt">
      <div class="dot">RECEIPT</div>
      <div class="OrderD"></div>
      <div class="OrderD">
        <div>주문서 #</div>
        <div class="SmallNumber">
          <div>253</div>
        </div>

        <div class="order-date">
          <div>2024-06-10</div>
        </div>
      </div>

      <div class="items">
        <ul>
          <li class="menuName">
            1.아이스 아메리카노
          </li>
          <li class="menuQuantity">
            1잔
          </li>
          <li class="menuPrice">
            5,000 원
          </li>
        </ul>
      </div>
      <div class="total">
        <p>
          <strong>TOTAL</strong>
        <div class="price">23000원</div>
        </p>
    </div>
      </div>
    </ReceiptBox>  
        <div class="logo1">cafe.js</div>
        <div class="logo2">cafe.js</div>
    </div>

    



      <!-- 주문서 번호와 날짜 -->
      <!-- <div class="order-info">
                <div class="order-number">{{ orderNumber }}</div>
                <div class="order-date">{{ currentDate }}</div>
              </div> -->

      <!-- 영수증 박스 -->

  </template>

<style>
.container {
    position: relative;
    width: 1080px;
    height: 1920px;
    margin: auto;
    background: linear-gradient(180deg,
            #5e7153 20%,
            #af9544 50%,
            #d7a63c 75%,
            #ffb834 100%);
}

.logo2 {
    position: relative;
    top: -165px;
    left: 320px;
    /* right:50px; */
    /* bottom:1729px; */
    margin: center;
    width: 394px;
    height: 146px;
    font-family: "DNF Bit Bit v2";
    font-style: normal;
    font-weight: 100;
    font-size: 60px;
    line-height: 146px;
    text-align: center;

    color: #ffb834;
}

.logo1 {
    position: relative;
    top: 80px;
    left: 310px;
    margin: center;
    width: 394px;
    height: 146px;
    font-family: "DNF Bit Bit v2";
    font-style: normal;
    font-weight: 100;
    font-size: 60px;
    line-height: 146px;
    text-align: center;

    color: #783e19;
}
.receipt {

  position: relative;
  width: 306px;
  height: 124px;
  font-family: 'BM JUA_TTF';
  font-style: normal;
  font-weight: 400;
  font-size: 120px;
  line-height: 124px;
  display: flex;
  align-items: center;
  text-align: center;
  color: #282808;
}



.receipt-header {
  position: relative;
  width: 626px;
  height: 0px;
  border: 5px dashed #797979;
}

.dashed-line {
  position: relative;
  width: 626px;
  height: 0px;
  border: 5px dashed #959595;
}

.order-info {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}

.order-number,
.order-date {
  font-weight: bold;
}

.order-number {
  text-align: left;
}

/* 2024-06-12 */
.order-date {
  position: relative;
  width: flex;
  height: 36px;
  font-family: 'BM JUA_TTF';
  font-style: normal;
  font-size: 35px;
  line-height: flex;
  display: flex;
  align-items: center;
  text-align: right;
  color: #949494;
}
</style>
