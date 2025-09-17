<template>
  <div class="slidev-layout blue-sidebar">
    <div class="blue-sidebar-left">
      <slot name="header">
        <h1>{{ $slidev.nav.currentPage.title }}</h1>
      </slot>
    </div>
    <div class="slidev-content">
      <slot name="content"/>
    </div>
  </div>
</template>

