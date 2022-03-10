<template>
<div class="home-page page-box">
  <section class="home-page__news">
    <Card title="NÓTICIAS">
      IHULLLL
    </Card>
  </section>
  <aside class="home-page__cards">
    <Card title="SERVIDOR">
      Online
    </Card>
    <Card title="TOP LEVEL">
      <u>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        <li>6</li>
        <li>7</li>
        <li>8</li>
        <li>9</li>
        <li>10</li>
      </u>
    </Card>
    <Card title="TOP PVP">
     <u>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        <li>6</li>
        <li>7</li>
        <li>8</li>
        <li>9</li>
        <li>10</li>
      </u>
    </Card>
    <Card title="TOP BELLATRA">
      <u>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        <li>6</li>
        <li>7</li>
        <li>8</li>
        <li>9</li>
        <li>10</li>
      </u>
    </Card>
  </aside>
</div>
</template>

<script>
import Card from '../components/Card/Card.vue'
export default {
  components: { Card },
  name: 'IndexPage'
}
</script>

<style lang="scss" scoped>
.home-page {
  display: flex;

  &__news {
    width: 70%;
    margin-right: 20px;
    box-sizing: border-box;
  }

  &__cards {
    width: 30%;

    .card {
      margin-bottom: 20px;
    }
  }

  @media (max-width: 992px) {
    flex-direction: column;

    &__news, &__cards {
      width: 100%;
    }

    &__news {
      margin-right: 0;
    }
  }
}
</style>