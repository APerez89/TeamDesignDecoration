<template>
  <div class="about" id="about">
    <h1>About Team Design & Decoration</h1>
    <!-- eslint-disable -->
    <p>Rick Garofalo has been a champion in the design industry in the United States since the late 80's. Founded in 1988 by Rick, repertoire became one of the premier design ateliers in the United States bringing the worlds best design to Boston and eventually New York. Repertoire created residential and commercial projects of great distinction until 2005.</p>
    <p>Since 2005, originally based in New York City, reinvented as Team Design and Decoration has worked on projects in New York City, The Hamptons, Westchester County, Florida and Arizona.</p>
    <p>In 2015, having done a project in Rowayton, Connecticut, Rick fell in love with coastal Connecticut and moved the design office to Stamford, an easy commute to service New York City, Westchester and Farifield Counties.</p>
    <p>With almost 30 years in the design industry, Rick is known for his creativity, his hands on attention to detail, and sense of humor.</p>
  </div>
</template>

<script>
export default {
  name: 'About',
};
</script>

<style lang="scss" scoped>
  .about {
    width: 100%;
    background-color: var(--bkgr-light-gray);
    padding: 40px 15px;
    h1 {
      padding-bottom: 20px;
    }
    p {
      font-size: 15px;
      text-align: left;
      letter-spacing: 0.6px;
      line-height: 22px;
      color: var(--light-gray);
      margin-bottom: 8px
    }
    p:last-child {
      margin: 0px;
    }
  }
</style>
