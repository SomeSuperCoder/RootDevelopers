<div class="text-white">
    <header>
        <h1 class="text-5xl sm:text-7xl sm:ml-[10%] md:text-8xl md:ml-[20%] mt-[4rem] ml-[5%] font-extrabold team-name roll-in">Root Developers</h1>
        <h2 class="text-xl ml-[6%] sm:ml-[12%] md:ml-[24%] roll-in longer-roll">Передовая команда веб разработчиков</h2>
    </header>
    
    <main class="flex flex-col mt-[4rem] fade-in box-border px-[25%] gap-5">
        <article class="box-border p-5 rounded-2xl self-start blur-bg">
            <h1 class="text-5xl font-semibold color-neutral-700 border-b-2 border-neutral-400">О нас</h1>
            <p class="mt-2 ml-3 indent-[1ch] text-md md:text-lg max-w-2xl">Мы - команда веб-разработчиков. Мы создаём высокотехнологичные веб-приложения на <a class="underline" href="https://kit.svelte.dev/">SvelteKit</a>. При разработке мы используем самые передовые технологии в мире программирования, чтобы всегда быть на одной волне с прогрессом!</p>
        </article>
        <article class="box-border p-5 rounded-2xl self-end blur-bg">
            <h1 class="text-5xl font-semibold color-neutral-700 border-b-2 border-neutral-400">Наши услуги</h1> 
            <ol class="mt-2 ml-3 indent-[1ch] text-md md:text-lg max-w-2xl list-decimal">
                <li>Создание веб-сайтов и приложений</li>
                <li>Разработка мобильных приложений</li>
                <li>Интеграция с API</li>
                <li>Сопровождение и поддержка сайта</li>
            </ol>
        </article>
        <div class="circle-1 fixed w-[15vw] h-[15vw] top-[20vw] left-[20vw] rounded-full bg-yellow-700 -z-10 opacity-50"></div>
        <div class="circle-2 fixed w-[15vw] h-[15vw] top-[50vh] left-[50vw] rounded-full bg-purple-400 opacity-50 -z-10"></div>
        <div class="circle-3 fixed w-[15vw] h-[15vw] top-[70vh] left-[70vw] rounded-full bg-purple-800 opacity-50 -z-10"></div>
        <div class="circle-4 fixed w-[15vw] h-[15vw] top-[30vh] left-[65vw] rounded-full bg-green-500 opacity-50 -z-10"></div>
        <div></div>
    </main>
    
    <footer class="fixed bottom-0 px-4">
        &copy; 2024 Root Developers. All rights reserved.
    </footer>    
</div>

<style>
    @keyframes text-roll {
        0% {
            transform: translateX(-200vw);
        }

        100% {
            transform: translateX(0);
        }
    }

    @keyframes fade-in-animation {
        0% {
            opacity: 0;
        }

        100% {
            opacity: 1;
        }
    }

    @keyframes circle-1-animation {
        0% {
            transform: translateX(-200vw);
        }

        100% {
            transform: translateX(0);
        }
    }


    @keyframes circle-2-animation {
        0% {
            transform: translateX(-200vw) translateY(-100vw);
        }

        100% {
            transform: translateX(0) translateY(0);
        }
    }

    @keyframes circle-3-animation {
        0% {
            transform: translateX(200vw) translateY(100vw);
        }

        50% {
            transform: translateX(-30vw) translateY(-34vw);

        }

        100% {
            transform: translateX(0) translateY(0);
        }
    }

    @keyframes circle-4-animation {
        0% {
            transform: translateX(150vw) translateY(120vw);
        }

        50% {
            transform: translateX(50px) translateY(-28px);

        }

        60% {
            transform: translateX(100px) translateY(80px);

        }

        100% {
            transform: translateX(0) translateY(0);
        }
    }

    .team-name {
        background: rgb(2,0,36);
        background: linear-gradient(to right, red, blue);
        background-clip: text;
        color: transparent;
    }

    .roll-in {
        animation-name: text-roll;
        animation-duration: 0.8s;
        animation-timing-function: ease-out;
        animation-fill-mode: both;
    }

    .longer-roll {
        animation-delay: 0.5s;
    }

    .fade-in {
        animation-name: fade-in-animation;
        animation-duration: 2s;
        /* A function that starts slow and gets very fast at the end */
        /* animation-timing-function: cubic-bezier(0.215, 0.61, 0.355, 1); */
        animation-timing-function: cubic-bezier(0.55, 0.055, 0.675, 0.19);
        animation-fill-mode: both;
        animation-delay: 1.3s;
    }

    .blur-bg {
        background-color: rgba(255, 255, 255, 0);
        backdrop-filter: blur(100px);
    }

    .circle-1 {
        animation: circle-1-animation 1s ease-in-out 1.5s;
        animation-fill-mode: both;
    }

    .circle-2 {
        animation: circle-2-animation 1.5s ease-in-out 2.3s;
        animation-fill-mode: both;
    }

    .circle-3 {
        animation: circle-3-animation 2.5s ease-in-out 1.3s;
        animation-fill-mode: both;
    }

    .circle-4 {
        animation: circle-4-animation 2s cubic-bezier(0.445, 0.05, 0.55, 0.95) 1.7s;
        animation-fill-mode: both;
    }
</style>
