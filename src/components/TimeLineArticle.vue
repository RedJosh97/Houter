<template>
  <div class="timeline">
    <HeadlineProps subTitle="See our review" title="What Our User Say About Us" />
  </div>
  <div class="timeline-article">
    <div class="article-wrapper">
      <TimeLineTemplate
        :sampleImage="'/public/images/Rectangle 17.png'"
        title="I search of a better platform"
        content="I was finally able to sell my house quickly through Hounter by immediately setting me up with people who wanted my house. I also do not get a discount from the sale of my house. Awesome!"
        :profileImage="'/public/images/Ellipse 6-3.png'"
        profileName="Malcom Hitler"
        rating="7.2"
      />
      <TimeLineTemplate
        :sampleImage="'/public/images/Rectangle 17.png'"
        title="I search of a better platform"
        content="I was finally able to sell my house quickly through Hounter by immediately setting me up with people who wanted my house. I also do not get a discount from the sale of my house. Awesome!"
        :profileImage="'/public/images/Ellipse 6-3.png'"
        profileName="Malcom Hitler"
        rating="7.2"
      />
      <TimeLineTemplate
        :sampleImage="'/public/images/Rectangle 21 (2).png'"
        title="Best! I got the house I wanted through Hounter"
        content="Through this website I can get a house with the type and specifications I want very easily,
        without a complicated process to be able to find information on the house we want."
        :profileImage="'/public/images/Ellipse 6-2.png'"
        profileName="Dianne Rusell"
        rating="4.6"
      />
      <TimeLineTemplate
        :sampleImage="'/public/images/Rectangle 21.png'"
        title="Tour through the search globe"
        content="By looking for information about what kind of house we want, we managed to get the house we wanted very quickly, and directly connected with the seller to be able to ask about the details, very helpful!"
        :profileImage="'/public/images/Ellipse 6-2.png'"
        profileName="Andre Scot"
        rating="4.2"
      />
    </div>
  </div>
</template>

<script>
import HeadlineProps from './HeadlineProps.vue'
import TimeLineTemplate from './TimeLineTemplate.vue'
export default {
  name: 'TimeLineArticle',
  components: {
    TimeLineTemplate,
    HeadlineProps
  }
}
</script>

<style scoped>
.timeline {
  text-align: center;
  margin-top: 100px;
  padding: 0px 7rem;
}

.timeline-article {
  margin-top: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 10px;
}

/* .article-wrapper::-webkit-scrollbar {
  background: var(--light-color);
  height: 10px;
  border-radius: 4px;
  border-radius: 50px;
} */

.article-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 1240px;
  overflow-x: scroll;
}
</style>
