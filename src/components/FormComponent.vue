<template>
    <form @submit.prevent="submitForm">
        <div>
            <label for="placename">Place Name : </label>
            <input type="text" v-model.trim="additem.name" name="placename">
        </div>
        <div>
            <label for="placedetail">Place Detail : </label>
            <textarea v-model="additem.detail" cols="30" rows="3"></textarea>
        </div>
        <button @click="addPlace">Add Place</button>
    </form>
    {{ JSON.stringify(additem) }}
</template>

<script>
export default {
    name: 'Form',
    data() {
        return {
            additem: {
                id:99,
                name: "",
                detail: "",
                coverimage: null
            }
        }
    },
    methods: {
        submitForm() {
            this.$emit("savePlace", this.additem);
            console.log("submitForm : ", this.additem)
        }
    }
}
</script>

<style>

</style>