<template>
    <nav class="sidebar">
        <div class="sidebar-logo">
            <img src="../assets/logo.png" alt="Company logo">
        </div>

        <div class="sidebar-search">
            <img src="../assets/search.png" alt="Search icon">
        </div>

        <div class="sidebar-menu">
            <img src="../assets/home.png" alt="Home icon">
            <img src="../assets/diagram.png" alt="Diagram icon">
            <img src="../assets/bell.png" alt="Bell icon">
            <img src="../assets/pizza-diagram.png" alt="Pizza diagram icon">
            <img src="../assets/inbox.png" alt="Inbox icon">
        </div>

        <div class="sidebar-bottom">
            <img src="../assets/leave.png" alt="Leave icon">

            <div class="dark-mode-switch">
                <div class="switch-circle">
                    <img src="../assets/moon.png" alt="Moon icon for light or dark mode switch">
                </div>
            </div>


        </div>
    </nav>
</template>

<style scoped>
.sidebar {
    background: #FFFFFF;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.5rem;
    border-right: 1px solid #e0e0e0;
    top: 0;
    left: 0;
}

img {
    width: 2rem;
}

.sidebar-logo img{
    width: 4rem;
}

.sidebar-search {
    margin-top: 5rem;
    cursor: pointer;
}

.sidebar-menu {
    margin-top: 7rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 5rem;
    justify-content: flex-start;
    cursor: pointer;
}

.sidebar-bottom {
    margin-top: 24rem;
    margin-bottom: 2rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.5rem;
    cursor: pointer;
}

.dark-mode-switch {
    width: 4rem;
    height: 2.3rem;
    background-color: #0723304D;
    border-radius: 2rem;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: flex-end;
}

.switch-circle {
    width: 2rem;
    height: 2rem;
    margin-right: 2px;
    background-color: #0B2530;
    border-radius: 50%;
    display: flex;
    align-items: center;    
    justify-content: center;
}

.switch-circle img {
    width: 1.2rem;
    object-fit: contain;
}
</style>