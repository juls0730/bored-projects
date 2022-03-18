<template>
  <div class="terminal" id="terminal"> </div>
</template>

<script>
document.onkeydown = function(e) {
    e = e || window.event;
    var charCode = (typeof e.which == "number") ? e.which : e.keyCode;
    if (charCode == 8 && document.getElementById("terminal").innerHTML !== "") {
      document.getElementById("terminal").innerHTML = document.getElementById("terminal").innerHTML.substring(0, document.getElementById("terminal").innerHTML.length - 1)
    } else if (charCode) {
      console.log(charCode)
      document.getElementById("terminal").innerHTML += String.fromCharCode(charCode);
    }
};
</script>


<style>
@import './assets/base.css';
</style>
