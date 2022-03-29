<template>
  <div class="home-page">
    <div class="home-page__carousel">
      <client-only placeholder="Loading...">
        <agile>
          <img
            class="slide"
            src="~/assets/images/banner-pike.png"
          />
          <img
            class="slide"
             src="~/assets/images/banner-pike.png"
          />
        </agile>
      </client-only>
    </div>
    <div class="page-box home-page__content">
      <section class="home-page__news">
        <Card title="NÓTICIAS"> IHULLLL </Card>
      </section>
      <aside class="home-page__cards">
        <Card title="SERVIDOR" :icon="require('~/assets/images/servericon.png')"> Online </Card>
        <Card title="TOP LEVEL" :icon="require('~/assets/images/toplevel.svg')">
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
        <Card title="BLESS CASTLE" :icon="require('~/assets/images/bc.svg')">
          Online
        </Card>
        <Card title="TOP PVP" :icon="require('~/assets/images/pvp.svg')">
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
        <Card title="TOP BELLATRA" :icon="require('~/assets/images/sod.svg')">
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
  </div>
</template>

<script>
import Card from "../components/Card/Card.vue";

export default {
  components: { Card },
  name: "IndexPage",
};
</script>

<style lang="scss">
.home-page {
  display: flex;
  flex-direction: column;

  &__content {
    display: flex;
    margin-top: 0;
  }

  &__carousel {
    .agile {
      &__nav-button {
        background: transparent;
        border: none;
        color: #fff;
        cursor: pointer;
        font-size: 24px;
        height: 100%;
        position: absolute;
        top: 0;
        transition-duration: 0.3s;
        width: 80px;
        &:hover {
          background-color: rgba(#000, 0.5);
          opacity: 1;
        }

        &--prev {
          left: 0;
        }

        &--next {
          right: 0;
        }
      }

       &__dots {
          bottom: 10px;
          left: 50%;
          position: absolute;
          transform: translateX(-50%);
        }

        &__dot {
          margin: 0 10px;
          button {
            background-color: transparent;
            border: 1px solid #fff;
            border-radius: 50%;
            cursor: pointer;
            display: block;
            height: 10px;
            font-size: 0;
            line-height: 0;
            margin: 0;
            padding: 0;
            transition-duration: 0.3s;
            width: 10px;
          }

          &--current,
          &:hover {
            button {
              background-color: #fff;
            }
          }
        }
    }
  }

  &__news {
    width: 70%;
    margin-right: 20px;
    box-sizing: border-box;
  }

  &__cards {
    width: 30%;

    .card {
      margin-bottom: 20px;

      &__icon {
        filter: invert(65%) sepia(52%) saturate(6375%) hue-rotate(328deg)
          brightness(100%) contrast(101%);
          width: 24px;
          height: 24px;
      }
    }
  }

  @media (max-width: 992px) {
    &__content {
      flex-direction: column;
    }

    &__carousel {
      .agile {
        img {
          height: 300px;
        }
      }
    }

    &__news,
    &__cards {
      width: 100%;
    }

    &__news {
      margin-right: 0;
    }
  }
}
</style>