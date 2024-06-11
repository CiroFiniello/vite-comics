<script>
export default {
    data() {
        return {
            navbarLinks: [
                { id: 1, title: 'CHARACTERS', active: false },
                { id: 2, title: 'COMICS', active: false },
                { id: 3, title: 'MOVIES', active: false },
                { id: 4, title: 'TV', active: false },
                { id: 5, title: 'GAMES', active: false },
                { id: 6, title: 'COLLECTIBLES', active: false },
                { id: 7, title: 'VIDEOS', active: false },
                { id: 8, title: 'FANS', active: false },
                { id: 9, title: 'NEWS', active: false },
                { id: 10, title: 'SHOP', active: false },
            ]
        };
    }
}
</script>

<template>
    <nav>
        <ul>
            <li class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </li>
        </ul>
        <ul class="menu">
            <li v-for="link in navbarLinks" :key="link.id">
                {{ link.title }}
                
            </li>
        </ul> 
    </nav>

</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;
nav{
    background-color: white;
    height: 150px;
    width: 100%;
    display: flex;
    align-items: center;
        .menu{
                justify-content: flex-end;
                gap: .25rem;
                align-self: baseline;
                margin-top: 2rem;
            }
            ul{
            align-items: center;
            display: flex;
            width: 100%;
            // justify-content: space-between;
            // justify-content: space-evenly;
            .logo{
                position: absolute;
                left: 13%;
                transform: scale(.8);
            }
            li{
                padding: .5rem;
                list-style-type: none;
                font-size: .8rem;
                font-weight: bold;
                color: $font_color;
                &.active{
                    color: $active_color;
                }
            }
        }
}
</style>