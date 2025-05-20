<template>
    <div class="employees">
        <div class="boss-card">
            <img src="../assets/boss.png" alt="Profile picture off boss">
            <div class="boss-info">
                <h4>Lars-Olof Svensson</h4>
                <p>Chef</p>
            </div>
        </div>

        <div class="employee-controls">
            <div class="sort-filter-buttons">
                <button class="sort-button">
                    <img src="../assets/sort.png" alt="Sort button">
                    Sortering
                </button>

                <button class="filter-button">
                    <img src="../assets/filter.png" alt="Filter button">
                    Filter
                </button>
            </div>
            <div class="employee-label">Anställda</div>
        </div>

        <div class="employee-card" v-for="(em, index) in employeeNames" :key="index">
            <img src="../assets/profile-picture.webp" alt="Profile-picture">
            <div class="employee-info">
                <h4>{{ em }}</h4>
                <p>{{ employeeProfessions[index] }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
const employeeNames = ["Albert Svensson", "Doris Johnson", "Moa Haag", "Stefan Holm", "Fatima Diame", "Harrison Ford", "Daniel García", "Joanna Rudzki", "David Lynch", "Anders Ofvegard"]
const employeeProfessions = ["Elektriker, Murare, Snickare, VVS", "Snickare", "Elektriker", "Elektriker, VVS", "Murare", "Snickare", "Målare", "Murare, Målare", "Målare", "Arg snickare"]
</script>

<style scoped>
.employees {
    margin-left: 3rem;
    width: 15rem;
}

.boss-card {
    display: flex;
    align-items: center;
    background-color: #E9E9E9;
    border-radius: 0 0 2rem 2rem;
    padding: 2rem 2.5rem;
    margin-bottom: 6.5rem;
}

.boss-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.employee-card {
    display: flex;
    align-items: center;
    padding: 1rem;
}

.employee-card img,
.boss-card img {
    width: 4rem;
    border-radius: 50%;
    margin-right: 1rem;
}

.employee-info h4,
.boss-info h4 {
    margin: 0;
    font-size: medium;
}

.employee-info p,
.boss-info p {
    margin: 0;
    font-size: medium;
    color: #888;
}

.employee-controls {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    align-items: flex-start;
    margin-bottom: 1.5rem;
    margin-left: 1rem;
}

.sort-filter-buttons {
    display: flex;
    flex-direction: row;
    gap: 0.5rem;
    font-family: Inter;
}

.sort-button,
.filter-button {
    display: flex;
    align-items: center;
    gap: 0.2rem;
    background-color: #E9E9E9;
    border: none;
    padding: 0.4rem 1rem;
    border-radius: 1.2rem;
    font-size: small;
    cursor: pointer;
}

.sort-button img,
.filter-button img {
    width: 1rem;
}

.employee-label {
    background-color: #E9E9E9;
    border-radius: 0.5rem;
    padding: 0.5rem 8rem;
    padding-left: 0.5rem;
    font-size: small;
    margin-left: 0.3rem;
}
</style>