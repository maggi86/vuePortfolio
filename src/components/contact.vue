<template>
    <div id="form">
        <h2>Feel free to Contact me</h2>

        <form action="https://formspree.io/f/xayvrnkd" method="POST">
            <label>
                Name:
                <input type="name" name="name" placeholder="Enter your Name">
            </label>
            <label>
                Email Address:
                <input type="email" name="email" placeholder="name@number.com">
            </label>
            <label>
              Your Message:
              <textarea name="message" rows="3"></textarea>
            </label>
  <!-- your other form fields go here -->
            <button type="submit">Send</button>
        </form>
    </div>
</template>

<script>
// import Foot from "@/components/footer.vue";

export default {
    data() {
        return {
            name: "",
            email: "",
        }     
    },

};
</script>

<style scoped>
h1{
  margin-top: 50px;
}
</style>
