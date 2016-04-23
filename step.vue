<template>
    <div class="vux-step">
        <div class="vux-step-tail"></div>
        <div class="vux-step-head">

        </div>
        <div class="vux-step-content">
            <div class="vux-step-title">{{title}}</div>
            <div class="vux-step-description">{{description}}</div>
        </div>
    </div>
</template>

<style lang="less">

	.vux-step {
        position: relative;
    }

    .vux-step-tail {
        position: absolute;

    }

    .horizon-steps {
        .vux-step {
            display: inline-block;
        }

        .vux-step-tail {
            width: 100%;
            height: 1px;
            background-color: #04be02;
        }
    }

    .vux-step-head {

    }
</style>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: ''
    }
  }
}
</script>