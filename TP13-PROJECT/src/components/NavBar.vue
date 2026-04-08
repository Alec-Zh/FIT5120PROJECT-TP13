<template>
  <header class="header">
    <div class="header-container">
      <div class="brand">
        <span class="brand-name">CoolPath</span>
        <img src="/logo.png" alt="CoolPath Melbourne" class="logo" />
      </div>

      <nav class="nav">
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/heatmap" class="nav-link">HeatMap</RouterLink>
        <RouterLink to="/cool-refuges" class="nav-link">Cool Refuges</RouterLink>
      </nav>

      <button class="btn-alerts">Get Alerts</button>
    </div>
  </header>
</template>

<style scoped>
.header {
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-container {
  max-width: var(--max-width);
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
}

.brand {
  display: flex;
  align-items: center;
  gap: 0.25rem;
}

.brand-name {
  color: var(--color-primary);
  font-weight: bold;
  font-size: 20px;
}

.logo {
  width: 120px;
  object-fit: contain;
}

.nav {
  display: flex;
  gap: 2rem;
}

.nav-link {
  text-decoration: none;
  color: var(--color-text-muted);
  font-size: 1rem;
  padding: 0.5rem 0;
  cursor: pointer;
  transition: color 0.3s ease;
}

.nav-link:hover {
  color: var(--color-primary);
}

.nav-link.router-link-active {
  color: var(--color-primary);
  border-bottom: 2px solid var(--color-primary);
}
</style>
