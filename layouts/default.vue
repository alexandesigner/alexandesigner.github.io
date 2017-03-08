<template>
  <main>
    <nuxt/>
  </main>
</template>

<style>
.container
{
  margin: 0;
  width: 100%;
  padding: 100px 0;
  text-align: center;
}

.button, .button:visited
{
  display: inline-block;
  color: #0076F8;
  letter-spacing: 1px;
  background-color: #fff;
  border: 2px solid #0076F8;
  text-decoration: none;
  text-transform: uppercase;
  padding: 15px 45px;
  border-radius: 28px;
}

.button:hover, .button:focus
{
  color: #fff;
  background-color: #0076F8;
}

.title
{
  color: #555;
  font-weight: 300;
  font-size: 2.5em;
  margin: 0;
}

main {
  display: table-cell;
  vertical-align: middle;
  width: 100%;
}

</style>
