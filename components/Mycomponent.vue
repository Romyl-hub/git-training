<template>
    <div clas="root">
        <label> 
            Введите email:
            <input
             type="email"
             :value="email"
             @input="emailInput ($event.target.value)"
             />
            
       </label>
       <label> 
            Введите Пароль:
            <input
             type="password" 
            :value="password"
            @input="passwordInput ($event.target.value)"
            />
       </label>
       password:{{pasword}}
       email:{{email}}
       
    </div>
</template>
<script>
    export default {
        name: 'MyComponent',
        data() {
            return {
             email: 'warm@example',
             password:'1231425'
            }
        },
        methods:{
            emailInput(value) {
                this.email = value
                
            },
            passwordInput(value) {
                this.password = value
            }

        }
    }
</script>