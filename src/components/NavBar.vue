
<template>
	
<nav class="navbar navbar-expand-lg site-navbar navbar-light " id="pb-navbar">

      <div class="container">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExample09" aria-controls="navbarsExample09" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <a class="navbar-brand" href="index.html">Alias</a>
        <div class="collapse navbar-collapse justify-content-md-center" id="navbarsExample09">
          <ul class="navbar-nav">
            <li class="nav-item" 
                 v-for="linkNav in linksNav"
                 v-bind:section="linksNav.section"
                 v-bind:text="linksNav.text"   
            ><a class="nav-link" v-bind:href="linkNav.section">{{ linkNav.text }}</a></li>
            
          </ul>
        </div>
      </div>
    </nav>

</template>

<script type="text/javascript">

   

	export default{

         data: function(){
        return{

            linksNav: [{section:'#section-home', text: 'Home' },
                        {section:'#section-about', text: 'About' },
                        {section:'#section-services', text: 'Services' },
                        {section:'#section-portfolio', text: 'Portfolio' },
                        {section:'#section-resume', text: 'Resume' },
                        {section:'#section-blog', text: 'Blog' },
                        {section:'#section-contact', text: 'Contact' },

                            ]
                                   }
    },

	name: 'NavBar'	
}
</script>
<style type="text/css" scoped>

nav{

	z-index: 200px;
	
}	

.site-navbar {
    border: none;
    -webkit-box-shadow: none;
    box-shadow: none;
    border-radius: 0px;
    margin-bottom: 0px;
    background: none;
    position: absolute;
    top: 20px;
    width: 100%;
    z-index: 200;
    background: #fff;
}

.site-navbar.bg-light {
    background: transparent !important;
}



</style>