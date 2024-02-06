<template>
  <h3>History</h3>
  <ul id="list" class="list">

    <li v-for="transaction in transactions" :key="transaction.id">


           {{transaction.text}} <span>${{transaction.amount}}</span><button class="delete-btn">x</button>


    </li>


  </ul>
</template>

<script>
export default{
  data (){

    return {
      transactions: [
        {id: 1, text: 'Groceries', amount: 1000},
          {id: 2, text: 'Books', amount: 150},
          {id: 3, text: 'Allowances', amount: 10000},
          {id: 4, text: 'Gadgets', amount: 30000},

      ]
    }
  }
}


</script>
