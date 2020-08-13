<template>
  <div>
    <Navigation
      logoURL='/img/logo.png'
    />
    <Content id="home"
      imgURL="https://images.pexels.com/photos/326569/pexels-photo-326569.jpeg?cs=srgb&dl=pexels-pixabay-326569.jpg&fm=jpg"
      name="I'm Francis Lee"
      job="Services Delivery Manager | Technical Project Manager | Freelance Data Analysts"
    />
    <Portfolio id="portfolio">
      <template v-slot:project>
        <Project
          imgURL="https://images.pexels.com/photos/3781895/pexels-photo-3781895.jpeg?cs=srgb&dl=pexels-andrea-piacquadio-3781895.jpg&fm=jpg"
          linkURL="https://gifthub.com"
          name="Service Delivery Management"
          description="Experienced Service Delivery Manager"
        />
        <Project
        imgURL="https://images.pexels.com/photos/372787/pexels-photo-372787.jpeg?cs=srgb&dl=pexels-pixabay-372787.jpg&fm=jpg"
        linkURL="https://github.com"
        name="Technical Project Management"
        description="All about technical projects involved"
      />
      <Project
        imgURL="https://images.pexels.com/photos/3183145/pexels-photo-3183145.jpeg?cs=srgb&dl=pexels-fauxels-3183145.jpg&fm=jpg"
        linkURL="https://github.com"
        name="Data Analysis"
        description="Show you the figures and scorecard"
        />
      </template>
    </Portfolio>
    <About id="strength"
      profileImgURL_1='/img/grid_1.jpeg'
      profileHeader1='MORE THAN'
      profileHeader1_2='RESPONSIVE'
      profileDescription1="Description"

      profileImgURL_2='/img/grid_2.jpeg'
      profileHeader2='POWERFUL'
      profileHeader2_2='PERFORMANCE'
      profileDescription2="Description"
      />
      <Contact id="contact"
        email="chinhoon.lee@gmail.com"
        phone="+6012 2841288"/>
      />
      <Footer />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Portfolio of Francis Lee'
    }
  }
}
</script>
