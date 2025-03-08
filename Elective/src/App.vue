<script setup>
   // var, let, const
   let str1 = "Hello 'world'"
    let str2 = 'Hello "world"'
    var num2 = 2
    const num3 = 3

    let str = `Hello ${num3 + num2} test ${num3} `
    console.log(str1)
    console.log(str2)
    console.log(num2)
    console.log(num3)
    console.log(str)

    let supplier1 = {
        name: 'JMR',
        number: '099-3333-902',
        address: {
            street: 'National HighWay',
            provice: 'davao del sur',
            zipcode: '8002',
        }
    }

    let supplier2 = {
        name: 'J&J',
        number: '099-1111-222',
        address: {

        }

    }


    console.log('supplier1 name :' + supplier1.name)
    console.log('supplier1 address :' + supplier1.address.street)
    console.log('supplier2 name :' + supplier2.name)
    console.log('supplier2 address : ' + (supplier2?.address?.street || "no address"))




</script>


<template>
  <div>
    <span>test</span>
    <h1> CALENDAR</h1>
    <h1> Febuary 2025</h1>
    <br>
    <div v-for="i in 10" :key="i">
      item - {{ i }}
    </div>


    <div class="calendar-container">
      <div class="flex-container">
        <div>SUN</div>
        <div>MON</div>
        <div>TUE</div>
        <div>WED</div>
        <div>THUR</div>
        <div>FRI</div>
        <div>SAT</div>
      </div>

      <div class="flex-container">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
        <div>7</div>
      </div>

      <div class="flex-container">
        <div>8</div>
        <div>9</div>
        <div>10</div>
        <div>11</div>
        <div>12</div>
        <div>13</div>
        <div>14</div>
      </div>

      <div class="flex-container">
        <div>15</div>
        <div>16</div>
        <div>17</div>
        <div>18</div>
        <div>19</div>
        <div>20</div>
        <div>21</div>
      </div>

      <div class="flex-container">
        <div>22</div>
        <div>23</div>
        <div>24</div>
        <div>25</div>
        <div>26</div>
        <div>27</div>
        <div>28</div>
      </div>

      <div class="flex-container">
        <div>29</div>
        <div>30</div>
        <div>31</div>
        <div> </div>
        <div> </div>
        <div> </div>
        <div> </div>
      </div>

      <div class="flex-container">
        <div>SUN</div>
        <div>MON</div>
        <div>TUE</div>
        <div>WED</div>
        <div>THUR</div>
        <div>FRI</div>
        <div>SAT</div>
      </div>
    </div>
  </div>
</template>



<style scoped>
       body {
            width: 100%;
            height: 100vh;
            background-color: lightblue;
            display: flex;
            justify-content: center;
            flex-direction: column;
            align-items: center;

        }



        .flex-container {
            display: flex;
            flex-direction: row;
            /* Align items in a row */
            background-color: rgb(255, 255, 255);
            margin: 0 auto;
        }

        .flex-container>div {
            border: 1px solid rgb(255, 255, 255);
            background-color: #ff0000;
            margin: 0px;
            padding: 20px;
            font-size: 25px;
            width: 68px;
            height: 40px;
            text-align: center;
            color: white;

        }
</style>
