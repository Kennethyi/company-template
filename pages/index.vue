<template>
  <div class="relative">
    <div class="h-screen">
      <div class="flex flex-col">
        <!-- 
          Header Content ( Landing Page )

          PARAMETERS
          :imgURL (URL for Background)
          :header_txt ( Header Text )
          :second_header ( Header 2 Text)
          :descriptions ( Descriptions )
        -->
        <HeaderContent
          imgURL="https://cupofcoffee.biz/storage/2018/11/coffee-photo-1-e1542207744727.jpg"
          header_txt="The Lead"
          second_header="Institude of Growth"
          descriptions="FullStack Web Development Workshop"
        ></HeaderContent>
        <!-- 
          About Content 

          PARAMETERS
          :imgURL ( URL for about us )
        -->
        <AboutContent
          imgURL="https://www.impactbnd.com/hubfs/blog-image-uploads/best-about-us-pages.jpg"
        >
          <template
            v-slot:about
          >LEAD, is the institude that focus on growth. We help those that want to change theri career.</template>
        </AboutContent>

        <ServiceContent>
          <template v-slot:services>
            <!-- 

              Service 

              PARAMETERS

              :imgURL (image url)
            -->
            <Service imgURL="/img/icon1.png" title="Turn idea into Reality">
              <template v-slot:content>Help and guide to turn ideas into Applications</template>
            </Service>

            <Service imgURL="/img/icon2.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon3.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon4.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon1.png" title="Turn idea into Reality">
              <template v-slot:content>Help and guide to turn ideas into Applications</template>
            </Service>
          </template>
        </ServiceContent>

        <!-- 
          Portfolio
        -->
        <PortfolioContent>
          <template v-slot:portfolio>
            <!-- 
              Project

              PARAMETERS
              :imgURL ( img URL for Project )
              :name ( Name of the Project )
              :project ( Name of Project Type)
              :projectURL ( Link Address to project)
            -->
            <Project
              imgURL="https://i.pinimg.com/originals/52/ea/be/52eabecf424b217807d0e557b9a0c38e.jpg"
              name="Company Template"
              project="NuxtJS.app"
              projectURL="https://github.com/Kennethyi/company-template"
            />
            <Project
              imgURL="https://i.pinimg.com/originals/52/ea/be/52eabecf424b217807d0e557b9a0c38e.jpg"
              name="Company Template"
              project="NuxtJS.app"
              projectURL="https://github.com/Kennethyi/company-template"
            />
          </template>
        </PortfolioContent>
        <ContactContent
          address="Level 11, Menara KEN TTDI, No.37 Jalan Burhanuddin Helmi, Taman Tun Dr. Ismail"
          email="support@thelead.io"
          phone="6016-473 7281"
          imgURL="/img/lead-white-logo.png"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: "theLEAD"
    };
  }
};
</script>