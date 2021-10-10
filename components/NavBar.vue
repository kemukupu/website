<template>
    <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
        <a class="navbar-item" href="#">
            <img src="~/assets/MainTitle.png" width="112" height="28">
        </a>

        <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navBar">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
        </a>
    </div>

    <div id="navBar" class="navbar-menu">
        <div class="navbar-end">
        <a href="#about" class="navbar-item">
            About
        </a>
        <a href="#team" class="navbar-item">
            The Team
        </a>
        <NuxtLink to="/api/docs" class="navbar-item">
            Api
        </NuxtLink>
        <div class="navbar-item">
            <a class="button is-primary" href="https://github.com/SOFTENG206-2021/assignment-3-and-project-team-11">
                Download
            </a>
        </div>
        </div>
    </div>
    </nav>
</template>


<style>

</style>