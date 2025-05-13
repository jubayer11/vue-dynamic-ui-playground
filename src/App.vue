<template>
  <div class="app-container">
    <!-- 🌟 Header -->
    <header class="app-header">
      <h1 class="title gradient-text">Vue Dynamic System Showcase</h1>
      <p class="subtitle">Form Builder + Table Builder — Real World Usage Example</p>
    </header>

    <!-- 🧾 Form Section -->
    <section class="section">
      <h2 class="section-title">📄 Dynamic Form</h2>
      <p class="section-description">
        This form is powered by <strong>Vue Dynamic Form Builder</strong>, a schema-based form engine that supports built-in and custom validations, backend error handling, and full layout control.
      </p>
      <div class="section-box">
        <Form />
      </div>
    </section>

    <!-- 📊 Table Section -->
    <section class="section">
      <h2 class="section-title">📊 Dynamic Table</h2>
      <p class="section-description">
        This table is built using <strong>Vue Dynamic Table Builder</strong>. It supports expandable rows, action icons, pagination modes, and full styling via configuration.
      </p>
      <div class="section-box">
        <Table />
      </div>
    </section>

    <!-- 🦶 Footer -->
    <footer class="app-footer">
      <p>Made with ❤️ by <a href="https://www.jubayerahmed.com" target="_blank">Jubayer Ahmed</a></p>
    </footer>
  </div>
</template>

<script setup>
import Form from "@/components/form/index.vue";
import Table from "@/components/table/index.vue";
</script>

<style scoped>
/* 🎨 Base Layout */
.app-container {
  font-family: 'Segoe UI', sans-serif;
  padding: 2rem 1rem;
  max-width: 1200px;
  margin: auto;
  line-height: 1.6;
  transition: all 0.3s ease;
}

/* 🌟 Header */
.app-header {
  text-align: center;
  margin-bottom: 3rem;
}
.title {
  font-size: 2.2rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
}
.gradient-text {
  background: linear-gradient(to right, #6366f1, #14b8a6);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.subtitle {
  font-size: 1.1rem;
  color: #475569;
}

/* 🧾 Section Blocks */
.section {
  margin-bottom: 3rem;
}
.section-title {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 0.3rem;
  color: #1f2937;
}
.section-description {
  color: #4b5563;
  font-size: 1rem;
  margin-bottom: 1.2rem;
}
.section-box {
  background-color: #f9fafb;
  border: 1px solid #e5e7eb;
  padding: 1.5rem;
  border-radius: 1rem;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.03);
}

/* 🦶 Footer */
.app-footer {
  margin-top: 4rem;
  text-align: center;
  font-size: 0.95rem;
  color: #6b7280;
}
.app-footer a {
  color: #2563eb;
  text-decoration: none;
  font-weight: 600;
}
.app-footer a:hover {
  text-decoration: underline;
}

/* 🌙 Dark Mode */
:deep(.dark-mode) .app-container {
  background-color: #111827;
  color: #e5e7eb;
}
:deep(.dark-mode) .subtitle,
:deep(.dark-mode) .section-description,
:deep(.dark-mode) .app-footer {
  color: #94a3b8;
}
:deep(.dark-mode) .section-box {
  background-color: #1f2937;
  border-color: #334155;
}
:deep(.dark-mode) .section-title {
  color: #f3f4f6;
}
</style>
