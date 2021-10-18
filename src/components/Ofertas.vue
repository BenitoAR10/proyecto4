<template>
<div id="menu">
<ul>
  <li><a href="http://www.google.com.ar">Google</a></li>
  <li><a href="#">Periodicos >>></a>
    <ul>
      <li><a href="http://www.la-razon.com/">La Razon</A></li>
      <li><a href="https://eldeber.com.bo/">El Deber</A></li>
      <li><a href="https://www.eldiario.net/">El Diario</a></li>
    </ul>
  </li>
  <li><a  href="#">Lenguajes >>></a>
    <ul>
      <li><a href="http://www.php.net">PHP</a></li>
      <li><a href="http://www.rubyonrails.org">Ruby on rails</a></li>
      <li><a href="http://www.python.org">Python</a></li>
    </ul>
  </li>
  <li><a  href="http://www.msn.com">MSN</a></li>
</ul>
</div>
</template>

<script>
window.addEventListener('load',inicializarEventos,false);

function inicializarEventos()
{
  inicializarMenu('menu');
}

function inicializarMenu(m)
{
  var ob=document.getElementById(m);
  var menu=ob.getElementsByTagName('ul');
  for(f=1;f<menu.length;f++)
  {
    menu[f].style.display='none';
  }
  var enlaces=ob.getElementsByTagName('a');
  for(f=0;f<enlaces.length;f++)
  {
    enlaces[f].addEventListener('click',itemSeleccionado,false);
  }
}
function itemSeleccionado(e)
{
  var enlace;
  enlace=e.target;
  var padre=enlace.parentNode;
  var ul=padre.getElementsByTagName('ul');
  if (ul.length>0)
  {
    if (ul[0].style.display=='none')
      ul[0].style.display='block';
    else
      ul[0].style.display='none';
  }
}

function addEvent(elemento,nomevento,funcion,captura)
{
  elemento.addEventListener(nomevento,funcion,captura);
  return true;
}
</script>

<style>
#menu {
  font-family: Arial;
  margin:0px;
  padding:0px;
}

#menu ul {
  margin:0px;
  padding:0px;
  list-style-type:none;
}

#menu a {
  display: block;
  padding: 3px;
  width: 160px;
  background-color: #f7f8e8;
  border-bottom: 1px solid #eee;
  text-align:center;
}

#menu a:link, #menu a:visited {
  color: #f00;
  text-decoration: none;
}

#menu a:hover {
  background-color: #369;
  color: #fff;
}

#submenu a {
  display: block;
  padding: 3px;
  width: 160px;
  background-color: #ffa;
  border-bottom: 1px solid #eee;
  text-align:center;
}
</style>
