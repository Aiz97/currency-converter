<template>
  <div class="container">
    <div class="logo">
      <img src="./assets/logo.svg" alt="">
    </div>
    <h1>Конвертер валюты</h1>
    <div class="currency-cards">
      <div class="card">
        <h2>USD</h2>
        <p class="cards-rate">$ 1 = 432 KZT</p>
      </div>
      <div class="card">
        <h2>EURO</h2>
        <p class="cards-rate">	&#8364; 1 = 464 KZT</p>
      </div>
      <div class="card">
        <h2>РУБЛЬ</h2>
        <p class="cards-rate">	&#8381; 1 = 6.59 KZT</p>
      </div>
    </div>
    <div class="main-section">
      <div class="exchange-rate">
        <table>
          <tr class="gray-tr">
            <td>USD</td>
            <td>Доллар США</td>
            <td>432.07</td>
          </tr>
          <tr class="white-tr">
             <td>EUR</td>
            <td>Евро</td>
            <td>464.31</td>
          </tr>
          <tr class="gray-tr">
            <td>RUB</td>
            <td>Российский рубль</td>
            <td>6.59</td>
          </tr>
          <tr class="white-tr">
            <td>KGS</td>
            <td>Кыргызский сом</td>
            <td>5.30</td>
          </tr>
          <tr class="gray-tr">
            <td>UZS</td>
            <td>Узбекский сум</td>
            <td>0.04</td>
          </tr>
          <tr class="white-tr">
            <td>CNY</td>
            <td>Китайский юань</td>
            <td>64.51</td>
          </tr>
        </table>
      </div>
      <div class="converter">
        <span>Конвертировать из</span>
        <div class="container-from">
          <select name="first-currency" id="first-currency" v-model="currency_one">
            <option value="AED">AED</option>
            <option value="AFN">AFN</option>
            <option value="XCD">XCD</option>
            <option value="ALL">ALL</option>
            <option value="AMD">AMD</option>
            <option value="ANG">ANG</option>
            <option value="AOA">AOA</option>
            <option value="AQD">AQD</option>
            <option value="ARS">ARS</option>
            <option value="AUD">AUD</option>
            <option value="AZN">AZN</option>
            <option value="BAM">BAM</option>
            <option value="BBD">BBD</option>
            <option value="BDT">BDT</option>
            <option value="XOF">XOF</option>
            <option value="BGN">BGN</option>
            <option value="BHD">BHD</option>
            <option value="BIF">BIF</option>
            <option value="BMD">BMD</option>
            <option value="BND">BND</option>
            <option value="BOB">BOB</option>
            <option value="BRL">BRL</option>
            <option value="BSD">BSD</option>
            <option value="NOK">NOK</option>
            <option value="BWP">BWP</option>
            <option value="BYR">BYR</option>
            <option value="BZD">BZD</option>
            <option value="CAD">CAD</option>
            <option value="CDF">CDF</option>
            <option value="XAF">XAF</option>
            <option value="CHF">CHF</option>
            <option value="CLP">CLP</option>
            <option value="CNY">CNY</option>
            <option value="COP">COP</option>
            <option value="CRC">CRC</option>
            <option value="CUP">CUP</option>
            <option value="CVE">CVE</option>
            <option value="CYP">CYP</option>
            <option value="CZK">CZK</option>
            <option value="DJF">DJF</option>
            <option value="DKK">DKK</option>
            <option value="DOP">DOP</option>
            <option value="DZD">DZD</option>
            <option value="ECS">ECS</option>
            <option value="EEK">EEK</option>
            <option value="EGP">EGP</option>
            <option value="ETB">ETB</option>
            <option value="EUR">EUR</option>
            <option value="FJD">FJD</option>
            <option value="FKP">FKP</option>
            <option value="GBP">GBP</option>
            <option value="GEL">GEL</option>
            <option value="GGP">GGP</option>
            <option value="GHS">GHS</option>
            <option value="GIP">GIP</option>
            <option value="GMD">GMD</option>
            <option value="GNF">GNF</option>
            <option value="GTQ">GTQ</option>
            <option value="GYD">GYD</option>
            <option value="HKD">HKD</option>
            <option value="HNL">HNL</option>
            <option value="HRK">HRK</option>
            <option value="HTG">HTG</option>
            <option value="HUF">HUF</option>
            <option value="IDR">IDR</option>
            <option value="ILS">ILS</option>
            <option value="INR">INR</option>
            <option value="IQD">IQD</option>
            <option value="IRR">IRR</option>
            <option value="ISK">ISK</option>
            <option value="JMD">JMD</option>
            <option value="JOD">JOD</option>
            <option value="JPY">JPY</option>
            <option value="KES">KES</option>
            <option value="KGS">KGS</option>
            <option value="KHR">KHR</option>
            <option value="KMF">KMF</option>
            <option value="KPW">KPW</option>
            <option value="KRW">KRW</option>
            <option value="KWD">KWD</option>
            <option value="KYD">KYD</option>
            <option value="KZT">KZT</option>
            <option value="LAK">LAK</option>
            <option value="LBP">LBP</option>
            <option value="LKR">LKR</option>
            <option value="LRD">LRD</option>
            <option value="LSL">LSL</option>
            <option value="LTL">LTL</option>
            <option value="LVL">LVL</option>
            <option value="MAD">MAD</option>
            <option value="MDL">MDL</option>
            <option value="MGA">MGA</option>
            <option value="MKD">MKD</option>
            <option value="MMK">MMK</option>
            <option value="MNT">MNT</option>
            <option value="MOP">MOP</option>
            <option value="MRO">MRO</option>
            <option value="MTL">MTL</option>
            <option value="MUR">MUR</option>
            <option value="MVR">MVR</option>
            <option value="MWK">MWK</option>
            <option value="MXN">MXN</option>
            <option value="MYR">MYR</option>
            <option value="MZN">MZN</option>
            <option value="NAD">NAD</option>
            <option value="XPF">XPF</option>
            <option value="NGN">NGN</option>
            <option value="NIO">NIO</option>
            <option value="NPR">NPR</option>
            <option value="NZD">NZD</option>
            <option value="OMR">OMR</option>
            <option value="PAB">PAB</option>
            <option value="PHP">PHP</option>
            <option value="PKR">PKR</option>
            <option value="PLN">PLN</option>
            <option value="PYG">PYG</option>
            <option value="QAR">QAR</option>
            <option value="RON">RON</option>
            <option value="RSD">RSD</option>
            <option value="RUB">RUB</option>
            <option value="RWF">RWF</option>
            <option value="SAR">SAR</option>
            <option value="SBD">SBD</option>
            <option value="SCR">SCR</option>
            <option value="SDG">SDG</option>
            <option value="SEK">SEK</option>
            <option value="SGD">SGD</option>
            <option value="SKK">SKK</option>
            <option value="SLL">SLL</option>
            <option value="SOS">SOS</option>
            <option value="SRD">SRD</option>
            <option value="STD">STD</option>
            <option value="SVC">SVC</option>
            <option value="SYP">SYP</option>
            <option value="SZL">SZL</option>
            <option value="THB">THB</option>
            <option value="TJS">TJS</option>
            <option value="TMT">TMT</option>
            <option value="TND">TND</option>
            <option value="TOP">TOP</option>
            <option value="TRY">TRY</option>
            <option value="TTD">TTD</option>
            <option value="TWD">TWD</option>
            <option value="TZS">TZS</option>
            <option value="UAH">UAH</option>
            <option value="UGX">UGX</option>
            <option value="USD">USD</option>
            <option value="UYU">UYU</option>
            <option value="UZS">UZS</option>
            <option value="VEF">VEF</option>
            <option value="VND">VND</option>
            <option value="VUV">VUV</option>
            <option value="YER">YER</option>
            <option value="ZAR">ZAR</option>
            <option value="ZMK">ZMK</option>
            <option value="ZWD">ZWD</option>
          </select>
          <input type="number" id="amount-one" v-model="amountOne" @input="fetchData()">
        </div>
        <div class="switch-container">
          <button @click="switchValues()">&#9650;	&#9660;</button>
          <h4 id="baseValue" >1 {{ currency_two }} = {{rate}} {{currency_one}}</h4>
        </div>
        <span>Конвертировать в</span>
        <div class="container-to">
          <select name="second-currency" id="second-currency" v-model="currency_two">
            <option value="AED">AED</option>
            <option value="AFN">AFN</option>
            <option value="XCD">XCD</option>
            <option value="ALL">ALL</option>
            <option value="AMD">AMD</option>
            <option value="ANG">ANG</option>
            <option value="AOA">AOA</option>
            <option value="AQD">AQD</option>
            <option value="ARS">ARS</option>
            <option value="AUD">AUD</option>
            <option value="AZN">AZN</option>
            <option value="BAM">BAM</option>
            <option value="BBD">BBD</option>
            <option value="BDT">BDT</option>
            <option value="XOF">XOF</option>
            <option value="BGN">BGN</option>
            <option value="BHD">BHD</option>
            <option value="BIF">BIF</option>
            <option value="BMD">BMD</option>
            <option value="BND">BND</option>
            <option value="BOB">BOB</option>
            <option value="BRL">BRL</option>
            <option value="BSD">BSD</option>
            <option value="NOK">NOK</option>
            <option value="BWP">BWP</option>
            <option value="BYR">BYR</option>
            <option value="BZD">BZD</option>
            <option value="CAD">CAD</option>
            <option value="CDF">CDF</option>
            <option value="XAF">XAF</option>
            <option value="CHF">CHF</option>
            <option value="CLP">CLP</option>
            <option value="CNY">CNY</option>
            <option value="COP">COP</option>
            <option value="CRC">CRC</option>
            <option value="CUP">CUP</option>
            <option value="CVE">CVE</option>
            <option value="CYP">CYP</option>
            <option value="CZK">CZK</option>
            <option value="DJF">DJF</option>
            <option value="DKK">DKK</option>
            <option value="DOP">DOP</option>
            <option value="DZD">DZD</option>
            <option value="ECS">ECS</option>
            <option value="EEK">EEK</option>
            <option value="EGP">EGP</option>
            <option value="ETB">ETB</option>
            <option value="EUR">EUR</option>
            <option value="FJD">FJD</option>
            <option value="FKP">FKP</option>
            <option value="GBP">GBP</option>
            <option value="GEL">GEL</option>
            <option value="GGP">GGP</option>
            <option value="GHS">GHS</option>
            <option value="GIP">GIP</option>
            <option value="GMD">GMD</option>
            <option value="GNF">GNF</option>
            <option value="GTQ">GTQ</option>
            <option value="GYD">GYD</option>
            <option value="HKD">HKD</option>
            <option value="HNL">HNL</option>
            <option value="HRK">HRK</option>
            <option value="HTG">HTG</option>
            <option value="HUF">HUF</option>
            <option value="IDR">IDR</option>
            <option value="ILS">ILS</option>
            <option value="INR">INR</option>
            <option value="IQD">IQD</option>
            <option value="IRR">IRR</option>
            <option value="ISK">ISK</option>
            <option value="JMD">JMD</option>
            <option value="JOD">JOD</option>
            <option value="JPY">JPY</option>
            <option value="KES">KES</option>
            <option value="KGS">KGS</option>
            <option value="KHR">KHR</option>
            <option value="KMF">KMF</option>
            <option value="KPW">KPW</option>
            <option value="KRW">KRW</option>
            <option value="KWD">KWD</option>
            <option value="KYD">KYD</option>
            <option value="KZT">KZT</option>
            <option value="LAK">LAK</option>
            <option value="LBP">LBP</option>
            <option value="LKR">LKR</option>
            <option value="LRD">LRD</option>
            <option value="LSL">LSL</option>
            <option value="LTL">LTL</option>
            <option value="LVL">LVL</option>
            <option value="MAD">MAD</option>
            <option value="MDL">MDL</option>
            <option value="MGA">MGA</option>
            <option value="MKD">MKD</option>
            <option value="MMK">MMK</option>
            <option value="MNT">MNT</option>
            <option value="MOP">MOP</option>
            <option value="MRO">MRO</option>
            <option value="MTL">MTL</option>
            <option value="MUR">MUR</option>
            <option value="MVR">MVR</option>
            <option value="MWK">MWK</option>
            <option value="MXN">MXN</option>
            <option value="MYR">MYR</option>
            <option value="MZN">MZN</option>
            <option value="NAD">NAD</option>
            <option value="XPF">XPF</option>
            <option value="NGN">NGN</option>
            <option value="NIO">NIO</option>
            <option value="NPR">NPR</option>
            <option value="NZD">NZD</option>
            <option value="OMR">OMR</option>
            <option value="PAB">PAB</option>
            <option value="PHP">PHP</option>
            <option value="PKR">PKR</option>
            <option value="PLN">PLN</option>
            <option value="PYG">PYG</option>
            <option value="QAR">QAR</option>
            <option value="RON">RON</option>
            <option value="RSD">RSD</option>
            <option value="RUB">RUB</option>
            <option value="RWF">RWF</option>
            <option value="SAR">SAR</option>
            <option value="SBD">SBD</option>
            <option value="SCR">SCR</option>
            <option value="SDG">SDG</option>
            <option value="SEK">SEK</option>
            <option value="SGD">SGD</option>
            <option value="SKK">SKK</option>
            <option value="SLL">SLL</option>
            <option value="SOS">SOS</option>
            <option value="SRD">SRD</option>
            <option value="STD">STD</option>
            <option value="SVC">SVC</option>
            <option value="SYP">SYP</option>
            <option value="SZL">SZL</option>
            <option value="THB">THB</option>
            <option value="TJS">TJS</option>
            <option value="TMT">TMT</option>
            <option value="TND">TND</option>
            <option value="TOP">TOP</option>
            <option value="TRY">TRY</option>
            <option value="TTD">TTD</option>
            <option value="TWD">TWD</option>
            <option value="TZS">TZS</option>
            <option value="UAH">UAH</option>
            <option value="UGX">UGX</option>
            <option value="USD">USD</option>
            <option value="UYU">UYU</option>
            <option value="UZS">UZS</option>
            <option value="VEF">VEF</option>
            <option value="VND">VND</option>
            <option value="VUV">VUV</option>
            <option value="YER">YER</option>
            <option value="ZAR">ZAR</option>
            <option value="ZMK">ZMK</option>
            <option value="ZWD">ZWD</option>
          </select>
          <input type="number"  id="amount-two" placeholder="0" v-model="amountTwo" disabled>
      </div>
    </div>
  </div>
</div>
</template>

<script>
  export default {
    data() {
      return{
        data: [],
        currency_one: "KZT",
        currency_two: "USD",
        rate: "",
        amountOne: 10000,
        amountTwo: 0,
      }
    },
    methods: {
      fetchData() {
        fetch(`https://v6.exchangerate-api.com/v6/3cf4b37ef50ffad0a8ace165/latest/${this.currency_two}`)
        .then(res => res.json())
        .then(data => {
          this.data = data;
          this.rate = data.conversion_rates[this.currency_one];
          this.amountTwo = (this.amountOne / this.rate).toFixed(2);
          
        });
      },
      switchValues(){
        const temporaryValue = this.currency_one
        this.currency_one = this.currency_two
        this.currency_two = temporaryValue;
        this.fetchData();
      }
    },
    mounted(){
      this.fetchData();
    }
  }
</script>

<style>
#app {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  color:black;
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
}
.container{
  margin: 0 5rem;
}
h2 {
  font-size: 1.5rem;
  font-weight: 300;
}
.cards-rate{
  font-size: 1.5rem;
  font-weight: 600;
  margin-top: 6rem;
}
.currency-cards {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.card { 
  width: 336px;
  height: 209.32px;
  padding: 1rem;
  color: white;
  background: linear-gradient(to right top, #000000, #000000,#1A7579);
  border-radius: 10px;
  
}
table {
  width: 600px;
  height: 530px;
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  border-collapse: collapse;
  justify-content: center;
  text-align: center;
  background: #000000;
  color: white;
  border: #1A7579 1px solid;
  
}
tr, td{
  border-radius: 7px;
}
.gray-tr {
  background: #0c5a5f;
}
.main-section{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-top: 4rem;
}
span{
  color:gray;
}
.switch-container{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
}
.switch-container button {
  padding: 3px;
  font-size: 1.2rem;
  background-color: black;
  color: white;
  width: 150px;
  height: 40px;
  cursor: pointer;
}
.switch-container button:hover{
  background-color: #1A7579;
  color:black;
  transition: ease-in-out .3s;
}
.container-from, .container-to{
  width: 600px;
  height: 188px;
  margin-top: 10px;
  margin-bottom: 10px;
  box-shadow: 0px 4px 25px rgba(0, 0, 0, 0.25);
  border-radius: 5px;
  color: white;
  background: linear-gradient(to right top, #000000, #000000,#1A7579);
}
select{
  width: 250px;
  height: 36px;
  border: none;
  background: 0;
  font-size: 1.5rem;
  margin: 30px 30px;
  color: white;
}
option{
  background: black;
}
input{
  width: 500px;
  height: 40px;
  margin: 30px 30px;
  border: 1px solid black;
  border-radius: 6px;
}
input[type="number"]:disabled {
  background: white;
}
@media screen and (max-width: 768px){
  .container {
    margin: 0 3rem;
  }
  .currency-cards {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .card { 
    width: 250px;
    height: 200px;
  }
  .main-section {
    display: flex;
    flex-direction: column;
  }
  table{
    max-width: 300px;
  }
  .switch-container button {
    padding: 1px;
    width: 100px;
  }
  .container-from, .container-to{
    max-width: 300px;
  }
  input{
    max-width: 250px;
  }
}

</style>
