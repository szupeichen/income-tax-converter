<template>
  <div class="app">
    <!-- 上區塊 -->
    <div class="upper-section">
      <h2>基本資訊</h2>
      <form>
        <label for="name">姓名:</label>
        <input type="text" id="name" v-model="formData.name" placeholder="請輸入姓名" />

        <label for="idNumber">身分證字號:</label>
        <input type="text" id="idNumber" v-model="formData.idNumber" placeholder="請輸入身分證字號" />

        <label for="houseAddress">戶籍地址:</label>
        <input type="text" id="houseAddress" v-model="formData.houseAddress" placeholder="請輸入戶籍地址" />

        <label for="contactAddress">通訊地址:</label>
        <input type="text" id="contactAddress" v-model="formData.contactAddress" placeholder="請輸入通訊地址" />
      </form>
    </div>

    <!-- 下區塊 -->
    <div class="lower-section">
      <h2>交易資訊</h2>
      <form>
        <label for="saleAddress">出售地址:</label>
        <input type="text" id="saleAddress" v-model="formData.saleAddress" placeholder="請輸入出售地址" />

        <label for="buildingShare">建物持分:</label>
        <input type="text" id="buildingShare" v-model="formData.buildingShare" placeholder="請輸入建物持分" />

        <label for="acquisitionDate">取得日期:</label>
        <input type="date" id="acquisitionDate" v-model="formData.acquisitionDate" />

        <label for="acquisitionPrice">取得價格:</label>
        <input type="number" id="acquisitionPrice" v-model="formData.acquisitionPrice" placeholder="請輸入取得價格" />

        <label for="saleNumber">出售地號:</label>
        <input type="text" id="saleNumber" v-model="formData.saleNumber" placeholder="請輸入出售地號" />

        <label for="landShare">土地持分:</label>
        <input type="text" id="landShare" v-model="formData.landShare" placeholder="請輸入土地持分" />

        <label for="acquisitionCost">取得成本 ZA1:</label>
        <input type="number" id="acquisitionCost" v-model="formData.acquisitionCost" placeholder="請輸入取得成本" />
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        name: "",
        idNumber: "",
        houseAddress: "",
        contactAddress: "",
        saleAddress: "",
        buildingShare: "",
        acquisitionDate: "",
        acquisitionPrice: null,
        saleNumber: "",
        landShare: "",
        acquisitionCost: null,
      },
    };
  },
};
</script>

<style>
.app {
  font-family: Arial, sans-serif;
  padding: 20px;
}

.upper-section,
.lower-section {
  margin-bottom: 20px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
}

h2 {
  margin-bottom: 10px;
}

form {
  display: flex;
  flex-direction: column;
}

label {
  margin-top: 10px;
  font-weight: bold;
}

input {
  margin-top: 5px;
  padding: 8px;
  font-size: 14px;
  border: 1px solid #ccc;
  border-radius: 4px;
}
</style>
