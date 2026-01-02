<script setup>
import Menu from '../components/Menu.vue'
</script>

<template>
    <header class="header-section">
        <router-link to="/">
            <h1>Motion Palette</h1>
            <p>– CSS Animation Style Book –</p>
        </router-link>
        <Menu/>
    </header>
</template>

<style scoped>
.header-section {
    width: 100%;
    height: 80px;
    background-image: linear-gradient(90deg, skyblue, pink);
    color: white;
    flex-shrink: 0;
    padding: 10px 30px;
    display: flex;
    justify-content: space-between;
}


a{
    margin: auto 0;
}

h1 {
    font-size: 36px;
    color: white;
}

p{
    font-size: 12px;
    color: white;
}

/* タブレット → スマホ（必須） */
@media (max-width: 768px) {
    .header-section h1 {
    font-size: 30px;
    }

    .header-section p {
    font-size: 9px;
    }
}

/* 小さめスマホ */
@media (max-width: 480px) {
    .header-section {
        padding: 10px 20px;
    }
    .header-section h1 {
    font-size: 28px;
    }

}
</style>