<script >
export default {
  name: "toolbar-bar-owner",
}
</script>

<template>
  <div class="toolbar-1">
  <pv-toolbar  class="toolbar-1 mx-auto">
    <template #start>
      <div class="imglogo">
        <pv-images src="https://i.postimg.cc/8Cdxqmbc/ai-de-logwww-Mesa-de-trabajo-1.png" alt="logo" width="100"/>
      </div>
    </template>
    <template #end>
      <div class="control">

        <router-link to="/home-owner"> <pv-button  id="btnrouter">{{$t("start")}}</pv-button> </router-link>
        <router-link to="/register-car"> <pv-button id="btnrouter">{{$t("vehicule_registration")}}</pv-button> </router-link>
        <router-link to="/notifications-owner"> <pv-button id="btnrouter">{{$t("notifications")}}</pv-button> </router-link>
        <router-link to="/rent-owner-major"> <pv-button id="btnrouter">{{$t("rent")}}</pv-button> </router-link>

        <router-link to="/profile-owner"> <a><pv-images id="btnrouter" src="https://i.postimg.cc/FFqf7CRJ/usuario-1.png" alt="logo" width="40"/></a> </router-link>
      </div>
    </template>
  </pv-toolbar>
  </div>
</template>

<style scoped>

.toolbar-1{
  background-color: white;
  padding:9px;
  border: none;
}
.control{

}
#btnrouter{
  margin-left: 10px;
  margin-right:10px;
  width: 200px;
  justify-content: center;
  background-color: white ;
  color:black;
  border: 3px white;
  border-radius:30px;
  box-shadow: black;
  font-weight: bold;

}
#btnrouter:hover{
  background-color:#01A1FF;
  box-shadow: none;
  border: none;
  font-weight: bold;
  color:white;
}
#btnrouter:focus{
  color:black;
  box-shadow: none;
  font-weight: bold;
}
@media all and (max-width: 840px) {
  .imglogo{
    place-content: center;
  }

  .control{
    display:inline-block;
    float:none;
    align-content: center;
    text-align: center;
  }
  #btnrouter{
    margin-left: 10px;
    margin-right:10px;
    width: 150px;
    font-size:10px ;
    justify-content: center;
    background-color: white ;
    color:black;
    border:none;
    box-shadow: black;
    font-weight: bold;
  }
  #btnrouter:hover{
    background-color:white;
    box-shadow: none;
    font-weight: bold;
    color:white;
  }
  #btnrouter:focus{
    color:white;
    box-shadow: none;
    font-weight: bold;
  }
}
</style>
