<template>
    <div class="form-check">
        <input class="form-check-input" :checked="checked" :required="required" type="checkbox">
        <label :for="name" class="form-check-label">
            {{ label }}
        </label>
    </div>
</template>

<script>
export default {
    props: {
        checked: {
            type: Boolean,
            required: true
        },
        required: {
            type: Boolean,
            default: false
        },
        name: {
            type: String,
            required: true
        },
        label: {
            type: String,
            required: true
        }
    }
}
</script>