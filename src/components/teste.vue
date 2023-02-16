<script setup>

defineProps({
    msg: String,
    partidas: Number,
    vitorias: Number,
    derrotas: Number,
    tiros: Number,
    winrate: Number,
    abates: Number,
    mortes: Number,
    derrotas: Number,
    tiros: Number,
    winrate: Number,
})

</script>

<template>
    <header>
        <div>
            <a href=""><img src="" alt=""></a>
            <a href=""><img src="" alt=""> <p> INÍCIO</p> </a>
            <a href=""><img src="" alt=""></a>
            <a href=""><img src="" alt=""></a>
            <a href=""><img src="" alt=""></a>
            <a href=""><img src="" alt=""></a>
        </div>
    </header>
    <h1> {{ msg }}</h1>
    <div class="left-title">
        <p> Estatísticas com o agente</p>
        <h1>RESUMO</h1>
    </div>
    <div class="left-li-start">
        <ul>
            <li>
                <p>Partidas jogadas</p>
                <span>{{ partidas }}</span>
            </li>
            <li>
                <p>Vitórias</p>
                <span>{{ vitorias }}</span>
            </li>
            <li>
                <p>Derrotas</p>
                <span>{{ derrotas }}</span>
            </li>
            <li>
                <p>Tiros na cabeça</p>
                <span>{{ tiros }}</span>
            </li>
            <li>
                <p>Winrate</p>
                <span>{{ winrate }}</span>
            </li>
        </ul>
    </div>

    <div class="left-li-end">
        <ul>
            <li>
                <p>Abates</p>
                <span>{{ abates }}</span>
            </li>
            <li>
                <p>Mortes</p>
                <span>{{ mortes }}</span>
            </li>
            <li>
                <p>Assistências</p>
                <span>{{ derrotas }}</span>
            </li>
            <li>
                <p>Tiros na cabeça</p>
                <span>{{ tiros }}</span>
            </li>
            <li>
                <p>Winrate</p>
                <span>{{ winrate }}</span>
            </li>
        </ul>
    </div>
    
</template>
