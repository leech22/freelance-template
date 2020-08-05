<template>
  <div>
    <Navigation 
      logoURL='/img/logo.png'
    />
    <Content id="home"
      imgURL='/img/bg_1.jpg'
      name="I'm Edmund Hee"
      job="FullStack Developer | Data Scientist"
    />
    <Portfolio id="portfolio">
      <template v-slot:project>
        <Project 
          imgURL="/img/product-1.jpg"
          linkURL="https://github.com"
          name="Project Name"
          description="Description"
        />
        <Project 
          imgURL="/img/product-1.jpg"
          linkURL="https://github.com"
          name="Project Name"
          description="Description"
        />
        <Project 
          imgURL="/img/product-1.jpg"
          linkURL="https://github.com"
          name="Project Name"
          description="Description"
        />
      </template>
    </Portfolio>
    <About id="about"
      profileImgURL_1='/img/grid_1.jpg'
      profileHeader1='MORE THAN'
      profileHeader1_2='RESPONSIVE'
      profileDescription1="Description"

      profileImgURL_2='/img/grid_2.jpg'
      profileHeader2='POWERFUL'
      profileHeader2_2='PERFORMANCE'
      profileDescription2="Description"
      />
      <Contact id="contact"
        email="EDMUND@THELEAD.IO"
        phone="+60123456789"
      />
      <Footer />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Name'
    }
  }
}
</script>
