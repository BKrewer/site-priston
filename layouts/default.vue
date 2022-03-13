<template>
    <div class="wrapper">
        <header>
            <NuxtLink to="/" class="site-logo">
                <h1>
                  <img src="~/assets/images/logo.png" alt="Hells Tale"/>  
                </h1>
            </NuxtLink>
           <NavBar /> 
        </header>
        
        <Nuxt />
        <Footer />
    </div>
</template>