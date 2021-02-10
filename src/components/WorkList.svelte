<script>
    export const works = [
        {
            id: 1,
            title: "Convictus",
            info:
                "Convictus is a non-profit organization with a focus on helping the homeless and addicts. My role, in a project that aimed to develop a new web for the organization, was to produce an easy-to-navigate website for a customer with high demands on user-friendliness. The result was a new website with payment solution and integration to CRM.",

            chips: ["Vue", "Vuetify", "Vuex", "Nuxt", "Contentful"],
            link: "https://www.convictus.org/",
            img: "/assets/img/svg.svg",
            type: 1,
        },
        {
            id: 2,
            title: "Gestricia Redovisning",
            info:
                "Developed a web application for an accounting firm. The result was a clear and intriguing site with playful colours. Design elements, icons and logo are made in Illustrator.",
            chips: [
                "Vue",
                "Vuetify",
                "Vuex",
                "Nuxt",
                "Contentful",
                "Illustrator",
            ],
            link: "https://gestricia.se/",
            img: "/assets/img/convictus_logo.png",
            type: 1,
        },
        {
            id: 3,
            title: "Frk Karlsson Couture",
            info:
                "Developed a website for my friend who is a master tailor at Drottningholms Slottsteater. I've also designed her logo for frk Karlsson Couture.",
            chips: [
                "Vue",
                "Vuetify",
                "Vuex",
                "Nuxt",
                "Contentful",
                "Illustrator",
                "Logo",
                "Design",
            ],
            link: "http://frkkarlssoncouture.com/",
            img: "/assets/img/convictus_logo.png",
            type: 1,
        },
        {
            id: 3,
            title: "Band Site",
            info:
                "This site was developed during last year of my education. Togheter with two other classmates we've created a site for a made up band (this case Bob Marley) using Jekyll. We went banans on CSS and animations to make this a playful site. When do you ever get to play around like that if not in school, a very fun project.",
            chips: ["Jekyll", "Parallax", "CSS"],
            link: "https://band-site-jekyll.netlify.app/index.html",
            img: "/assets/img/convictus_logo.png",
            type: 2,
        },
    ];

    function handleScroll(event) {
        let path = document.querySelectorAll("path");
        let lengthOfEachEl = new Array();

        for (let i = 0; i < path.length; i++) {
            lengthOfEachEl[i] = +path[i].getTotalLength();
            let arr = lengthOfEachEl[i];
            lengthOfEachEl[arr - 1]++;
            let scrollpercent =
                (document.body.scrollTop + document.documentElement.scrollTop) /
                (document.documentElement.scrollHeight -
                    document.documentElement.clientHeight);

            for (let i = 0; i < lengthOfEachEl.length; i++) {
                let draw = lengthOfEachEl[i] * scrollpercent;
                path[i].style.strokeDasharray =
                    lengthOfEachEl[i] + " " + lengthOfEachEl[i];
                path[i].style.strokeDashoffset = lengthOfEachEl;
                path[i].style.strokeDashoffset = (lengthOfEachEl[i] - draw) * 9;
            }
        }
    }
</script>

<svelte:window on:scroll={handleScroll} />

<div class="item-3 sticky-box">
    <svg
        version="1.1"
        id="Layer_1"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        x="0px"
        y="0px"
        viewBox="0 0 148.26 227.04"
        enable-background="new 0 0 148.26 227.04"
        xml:space="preserve"
    >
        <g>
            <path
                fill="none"
                stroke="#000000"
                stroke-width=".5"
                stroke-miterlimit="10"
                d="M147.13,74.46c0-40.32-32.68-73-73-73c-40.32,0-73,32.68-73,73
		c0,34.74,24.27,63.81,56.77,71.19v18.98c0,0.28-0.23,0.51-0.52,0.51H31c-0.29,0-0.52,0.23-0.52,0.51v24.68
		c0,0.28,0.23,0.51,0.52,0.51h26.39c0.28,0,0.52,0.23,0.52,0.51v33.71c0,0.28,0.23,0.51,0.51,0.51h29.82c0.28,0,0.52-0.23,0.52-0.51
		v-33.71c0-0.28,0.23-0.51,0.51-0.51h26.39c0.28,0,0.52-0.23,0.52-0.51v-24.68c0-0.28-0.23-0.51-0.52-0.51H89.26
		c-0.28,0-0.51-0.23-0.51-0.51V146C122.06,139.22,147.13,109.77,147.13,74.46z M23.5,74.46c0-27.96,22.67-50.63,50.63-50.63
		c27.97,0,50.64,22.67,50.64,50.63c0,22.88-15.18,42.2-36.01,48.48v-12.4c0-0.28,0.15-0.69,0.34-0.89L102,95.56
		c0.19-0.21,0.34-0.61,0.32-0.89l-0.59-12.35c-0.01-0.28-0.26-0.49-0.53-0.46l-18.42,2.02c-0.28,0.03-0.56,0.28-0.63,0.56L80,93.63
		c-0.07,0.27-0.25,0.31-0.42,0.08l-0.04-0.05c-0.17-0.23-0.29-0.65-0.28-0.93l0.46-10.05c0.01-0.28-0.19-0.6-0.45-0.7l-18.58-7.32
		c-0.26-0.1-0.57-0.4-0.69-0.66l-0.49-1.09c-0.11-0.26,0.02-0.43,0.3-0.37l15.03,2.79c0.28,0.05,0.55-0.13,0.61-0.41l1.6-7.38
		c0.06-0.28-0.11-0.57-0.38-0.65l-22.89-6.83c-0.27-0.08-0.59,0.07-0.7,0.32L44.14,80.8c-0.11,0.26-0.08,0.67,0.07,0.9l13.41,21.01
		c0.15,0.24,0.28,0.67,0.28,0.95v18.76C37.9,115.66,23.5,96.75,23.5,74.46z"
            />
            <path
                fill="none"
                stroke="#000000"
                stroke-width=".5"
                stroke-miterlimit="10"
                d="M90.13,78.06l9.05,1.64c0.28,0.05,0.55-0.14,0.6-0.41l3.01-15.44
		c0.05-0.28-0.13-0.55-0.41-0.6l-9.06-1.76c-0.28-0.05-0.55,0.13-0.6,0.41l-3,15.57C89.67,77.74,89.85,78.01,90.13,78.06z"
            />
            <path
                fill="none"
                stroke="#000000"
                stroke-width=".5"
                stroke-miterlimit="10"
                d="M77.53,77.38l9.6,2.45c0.27,0.07,0.54-0.1,0.6-0.38l4.96-25.5
		c0.05-0.28-0.13-0.55-0.41-0.6l-9.7-1.89c-0.27-0.05-0.55,0.13-0.6,0.41l-4.85,24.89C77.07,77.03,77.26,77.31,77.53,77.38z"
            />
            <path
                fill="none"
                stroke="#000000"
                stroke-width=".5"
                stroke-miterlimit="10"
                d="M68.54,61.78l8.74,2.62c0.27,0.08,0.54-0.08,0.59-0.36l3-15.09
		c0.06-0.28-0.13-0.55-0.41-0.6L71.5,46.6c-0.28-0.05-0.55,0.13-0.6,0.41l-2.75,14.11C68.09,61.4,68.27,61.69,68.54,61.78z"
            />
            <path
                fill="none"
                stroke="#000000"
                stroke-width=".5"
                stroke-miterlimit="10"
                d="M57.16,58.39l8.81,2.69c0.27,0.08,0.53-0.08,0.59-0.35l2.18-11.05
		c0.05-0.28-0.13-0.55-0.41-0.6l-9.01-1.75c-0.27-0.05-0.55,0.13-0.6,0.41l-1.95,10C56.72,58.01,56.89,58.31,57.16,58.39z"
            />
        </g>
    </svg>
</div>

<div class="container">
    {#each works as work, i}
        <div class="item">
            <div>
                <h4 class="title">{work.title}</h4>
                <p>
                    {work.info}
                    <strong target="_blank" href={work.link}>
                        <a target="_blank" href={work.link}
                            >Link to {work.title}</a
                        ></strong
                    >
                </p>
            </div>

            <div class="chips-container">
                {#each work.chips as chip}
                    <div class="chips">{chip}</div>
                {/each}
            </div>
        </div>
    {/each}
</div>

<style>
    h4 {
        font-weight: 400;
        text-align: right;
        letter-spacing: 0.3rem;
        background: linear-gradient(to right, #f2498704 0%, #202426 80%);
        text-transform: uppercase;
        padding: 1% 8% 1% 8%;
        margin-right: -5%;
    }
    p {
        min-height: 20vh;
        padding: 0% 4% 0% 4%;
        text-align: left;
        line-height: 1.6rem;
    }
    a {
        text-decoration: none !important;
        color: var(--light);
    }

    a:hover {
        text-decoration: none;
        color: var(--neonPink);
        text-shadow: 1px 1px 3px #333;
    }
    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        align-content: space-between;
        width: 80vw;
        margin: auto;
    }

    .item {
        flex: 0 49%;
        min-height: 25vh;
        padding: 1% 0% 2% 0%;
        margin: 0% 0% 2% 0%;
        border-width: 7px;
        border-style: outset;
        border-color: #f249873d;
        background-color: var(--neonPinkOpacity);
        box-shadow: 1px 1px 80px 8px var(--grey) inset;
        box-shadow: 2px 2px 40px 8px var(--bg);
    }
    .chips-container {
        margin: 3%;
    }
    .chips {
        display: inline-flex;
        color: var(--light);
        border-width: 2px;
        border-style: dotted;
        border-radius: 25px;
        text-align: left;
        margin: 1% 1% 1% 1%;
        padding: 1% 2% 1% 2%;
    }
    .sticky-box {
        position: sticky;
        position: -webkit-sticky;
        top: 10%;
    }

    .item-3 {
        margin: 0% 0% 0% 0%;
        position: absolute;
        z-index: -2;
        width: 35%;
    }
    @media (max-width: 1024px) {
        .item {
            flex: 99%;
            margin: 0% 1% 4% 1%;
        }
        h4 {
            margin-right: -1%;
        }
    }
    @media (max-width: 640px) {
        .item {
            width: 100%;
            margin: 0% 3% 4% 3%;
        }

        p {
            font-size: 0.8rem;
            line-height: 1.3rem;
        }
    }
</style>
