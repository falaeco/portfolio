<template>
  <div>
    <cover>
      <div v-lazy-container="{ selector: 'img' }">
        <img
          :data-src="require('~/assets/img/stupefiant/stupefiant_final_cover.jpg')"
          :data-loading="require('~/assets/img/stupefiant/stupefiant_final_cover.jpg?lqip')"
          alt="Stupefiant project cover"
        >
      </div>
    </cover>
    <p-text-box>
      <template v-slot:header>
        <h1 class="title">
          Stupéfiant
        </h1>
        <h2 class="date">
          April 2020
        </h2>
      </template>
      <p class="text">
        Alcohol, substance intoxication and their effect on society is a recurring major topic through art history. From
        festive scene featuring merry characters to bleak portrayal highlighting substance misuses and abuses, depiction
        of alcohol and drug use wildly varies between different artists. For this project, I wanted to highlight the
        multifaceted aspects of alcohol and drugs using modern methods and technologies.
      </p>
      <p class="text">
        Stupéfiant is a series of three generative compositions exploring the different faces of substance intoxication
        and its ramifications on modern societies. It aims to abstractly depict the experiences of mind-altering
        substance consumptions and dress a contrasting portrait which highlights both the negative and positive aspects
        of alcohol and drug uses. These three compositions are based on three alcoholic beverages, each having their own
        narratives and tackling different aspect linked to alcohol and drug consumption. These three beverages are Rosé
        Wine, which represents the social and agreeable aspect of mild intoxication in social contexts, Whiskey, which
        pictures the darker aspect of alcohol and drug abuse and the hardship associated with withdrawal symptoms and
        other undesirable side-effects, and finally Absinthe, which depicts an intense and psychedelic journey. As an
        installation, the participants are free to choose the composition they would like to see, which will run
        continuously until a new composition is selected. Because of the generative nature of the piece, the audiovisual
        experience will be slightly different for each spectator.
      </p>
      <p>
        I created these compositions using TouchDesigner, a node based visual programming environment for real time
        interactive multimedia content.
      </p>
    </p-text-box>
    <m-vimeo-player id="412561683" title="Rosé Wine Visuals" />
    <m-vimeo-player id="412561942" title="Rosé Wine Visuals: Music clips are chosen randomly" />
    <m-vimeo-player id="412561380" title="Whiskey Visuals" />
    <m-vimeo-player id="412560280" title="Absinthe Visuals" />
    <mobile-projects-nav
      :prev="{
        link: '/projects/voidfilling',
        title: 'Voidfilling',
      }"
      :next="{
        link: '/projects/infinite',
        title: 'In.finite'
      }"
    />
  </div>
</template>

<script>
import MobileProjectsNav from '~/components/MobileProjectsNav'
import PTextBox from '~/components/PTextBox'
import Cover from '~/components/Cover'
import MVimeoPlayer from '~/components/MVimeoPlayer'

export default {
  name: 'Stupefiant',
  components: { PTextBox, Cover, MobileProjectsNav, MVimeoPlayer },
  layout: 'project',
  head () {
    return {
      title: 'Stupéfiant'
    }
  }
}
</script>

<style>
</style>
