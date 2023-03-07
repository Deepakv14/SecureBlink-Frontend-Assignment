<template>
<div class="footer">
<p>2021-2022 © Course Pro Private Limited</p>
     <p>Term & Condition</p>
        <p>Privacy Policy</p>
</div>
</template>

<script>
export default {
    name: 'FooterPart',
}
</script>

<style scoped>
.footer {
    display: grid;
    grid-template-columns: 2.5fr 1fr 1fr;
}
p{
    font-weight: bold;
}
</style>
