<template>
    <header ng-controller="PrincipalCtrl">
        <h2>
            <a href="/" class="logo"><p class="swing">Top Stickers</p></a>
        </h2>
        <nav>
            <li>
                <a href="/filmes" class="filmes"><p class="swing">Cultura Nerd</p></a>
            </li>
            <li>
                <a href="/animes" class="animes"><p class="swing">Devs</p></a>
            </li>
        </nav>
    </header>
</template>

<style>
header {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 10;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  padding: 20px 150px 20px;
}

header h2 {
  font-family: "GothamRnd-Book", sans-serif;
}

header nav {
  display: flex;
}

header nav li {
  margin: 0 15px;
}

header nav li:first-child {
  margin-left: 0;
}

header nav li:last-child {
  margin-right: 0;
}
</style>
