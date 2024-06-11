<script>
export default {
    data() {
        return 
            {
        }
    }
}
</script>

<template>
    <nav>
        <ul>
            <li>
                <img src="../assets/img/dc-logo.png" alt="logo">
            </li>
        </ul>
        <ul class="menu">
            <li>
                test 
            </li>
            <li>
                test 
            </li>
            <li>
                test 
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
            }
            ul{
            align-items: center;
            display: flex;
            width: 100%;
            // justify-content: space-between;
            
            li{
                padding: 1rem;
                list-style-type: none;
                &.active{
                    color: $active_color;
                }
            }
        }
}
</style>