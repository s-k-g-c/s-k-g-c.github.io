<template>

    <ul class="">
        <li class="">
            <router-link to="/" class="menu-color">Home</router-link>
        </li>
        <li class="">
            <router-link to="/gallery" class="menu-color">Gallery</router-link>
        </li>
    </ul>

</template>

<style scoped>
ul{
    list-style: none;
    display: flex;
    gap: 10px;
}

li{
    display: flex;
    color: white;
    width: 100px;
    align-self: center;
    justify-content: center;
}

li > a{
    display: inline-block;
    transition: transform 0.6s ease;
}

li > a:hover{
    transform: translateY(-5px) rotateY(360deg);
    transition: 0.8s;
}

.menu-color{
    color: white;
}

/* タブレット → スマホ（必須） */
@media (max-width: 768px) {
    li{
        width: 70px;
    }
}

/* 小さめスマホ */
@media (max-width: 480px) {
    li{
        width: 50px;
    }

}



</style>