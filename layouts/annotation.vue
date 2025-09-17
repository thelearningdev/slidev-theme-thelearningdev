<template>
   <div class="slidev-layout blue-sidebar">
     <div class="blue-sidebar-left">
      <slot name="header">
      </slot>
      <div class="annotation-box">
        <slot name="annotation" />
      </div>
    </div>
    <div class="content">
      <slot />
    </div>
  </div>
</template>

<style>
.annotation-layout {
  display: grid;
  grid-template-columns: 30% 70%;
  height: 100%;
}

.sidebar {
  background-color: var(--blue-light);
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
}

.content {
  padding: 2rem;
  position: relative;
}

.annotation-box {
  width: 100%;
}
</style>

