<template>
  <portfolio-project
    :title="title"
    :year="year"
    :company="company"
    :companyHref="companyHref"
    :projectHref="projectHref"
    :projectImages="projectImages" />
</template>

<script>
  import PortfolioProject from 'Components/PortfolioProject';
  import imageHome from './assets/spectrum-home.png';
  import imageSearch from './assets/spectrum-search.png';
  import imageEvents from './assets/spectrum-events.png';

  export default {
    meta: {
      ...PortfolioProject.meta,
      pageTitle: 'Spectrum Health - Stumptown Bear'
    },
    data() {
      return {
        title: 'Spectrum Health',
        year: 2016,
        company: 'ConnectiveDX',
        companyHref: 'https://www.connectivedx.com/',
        projectHref: 'http://www.spectrumhealth.org/',
        projectImages: [{
          alt: 'Homepage',
          asset: imageHome
        }, {
          alt: 'Search application',
          asset: imageSearch
        }, {
          alt: 'Events page',
          asset: imageEvents
        }]
      }
    },
    components: {
      PortfolioProject
    }
  }
</script>
