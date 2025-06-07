<script setup>
definePageMeta({
  layout: "default",
});

const page = {
  hero: {
    title: "When Crows Wore Sunglasses",
    description:
      "A noir-inspired collection of surreal short stories exploring fractured identity, guilt, and myth in a modern world. Each tale lingers like smoke in the air.",
    image: "/images/book-cover.png", // Add this image to your /public/images
    imageAlt: "Book cover of When Crows Wore Sunglasses",
    buttons: [
      {
        text: "Buy on Amazon",
        href: "https://www.amazon.com/s?k=B09V1S16LR&i=digital-text&_encoding=UTF8&isDramIntegrated=true&shoppingPortalEnabled=true",
        primary: true,
      },
    ],
  },
  logos: {
    title: "Seen on",
    icons: [
      "/images/logos/kindle.svg",
      "/images/logos/booktok.svg",
      "/images/logos/goodreads.svg",
    ],
  },
  features: {
    title: "What Makes This Book Unmissable",
    description: "It's not just fiction—it's a lens into forgotten corners of the human psyche.",
    items: [
      {
        title: "Gritty & Surreal",
        description: "Mashes noir storytelling with surrealism to create unforgettable vignettes.",
        icon: "mdi:weather-night",
      },
      {
        title: "Themes That Linger",
        description: "Each story digs into guilt, identity, and strange beauty.",
        icon: "mdi:drama-masks",
      },
      {
        title: "Visual Storytelling",
        description: "Written with a cinematic touch that evokes vivid, lasting images.",
        icon: "mdi:camera-outline",
      },
    ],
  },
  testimonials: {
    title: "Reader Reviews",
    description: "Here’s what early readers are saying:",
    items: [
      {
        quote: "Haunting, cinematic, and devastatingly human.",
        author: "Dev M., Scriptwriter",
      },
      {
        quote: "It’s like stepping into a dream that knows your secrets.",
        author: "Maya R., Blogger",
      },
      {
        quote: "Each story hits like a quiet thunderstorm. A must-read.",
        author: "Alex J., Editor",
      },
    ],
  },
  cta: {
    title: "Experience the Stories.",
    description:
      "Available now on Amazon. Get your copy and step into the shadows.",
    buttons: [
      {
        text: "Buy Now",
        href: "https://www.amazon.com/s?k=B09V1S16LR&i=digital-text&_encoding=UTF8&isDramIntegrated=true&shoppingPortalEnabled=true",
        primary: true,
      },
    ],
  },
};
</script>

<template>
  <Container>
    <Hero
      :title="page.hero.title"
      :description="page.hero.description"
      :image="page.hero.image"
      :imageAlt="page.hero.imageAlt"
      :buttons="page.hero.buttons"
    />
    <Logos :title="page.logos.title" :icons="page.logos.icons" />
    <Features
      :title="page.features.title"
      :description="page.features.description"
      :items="page.features.items"
    />
    <Testimonials
      :title="page.testimonials.title"
      :description="page.testimonials.description"
      :items="page.testimonials.items"
    />
    <Cta
      :title="page.cta.title"
      :description="page.cta.description"
      :buttons="page.cta.buttons"
    />
  </Container>
</template>
