<template>
<div class="records">
    <div class="space">
        <p>Total Students</p>
        <h2>5140</h2>
    </div>
    <div class="space">
        <p>Parents</p>
        <h2>4123</h2>
    </div>
    <div class="space">
        <p>Affiliate Distribution</p>
        <h2>4.18 Lac</h2>
    </div>
</div>
</template>

<script>
export default {
    name: 'DataRecords',
}
</script>

<style scoped>
.records {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    background: url(../assets/records.svg);
    height: auto;
    width: auto;
    font-weight: bold;
    padding: 2rem;
}
.space{
    padding:1rem;
}

h2 {
    border-bottom: 0.5rem solid #01CB63;
    padding-bottom: 1rem;
    font-weight: bold;
}

p {
    color: #86919D;
    margin-top: 2rem;
    font-size: 1.5rem;
}
</style>
