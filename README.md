/* Add these styles to your globals.css */
.loading {
  display: inline-block;
  width: 20px;
  height: 20px;
  border: 3px solid rgba(255,255,255,.3);
  border-radius: 50%;
  border-top-color: #fff;
  animation: spin 1s ease-in-out infinite;
}

@keyframes spin {
  to { transform: rotate(360deg); }
}

/* Custom styling for form elements */
.input, .textarea {
  @apply transition-all duration-200;
}

.input:focus, .textarea:focus {
  @apply ring-2 ring-blue-500 border-transparent;
}

.radio-group-item {
  @apply w-4 h-4 border-2 border-gray-300;
}

.radio-group-item:checked {
  @apply border-blue-500 bg-blue-500;
}

/* Card styling */
.card {
  @apply shadow-lg hover:shadow-xl transition-shadow duration-300;
}

/* Tab styling */
.tabs-trigger {
  @apply transition-all duration-200;
}

.tabs-trigger[data-state="active"] {
  @apply bg-blue-500 text-white;
}

/* Error styling */
.error-message {
  @apply text-red-500 text-sm mt-1;
}

.input-error {
  @apply border-red-500 focus:ring-red-500;
}
