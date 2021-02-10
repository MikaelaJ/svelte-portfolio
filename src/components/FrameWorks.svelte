<script>
    export const icons = [
        {
            title: "Vue JS",
            img: "/assets/img/logos_vuejs.png",
            width: "60",
        },
        {
            title: "Nuxt JS",
            img: "/assets/img/logos_nuxtjs.png",
            width: "50",
        },
        {
            title: "Svelte",
            img: "/assets/img/logos_svelte.png",
            width: "50",
        },
        {
            title: "Angular",
            img: "/assets/img/logos_angular.png",
            width: "50",
        },
        {
            title: "Jekyll",
            img: "/assets/img/logos_jekyll.png",
            width: "100",
        },
        {
            title: "Gatsby & React",
            img: "/assets/img/logos_gatsby_react.png",
            width: "100",
        },
    ];
</script>

<div class="container">
    {#each icons as icon}
        <div class="item">
            <p>{icon.title}</p>
            <img src={icon.img} alt={icon.title} width={icon.width} />
        </div>
    {/each}
</div>

<style>
    p {
        color: var(--light);
        text-transform: uppercase;
        padding: 0% 0% 3% 0%;
    }
    .container {
        display: flex;
        flex-wrap: wrap;
        width: 80vw;
        height: 100%;
        padding: 3% 3% 3% 3%;
        color: #fff;
        text-align: center;
        border-width: 7px;
        border-style: outset;
        border-color: #20242623;
        text-shadow: 1px 1px 3px #333;
        margin: 3% auto 3% auto;
        background-image: linear-gradient(
            135deg,
            #8c8c8857 10%,
            #20242675 100%
        );
    }
    .item {
        flex: 0 33%;
        margin: 1% 0% 1% 0%;
        padding: 1% 1% 1% 1%;
    }
    @media (max-width: 1024px) {
        .item {
            flex: 0 48%;
            margin: 0% 1% 3% 1%;
        }
    }
    @media (max-width: 640px) {
        .item {
            width: 99%;
            margin: auto;
        }
        .container {
            width: 95vw;
        }
    }
</style>
