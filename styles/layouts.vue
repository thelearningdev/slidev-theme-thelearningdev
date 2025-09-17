<template>
  <div>
    <!-- Default layout is inherited -->
    
    <!-- Blue sidebar layout -->
    <template v-if="$slidev.nav.currentLayout === 'blue-sidebar'">
      <div class="blue-sidebar-layout">
        <div class="sidebar">
          <slot name="sidebar">
            <h1>{{ $slidev.nav.currentPage.title }}</h1>
          </slot>
        </div>
        <div class="content">
          <slot />
        </div>
      </div>
    </template>
    
    <!-- Default slot for other layouts -->
    <slot v-else />
  </div>
</template>

