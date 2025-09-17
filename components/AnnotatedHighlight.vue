<template>
  <div class="annotated-highlight-container">
    <div class="highlight-content">
      <slot name="content" />
    </div>
    <div class="annotation-bubble">
      <slot name="annotation" />
    </div>
  </div>
</template>

<style scoped>
.annotated-highlight-container {
  position: relative;
  display: inline-block; /* Allows the container to wrap its content */
  margin-bottom: 1rem; /* Add some space below */
}

.highlight-content {
  background-color: var(--yellow-light);
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  display: inline-block; /* So it wraps the text */
  white-space: pre-line;
}

.annotation-bubble {
  width: 20rem;
  white-space: pre-wrap !important;
  position: absolute;
  top: 50%; /* Vertically center with the highlight */
  right: calc(100% + 1rem); /* Position to the left of the highlight, with some space */
  transform: translateY(-50%); /* Adjust for vertical centering */
  background-color: var(--blue-dark);
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  white-space: nowrap; /* Prevent text from wrapping inside the bubble */
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
  z-index: 10;
  font-family: sans-serif;
}
</style>

