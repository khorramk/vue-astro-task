

<template>
  <header class="cta-hero" role="banner" aria-label="Hero Section">
    <div class="cta-img-container">
        <img
          src="img/ctaMobilePlacheolder.svg"
          width="600"
          height="1000"
          role="img"
          loading="eager"
          srcset="
            img/ctaMobilePlacheolder.svg  600w,
            img/ctaPlaceholder.svg       1200w
          "
          sizes="(max-width: 700px) 400px, (max-width: 800px) 1400px"
        />
    </div>

    <div class="cta-hero__content">
      <h1 class="cta-hero__title">Get Online week 2021</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Delectus ea
        repudiandae soluta enim modi ratione minima illo rerum facere aliquam
        consequuntur, neque at qui, culpa adipisci praesentium. Nesciunt, magnam
        deleniti.
      </p>

      <div class=" link-tag no-border">
          <a href="learn-more">learn more</a>
      </div>
      
    </div>
  </header>
</template>
