<template>
    <div>
        <h3>Historial</h3>
        <ul id="list" class="list">
            <li v-for="transaction in transactions" v-bind:key="transaction.id">
                {{ transaction.text }} 
                <span>-${{ transaction-amount }}</span>
                <button class="deleta-btn">X</button>
            </li>
            <button class="delate-btn"></button>
        </ul>
    </div>
</template>

<script>
export default{
    data(){
        return{
            AddTransaction: [
                {id: 1, text: 'Floristeria', amount: -20},
                {id: 2, text: 'Salario', amount: 300},
                {id: 3, text: 'Libro', amount: -10},
                {id: 4, text: 'Camara', amount: 150},
            ]
        }
    }
}
</script>