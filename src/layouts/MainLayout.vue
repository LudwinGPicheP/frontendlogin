<template>
    <div class="layout">
        <header class="header">
            <NavMenu />
        </header>
        <main class="content">
            <slot></slot>
        </main>
        <footer class="footer">
            <FooterPage/>
        </footer>
    </div>
</template>

<script lang="ts" setup>
import NavMenu from '@/components/NavMenu.vue';
import FooterPage from '@/components/FooterPage.vue';
</script>

<style scoped>
.layout {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    font-family: Arial, sans-serif;
    color: #333;
}

.header {
    background: #FF2800;
    /* Ferrari red */
    color: white;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.content {
    flex: 1;
    padding: 20px;
    background: #f8f9fa;
}

.footer {
    background: #FF2800;
    /* Ferrari red */
    color: white;
    text-align: center;
    padding: 10px 20px;
    box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
}
</style>