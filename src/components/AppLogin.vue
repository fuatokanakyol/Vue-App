<template>
    <div class="container">
        <div class="row">
            <div class="col">
                <h1>Login</h1>
                <hr>
                <form method="post" action="/login" class="needs-validations" novalidate>
                    <TextInput 
                        label="Email" 
                        name="email" 
                        type="email" 
                        required 
                        placeholder="Enter your email"
                    />
                    <TextInput
                        label="Password"
                        name="password"
                        type="password"
                        required="true"
                        placeholder="Enter your password"
                    />
                </form>
                <input type="submit" class="btn btn-primary" value="Login">
            </div>
        </div>
    </div>
</template>

<script>
import TextInput from './forms/TextInput.vue'

export default {
    name: 'AppLogin',
    components: {
        TextInput
    }
}
</script>