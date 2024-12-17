<template>
    <div class="mb-3">
        <label :for="name" class="form-label">{{ label }}</label>
        <input 
        :type="type"
        :name="name"
        :placeholder="placeholder"
        :required="required"
        :min="min"
        :max="max"
        :value="value"
        :autocomplete="autocomplete"
        class="form-control"
        >
    </div>
</template>

<script>
export default {
    name: 'TextInput',
    props: {
        name: {
            type: String,
            
        },
        label: {
            type: String,
            
        },
        type: {
            type: String,
           
        },
        placeholder: {
            type: String,
            
        },
        required: {
            type: Boolean,
            default: true
           
        },
        min: {
            type: [String, Number],
          
        },
        max: {
            type: [String, Number],
     
        },
        value: {
            type: [String, Number],
          
        }
    }
}
</script>