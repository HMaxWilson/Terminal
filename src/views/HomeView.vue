<template>
  <div>
    <p>Greetings Explorer,</p>

    <p class="clear"><br/></p>

    <p>
      You've ventured into the heart of WILSON, where digital fortifications stand tall,
      guarding the gateway to your secure digital identity. Here, trust is the currency,
      and every bit and byte is shielded with an impenetrable layer of encryption.
    </p>

    <p class="clear"><br/></p>

    <p>
      Enough of that... This is more of an attempt at matching a style from my favourite game series, Fallout!
      Hopefully you enjoy the effort put into this project, and if you have any questions, feel free to reach out to me
      on my Socials.
    </p>

    <p class="clear"><br/></p>

    <p>
      Safe travels, Digital Voyager.
    </p>
  </div>
</template>

<style scoped>
form {}

label {
  clear: left;
  display: block;
  float: left;
  margin-right: 10px;
  padding-top: 5px;
}

input[type=text],
textarea {
  background: transparent;
  border: none;
  color: #00dd00;
  display: block;
  float: left;
  font-family: 'VT323', Courier, monospace;
  font-size: 1.2em;
  position: relative;
  width: 80%;
  z-index: 10
}

textarea {
  margin-bottom: 20px;
  overflow: auto;
  resize: none;
}

input[type=text]:focus,
textarea:focus,
input[type=submit]:focus,
a.button:focus {
  outline: 0;
}

input[type=submit],
a.button {
  background: transparent;
  border: 1px solid #00dd00;
  clear: both;
  color: #00dd00;
  cursor: hand;
  display: inline-block;
  font-family: 'VT323', Courier, monospace;
  font-size: 1em;
  margin-bottom: 20px;
  opacity: 0.25;
  padding: 10px 100px;
  position: relative;
  text-decoration: none;
  text-transform: uppercase;
  z-index: 10;
}

input[type=submit]:hover,
a.button:hover {
  background: #00dd00;
  color: #383838;
  opacity: 0.8;
}

</style>