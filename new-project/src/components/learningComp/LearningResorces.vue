<template>
<li>
<BaseCard>
    <header>
        <h3>{{ title }}</h3>
        <button>Delete</button>
    </header>
<p>{{ descriptions }}</p>
<nav>
    <a :href="link">view resource</a>
</nav>
</BaseCard>
</li>
</template>

<script>

export default{
props:['title','descriptions','link','id']
}
</script>

<style scoped>
li{
    margin:auto;
    max-width:40rem;
}
header{
    display:flex;
    justify-content:space-between;
    align-items:center;
}
h3{
    font-size:1.25rem;
    margin:00.5rem 0;
}


p{
    margin: 0.5rem 0;
}
a{
    text-decoration:none;
    color:#ce5c00
}

a:hover,
a:active{
    color:#c89300
}
div{
    border-radius: 12px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.26);
    padding: 1rem;
    margin: 2rem auto;
    max-width: 40rem;
}

</style>