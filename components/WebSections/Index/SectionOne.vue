<template>
  <div class="outer-container">
    <canvas ref="backgroundCanvas" class="canvas-background"></canvas>
    <section class="speed-section">
      <div class="content-wrapper">
        <div class="tag">Speed</div>
        <h2 class="title">Why Are My Conversion Rates So Low?</h2>
        <p class="subtitle">
          Research from Google Analytics shows that 53% of users abandon
          websites that take longer than 3 seconds to load. Template-based
          platforms like Shopify have limited speed optimizations, making a
          custom-coded solution essential for improving performance and boosting
          conversions.
        </p>
        <div class="button-group">
          <NuxtLink
            to="/forms/67661cba3a14e729ae1777a1"
            class="btn get-store"
            @click="handleGetNewStore"
          >
            Get My New Store
          </NuxtLink>
          <NuxtLink
            to="https://pagespeed.web.dev"
            class="btn test-speed"
            @click="handleTestSpeed"
          >
            Test My Store Speed
          </NuxtLink>
        </div>
      </div>
      <div class="image-container">
        <img src="/Backgrounds/SectionOneBG.webp" alt="Speed Graphic" />
      </div>
    </section>
  </div>
</template>

<script setup>
import { useNuxtApp } from "#app";

// Function to handle "Get My New Store" click with pixel tracking
const handleGetNewStore = (event) => {
  const { $fbq } = useNuxtApp();
  $fbq("track", "Lead", { content_name: "Get My New Store" });
  // Navigation happens automatically via NuxtLink
};

// Function to handle "Test My Store Speed" click with pixel tracking
const handleTestSpeed = (event) => {
  const { $fbq } = useNuxtApp();
  $fbq("trackCustom", "ClickedStoreSpeedCheck");
  // Navigation to external URL happens automatically via NuxtLink
};
</script>

<style scoped>
.canvas-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 80vh;
  z-index: 0;
  pointer-events: none;
}

.outer-container {
  width: 100%;
  padding: 0;
  position: relative;
}

.speed-section {
  background: black;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  text-align: left;
  padding: 2rem;
  color: white;
  max-width: calc(1300px + 2rem);
  margin: 0 auto;
  background: none;
  gap: 4rem;
}

.content-wrapper {
  z-index: 2;
  padding: 2rem 0;
  flex: 1;
}

.tag {
  font-family: "Source Sans Pro", sans-serif;
  font-size: 0.9rem;
  background-color: #0072a3;
  color: white;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  display: inline-block;
  margin-bottom: 1rem;
}

.title {
  font-family: "Source Sans Pro", sans-serif;
  font-size: 3rem;
  /* line-height: 3.3rem; */
  font-weight: 600;
  margin-bottom: 1rem;
}

.subtitle {
  font-family: "Source Sans Pro", sans-serif;
  font-size: 1.2rem;
  color: white;
  margin-bottom: 2rem;
  /* line-height: 1.5; */
}

.button-group {
  display: flex;
  gap: 1rem;
  flex-wrap: nowrap;
}

.btn {
  font-family: "Source Sans Pro", sans-serif;
  font-size: 1.1rem;
  padding: 10px;
  width: 200px;
  border: none;
  cursor: pointer;
  transition: all 0.1s;
  font-weight: bold;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 0;
}

.get-store {
  background-color: #0072a3;
  color: white;
}

.get-store:hover {
  background-color: #004280;
}

.test-speed {
  background-color: white;
  color: black;
}

.test-speed:hover {
  background-color: #e0e0e0;
}

.image-container {
  z-index: 2;
  padding: 0;
  flex: 1;
}

.image-container img {
  width: 100%;
  height: auto;
}

/* Responsive adjustments */
@media (max-width: 1024px) {
  .speed-section {
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    gap: 4rem;
  }

  .image-container {
    width: 100%;
    max-height: 25rem;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0;
  }

  .image-container img {
    width: 90%;
    height: auto;
    object-fit: cover;
  }

  .button-group {
    justify-content: center;
  }
}

@media (max-width: 992px) {
  .title {
    font-size: 2.2rem;
  }
  .subtitle {
    font-size: 1rem;
  }
}

@media (max-width: 480px) {
  .content-wrapper {
    padding: 0;
  }

  .speed-section {
    padding: 1rem;
  }

  .title {
    font-size: 2.2rem;
    /* line-height: 1.8rem; */
  }

  .subtitle {
    font-size: 0.9rem;
  }

  .button-group {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .btn {
    font-size: 1rem;
    width: 100%;
  }

  .image-container {
    max-width: 100%;
    min-width: 100%;
  }
  img {
    min-width: 100%;
  }
}
</style>