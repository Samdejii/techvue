<template> 
  <div id="app">
   <div id="nav">


        <nav id="topnav" class="defaultscroll is-sticky">
            <div class="container">
            
                    <a class="logo" href="index.html">
                    <img src="assets/images/logo-dark.png" class="inline-block dark:hidden" alt="">
                    <img src="assets/images/logo-light.png" class="hidden dark:inline-block" alt="">
                </a>


                <div class="menu-extras">
                    <div class="menu-item">
                    
                        <a class="navbar-toggle" id="isToggle" onclick="toggleMenu()">
                            <div class="lines">
                                <span></span>
                                <span></span>
                                <span></span>
                            </div>
                        </a>
                        
                    </div>
                </div>

                <div id="navigation">

                    <ul class="navigation-menu">
                        <li><router-link to="/">Home</router-link></li>
                        <li><router-link to="/about">About</router-link></li>
                        <li><router-link to="/contact">Contact</router-link></li>
                
                       
                    </ul>
                </div>
            </div>
        </nav>


    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;*/
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
