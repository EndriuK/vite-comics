<script>
export default {
    data(){
        return{
            links: [
                {
                    label: 'characters',
                    url: '#',
                    current: false
                },
                {
                    label: 'comics',
                    url: '#',
                    current: true
                },
                {
                    label: 'movies',
                    url: '#',
                    current: false
                },
                {
                    label: 'tv',
                    url: '#',
                    current: false
                },
                {
                    label: 'games',
                    url: '#',
                    current: false
                },
                {
                    label: 'collectibles',
                    url: '#',
                    current: false
                },
                {
                    label: 'videos',
                    url: '#',
                    current: false
                },
                {
                    label: 'fans',
                    url: '#',
                    current: false
                },
                {
                    label: 'news',
                    url: '#',
                    current: false
                },
                {
                    label: 'shop',
                    url: '#',
                    current: false
                },
            ]
        }
    }
}
</script>
<template lang="">
    <header>
        <div class="container">
            <div class="row">
                <div class="col-12 my-3">
                    <img src="../assets/img/dc-logo.png" />
                </div>
                <div class="col-12 d-flex flex-row-reverse">
                    <ul class="list-unstyled mt-5 justify-content-center d-flex">
                        <li v-for="link, index in links" :key="index" :class="link.current ? 'active' : ''">
                            <a href="link.url">{{link.label}}</a>
                        </li>
                        
                    </ul>
                </div>
            </div>
        </div>
         
    </header>
</template>
<style lang="scss" scoped>
    ul {
        li{
            padding:20px 15px;

            a {
                text-decoration: none;
                color: #000;
                transition: font-weight 0.3s;
                text-transform: uppercase;

                &:hover {
                    font-weight: 500;
                }
            }
        }

        .active {
            color: blue;
        }
    }
</style>