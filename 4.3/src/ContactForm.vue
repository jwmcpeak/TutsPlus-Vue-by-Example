<template>
    <form>
        <div class="form-group">
            <label for="sender-email">Email</label>
            <input 
                type="email" 
                id="sender-email"
                class="form-control" 
                v-model="email"
            />
        </div>
        <div class="form-group">
            <label for="sender-message">Message</label>
            <textarea 
                id="sender-message"
                rows="10"
                class="form-control" 
                v-model="message"
            ></textarea>
        </div>
        <div class="form-group">
            <button 
                class="btn btn-primary"
                @click.prevent="submitForm"
                :disabled="!email || !message"
            >Send Message</button>
        </div>
    </form>
</template>

<script>
export default {
    data() {
        return {
            email: '',
            message: ''
        };
    },
    methods: {
        submitForm(e) {
            // validate form
            // submit form

            alert(`Thanks for the message. We will reply to ${this.email} soon.`)
        }
    }
}
</script>

<style>

</style>
