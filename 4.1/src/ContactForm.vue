<template>
    <form>
        <div class="form-group">
            <label for="sender-email">Email</label>
            <input 
                type="email" 
                id="sender-email"
                class="form-control" 
            />
        </div>
        <div class="form-group">
            <label for="sender-message">Message</label>
            <textarea 
                id="sender-message"
                rows="10"
                class="form-control" 
            ></textarea>
        </div>
        <div class="form-group">
            <button 
                class="btn btn-primary"
            >Send Message</button>
        </div>
    </form>
</template>

<script>
export default {
    
}
</script>

<style>

</style>
