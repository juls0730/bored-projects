<template>
  <p id="login-message" class="typing"></p>
</template>

<script>
let input = "";
let command = "";
let echo = "";
let commandID = 1;
let terminalID = 1;
window.onload = function() {
  var i = 0;
  var txt = 'Welcome to this fake terminal, I made this project because I was bored scrolling through an idea website and it had an _ at the end of each header and reminded me of a terminal. The only command is echo and you must use the right arrow to make a \'. The license is distributed in the main bored project folder and the terminal-fake folder.';
  var speed = 35;

  function typeWriter() {
    if (i < txt.length) {
      document.getElementById("login-message").innerHTML += txt.charAt(i);
      i++;
      setTimeout(typeWriter, speed);
    } else {
      document.getElementById("login-message").classList.toggle("typing");
      let terminal = document.createElement('div');
      terminal.id = 'terminal-' + terminalID;
      terminal.className = 'terminal terminal-blink';
      document.getElementById("app").appendChild(terminal);
    }
  }

  typeWriter();
};

document.onkeydown = function(e) {
    e = e || window.event;
    var charCode = (typeof e == "number") ? e.which : e.keyCode;
    if (charCode == 8 && document.getElementById("terminal-" + terminalID).innerHTML !== "") {
      document.getElementById("terminal-" + terminalID).innerHTML = document.getElementById("terminal-" + terminalID).innerHTML.substring(0, document.getElementById("terminal-" + terminalID).innerHTML.length - 1)
    } else if (charCode == 13) {
      input = document.getElementById("terminal-" + terminalID).innerHTML;
      command = input.replace(/ .*/,'');
      terminalID += 1;

      if (command !== '') {
        let commandElement = document.createElement("p");
        commandElement.id = "output-" + commandID;
        commandID += 1;
        if (command.toLowerCase() == 'echo') {
          echo = input.split("'")[1]
          commandElement.innerHTML = echo;
        } else {
          commandElement.innerHTML = "trash: command not found: " + command;
        }
        document.getElementById("app").appendChild(commandElement);
      }

      let div = document.createElement('div');
      div.id = 'terminal-' + terminalID;
      div.className = 'terminal terminal-blink';
      document.getElementById("app").appendChild(div);
      document.getElementById("terminal-" + (terminalID-1)).classList.toggle("terminal-blink");
      window.scrollTo(0,document.body.scrollHeight);
    } else if (charCode && charCode !== 8 && charCode !== 16) {
      document.getElementById("terminal-" + terminalID).innerHTML += String.fromCharCode(charCode);
    }
};
</script>


<style>
@import './assets/base.css';
</style>
